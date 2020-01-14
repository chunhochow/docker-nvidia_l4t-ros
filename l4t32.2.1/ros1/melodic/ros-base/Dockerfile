FROM chunhochow/nvidia_l4t-ros:r32.2.1-melodic-ros-core

# install ros packages
RUN apt-get update && apt-get install -y \
    ros-melodic-ros-base=1.4.1-0* \
    && rm -rf /var/lib/apt/lists/*

