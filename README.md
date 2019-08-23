This is a clone of MaMe82's Python port of infamous hak5 DuckEncoder


      _      _      _      USB       _      _      _
   __(.)< __(.)> __(.)=   Rubber   >(.)__ <(.)__ =(.)__
   \___)  \___)  \___)    Ducky!    (___/  (___/  (___/ 

The USB Rubber Ducky is a Human Interface Device programmable with a simple scripting language allowing penetration testers to quickly and easily craft and deploy security auditing payloads that mimic human keyboard input. The source is written in C and requires the AVR Studio 5 IDE from atmel.com/avrstudio. Hardware is commercially available at hakshop.com. Tools and payloads can be found at usbrubberducky.com. Quack!

Usage

    Duckencoder python port 1.0 by MaMe82
    =====================================
    
    Creds to:	hak5Darren for original duckencoder
    		https://github.com/hak5darren/USB-Rubber-Ducky
    
    Converts payload created by DuckEncoder to sourcefile for DigiSpark Sketch
    
    Usage: python duckencoder.py -i [file ..]			        Encode DuckyScript source given by -i file
       or: python duckencoder.py -i [file ..] -o [outfile ..]	Encode DuckyScript source to outputfile given by -o
    
    Arguments:
       -i [file ..]      	Input file in DuckyScript format
       -o [file ..] 	    Output File for encoded payload, defaults to inject.bin
       -l <layout name>	    Keyboard Layout (us/fr/pt/de ...)
       -p, --pastthru	    Read script from stdin and print result on stdout (ignore -i, -o)
       -r, --rawpassthru    Like passthru, but input is read as STRING instead of duckyscript
       -h			        Print this help screen
