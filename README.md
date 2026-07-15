# lvm_dr20_binderhub

# Instructions


Access to the BinderHub, following the instructions in here:

https://github.com/andycasey/sdss-binder

Remember that you need a *@gmail.com account to access it.


Once you have access the BinderHub, you will need to:

# Install the required packages: ipyml, gdown & rsync

Open a terminal and run the following commands

pip install --user --upgrade ipympl

python -m pip install --user gdown

conda create \
  --override-channels \
  -p "$HOME/.conda/envs/rsync" \
  -c conda-forge \
  rsync
  
  

echo 'export PATH="$HOME/.local/bin:$HOME/.conda/envs/rsync/bin/:$PATH"' >> ~/.bashrc

source .bashrc

# Clone the following repository
git clone https://github.com/sfsanchez72/lvm_dr20_binderhub

# Run the following script in the terminal

python create_netrc.py

within the lvm_dr20_binderhub



# Now you can proceed with the different notebooks


