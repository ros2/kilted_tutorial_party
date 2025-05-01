# ROS 2 Kilted Tutorial Party

Welcome! The purpose of this repository is to guide the testing of various functionalities of ROS 2 Kilted Kaiju prior to official release.
In other words, welcome to the Tutorial Party!

The tutorial party will run between May 1, 2025 and May 15, 2025 (inclusive).
Testing after that is welcome, but will not be included in the official statistics.

## Who can contribute?

Everyone, all contributions are welcome!

## How to contribute?

The [Issues](https://github.com/ros2/kilted_tutorial_party/issues) page has several tickets each containing specific instructions to test a particular functionality of ROS 2 Kilted Kaiju.
Each ticket will have the following sections:

1. **Setup**: Details on the desired hardware and software setup for this test. The following combinations are possible.
   1. RMW Implementation: `FASTDDS`, `CYCLONEDDS`, `CONNEXTDDS` or `ZENOH`
   2. BuildType:
      * `binary`: pre-built packaged ROS 2 workspace from [the releases page](https://github.com/ros2/ros2/releases/tag/release-kilted-beta-20250430)
      * `debian`: pre-built debian packages from the apt repository
      * `source`: building your own workspace from source
   3. Os: `Ubuntu Noble`, `Windows` and `RHEL-9`
   4. Chip: `Amd64` or `Arm64`
2. **Links**: Any relevant references for this test.
3. **Checks**: A list of functionalities to validate.

To contribute, first ensure if you have the relevant setup as described in the ticket.
If you don't have the setup, you can find the installation instructions at http://docs.ros.org/en/kilted/Installation.html.
Next, assign the ticket to yourself via the `Assignees` option or comment on the ticket indicating your interest.
Then follow the instructions to perform the necessary checks.

**All checks passed?**
Great! Please tick the checkboxes if you can or else leave a comment indicating your successful testing.
Attaching your terminal output (codeblock comment or gist file) as a form of verification is greatly appreciated.
If you have the necessary permission, go ahead and close the ticket by clicking `Close as completed`.

**Encountered failures?**
If one or more checks fail, please provide the error message in a codeblock comment or as a gist file attachment.

## What to prioritize?

The goal is to close all tickets after successful validation. But we would like to prioritize the following sets in order:

> **Note**: If you have access to a `Windows` machine, please prioritize testing on `Windows`. The next priority is `RHEL-9` followed by `Ubuntu Noble`.
- [ ] [Tutorials from docs.ros.org](https://github.com/ros2/kilted_tutorial_party/issues?q=is%3Aissue+is%3Aopen+label%3Adocs)
  - [ ] [Installation on various platforms](https://github.com/ros2/kilted_tutorial_party/issues?q=is%3Aissue+is%3Aopen+label%3Ainstallation+)
  - [ ] [Beginner CLI](https://github.com/ros2/kilted_tutorial_party/issues?q=is%3Aopen+label%3Adocs+label%3Abeginner-cli-tools+)
  - [ ] [Beginner Client Libraries](https://github.com/ros2/kilted_tutorial_party/issues?q=is%3Aopen+label%3Adocs+label%3Abeginner-client-libraries+)
  - [ ] [Intermediate](https://github.com/ros2/kilted_tutorial_party/issues?q=is%3Aopen+label%3Adocs+label%3Aintermediate+)
  - [ ] [Advanced](https://github.com/ros2/kilted_tutorial_party/issues?q=is%3Aopen+label%3Adocs+label%3Aadvanced+)
- [ ] [Core functionality](https://github.com/ros2/kilted_tutorial_party/labels/core)
  - [ ] [noble, debian](https://github.com/ros2/kilted_tutorial_party/issues?q=is%3Aissue+is%3Aopen+label%3Acore+label%3A%22OS%3A+Ubuntu+Noble+24.04%22+label%3A%22Build+type%3A+Debian%22)
  - [ ] [noble, binary](https://github.com/ros2/kilted_tutorial_party/issues?q=is%3Aissue+is%3Aopen+label%3Acore+label%3A%22OS%3A+Ubuntu+Noble+24.04%22+label%3A%22Build+type%3A+Binary%22+)
  - [ ] [windows, binary](https://github.com/ros2/kilted_tutorial_party/issues?q=is%3Aissue+is%3Aopen+label%3Acore+label%3A%22Build+type%3A+Binary%22+label%3A%22OS%3A+Windows%22+)
  - [ ] [windows, source](https://github.com/ros2/kilted_tutorial_party/issues?q=is%3Aissue+is%3Aopen+label%3Acore+label%3A%22Build+type%3A+Source%22+label%3A%22OS%3A+Windows%22+)
  - [ ] [rhel, source](https://github.com/ros2/kilted_tutorial_party/issues?q=is%3Aissue+is%3Aopen+label%3Acore+label%3A%22Build+type%3A+Source%22+label%3A%22OS%3A+RHEL+9%22+)
- [ ] [Features](https://github.com/ros2/kilted_tutorial_party/issues?q=is%3Aissue+is%3Aopen+label%3Afeature+)
  - [ ] [noble](https://github.com/ros2/kilted_tutorial_party/issues?q=is%3Aissue+is%3Aopen+label%3Afeature+label%3A%22OS%3A+Ubuntu+Noble+24.04%22++)
  - [ ] [windows](https://github.com/ros2/kilted_tutorial_party/issues?q=is%3Aissue+is%3Aopen+label%3Afeature+label%3A%22OS%3A+Windows%22+)

## What if I want to test something else?

If you would like to test the functionality of any other package or extend the capabilities tested above, please open additional tickets while following the format described above.

## Questions

Questions related to testing may be posted on the [Discussions](https://github.com/ros2/kilted_tutorial_party/discussions) board.
Kindly ensure to link the relevant issue ticket when starting a new discussion.
