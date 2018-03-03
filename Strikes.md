## 🚩 What are strikes?
Strikes are points that users accumulate for misbehaving. Strikes are often represented by the triangular-flag emoji (🚩). Whenever a user receives strikes, they are sent a private message detailing the amount and reason for their strikes. When a user accumulates too many strikes, they are automatically punished according to the server's settings!

## 🚩 How do I set what punishments are given at different numbers of strikes?
Easy! Just use the `>>punishment` command. Here's the usage:
```
>>punishment <number> <action> [time]
```
This will cause the given action to be taken on a user when they reach the designated number of strikes. For example, if you want to ban people when they reach 3 strikes, you'd use:
```
>>punishment 3 ban
```
The available actions include **Ban**, **Softban**, **Kick**, **Mute**, and **None**. For Ban and Mute, you can also specify an amount of time. So, let's say that at 2 strikes you want to mute someone for 10 minutes; simply use:
```
>>punishment 2 mute 10 minutes
```

## 🚩 How do I give/take away strikes?
To manually give someone strikes, use the `>>strike` command. To remove strikes, use the `>>pardon` command. The usage for these commands is as follows:
```
>>strike [number of strikes] <users...> <reason>
>>pardon [number of strikes] <users...> <reason>
```
For example, to give 3 strikes to allthefoxes#9999, quikblend#0001, and Jake#0001 for being rude, you'd do:
```
>>strike 3 @allthefoxes#9999 @quikblend#0001 @Jake#0001 being rude
```
To pardon 2 of those strikes from Jake#0001 (let's say it was an accident), you'd do:
```
>>pardon 2 @Jake#0001 accident
```
To check a user's strikes, use the `>>check` command
```
>>check @Generic#5555
```


## 🚩 How do I make Vortex automatically give strikes?
Vortex automatically gives strikes via AutoMod. To have Vortex give strikes automatically for bad behavior, please check out the [[Auto-Moderation]] section.