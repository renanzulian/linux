# Questions

## Determine and configure hardware settings

1. Check hardware's information below:
- Audio device name that are running
- IRQ Number from Audio device
- How much devices are plugged in USB
- CPU Name
- Storage device name (tag)

2. Which is "snd" dependencies?

3. Insert the module "batman-adv", check if It was inserted all right and remove it.

4. Which is the advantages to use modprobe instead of insmod or rmmod?


## Answers

Question 1:
- `lspci | grep Audio`
- `lspci -v -s 00:1f.3` (Insert your id after the tag -s)
- `lsusb | wc -l`
- `cat /proc/cpuinfo | grep "model name"`
- `sudo fdisk -l` (or a ls in /dev)

Question 2:

`lsmod | grep snd`
"snd" is used by 22 another modules. They are snd_hda_codec_generic,snd_seq,snd_seq_device,snd_hda_codec_hdmi,snd_hwdep,snd_hda_intel,snd_hda_codec,snd_timer,snd_compress,snd_soc_core,snd_pcm.

Question 3:

Adding: `sudo modprobe batman-adv`

Checking: `lsmod | grep batman`

Removing: `sudo modprobe -r batman-adv`

Question 4:

The modprobe command provides all dependencies of the module that you want to insert. 