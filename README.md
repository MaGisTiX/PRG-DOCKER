# DOCKER
- Docker je open-source platforma na kontejnerizaci aplikací, která umožŇuje balit aplikace a všechny jejich závoslosti do standardizovaných kontejnerů.
# Instalace přes Oracle VirtualBox
- Vytvořte novoý vyrtuální stroj v Oracle VirtualBox a přiřaďtě mu dostatek paměti a prostoru na disku.
- Nainstalujte Ubuntu do nového virtuálního stroje.
- Otevřete terminál a aktualizujte Ubuntu.
```
sudo apt-get update
```
- Nainstalujte balíčky potřebné pro instalaci dockeru:```
sudo apt-get install apt-transport-https ca-certificates curl gnupg lsb-release
- ```
- Přidejte Dockeru GPG klíč: ```
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
- ```
- Přidejte Docker repozitář do systému: ```
echo "deb [arch=amd64 signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
- ```
- Nainstalujte Docker: ```
sudo apt-get install docker-ce
- ```
- Ověřte, že Docker běží: ```
sudo docker run hello-world
- ```
