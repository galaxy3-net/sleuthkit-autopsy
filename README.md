# sleuthkit-autopsy

## Deploy

Deploy from the production version or development version based on the commands provided below.

This deployment currently only works on the UCIBOX (Trilogy Vagrant Machine).  Deployments to the Kali Linux boxes in the Galaxy3 lab or Azure lab are going to take more time to devlope.

### Production
sudo bash -c "$(curl -s https://raw.githubusercontent.com/galaxy3-net/sleuthkit-autopsy/main/Deploy)"

### Development
sudo bash -c "$(curl -s https://raw.githubusercontent.com/galaxy3-net/sleuthkit-autopsy/dev/Deploy)"


## Post Deployment

  To run autopsy (UCIBOX in Galaxy3):

    1.  sudo su -
    2.  source /etc/profile
    3.  cd /root/autopsy-4.17.0
    4.  sh ./unix_setup.sh
    5.  bin/autopsy
    6.  Yes - If window pops-up asking about enabling the main library.
    
  Note:  Autopsy & Sleuthkit files are written to /vagrant on Vagrant machines in order to conserve
         machine drive space.  If not a Vagrant machine, the files are in /root.