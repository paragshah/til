# Sleep Log

View the sleep/awake log of your machine.

Run this in terminal under any folder you want to serve:
```
pmset -g log|grep -e " Sleep  " -e " Wake  "
```

Create an alias in your bash profile:
```
alias sleeplog='clear;printf "\n";pmset -g log|grep -e " Sleep  " -e " Wake  ";printf "\n"'
```

Then using terminal, enter `sleeplog` to output the sleep/awake log of your machine. The output will look like:
```
2016-02-11 00:30:54 -0800 Sleep                 Entering Sleep state due to 'Maintenance Sleep': Using AC 6446 secs
2016-02-11 02:19:05 -0800 Sleep                 Entering Sleep state due to 'Maintenance Sleep': Using AC 6445 secs
2016-02-11 04:07:15 -0800 Sleep                 Entering Sleep state due to 'Maintenance Sleep': Using AC 6445 secs
2016-02-11 05:55:25 -0800 Sleep                 Entering Sleep state due to 'Maintenance Sleep': Using AC 6445 secs
2016-02-11 07:43:35 -0800 Sleep                 Entering Sleep state due to 'Maintenance Sleep': Using AC 6445 secs
2016-02-11 09:31:45 -0800 Sleep                 Entering Sleep state due to 'Maintenance Sleep': Using AC 6445 secs
2016-02-11 11:19:55 -0800 Sleep                 Entering Sleep state due to 'Maintenance Sleep': Using AC 6446 secs
2016-02-11 13:08:06 -0800 Sleep                 Entering Sleep state due to 'Maintenance Sleep': Using AC 6446 secs
2016-02-11 14:56:17 -0800 Sleep                 Entering Sleep state due to 'Maintenance Sleep': Using AC 6446 secs
2016-02-11 16:44:28 -0800 Sleep                 Entering Sleep state due to 'Maintenance Sleep': Using AC 6446 secs
2016-02-11 18:32:39 -0800 Sleep                 Entering Sleep state due to 'Maintenance Sleep': Using AC 6445 secs
2016-02-11 20:20:49 -0800 Sleep                 Entering Sleep state due to 'Maintenance Sleep': Using AC 64 secs
2016-02-11 20:21:53 -0800 Wake                  Wake [CDNVA] due to EHC2/HID Activity: Using AC
2016-02-11 22:14:14 -0800 Sleep                 Entering Sleep state due to 'Software Sleep pid=113': Using AC 3660 secs
2016-02-11 23:15:59 -0800 Sleep                 Entering Sleep state due to 'Maintenance Sleep': Using AC 6446 secs
2016-02-12 01:04:10 -0800 Sleep                 Entering Sleep state due to 'Maintenance Sleep': Using AC 6445 secs
2016-02-12 02:52:20 -0800 Sleep                 Entering Sleep state due to 'Maintenance Sleep': Using AC 6445 secs
2016-02-12 04:40:30 -0800 Sleep                 Entering Sleep state due to 'Maintenance Sleep': Using AC 6446 secs
2016-02-12 06:28:41 -0800 Sleep                 Entering Sleep state due to 'Maintenance Sleep': Using AC 6446 secs
2016-02-12 08:16:52 -0800 Sleep                 Entering Sleep state due to 'Maintenance Sleep': Using AC 4955 secs
2016-02-12 09:39:27 -0800 Wake                  Wake [CDNVA] due to EHC2/HID Activity: Using AC 6043 secs
2016-02-12 11:20:10 -0800 Sleep                 Entering Sleep state due to 'Software Sleep pid=113': Using AC 4288 secs
2016-02-12 12:32:23 -0800 Sleep                 Entering Sleep state due to 'Maintenance Sleep': Using AC 6445 secs
2016-02-12 14:20:33 -0800 Sleep                 Entering Sleep state due to 'Maintenance Sleep': Using AC 1567 secs
2016-02-12 14:46:40 -0800 Wake                  Wake [CDNVA] due to EHC2/HID Activity: Using AC
```

