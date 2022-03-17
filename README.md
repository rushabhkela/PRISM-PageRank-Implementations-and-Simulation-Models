<div id="top"></div>

<br />
<div align="center">
  <a href="https://github.com/rushabhkela/PRISM-PageRank-Implementations-and-Simulation-Models/">
    
  </a>

  <h3 align="center">PRISM</h3>

  <p align="center">
    PageRank Implementations and Simulation Models
    <br />
    <a href="https://github.com/rushabhkela/PRISM-PageRank-Implementations-and-Simulation-Models/blob/main/PRISM-Report.pdf"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/rushabhkela/PRISM-PageRank-Implementations-and-Simulation-Model">View Demo</a>
    ·
    <a href="https://github.com/rushabhkela/PRISM-PageRank-Implementations-and-Simulation-Model/issues">Report Bug</a>
    ·
    <a href="https://github.com/rushabhkela/PRISM-PageRank-Implementations-and-Simulation-Model/issues">Request Feature</a>
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#running-the-project">Running the Project</a></li>
      </ul>
    </li>
    <li><a href="#output">Output</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

<img src="https://user-images.githubusercontent.com/60788199/158873076-b48f82ac-e69b-4532-a4d5-43eae8795606.png">

PageRank (PR) is an algorithm developed by Google Search to rank web pages in their search engine results. It is named after both the term "web page" and co-founder Larry Page. It is a link-analysis algorithm which assigns numerical weighting to each element of the web graph. This weight measures the “relative” importance of the web page within the graph. PageRank works by counting the number of links to a page to determine a rough estimate of how important the website is. It was first used to rank web pages in the Google search engine. Nowadays, it is more and more used in many different fields, for example in social network graphs of users in social media, ranking authors based on research paper citations etc. The assumption is that more important websites are likely to receive more links from other websites.

In this project, I first analysed various literature articles in the PageRank domain and their various approaches. The traditional serial implementation of the PageRank algorithm is modified using OpenMP parallel processing methods to run on a parallel environment and improved on the shortcomings of previous approaches related to dead – ends and spider – traps. It was further improvised using Apache PySpark distributed processing approach deployed on Google Cloud. Finally, I present a personalised PageRank algorithm, taking into considerations the various factors the affect the results of a query put by a user. At the end, a comparative analysis of all the algorithms is done. The results were as desired and the running time of the algorithm was reduced substantially, with accurate results provided as the output.


<p align="right">(<a href="#top">back to top</a>)</p>



### Built With

This project was built with the following frameworks and technologies:

* [C++](https://www.cplusplus.com/)
* [Python](https://www.python.org/)
* [Google Cloud](https://cloud.google.com/)
* [Apache Spark](https://spark.apache.org/)



<p align="right">(<a href="#top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

Follow the steps given below to run the project locally on your system.

### Prerequisites

```sh
GCC compiler version > 8
```

### Running the Project

1. To run the serial implementation, run the following in the terminal with four command line arguments, file_name, maximum_number_of_nodes, error_threshold, beta as explained in the report.
  ```sh
  g++ -fopenmp Serial_PageRank.cpp
  .\a.exe "PageRank_Dataset.txt" 3774768 0.0001 0.85
  ```
2. To run the parallel implementation, run the following in the terminal.
```sh
g++ -fopenmp Parallel_PageRank.cpp
.\a.exe "PageRank_Dataset.txt" 3774768 0.0001 0.85
```

3. The distributed pagerank implementation can be seen from the small dataset Google Colab Notebook for the small dataset. For the larger dataset, a PySpark job must be configured in a DataProc cluster in Google Cloud and then the code must be run using distributed computing.

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- USAGE EXAMPLES -->
## OUTPUT
### Running Time Analysis

<div align="center">
    <img src="https://user-images.githubusercontent.com/60788199/158869161-0d13e657-4952-460c-8e2d-105448e7019e.png">
<br>
</div>


<p align="right">(<a href="#top">back to top</a>)</p>



<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- LICENSE -->
## License

This project is licensed under the Apache 2.0 License. See `LICENSE` for more information.

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

Rushabh Kela - +91 9834473257 - kelarushabh@gmail.com

Project Link: [https://github.com/rushabhkela/PRISM-PageRank-Implementations-and-Simulation-Models](https://github.com/rushabhkela/PRISM-PageRank-Implementations-and-Simulation-Models)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* [Choose an Open Source License](https://choosealicense.com)

<p align="right">(<a href="#top">back to top</a>)</p>
