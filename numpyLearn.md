about numpy     -----    import numpy as np

-  Creating Arrays

np.arange([start,] stop[, step,], dtype=None)

    a = np.arange(1, 10) -----[1 2 3 4 5 6 7 8 9]
    b = range(1, 10)     -----range(1, 10)
    print(list(b))       -----[1, 2, 3, 4, 5, 6, 7, 8, 9]
    x = np.arange(0.5, 10.4, 0.8, int)-----[ 0  1  2  3  4  5  6  7  8  9 10 11 12]

- Linspace

linspace(start, stop, num=50, endpoint=True, retstep=False)

    print(np.linspace(1, 10, 7))  # 7 values between 1 and 10
    print(np.linspace(2, 12, 7, endpoint=False))  # excluding the endpoint
    spacing = np.linspace(1, 10, 20, endpoint=False, retstep=True)
    print(spacing)

- Shape of an Array

    x = np.array([ [1,2,3],
                   [4,5,6]])
    print(np.shape(x))   -----(2,3)  同print(x.shape)

- Indexing and Slicing

    X = np.arange(6).reshape(2,3)
    print(X[::2,::3])

- Arrays of Ones and of Zeros

    E = np.ones((2,3))
    F = np.zeros((3,4),dtype=int)

- Copying Arrays

copy(obj, order='K')   /  a.copy(order='C')

- Identity Array 

two ways to create identity array: identy  &  eye

identity(n, dtype=None)

eye(N, M=None, k=0, dtype=float)

    np.identity(4, dtype=int) # equivalent to np.identity(3, int)
    np.eye(5, 8, k=1, dtype=int)


