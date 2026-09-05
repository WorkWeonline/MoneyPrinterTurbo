MoneyPrinter Kurulum Rehberi
Aşağıdaki komutlar harry0703/MoneyPrinterTurbo deposu içindir.

1. Normal Kurulum
Projeyi İndir
git clone https://github.com/harry0703/MoneyPrinterTurbo.git
cd MoneyPrinterTurbo
Python Ortamını Kur
uv python install 3.11
uv sync --frozen
Windows
.\webui.bat
macOS / Linux
sh webui.sh
Arayüz
http://127.0.0.1:8501
2. Docker ile Kurulum
Projeyi İndir
git clone https://github.com/harry0703/MoneyPrinterTurbo.git
cd MoneyPrinterTurbo
Yapılandırma Dosyasını Oluştur
Windows PowerShell
Copy-Item config.example.toml config.toml
macOS / Linux
cp config.example.toml config.toml
Docker'ı Başlat
docker compose -f docker-compose.release.yml up
Web Arayüzü
http://127.0.0.1:8501
API
http://127.0.0.1:8080/docs
3. Ollama Kullanımı
Modeli İndir
ollama pull qwen2.5:7b
Kurulu Modelleri Kontrol Et
ollama list
Normal Kurulumda Ollama Adresi
http://127.0.0.1:11434
Docker Desktop Kullanıyorsan Ollama Adresi
http://host.docker.internal:11434
Önerilen Ücretsiz Ayarlar
LLM Provider: Ollama
Model: qwen2.5:7b
Video Source: Pexels
TTS: Edge TTS / Azure TTS V1
Subtitle Provider: Edge
Video Ratio: 9:16
Resolution: 1080x1920
