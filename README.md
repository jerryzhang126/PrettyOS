<p align="center">
  <img src="logo.png">
</p>
<p align="center">
  <b>A Preemptive dynamic priority based hard real time kernel for embedded devices</b>.
</p>

#### ☑ List of supported Features

| Features      | Status        |
| ------------- |:-------------:|
| Preemptive Multitasking      | **Yes** |
| Maximum number of tasks      | Configurable     |
| Number of tasks at each priority level | 1      |
| Priority Change at run time | **Yes** |
| Support Round robin scheduling | No |
| Scheduling lock/Unlock | **Yes** |
|Task suspend/resume| **Yes** |
|Catch a task that returns| **Yes** |
|Semaphores| **Yes** |
| Mutual exclusion semaphores | No |
|Software timers| No|
| User definable hook functions | No |
| Message mailboxes | No |

#### 📜 List of PrettyOS Public APIs
| Core          | Task managment		| Semaphore 			| Time			| Hook Functions |
| ------------- |:---------------------:|:---------------------:|:-------------:|:--------------:|
|OS_Init		|OS_TaskCreate			|OS_SemCreate			|OS_DelayTicks	|OS_Hook_onIdle  |
|OS_Run			|OS_TaskDelete			|OS_SemPend				|OS_TimerTick	| 				 |
|OS_IntEnter    |OS_TaskChangePriority	|OS_SemPost				|OS_DelayTime	| 				 |
|OS_IntExit		|OS_TaskSuspend			|OS_SemPendNonBlocking	|				| 				 |
|OS_SchedLock	|OS_TaskResume			|OS_SemPendAbort		|				| 				 |
|OS_SchedUnlock	|OS_TaskStatus			|						|				|				 |

#### 💻 Porting availability
| System      			| BSP        	| CPU port 		|
| ----------------------|:-------------:|:-------------:|
| TI stellaris LM4F120 	| Done 			| Done 			|

#### 📝 License
Copyright © 2020 - present, Yahia Farghaly Ashour.<br>
This project is [MIT](https://github.com/yahiafarghaly/PrettyOS/blob/master/LICENSE) Licensed.