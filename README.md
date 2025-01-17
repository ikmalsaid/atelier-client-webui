# atelier-webui

A Gradio-based web interface for Atelier clients, providing a user-friendly interface for user to interact with the Atelier client.

## Features

- Support for multiple image generation models
- Image manipulation and styling capabilities
- LoRA model integration
- Controlnet support
- Various image processing modes
- Real-time image generation
- Customizable parameters for generation

## Requirements
- Python 3.8+
- atelier-client

## Installation

```bash
pip install atelier-client-webui
```

## Usage

```python
from atelier_client_webui import AtelierWebUI
from atelier_client import AtelierClient

# Initialize Atelier client
client = AtelierClient()

# Launch the web interface
AtelierWebUI(
    client,
    address="127.0.0.1",  # Optional: Server address
    port=7860,            # Optional: Server port
    browser=True,         # Optional: Auto-launch browser
    upload_size="4MB",    # Optional: Max upload size
    public=False,         # Optional: Enable public URL
    limit=10              # Optional: Max concurrent requests
)
```

## License

See [LICENSE](LICENSE) for details.
