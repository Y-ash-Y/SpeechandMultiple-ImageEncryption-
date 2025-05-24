# Speech and Multiple-Image Encryption using Chaotic Maps and FPGA

This project presents a chaotic physics-inspired approach to secure **audio and image encryption**, simulated in **Python** and later implemented using **FPGA (Verilog)**.

Chaotic maps like the **Logistic Map**, **Henon Map**, and **Arnold Cat Map** are used for their extreme sensitivity to initial conditions — even tiny changes in the key lead to wildly different results, making brute-force decryption nearly impossible.

## Key Features

- **Chaotic Map-Based Encryption**
  - Logistic Map (simple yet powerful)
  - Henon Map (2D chaos)
  - Arnold Cat Map (periodic pixel mixing)

- **Python Simulation**
  - Encrypt/decrypt audio & image files
  - Key sensitivity and auto-correlation analysis
  - Verifies theoretical feasibility

- **FPGA Implementation (Verilog)**
  - Verilog modules for each chaotic map
  - Control FSM to manage encryption flow
  - Real-time simulation (hardware testing pending due to cable issues)

## Why Chaotic Maps?

Chaotic maps:
- Are lightweight and fast
- Have strong key sensitivity
- Are great for multimedia encryption (audio/image)
- Require fewer resources than AES or RSA

## Results

-  Strong encryption confirmed via Python simulation
-  Auto-correlation analysis confirms randomness
-  Key sensitivity tests show excellent unpredictability
-  Scrambled images and audio waveforms show effective encryption

##  Languages Used

- Python (NumPy, PIL, etc.)
- Verilog (for FPGA simulation)
- Chaotic Maps: Logistic, Henon, Arnold Cat

## How to Run

### Python Simulation

```bash
# Clone this repo
git clone https://github.com/yourusername/speech-image-chaotic-encryption.git
cd speech-image-chaotic-encryption

# Run the encryption/decryption scripts
python encrypt_audio.py
python decrypt_audio.py
python encrypt_image.py
python decrypt_image.py
