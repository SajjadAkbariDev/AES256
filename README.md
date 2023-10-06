
# Android AES256 Encrypt & Decrypt

this is a easy tool for (AES 256) Encrypt and Decrypt in android.


## Documentation
 only need add this maven repository:

- delete _SPACE_ in password line in below code:

        maven {
            url uri("https://maven.pkg.github.com/SajjadAkbariDev/AndroidAES256")
            credentials {
                username = "SajjadAkbariDev"
                password = "ghp_1RmhPU1rOaz8U1j_SPACE_uhPiAxtlXeaYbkj3MeiBm"
            }
        }

 and a implement:

     implementation("sajjad.akbari:aes256:1.0")


## Demo

import sajjad.akbari.AES256
.
.
.

        val text = "this is a text or String."
        val aes = AES256("password11", 256, "password22")

        val data: String = aes.encrypt(text)
        Toast.makeText(applicationContext, ""+data, Toast.LENGTH_SHORT).show()

        val plainText: String = aes.decrypt(data)
        Toast.makeText(applicationContext, ""+plainText, Toast.LENGTH_SHORT).show()

## Authors

- [@SajjadAkbariDev](https://github.com/SajjadAkbariDev)


## Support

For support, email sajjad.akbari.dev@outlook.com

Telegram: https://t.me/UnlimitL
