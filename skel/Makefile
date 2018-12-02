DAY = 

.PHONY: run clean

run: build
	sudo docker run -it --rm aoc2018day$(DAY)

build: part* input
	sudo docker build -t aoc2018day$(DAY) .
	touch build

clean:
	rm -f build
