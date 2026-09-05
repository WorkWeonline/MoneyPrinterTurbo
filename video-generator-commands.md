# MoneyPrinter Kurulum Rehberi

> Aşağıdaki komutlar `harry0703/MoneyPrinterTurbo` deposu içindir.

## 1. Normal Kurulum

### Projeyi İndir

```bash
git clone https://github.com/harry0703/MoneyPrinterTurbo.git
cd MoneyPrinterTurbo
```

### Python Ortamını Kur

```bash
uv python install 3.11
uv sync --frozen
```

### Windows

```powershell
.\webui.bat
```

### macOS / Linux

```bash
sh webui.sh
```

### Arayüz

```text
http://127.0.0.1:8501
```

---

## 2. Docker ile Kurulum

### Projeyi İndir

```bash
git clone https://github.com/harry0703/MoneyPrinterTurbo.git
cd MoneyPrinterTurbo
```

### Yapılandırma Dosyasını Oluştur

#### Windows PowerShell

```powershell
Copy-Item config.example.toml config.toml
```

#### macOS / Linux

```bash
cp config.example.toml config.toml
```

### Docker'ı Başlat

```bash
docker compose -f docker-compose.release.yml up
```

### Web Arayüzü

```text
http://127.0.0.1:8501
```

### API

```text
http://127.0.0.1:8080/docs
```

---

## 3. Ollama Kullanımı

### Modeli İndir

```bash
ollama pull qwen2.5:7b
```

### Kurulu Modelleri Kontrol Et

```bash
ollama list
```

### Normal Kurulumda Ollama Adresi

```text
http://127.0.0.1:11434
```

### Docker Desktop Kullanıyorsan Ollama Adresi

```text
http://host.docker.internal:11434
```

---

## Önerilen Ücretsiz Ayarlar

```text
LLM Provider: Ollama
Model: qwen2.5:7b
Video Source: Pexels
TTS: Edge TTS / Azure TTS V1
Subtitle Provider: Edge
Video Ratio: 9:16
Resolution: 1080x1920
```