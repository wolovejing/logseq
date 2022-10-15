- ![](http://pic.1352.love/2022/10/20221007230748.png)
- 传递指针
	- ![Replaced by Image Uploader](http://pic.1352.love/2022/10/image_1665155385253_0.png)
	- ![Replaced by Image Uploader](http://pic.1352.love/2022/10/image_1665155445014_0.png)
- 结构体的值传递
	- ```C
	  #include <stdio.h>
	  #include<stdlib.h>
	  typedef struct Sqlist
	  {
	      int* elem;
	      int length;
	  }Sqlist;
	  
	  int Init_sqlist(Sqlist* pL){
	      printf("Init 函数中指针 pL中的地址%p\n",pL);
	      pL->elem = (int*)malloc(sizeof(int)*4);
	      if(!(pL->elem))
	      exit(-1); 
	      (*pL).length = 0;	
	      printf("Init函数中 结构体变量L->elem的地址%p\n",&(pL->elem));
	      printf("Init 函数中 结构体变量L->length的地址%p\n",&(pL->length));
	      
	      return 1;
	  }
	  
	  void modifyLength(Sqlist L){
	      L.length=100;
	  
	  }
	  void AdModifyLength(Sqlist* L){
	      L->length=100;
	  
	  }
	  int main(int argc, char const *argv[])
	  {
	      Sqlist L;
	      printf("主函数中 变量L的地址%p\n",&L);
	      printf("主函数中 结构体变量L->elem的地址%p\n",&(L.elem));
	      printf("主函数中 结构体变量L->elem的地址%p\n",&(L.length));
	      Init_sqlist(&L);
	      printf("主函数中 变量L的地址%p\n",&L);
	  
	      printf("%d\n",L.length);
	      modifyLength(L);
	      printf("%d\n",L.length);
	      AdModifyLength(&L);
	      printf("%d\n",L.length);
	      return 0;
	  }
	  .
	  ```