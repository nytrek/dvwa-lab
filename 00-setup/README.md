# Lab setup

How I run DVWA locally. Fill in the versions and exact steps you used so this
is reproducible later.

## Stack

- Host: <your OS, e.g. CachyOS / Kali VM>
- DVWA: <version or commit>
- Runtime: <Docker / XAMPP / manual LAMP>

## Docker

The quickest way to get DVWA up:

```
docker run --rm -it -p 8080:80 ghcr.io/digininja/dvwa:latest
```

Then open `http://localhost:8080`, log in with the default `admin` / `password`,
and click **Create / Reset Database** on the setup page.

Set the security level under **DVWA Security** before each writeup. The level is
stored in the `security` cookie and the session, so it has to match the writeup
you're reproducing.

## Notes

- Default creds: `admin` / `password`
- The database has to be initialised once from the setup page or nothing works
- <anything specific to your setup: network mode, host entry, etc.>
