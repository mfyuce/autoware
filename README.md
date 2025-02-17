# Autoware - the world's leading open-source software project for autonomous driving

![Autoware_RViz](https://user-images.githubusercontent.com/63835446/158918717-58d6deaf-93fb-47f9-891d-e242b02cba7b.png)

<!--- Contributors -->
<p align="center">
    <a href="https://github.com/autowarefoundation/autoware.universe/graphs/contributors">
        <img src="https://img.shields.io/github/contributors/autowarefoundation/autoware.universe?style=flat&label=Autoware%20Universe%20Contributors"
            alt="Autoware Universe Contributors" /></a>
    <a href="https://github.com/autowarefoundation/autoware/graphs/contributors">
        <img src="https://img.shields.io/github/contributors/autowarefoundation/autoware?style=flat&label=Autoware%20Contributors"
            alt="Autoware Contributors" /></a>
</p>

<!--- Commit Activity -->
<p align="center">
    <a href="https://github.com/autowarefoundation/autoware.universe/pulse">
        <img src="https://img.shields.io/github/commit-activity/m/autowarefoundation/autoware.universe?style=flat&label=Autoware%20Universe%20Commit%20Activity"
            alt="Autoware Universe Activity" /></a>
    <a href="https://github.com/autowarefoundation/autoware/pulse">
        <img src="https://img.shields.io/github/commit-activity/m/autowarefoundation/autoware?style=flat&label=Autoware%20Commit%20Activity"
            alt="Autoware Activity" /></a>
</p>

<!--- License -->
<p align="center">
    <a href="https://github.com/autowarefoundation/autoware/blob/main/LICENSE">
        <img src="https://img.shields.io/github/license/autowarefoundation/autoware?style=flat&label=License"
            alt="License" /></a>
</p>

<!--- CI Reports -->
<p align="center">
    <a href="https://github.com/autowarefoundation/autoware/actions/workflows/health-check.yaml?query=branch%3Amain">
        <img src="https://img.shields.io/github/actions/workflow/status/autowarefoundation/autoware/health-check.yaml?style=flat&label=health-check"
            alt="health-check CI" /></a>
    <a href="https://app.codecov.io/gh/autowarefoundation/autoware.universe">
        <img src="https://img.shields.io/codecov/c/gh/autowarefoundation/autoware.universe?style=flat&label=Coverage&logo=codecov&logoColor=white"
            alt="Code Coverage" /></a>
</p>

<!--- Social Media -->
<p align="center">
    <a href="https://discord.gg/Q94UsPvReQ">
        <img src="https://img.shields.io/discord/953808765935816715?logo=discord&logoColor=white&style=flat&label=Autoware%20Discord"
            alt="Autoware Discord"></a>
    <a href="https://twitter.com/intent/follow?screen_name=AutowareFdn">
        <img src="https://img.shields.io/twitter/follow/AutowareFdn?logo=x&logoColor=white&style=flat"
            alt="Autoware Twitter / X"></a>
    <a href="https://www.linkedin.com/company/the-autoware-foundation/">
        <img src="https://img.shields.io/badge/Linkedin-Autoware%20Foundation-0a66c2?logo=linkedin&logoColor=white&style=flat"
            alt="Autoware Linkedin"></a>
</p>

Autoware is an open-source software stack for self-driving vehicles, built on the [Robot Operating System (ROS)](https://www.ros.org/). It includes all of the necessary functions to drive an autonomous vehicles from localization and object detection to route planning and control, and was created with the aim of enabling as many individuals and organizations as possible to contribute to open innovations in autonomous driving technology.

![Autoware architecture](https://static.wixstatic.com/media/984e93_552e338be28543c7949717053cc3f11f~mv2.png/v1/crop/x_0,y_1,w_1500,h_879/fill/w_863,h_506,al_c,usm_0.66_1.00_0.01,enc_auto/Autoware-GFX_edited.png)

## Documentation

To learn more about using or developing Autoware, refer to the [Autoware documentation site](https://autowarefoundation.github.io/autoware-documentation/main/). You can find the source for the documentation in [autowarefoundation/autoware-documentation](https://github.com/autowarefoundation/autoware-documentation).

## Repository overview

- [autowarefoundation/autoware](https://github.com/autowarefoundation/autoware)
  - Meta-repository containing `.repos` files to construct an Autoware workspace.
  - It is anticipated that this repository will be frequently forked by users, and so it contains minimal information to avoid unnecessary differences.
- [autowarefoundation/autoware_common](https://github.com/autowarefoundation/autoware_common)
  - Library/utility type repository containing commonly referenced ROS packages.
  - These packages were moved to a separate repository in order to reduce CI execution time
- [autowarefoundation/autoware.core](https://github.com/autowarefoundation/autoware.core)
  - Main repository for high-quality, stable ROS packages for Autonomous Driving.
  - Based on [Autoware.Auto](https://gitlab.com/autowarefoundation/autoware.auto/AutowareAuto) and [Autoware.Universe](https://github.com/autowarefoundation/autoware.universe).
- [autowarefoundation/autoware.universe](https://github.com/autowarefoundation/autoware.universe)
  - Repository for experimental, cutting-edge ROS packages for Autonomous Driving.
  - Autoware Universe was created to make it easier for researchers and developers to extend the functionality of Autoware Core
- [autowarefoundation/autoware_launch](https://github.com/autowarefoundation/autoware_launch)
  - Launch configuration repository containing node configurations and their parameters.
- [autowarefoundation/autoware-github-actions](https://github.com/autowarefoundation/autoware-github-actions)
  - Contains [reusable GitHub Actions workflows](https://docs.github.com/ja/actions/learn-github-actions/reusing-workflows) used by multiple repositories for CI.
  - Utilizes the [DRY](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself) concept.
- [autowarefoundation/autoware-documentation](https://github.com/autowarefoundation/autoware-documentation)
  - Documentation repository for Autoware users and developers.
  - Since Autoware Core/Universe has multiple repositories, a central documentation repository is important to make information accessible from a single place.

## Using Autoware.AI

If you wish to use Autoware.AI, the previous version of Autoware based on ROS 1, switch to [autoware-ai](https://github.com/autowarefoundation/autoware_ai) repository. However, be aware that Autoware.AI has reached the end-of-life as of 2022, and we strongly recommend transitioning to Autoware Core/Universe for future use.

## Contributing

- [There is no formal process to become a contributor](https://github.com/autowarefoundation/autoware-projects/wiki#contributors) - you can comment on any [existing issues](https://github.com/autowarefoundation/autoware.universe/issues) or make a pull request on any Autoware repository!
  - Make sure to follow the [Contribution Guidelines](https://autowarefoundation.github.io/autoware-documentation/main/contributing/).
  - Take a look at Autoware's [various working groups](https://github.com/autowarefoundation/autoware-projects/wiki#working-group-list) to gain an understanding of any work in progress and to see how projects are managed.
- If you have any technical questions, you can start a discussion in the [Q&A category](https://github.com/autowarefoundation/autoware/discussions/categories/q-a) to request help and confirm if a potential issue is a bug or not.

## Useful resources

- [Autoware Foundation homepage](https://www.autoware.org/)
- [Support guidelines](https://autowarefoundation.github.io/autoware-documentation/main/support/support-guidelines/)
- [CI metrics](https://autowarefoundation.github.io/autoware-ci-metrics/)



# Local tries

source /opt/ros/humble/setup.bash
vcs import src < autoware.repos
vcs pull src
colcon build --packages-up-to autoware_v2x --symlink-install --cmake-args -DCMAKE_BUILD_TYPE=Release
colcon build  --symlink-install --cmake-args -DCMAKE_BUILD_TYPE=Release
rocker -e LIBGL_ALWAYS_SOFTWARE=1 --x11 --user --privileged --volume $HOME/workspace/autoware_docker --volume $HOME/data -- ghcr.io/autowarefoundation/autoware:humble-2024.01-cuda-amd64
rocker -e LIBGL_ALWAYS_SOFTWARE=1 --x11 --user --privileged --volume $HOME/workspace/autoware_docker --volume $HOME/data -- ghcr.io/autowarefoundation/autoware:humble-2024.01-cuda-amd64
docker pull ghcr.io/autowarefoundation/autoware:humble-2024.01-cuda-amd64
https://github.com/autowarefoundation/autoware/pkgs/container/autoware/246009897?tag=humble-2024.01-cuda-amd64
https://github.com/orgs/autowarefoundation/discussions/4990


./docker/run.sh --map-path $HOME/data/map/sample-map-rosbag ros2 launch autoware_launch planning_simulator.launch.xml map_path:=/autoware_map vehicle_model:=sample_vehicle sensor_model:=sample_sensor_kit




# Running first tests 

rocker --nvidia --x11 --user --privileged --volume /home/fatihyuce/workspace/autoware_docker --volume /home/fatihyuce/data --network=v2x_net --name autoware_1 --oyr-run-arg "--ip 10.0.0.2 --hostname autoware_1" -- ghcr.io/autowarefoundation/autoware:universe-cuda
rocker --nvidia --x11 --user --privileged --volume /home/fatihyuce/workspace/autoware_docker --volume /home/fatihyuce/data --network=v2x_net --name autoware_2 --oyr-run-arg "--ip 10.0.0.3 --hostname autoware_2" -- ghcr.io/autowarefoundation/autoware:universe-cuda




cd /home/fatihyuce/workspace/autoware_docker/


source /home/fatihyuce/workspace/autoware_docker/src/v2x/autowarev2x/setup.sh

ros2 launch autoware_launch planning_simulator.launch.xml map_path:=/home/fatihyuce/data/maps/sample-map-planning vehicle_model:=sample_vehicle sensor_model:=sample_sensor_kit

# Running simulations

rocker --nvidia --x11 --user --volume /home/fatihyuce/workspace/autoware_docker --volume /home/fatihyuce/workspace/data -- ghcr.io/autowarefoundation/autoware:universe-cuda


sudo apt update
rosdep update
rosdep install --from-paths src --ignore-src --rosdistro humble -r -y


source install/setup.bash
ros2 launch scenario_test_runner scenario_test_runner.launch.py map_path:=/home/fatihyuce/data/maps/sample-map-planning sensor_model:=sample_sensor_kit vehicle_model:=sample_vehicle scenario:=/home/fatihyuce/data/scenarios/busy_kashiwa_scenario.yaml launch_autoware:=true

