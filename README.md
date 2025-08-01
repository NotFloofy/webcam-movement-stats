# how this works

so every frame, the script takes a snapshot of the video pixels
then it looks at the previous frames pixels and does math on each pixel colour rgb values
it checks how much they changed by doing abs(current - previous) on r g and b and adds that up

if that total difference is bigger than some number (like 50) it counts that pixel as moved
and paints it red on the hidden canvas just so it knows which ones moved
