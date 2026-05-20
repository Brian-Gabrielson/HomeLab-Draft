# Setup Github, Gitlab & Gitbook









Create a shell project in Gitlab to push changes to



Below are the token settings in Gitlab

<figure><img src=".gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>









First run did not work, the specific tool used in the first attempt did not want to use tokens, only ssh.

<figure><img src=".gitbook/assets/image (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

Chose a new tool that will accept username and password, allowing me to use the token i generated earlier.

<figure><img src=".gitbook/assets/image (3) (1) (1).png" alt=""><figcaption></figcaption></figure>

The sync action contacted Gitlab but the main branch is protected.

<figure><img src=".gitbook/assets/image (4) (1) (1).png" alt=""><figcaption></figcaption></figure>

Toggled on 'Allowed to force push'

<figure><img src=".gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

Success! The action completed without any hangups.

<figure><img src=".gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

Content was successfully mirrored from Github to Gitlab

<figure><img src=".gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>
