version=0.8.0

.PHONY: all

clean:
	@rm -Rf bin

build:
	@docker build -t abh1nav/exa:$(version) .

push:
	@docker push abh1nav/exa:$(version)

artifact: clean
	@mkdir bin
	@docker run -it --rm -v `pwd`/bin:/output abh1nav/exa:0.8.0
	@echo Copied binary into ./bin
