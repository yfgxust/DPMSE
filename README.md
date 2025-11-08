 The running enviroment can be found in our paper.


In the c++ file named "test.cpp", the main code parts corresponding to DPMSE algorithm are as follows,

void source::NST_SET_PROCESSING(){
	...
}
In this function, "DUP" represents the test number, "cur_NST" represents current node state table corresponding to current test. For each test, DPMSE is mainly implemented by "source::NST_CONCORDANT_TABLE()" and "source::DYNAMIC_PROGRAMMING()".

void source::NST_CONCORDANT_TABLE(){
	...
}
This function is to calculate ITSCs and ITSDs.

int source::CONCORDNT_CALCULATING(igraph_matrix_t current_NST, int ROOT){
	...
}
This function is Fast ITSC algorithm.

void source::DYNAMIC_PROGRAMMING(){
	...
}
This function is DPMSE algorithm.
