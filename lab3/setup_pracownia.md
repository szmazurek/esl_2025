1. Będziemy pracować na systemie Linux używając WSL (nie oracle VM).
2. Z pendrive skopiować do folderu z filesystemem Linux do katalogu `/home/student/` (lub podkatalogu w tym folderze) pliki:
    - `vitis-ai-container.tar`
    - `vitis-ai.tar.gz`
    - `resnet18.pt`
    - `vitis_ai_library_r3.0.0_images.tar.gz`
    - `archive.zip`

3. W terminalu WSL przejść do katalogu `/home/student/` (lub podkatalogu w tym folderze) i wykonać poniższe polecenia:
```bash
# załadowanie kontenera vitis-ai
sudo docker load -i vitis-ai-container.tar
# rozpakowanie plików vitis-ai
tar -xvzf vitis-ai.tar.gz
# rozpakowanie obrazów biblioteki vitis-ai
tar -xvzf vitis_ai_library_r3.0.0_images.tar.gz
# rozpakowanie archiwum z plikami do laboratorium
unzip archive.zip
```
4. Po rozpakowaniu plików można przejść do punktu 5 głównej instrukcji laboratorium.
UWAGA! Przy wywołaniu skryptu `host_cross_compiler_setup.sh` pliki, które pobiera skrypt powinny juz znajodować się w katalogu. Nie należy rozpoczynać ponownego pobierania (skrypt o to zapyta), ponieważ zajmuje to sporo czasu.