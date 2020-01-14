all: help

help:
	@echo ""
	@echo "-- Help Menu"
	@echo ""
	@echo "   1. make build            - build all images"
	@echo "   1. make push             - push all images"
	@echo "   3. make clean            - remove all images"
	@echo ""

build:
	@sudo docker build --tag=chunhochow/nvidia_l4t-ros:r32.2.1-melodic-ros-core   ros-core/.
	@sudo docker build --tag=chunhochow/nvidia_l4t-ros:r32.2.1-melodic-ros-base   ros-base/.
push:
	@sudo docker login
	@sudo docker push chunhochow/nvidia_l4t-ros:r32.2.1-melodic-ros-core
	@sudo docker push chunhochow/nvidia_l4t-ros:r32.2.1-melodic-ros-base
	@sudo docker logout
clean:
	@sudo docker rmi -f nvidia_l4t-ros:r32.2.1-melodic-ros-core
	@sudo docker rmi -f nvidia_l4t-ros:r32.2.1-melodic-ros-base
