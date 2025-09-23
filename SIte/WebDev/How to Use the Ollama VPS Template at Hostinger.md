
Updated 1 year ago

Ollama is a versatile platform for running and fine-tuning machine learning models (including language models like Llama3). The Ubuntu 24.04 with Ollama VPS template on Hostinger comes preinstalled with Ollama, the Llama3 model, and Open WebUI, giving you a ready-made environment to manage and run models. This guide walks you through accessing and setting up Ollama.
  

Accessing Ollama
  

Open your web browser and go to:

https://[your-vps-ip]:8080

Replace [your-vps-ip] with the actual IP address of your VPS.

  

The first time you access it, you’ll be prompted to create an account. These credentials will be used for all future logins.

  

  

  

  

Getting to Know Open WebUI

  

  

Once logged in, you’ll land at the Open WebUI dashboard, where you can:

  

- Monitor active models
- Upload new datasets and models
- Track model training and inference tasks

  

  

The Llama3 model is preinstalled and can be managed / fine-tuned from this UI. You can add more models via the settings (gear icon → Models).

  

  

  

  

Running Inference with Llama3

  

  

You can run inference (i.e. input prompts and get outputs) via Open WebUI using the Llama3 model. You can:

  

- Input custom prompts or datasets
- Adjust hyperparameters
- Experiment with fine-tuning based on your data

  

  

Be aware: performance depends heavily on which model you use and how many CPU cores your VPS has. Big models = more compute demand. If needed, you can upgrade your VPS to get more CPU cores for better performance.

  

  

  

  

Additional Resources

  

  

- Official Ollama documentation (on GitHub)
- Tutorials
- Hostinger Blog
- Hostinger Academy

  

  

  

  

Do you want me to go one step further and turn this into a ready-to-use README.md file (with images, proper links, etc.), so you can just drop it into your project?