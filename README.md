We want to create a set of features representing the colors appearing in an image, Compute the histograms for each color channel, In the RGB color model, each color is the combination of three color channels (i.e., red, green, blue). In
turn, each channel can take on one of 256 values (represented by an integer between 0 and 255). For
example, the top-leftmost pixel in our image has the following channel values, A histogram is a representation of the distribution of values in data. Here is a simple example, In this example, we have some data with two 1s, two 2s, three 3s, one 4, and one 5. In the histogram,
each bar represents the number of times each value (1, 2, etc.) appears in our data.
We can apply this same technique to each of the color channels, but instead of five possible values, we
have 256 (the range of possible values for a channel value). The x-axis represents the 256 possible
channel values, and the y-axis represents the number of times a particular channel value appears across
all pixels in an image, As we can see in the histogram, barely any pixels contain the blue channel values between 0 and \~180,
while many pixels contain blue channel values between ~190 and ~210. This distribution of channel
values is shown for all three channels. The histogram, however, is not simply a visualization; it is 256
features for each color channel, making for 768 total features representing the distribution of colors in
an image.
