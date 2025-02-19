test: test_mux test_alu
	./test_mux
	./test_alu

test_mux: testbench_mux.v mux.v
	iverilog $^ -o $@

test_alu: testbench_alu.v alu.v
	iverilog $^ -o $@

clean:
	rm -f test_mux test_alu

help:
	@echo "  test_mux  - Run testbench for mux4"
	@echo "  test_alu  - Run testbench for alu"
	@echo "  clean 	   - Remove most generated files"
	@echo "  help  	   - Display this text"

.PHONY: clean test help
