#updated 12/14/22

Just a little ansible playbook to configure my laptop
I **couldn't** get the rpmfusion database to install, working on that, but in the meantime you can do the following
**prior** to running the playbook

    # sudo dnf install https://download1.rpmfusion.org/nonfree/fedora/rpmfusion-nonfree-release-$(rpm -E %fedora).noarch.rpm

    # sudo dnf update

Then its just a simple matter of grabbing the file in your choice of methods and running the playbook

    # ansible-playbook post_install.yml --ask-become-pass

