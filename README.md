
<br />
<p align="center">
  <img src="https://image.flaticon.com/icons/png/512/28/28842.png" height="225" width="200"></img>
  <h3 align="center">CsvLib</h3>

  <p align="center">
    A small C library for using csv files
    <br />
</p>

<pre>
<code>
#include "CsvLib.h" // Header

int main()
{
    /*
        Simple Example for reading csv, changing the delimiter and 
        writing it into a new file
    */

    char *file_content = NULL; // Buffer for string
    CsvData *csv_data = read_csv("./tests/100.csv", ',', file_content);

    csv_data->delimiter = ';';
    write_csv("./tests/new.csv", csv_data); // rewriing csv

    free_csv_data(csv_data); // freeing the csv_data
    free(file_content);      // freeing the buffer
    file_content = NULL;

    return 0;
}
</code>

</pre>


## Features

Here are a few of the features of this Library...
 
Features:
* It is very lightweight
* It is fast
* Can parse any csv file

NOTE:
  This project is not finished yet so it does not have that many features!!!!!



### Built With
* [C](http://cppreference.com)




## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request



<!-- LICENSE -->
## License

This has no license so feel free to take it :)



<!-- CONTACT -->
## Contact

Project Link: [https://github.com/ferdinandlb/CsvLib](https://github.com/ferdinandlb/CsvLib)
