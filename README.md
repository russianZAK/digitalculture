#    <center>  ★***First project***★</center>

<font size="5">It's our homework ;)<br>
- [Что может?](https://github.com/russianZAK/Programming_in_C/blob/84d6113dd0b352575436fb98cddc650c94ccdfc8/Lab%20%E2%84%961/C.%20%D0%9B%D0%B0%D0%B1%D0%BE%D1%80%D0%B0%D1%82%D0%BE%D1%80%D0%BD%D0%B0%D1%8F%20%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D0%B0%201.%20%D0%A3%D1%82%D0%B8%D0%BB%D0%B8%D1%82%D0%B0%20WordCount.pdf)
</font> 

# <center><**Functions**></center>

# - File size
```javascript
int count_bytes(FILE*file){

    long size;
    fseek(file, 0, SEEK_END); 
    size = ftell(file); 
    return size;
}
```
# - Count of lines


```javascript
int count_lines(FILE *file){
    int count_line=0;
    char line[255];
    while(fgets(line,255,file)!= NULL){

        count_line++;

    }

    return count_line;
}
```

# - Count of lines
```javascript
int count_words(FILE*file)
{
    char line[255];
    int count_line=0, word=0,words=0;
    while(fgets(line,255,file)!= NULL){
        count_line++;
        for(int i=0; i<strlen(line);i++){

            if (line[i]!=' ' && line[i-1]==' '){
                word++;
            }
        }
        }

    words=word+count_line;
    return words;
}
```

# <center>**DATA**</center>
<font size="5">

| Входные данные | Выходные данные |
| ------------- | ------------- |
| Текстовый файл | Количество строк  |
| Текстовый файл  | Количество слов  |
| Текстовый файл  | Размер файла  |


</font>


# <center> ©russianZAK</center>

# <center> ![](https://i.ibb.co/myR3Y6r/Fznp-QALpexc.jpg)</center>

![](https://img.shields.io/github/release/pandao/editor.md.svg)
