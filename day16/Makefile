DAY = 16

.PHONY: run clean push

run: build
	docker run -it --rm aoc2018day$(DAY)

build: part* input
	docker build -t aoc2018day$(DAY) .
	touch build

clean:
	rm -f build

push: build
	docker tag aoc2018day$(DAY) advent.4574.co.uk/aoc2018day$(DAY)
	docker push advent.4574.co.uk/aoc2018day$(DAY)
