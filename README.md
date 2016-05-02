# playgroundOS manifest

playgroundOS is just a way for me to familiarize with seL4 kernel and what it has to offer. As I cannot seem to buid their RefOS because it is outdated at this moment I'll try to build something similar.

## Quick start

### Building playground OS

1. Make sure you read http://sel4.systems/Download/. Set up the environment (repo tool, cross compilers...etc) as per the instructions on the page. 

2. After this init and sync the repo
  > repo init -u https://github.com/atraari/playground-manifest -b master

  > repo sync

3. Make sure to install mkisofs. On Debian/Ubuntu you can do itlike this:
  > sudo apt-get install genisoimage

4. > make help (to list the configs)

5. > make menuconfig (to configure the build)

6. > make (to build)

7. And finally you can test it with a simulator with
  > make simulate-kzm
  or
  > make simulate-ia32
  or
  > simulate-ia32-graphics
