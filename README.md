<div align="center">

# ⚡ Parallel Distance Calculation - Fork/Join

### Java · Concurrency · Fork/Join · Performance

Distance calculation over 10 million point pairs, comparing single-threaded time with Fork/Join parallelism at several thresholds.

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Concurrency](https://img.shields.io/badge/Concurrency-5382A1?style=for-the-badge&logoColor=white)
![Fork/Join](https://img.shields.io/badge/Fork_Join-6E4C13?style=for-the-badge&logoColor=white)

</div>

## What it does

| Feature | Detail |
|---|---|
| Fork/Join parallelism | Splits the workload across tasks with configurable thresholds |
| 10 million point pairs | A workload large enough for parallelism to actually matter |
| Single-threaded comparison | The same calculation run sequentially, so the speedup is measured, not claimed |
| Threshold tuning | Compares Fork/Join performance at several split thresholds |

## Run

```bash
javac *.java
java Main
```

## Files

- `Main.java` - driver and timing comparison
- `DistanceCalculator.java`, `DistanceTask.java` - Fork/Join task implementation
- `Point.java` - point representation

> Originally a Java Programming II (CIS 36B) project, extracted here as a standalone repo from [java-algorithms-and-concurrency](https://github.com/afshinmalek/java-algorithms-and-concurrency).
