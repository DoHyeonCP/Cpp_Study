# Cpp_Study

// 여러가지 생성자들과 형변환
int main()
{
  std::vector<char> vec;
  for (auto e : "Today is good day.")
    vec.push_back(e);
  
  std::string second_string(vec.begin(), std::find(vec.begin(), vec.end(), 'y'));
  
  std::cout << second_string  << std::endl; //toda
  
  return 0;
}

int main2()
{
  std::string my_str(std:to_string(1234)); //to_string 문자로 바꿔준다.
  
  float f =  std::stof(my_str); // sto?는 형변환 해줌
  
  std::cout << my_str << std::endl;
  std::cout << f << << std::endl;
  
  return 0;
}

//길이와 용량
int main()
{
  string my_str("01234567");
  my_str.reserve(1000); // capacity가 1007이 된다.
  
  return 0;
}

// 대입, 덧붙이기
int main()
{
  string str1("one");
  
  string str2;
  str2 = str1;
  str2 = "two";
  str2.assign("two").append("three"); 
  str2 += "four";
  str2 = str2 + "five";
  str2.push_back('S');
  cout << str2 << endl;
  
  retur 0;
}

// 교환
int main()
{
  string str1("one");
  string str2("two");
  
  cout << str1 << " "  << str2 << endl;
  
  std::swap(str1, str2);
  cout << str1 << " "  << str2 << endl;
  
  std1.swap(str2);
  
  cout << str1 << " "  << str2 << endl;
  
  return 0;
}

//삽입
int main()
{
  string str("aaaa");
  
  str.insert(2, "bbb");
  
  cout << str << endl;
  
  return 0;
}
