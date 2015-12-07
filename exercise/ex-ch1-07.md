**练习 1.7:** 函数调用io.Copy(dst, src)会从src中读取内容，并将读到的结果写入到dst中，使用这个函数替代掉例子中的ioutil.ReadAll来拷贝响应结构体到os.Stdout，避免申请一个缓冲区(例子中的b)来存储。记得处理io.Copy返回结果中的错误。

