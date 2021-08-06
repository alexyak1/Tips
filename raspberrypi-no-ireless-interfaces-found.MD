# No wireless interfaces found

### Check if wifi locked by hardware or software
`rfkill list all`
### Allow wifi 
`sudo rfkill unblock wifi`

## If still have an issue 
`sudo dhcpcd -4`
