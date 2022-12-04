# Cpp_Study
--------------------------------------------------------------------------------------
// std:: array(정적배열 대체)
#include <array>
#include <algorithm>

using namespac std;

int main()
{
   //int array[] {1, 2, 3, 4, 5}
   
   array<int, 5> my_arr = {1, 2, 3, 4, 5};
   my_arr = {0, 78, 88, 45, 40}
   
   cout << my_arr[10] << endl;
   cout << my_arr.at(10) << endl;
   cout << my_arr.size() << endl;
   
   sort(my_arr.begin(), my_arr.end());// algoritm의 정렬
   
   for (auto &element : my_arr)
    cout << element << " ";
   cout << endl;
   
   return 0;
}
---------------------------------------------------------------------------------------------
// std::vector(동적배열 대체)
#include <vector>

using namespace std;

int main()
{
  int *my_arr = new int[5];
  
  vector<int> arr = {1, 2, 3, 4, 5}
  
  arr.resize(10);
  
  for (auto &itr : arr)
    cout << itr << " ";
  cout << endl;
  
  cout << arr.size() << endl; // vector는 사이즈를 알아서 정한다.
  cout << arr[1] << endl;
  cout << arr.at(1) << endl;
  
  //delete[] my_arr // vector를 사용할 경우 delete가 자동 실행되어 필요 없음.
    
  return 0;
  
