Solution link -- https://github.com/conda/conda/issues/8428

Solution options. 

Run in Powershell

`Get-ExecutionPolicy`

if it says `RemoteSigned`

then proceed to next step on line 17 below. 

If it says anything else, run this in admin mode

`set-executionpolicy remotesigned`

Then Run

`conda init powershell`

If your execution policy is already remotesigned, then just run

`conda init powershell`

This should resolve the problem. 

