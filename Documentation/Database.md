# Perencanaan Basis Data
---
## Revisi 0
| Code Revisi | Waktu | Pengembang |
|------------|-------|------------|
| SN-01 | 14 Juli 2018 09:27 | Herman Sugiharto|

### Daftar Tabel

#### 1. User

User adalah tabel untuk menyimpan data utama user, yang nantinya dapat digabungkan dan diolah bersama tabel - tabel lainnya.

| Atribut | Type |Keterangan|
|---------|------|----------|
| **id**  | Varchar (20)| `Primary Key`|
|  fname  | Varchar (20)|-|
|  lname  | Varchar (20)|-|
| name    | Varchar (40)|-|
|username | Varchar (20)|-|
|created_At| timestamp |-|
|verified_At| timestamp | `null`|

**keterangan** :
- **id** didapatkan dengan menggabungkan angka dan huruf dalam dua puluh karakter. pseudo for get id :


    function getId(){

        lastId = getLastID();
        lengthId = lastId.length;
        randomChar = 'a..z','A..Z','0..9';

        switch(lengthid){
            case <= 4 :
                        return random(randomChar, 4);
                        break
            case > 4 and <= 10 :
                        return random(randomChar, 10);
                        break
            case > 10 and <= 16 :
                        return random(randomChar, 16);
                        break
            case > 16 and <= 20 :
                        return random(randomChar, 20);
                        break
        }
    }

#### 2. User_Contact
User contact adalah tabel yang digunakan untuk menyimpan kontak user

| Atribut | Type | Keterangan |
|---------|------|------------|
|**id_user** | varchar (20) | `primary key, foreign key` |
|no_telepon | varchar (20) |`null`|
|email | varchar (20) |-|
|email_v| boolean |-|
|email_code| varchar(20) |- |

**keterangan** :
- email_v adalah adalah data apakah email pengguna sudah diverfikasi atau belum.
- email_code adalah code yang digunakan sebagai code verifikasi, pseudo code email_code :


    function email_code(){
        time = Time.New().Second();
        char = random('A..Z', 2);

        return char + time.to_str;
    }

#### 3. User_Network
Tabel ini akan digunakan untuk menyimpan social media lainnya dari user

| Attribut | Type | Keterangan |
|----------|------|------------|
| **id_user** | varchar (20) | `primary key, foreign key`|
|name | varchar (20) | - |
| user_link | varchar(50) | - |
| created_At | timestamp | - |
| update_At | timestamp | `null` |
