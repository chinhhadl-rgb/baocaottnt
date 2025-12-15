# baocaottnt
for i in range(n):
            if b[i][0] != ' ' and all(b[i][j] == b[i][0] for j in range(n)):
                return b[i][0]
        for j in range(n):
            if b[0][j] != ' ' and all(b[i][j] == b[0][j] for i in range(n)):
                return b[0][j]
        if b[0][0] != ' ' and all(b[i][i] == b[0][0] for i in range(n)):
            return b[0][0]
        if b[0][n-1] != ' ' and all(b[i][n-1-i] == b[0][n-1] for i in range(n)):
            return b[0][n-1]
        return None
