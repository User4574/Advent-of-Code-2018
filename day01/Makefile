DAY = 01

.PHONY: run

run: build
	sudo docker run -it --rm aoc2018day$(DAY)

build:
	sudo docker build -t aoc2018day$(DAY) .
	touch build
