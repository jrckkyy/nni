**How to contribute**
===
## Best practice for debug NNI source code

For debugging NNI source code, your development environment should be under Ubuntu 16.04 (or above) system with python 3 and pip 3 installed, then follow the below steps.

**1. Clone the source code**

Run the command
```
git clone https://github.com/Microsoft/nni.git
```
to clone the source code

**2. Prepare the debug environment and install dependencies**

Change directory to the source code folder, then run the command
```
make install-dependencies
```
to install the dependent tools for the environment

**3. Build source code**

Run the command
```
make build
```
to build the source code

**4. Install NNI to development environment**

Run the command
```
make dev-install
```
to install the distribution content to development environment, and create cli scripts

**5. Check if the environment is ready**

Now, you can try to start an experiment to check if your environment is ready
For example, run the command
```
nnictl create --config ~/nni/examples/trials/mnist/config.yml
```
And open WebUI to check if everything is OK

**6. Redeploy**

After you change some code, just use **step 4** to rebuild your code, then the change will take effect immediately

---
At last, wish you have a wonderful day.
For more contribution guidelines on making PR's or issues to NNI source code, you can refer to our [CONTRIBUTING](./docs/CONTRIBUTING.md) document. 