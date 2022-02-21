---
title: "GPG Key Update"
date: 2022-02-21T01:50:00-05:00
draft: false
---

Hello everyone! Writing this quick article to announce the rotation and subsequent retiring of my old GPG key to a new one! I'm doing this mainly because my key has grown rather large, and I'd like to transition my key from using a 4096-bit RSA key to a Ed25519 key, which should provide functionally the same amount of security (author of Ed25519 quotes it equivalent to ~3000 bit RSA key, but I do know that really isn't the best way to compare these two things :P )

So, with this announcement, I'd like to make the following points:
* My old key is not compromised, but will be revoked after making this announcement
* I will *not* use my old key to sign things, encrypt things, or authenticate with anything from this point onwards. If I do, something is terribly wrong.
* This new key has been cross signed by my old key, but I won't be cross signing my old key with my new one, since that seems to be a "can go either way" situation in this case, and I don't see the benefit as the key is being revoked regardless.

This is the information of the key that is being revoked:
```
pub   rsa4096 2020-09-29 [C]
      2BC5D27B47EE5632F97A668012FAE298AAD38D3D
uid           [ultimate] Ryan Schanzenbacher <ryan@rschanz.org>
uid           [ultimate] Ryan Schanzenbacher <rjs1877@rit.edu>
uid           [ultimate] Ryan Schanzenbacher <rschanzenbacher@stoicproductions.org>
uid           [ultimate] [jpeg image of size 3237]
sub   rsa4096 2020-09-29 [A] [expires: 2022-10-03]
sub   rsa4096 2020-09-29 [E] [expires: 2022-10-03]
sub   rsa4096 2020-09-29 [S] [expires: 2022-10-03]
```

And this is the information of my new key:
```
pub   ed25519 2022-02-21 [C]
      3E8745425417A3E388ACD906067DC3463E17741C
uid           [ultimate] Ryan Schanzenbacher <ryan@rschanz.org>
uid           [ultimate] [jpeg image of size 4437]
uid           [ultimate] Ryan Schanzenbacher <rjs1877@rit.edu>
uid           [ultimate] Ryan Schanzenbacher <rschanzenbacher@stoicproductions.org>
sub   ed25519 2022-02-21 [S] [expires: 2023-02-21]
sub   cv25519 2022-02-21 [E] [expires: 2023-02-21]
sub   ed25519 2022-02-21 [A] [expires: 2023-02-21]
```

I'd recommend to update your keychains if you happen to have my key, and the key hosted on the homepage of this website has been updated to reflect my new key.

[Here is the signed version of this message](/misc/gpg_key_rotation_signed.txt)

If you have any questions/comments/concerns, you can reach out to me at ryan@rschanz.org.

Thanks!
