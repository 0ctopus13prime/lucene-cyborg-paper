# lucene-cyborg-paper
Paper regarding to search improvement mades with hybrid approach to use C++ written Lucene compatible library.

## Abstract
Apache Lucene, the popular search engine library written in Java, has maintained its prominence for over 25 years. Despite its extensive usage, there have been numerous efforts to improve its performance by exploring implementations in compiled languages. However, the literature lacks clear empirical evidence on the performance benefits of such porting, leaving users to rely on speculative assessments. This paper introduces the concept and design of LuceneCyborg, a hybrid approach where Java delegates search requests to C++ for potentially enhanced performance. This paper aims to quantify the performance improvements possible with this design. The benchmarks focused on measuring execution times for conjunction and disjunction query types across three command types: TOP\_100, TOP\_100\_COUNT, and COUNT. The results demonstrate that LuceneCyborg consistently outperforms baseline for all types of conjunction queries. Specifically, LuceneCyborg exhibited a performance improvement of 26.9\% for COUNT-Conjunction queries and up to 27.7\% for TOP\_100-Conjunction queries. Additionally, it was 17.57\% faster for TOP\_100-Disjunction queries. However, LuceneCyborg's performance was slower for disjunction queries: it was 4\% \~{} 32\% slower than the baseline for COUNT, TOP\_100\_COUNT Disjunction queries.

# Repositories
- [lucene-cyborg-cpp](https://github.com/0ctopus13prime/lucene-cyborg-cpp)
- [lucene-cyborg-java](https://github.com/0ctopus13prime/lucene-cyborg-java)

# Reproduce the benchmark results
Please refer [lucene-cyborg-search-benchmark-game](https://github.com/0ctopus13prime/lucene-cyborg-search-benchmark-game)
