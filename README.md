# CT (Comamnd & Troll)

## About
CT is a command and control server that acts like a normal C2 server but is mainly for trolling purposes. Commanders will be able to connect to the C2 server and control any hosts that have connected back to the C2 server. CT will prob not do any AV evasion so this will only work if all AVs are turned off. CT will also only support infecting Windows clients

## How it works
For CT to work it needs to infect hosts. We will get this to happen by having hosts download and execute a program. All this program will do is connect back to the CT server. After the connection has been established CT will send the clients the current [modules](#modules) it has. Commanders can login to CT and execute whatever modules they want on the infected hosts 

![diagram](https://github.com/BeastieNate5/CT/blob/main/assets/diagram.jpeg?raw=true)

## Modules
CT will be built around modules. Modules are custom scripts that preform a action on the client. For example we could have a process opener module that allows commanders to open process on infected hosts. Modules will most likely be C programs that will be converted into indepedent shellcode then sent to the infected hosts
