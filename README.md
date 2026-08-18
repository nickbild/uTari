# µTari

µTari (pronounced micro-Tari) is an Atari 2600, only smaller. 

An original 2600 PCB measures about 9.75 x 5.25 inches. The µTari PCB is 4.7 x 3.5 inches, making it roughly one-third the size of the original. All of the original chips (6507 CPU, TIA, RIOT) were used in making the µTari — it's the real deal, not an emulator or FPGA.

<table>
  <tr>
    <td><img src="https://raw.githubusercontent.com/nickbild/uTari/refs/heads/main/media/compare_sm.jpg" alt="Original Atari 2600 PCB compared with the smaller µTari PCB"></td>
  </tr>
  <tr>
    <td align="center"><em>Original Atari 2600 PCB (top) compared with the µTari PCB (bottom).</em></td>
  </tr>
</table>

**Check out the video on YouTube:**
<a href="https://www.youtube.com/watch?v=0-NlkX1Ed90">![](https://raw.githubusercontent.com/nickbild/uTari/refs/heads/main/media/teaser_play.jpg)</a>

## How

The Atari 2600 has large switches, as well as controller and cartridge ports, that are quite nice to have for a home console. I have replaced the large switches with tiny switches and buttons. The ports have been replaced with pin headers because my eventual plan is to turn this into a handheld, so I don't want ports on the main board.

Aside from that, I removed the RF modulator (which is normally at the bottom right of the 2600 PCB) and did a composite mod that replaces it with a single transistor and two resistors. That saves a fair amount of space and produces a cleaner signal that is compatible with more modern TVs. Empty spaces on the original PCB were also cut out. 

The remainder of the circuit is copied from the original Atari PCB. The 6507, TIA, and RIOT were transplanted to the new board. Since the rest of the components (mostly resistors, capacitors, transistors, and such) can still be purchased new, I used brand-new parts to leave the original board as intact as possible. All I would need to do is pop the chips back in the IC sockets for the 2600 to work again — no Ataris were harmed in the making of the µTari.

I started by breadboarding the circuit:

![](https://raw.githubusercontent.com/nickbild/uTari/refs/heads/main/media/breadboard_running_sm.jpg)

![](https://raw.githubusercontent.com/nickbild/uTari/refs/heads/main/media/breadboard_close_sm.jpg)

Once I was convinced it was working properly, I drew the circuit diagram in KiCad before laying out a PCB and having it manufactured:

![](https://raw.githubusercontent.com/nickbild/uTari/refs/heads/main/media/utari_sm.jpg)

It plays just like the real thing, because it is the real thing:

![](https://raw.githubusercontent.com/nickbild/uTari/refs/heads/main/media/utari_ready_sm.jpg)

![](https://raw.githubusercontent.com/nickbild/uTari/refs/heads/main/media/space_invaders_sm.jpg)

## About the Author

[Nick A. Bild, MS](https://nickbild79.firebaseapp.com/#!/)
