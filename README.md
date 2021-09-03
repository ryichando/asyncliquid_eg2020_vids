# How To Compile This Demo

- Get a copy of Docker running (https://www.docker.com)

- Clone this repository and move into it

        git clone https://github.com/ryichando/asyncliquid_eg2020_vids.git
        mv asyncliquid_eg2020_vids

- Install [Veddy](https://github.com/ryichando/veddy) (skip if you already have it)

        git clone https://github.com/ryichando/veddy.git
        docker build ./veddy -t veddy

- Run the compilation

        docker run -v $PWD/veddy:/veddy -v $PWD:/mount \
        --rm veddy pass_1.xml pass_2.xml

- That's it! `main.mp4` should be there
