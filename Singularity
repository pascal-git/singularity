Bootstrap: docker
From: ubuntu:latest

%runscript

    echo "I can put here whatever I want to happen when the user runs my container!"
    #exec echo "Hello Monsoir Meatball" "$@"
    exec snakemake "$@"

%post

   echo "Here we are installing software and other dependencies for the container!"
   apt-get update
   apt-get install -y git python3 python3-pip
   mkdir /sw
   mkdir /pica
   mkdir /proj
   export LC_ALL=C
   pip3 install snakemake #
