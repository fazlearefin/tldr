# halt

> Hentikan seluruh proses dan jalannya CPU dalam sistem komputer.
> Informasi lebih lanjut: <https://manned.org/halt.8>.

- Hentikan sistem komputer:

`halt`

- Matikan sistem (sama seperti `poweroff`):

`halt {{[-p|--poweroff]}}`

- Nyalakan ulang sistem (sama seperti `reboot`):

`halt --reboot`

- Hentikan sistem secara segera tanpa menghubungi manajer sistem:

`halt {{[-f|--force]}}`

- Tulis entri wtmp shutdown tanpa menghentikan sistem:

`halt {{[-w|--wtmp-only]}}`
