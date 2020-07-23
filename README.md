# LZW Compression in c++

Implemented LZW Compression Algorithm in C++. Takes input from stream and writes coded output in text mode.
Instructions to run:
1. Compile using the following command
	*g++ lzw.cpp -o lzw -O3*
2. Usage:
	*lzw [-max max_code] -c input output #compress file input to file output*
	*lzw [-max max_code] -c - output     #compress stdin to file otuput*
	*lzw [-max max_code] -c input        #compress file input to stdout*
	*lzw [-max max_code] -c              #compress stdin to stdout*
	*lzw [-max max_code] -d input output #decompress file input to file output*
	*lzw [-max max_code] -d - output     #decompress stdin to file otuput*
	*lzw [-max max_code] -d input        #decompress file input to stdout*
	*lzw [-max max_code] -d              #decompress stdin to stdout*
max_code denotes the maximum size of the dictionary used for compression and is by default set to 32767.

Check this [link](https://marknelson.us/posts/2011/11/08/lzw-revisited.html) for deatiled explanation on working of the algorithm.
