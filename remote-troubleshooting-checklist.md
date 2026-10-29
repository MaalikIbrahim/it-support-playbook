# Remote Troubleshooting Checklist

Work top to bottom before dispatching anyone. Record each result in the ticket.

## 1. Is it online?
- [ ] Last check-in time on the monitoring dashboard
- [ ] Cellular or Wi-Fi status on the gateway or SIM portal (signal, data session, recent usage)
- [ ] Any carrier or provider incident or maintenance during the same window?

## 2. Is it powered?
- [ ] Power events or reboots in the logs
- [ ] Ask the site if the unit is plugged in and the outlet has power (cleaning crews unplug things)

## 3. What does the device say?
- [ ] Current state (idle, in session, error, rebooting)
- [ ] Hardware status: sensors, cameras, peripherals detected vs expected
- [ ] Error messages and the time they started
- [ ] For USB devices: is the device listed (`ls /dev/...`, Device Manager)? "Cannot enable" errors point to cable, hub port or board

## 4. Try a safe remote recovery
- [ ] Restart the affected service or module
- [ ] Reboot the device (only when not mid-transaction)
- [ ] Reload the SIM / reset the data session if connectivity is the issue

## 5. Compare
- [ ] Do other devices on the same software version show the same issue?
- [ ] Has this device had the same fault before? Check its ticket history

## 6. Decide
- [ ] Fixed: verify with a test transaction, close with root cause
- [ ] Software suspected: escalate to engineering with steps 1 to 5 attached
- [ ] Hardware suspected: dispatch a vendor with the [dispatch template](vendor-dispatch-template.md)
