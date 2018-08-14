# Windows

Chromedriver is the driver to control Chrome from Selenium. This driver and the Chrome browser are a prerequisite for using Tastee.

## Install Chrome

Make sure you have a Chrome browser installed on your Desktop.

If not, go to [https://www.google.fr/chrome/index.html](https://www.google.fr/chrome/index.html) and follow installation steps

## Install Chromedriver

Follow this [steps](http://chromedriver.chromium.org/getting-started) to install Chromedriver.

NOTE : Chromedriver have to be referenced in your System PATH, not only in your user PATH

## Download and launch Tastee

Tastee can be downloaded [here](https://github.com/tastee/tastee-ui/releases/download/0.9.4/tastee-ui.0.9.4.exe)

To launch Tastee, launch `tastee-ui-xxx.exe`

## Troubleshooting

### Chrome doesn't launch

You might have set Chromedriver executable path in your user profile PATH variable. To launch, Tastee needs to access ChromeDriver from the System PATH.