# Greb Floog
**Category:** forensic <br>
**Point:** 50

> Akan terdapat flag dalam aliran service berikut. Tangkap flagnya dengan format COMPFEST11{<string>}
> 
> nc 18.136.167.108 18018

---

Sudah diberikan clue dengan jelas pada judul dan deskpripsi bahwa kita diminta untuk menangkap flag dari stream yang datang ketika kita melakukan _netcatting_ ke remote host yang sudah disediakan. Untuk itu saya menggunakan perintah sebagai berikut :

```bash
nc 18.136.167.108 18018 | grep COMPFEST11
```

exploit : [script.sh](./script.sh)

flag : `COMPFEST11{grab_or_grep_0fa15c8fcc6d91096de46bfe812215fa}`