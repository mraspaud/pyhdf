
.PHONY: build
build: hdfext.py hdfext_wrap.c

hdfext.py: hdfext.i
	swig -python hdfext.i

hdfext_wrap.c: hdfext.py
	# Already generated by swig. Do nothing.

.PHONY: clean
clean:
	rm -rf __pycache__ *.so *.pyc
