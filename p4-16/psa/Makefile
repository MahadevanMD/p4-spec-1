
SPEC=PSA

all: build/${SPEC}.pdf

build/${SPEC}.pdf: ${SPEC}.mdk
	madoko --pdf -vv --odir=build $<

build/${SPEC}.pdf: p4.json
build/${SPEC}.pdf: psa.p4

clean:
	${RM} -rf build

P4C=p4test

check:
	${P4C} examples/psa-example-counters.p4
