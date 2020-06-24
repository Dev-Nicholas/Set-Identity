# About:
This allows you to set the identity of the lua state to 6.

6/24/2020:
The code fully works. It does need to be updated every roblox update.

## Code:
```c++
void identity_thread(int rstate, int base_one, int base_two){
	*(DWORD*)(*(DWORD*)(rstate + base_one) + base_two) = 6;
}
```

## Usage:
```c++
// rl - Roblox Lua State
identity_thread(rl, 108, 24);
```

## Info:
You will need to update this every week. It does not auto update.
