all: matrix_tests

include ../Makedefs

OBJS = gslMatrixUtils.o Matrices.o exceptions.o\
       main.o


# targets
matrix_tests: $(OBJS)
	@echo "--- matrix_tests ---"
	$(CXX) $(CFLAGS) $(LFLAGS) -o matrix_tests $(OBJS) $(LIBS)

clean:
	@echo "cleaning up.."
	rm -f matrix_tests core

clobber: clean
	rm -f *.o *~ $(COMMON)/*.o $(COMMON)/*~ *.out

depend:
	@echo "Updating dependancies..."
	makedepend -m -Y. -- $(CFLAGS) -- *.C *.h $(COMMON)/*.C $(COMMON)/*.h
#	makedepend -m -Y. -f.depend -- $(CFLAGS) -- *.C	

# DO NOT DELETE
