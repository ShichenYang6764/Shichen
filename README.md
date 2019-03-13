# Shichen
## The first part: Generating matrix and computing matrix rank.
# Generate several matrices, where any element is randomly selected from 0 to 9.
a <- matrix(sample(0:9, 9, replace = T), 3, 3)
b <- matrix(sample(0:9, 9, replace = T), 3, 3)
c <- matrix(sample(0:9, 9, replace = T), 3, 3)
d <- matrix(sample(0:9, 9, replace = T), 3, 3)

# Generate a 3*3 unit matrix
e <- diag(3)

# compute matrix rank
qr(a)$rank == 3
qr(b)$rank == 3
qr(c)$rank == 3
qr(d)$rank == 3
