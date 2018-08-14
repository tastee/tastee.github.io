# Linux

Chromedriver is the driver to control Chrome from Selenium. This driver and the Chrome browser are a prerequisite for using Tastee.

## Install Chromedriver

To install Chromedriver with a Chromium browser, you can use Ubuntu packages :

```sh
 sudo apt-get install chromium-chromedriver
 sudo ln -s /usr/lib/chromium-browser/chromedriver /usr/bin/chromedriver
```

## Download and Install Tastee

Tastee can be downloaded [here](https://github.com/tastee/tastee-ui/releases/download/0.9.6/tastee-ui-0.9.6-x86_64.AppImage)

To install Tastee, launch `tastee-ui-xxx.AppImage`

## Troubleshooting

### Tastee doesn't launch

The file downloaded might not be executable.  
To do so, in a Terminal, launch :

```sh
chmod +x tastee-ui-*.AppImage
```