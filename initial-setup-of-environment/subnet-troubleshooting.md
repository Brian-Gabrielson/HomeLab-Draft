# Subnet Troubleshooting

I intialay used the same subnet for my homelab that was used for by tthe home router. This caused all kinds of problems on my homenet work. Often my DC would handout DHCP addresses to my home network devices, causing them to not connect to certain webpages.

It turns out my DC was on the WAN side and kali was on the LAN side. The oposite of what i thoughtt i had configured, this explains every problem i was having witth this. The subnet has been set to a 10.0.0.x subnet and the bridges have been configured for the corect sides.

<figure><img src="../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>
