# i3litebar

## Usage
### Update CONFIG_PATH/i3/config
* Make sure the binary is covered by the PATH environment variable.
* Activate i3litebar script by modify the i3 config file. 
```
bar {
    status_command i3litebar
    ...
}
```

### Add/remove/modify options
Check the `i3lb_refresh()` function in the bash script. The order of the entries reflects the order of the items on the bar.

### Add a new function
Create a function, add the logic, then call `i3_json_entry` to append a new object to the generated JSON (Check the existing functions for example of usage). For consistency, the prefix `i3lb_` is used for functions representing a bar option.

### Contribution
Feel free to contirbute
