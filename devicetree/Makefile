
dtbs: 
	mkdir -p ./out &> /dev/null
	rm -R ./out/* &> /dev/null &
	wait

	cpp -nostdinc -I include -I ./  -undef -x assembler-with-cpp  sun50i-h5-redboxmini5.dts ./out/preprocessed
	dtc -I dts -O dtb -p 0x1000 ./out/preprocessed -o ./out/dtb

	mv ./out/dtb ./out/sun50i-h5-redboxmini5.dtb
	cp ./out/sun50i-h5-redboxmini5.dtb ../
