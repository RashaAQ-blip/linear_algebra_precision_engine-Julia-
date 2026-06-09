# High-Performance Computational Matrices & Numeric Precision Suite

A high-performance numerical computing repository implemented natively in Julia. This project optimizes high-dimensional sparse matrix operations, diagnoses convergence boundaries of iterative linear relaxation models, and analyzes bit-signal integrity under floating-point precision constraints.

## Tech Stack & Core Libraries
* **Language:** Julia
* **LinearAlgebra:** Analytical matrix calculations, norms, and factorization logic.
* **SparseArrays:** High-dimensional sparse matrix mapping to minimize memory overhead.
* **DataFrames & Printf:** Structured logging pipelines for floating-point error optimization matrices.

---

## System Architecture & Portfolio Breakdown

### 1. High-Dimensional Matrix Scaling & Invariance
* **Implementation:** Evaluates a strictly diagonally dominant sparse tridiagonal system ($A\mathbf{x} = \mathbf{b}$) across escalating scale layers from $N=100$ to an enterprise boundary of $N=100,000$.
* **Core Insight:** Establishes **scale invariance** by proving that localized row parameters dictate convergence rates uniformly—hitting convergence targets in exactly **36 iterations** regardless of overall system dimension dimensions. Bypasses standard dense memory bottlenecks by compressing footprint complexity from $O(N^2)$ down to $O(N)$.

### 2. Parameter Boundary Fractures
* **Implementation:** Models non-strictly diagonally dominant matrix frameworks to isolate performance degradation variables.
* **Core Insight:** Illustrates extreme algorithmic drag as iteration constraints explode from **36 up to 16,209 passes** when row boundaries match diagonal entries, proving how structural asset parameter choices directly impact backend CPU efficiency.

### 3. Convergence Velocity Tracking
* **Implementation:** Tracks the mechanical velocity properties of uncoupled vector snapshots (**Jacobi Method**) against immediate in-place spatial updates (**Gauss-Seidel Method**).
* **Core Insight:** Confirms Gauss-Seidel outpaces Jacobi tracking by **over 40%** (21 steps vs. 36 steps) by instantly re-injecting fresh coordinate updates back into the running calculation loop.

### 4. Topological Matrix Factorization Validation
* **Implementation:** Constructs real-time automated structural checkpoints to classify input matrix topologies before downstream processing.
* **Core Insight:** Successfully validates Symmetric Positive Definite (SPD) properties required for Cholesky factorization, capturing geometric layout failures and tracking negative eigenvalue constraints.

### 5. Bit-Signal Integrity & Loss of Precision
* **Implementation:** Profiles mathematical expression behavior approaching double-precision tracking limits ($x \rightarrow 10^{-14}$).
* **Core Insight:** Documents severe **subtractive cancellation** inside standard structural forms (dropping accuracy down to only 3 bits of true signal). Showcases optimization strategies via algebraic reformulation to bypass truncation boundaries and preserve bit integrity.

---

## Repository File Checklist
* **`linear_algebra_precision_engine.ipynb`**: The primary interactive Jupyter Notebook containing code cells, live execution tables, and comprehensive math interpretations.
* **`README.md`**: High-level repository breakdown and core engineering insights.

## Execution & Environment
To launch the notebook locally, clone the repository, ensure Julia and Jupyter are installed, and execute:
```bash
julia -e "using Pkg; Pkg.add([\"LinearAlgebra\", \"SparseArrays\", \"DataFrames\", \"Printf\"])"
jupyter notebook
