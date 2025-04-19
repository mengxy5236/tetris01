#  
wstring 是 C++ 标准库中的一种字符串类型，  
表示 宽字符字符串（wide string），  
它是 std::basic_string<wchar_t> 的一个 typedef。  
📌   
std::string 用的是 char，适合处理 ASCII 或 UTF-8 编码；  
std::wstring 用的是 wchar_t，适合处理宽字符（如 Unicode / UTF-16）文本，尤其是包含中文、日文等非英文字符时更安全。  

int main() {  
    std::wstring ws = L"你好，世界";  // 注意前面加了 L，表示宽字符字面值  
    std::wcout << ws << std::endl;  // 输出宽字符串时用 wcout  
    return 0;  
}  

