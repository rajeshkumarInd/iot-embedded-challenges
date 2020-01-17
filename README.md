# IoT Embedded Challenge

## Instructions
To take the challenge:

- Fork this repository
- In your own copy, implement the tasks outlined bellow.
- The challenge is considered "done" when:
  - The code/pseudo-code for a task has been written.
  - The documentation describes the approach taken to address a specific task.
  - This README has been updated to reflect the relevant information about the repo.
  
### Duration
We only expect candidates to spend about 4-6 hours on the challenge.

### Hints for success
- Organize your solutions logically, either by commits or even by branches. This makes it easier to see your process.
- Commit often, and use descriptive commit messages. Each commit should be easily summarized in a short phrase.
- Do not try to solve all of the tasks at once. Tackle each task on its own.
- If you get stuck on an task, or cannot easily satisfy all of the "done" criteria, move on to the next one. The open tasks can be discussed at your technical interview.

## The Challenge
Create an application that will keep room temperature between configured levels.
The application will monitor temperature sensors, actuate a valve to keep the room temperature between the desired range.
The range is configured from an external interface.
The application should report the temperature data and valve control event to an external interface.

*Notes*
- The physical external interface type is not relevant - this can be abstracted.
- The valve control and sensor reading logic is not relevant - those can be empty functions.
- The challenge is focused on the code organization, structure and high level approach to solve it.
- It's not required that the final solution builds successfully - but it's a BONUS if it does.

### Code Structure
- The solution is expected to be based on FreeRTOS
- Architecture is ARM Cortex-M4 (choose any MCU based on that architecture if you want to include its SDK libraries)
- Project build process management is preferable CMake
- Include all the 3rdparty libraries that you will use, e.g. FreeRTOS, etc..
- The toolchain is GCC v9.2.1

### Tasks
- Sample temperature data at a fixed interval period
- Process the temperature measurements
- Actuate the temperature valve to keep temperature within defined range
- Handle incoming temperature range configuration messages
- Send temperature messages through the external interface
