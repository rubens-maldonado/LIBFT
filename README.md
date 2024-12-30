# Libft

**Libft** é uma biblioteca em C que implementa funções utilitárias comuns para manipulação de **strings**, **memória** e **listas encadeadas**. Este projeto foi desenvolvido como parte do curso **42**, com o objetivo de criar uma coleção de funções que podem ser reutilizadas em diversos projetos.

## Funções Implementadas

### 1. **Manipulação de Caracteres**
- `ft_isalpha(int c)` - Verifica se o caractere é alfabético.
- `ft_isdigit(int c)` - Verifica se o caractere é um dígito.
- `ft_isalnum(int c)` - Verifica se o caractere é alfanumérico.
- `ft_isascii(int c)` - Verifica se o caractere é ASCII.
- `ft_isprint(int c)` - Verifica se o caractere é imprimível.
- `ft_toupper(int c)` - Converte um caractere para maiúsculo.
- `ft_tolower(int c)` - Converte um caractere para minúsculo.

### 2. **Manipulação de Strings**
- `ft_strlen(const char *s)` - Retorna o comprimento da string.
- `ft_strchr(const char *s, int c)` - Encontra a primeira ocorrência de um caractere na string.
- `ft_strrchr(const char *s, int c)` - Encontra a última ocorrência de um caractere na string.
- `ft_strncmp(const char *s1, const char *s2, size_t n)` - Compara duas strings até `n` caracteres.
- `ft_strlcat(char *dst, const char *src, size_t dstsize)` - Concatena duas strings com um limite.
- `ft_strlcpy(char *dst, const char *src, size_t dstsize)` - Copia uma string com um limite de tamanho.
- `ft_strnstr(const char *haystack, const char *needle, size_t len)` - Encontra uma substring em uma string, com limite de caracteres.
- `ft_strdup(const char *s1)` - Retorna uma cópia de uma string.
- `ft_substr(char const *s, unsigned int start, size_t len)` - Retorna uma substring de uma string.
- `ft_strjoin(char const *s1, char const *s2)` - Junta duas strings em uma nova string.
- `ft_strtrim(char const *s1, char const *set)` - Remove caracteres no início e no final de uma string.
- `ft_itoa(int n)` - Converte um número inteiro para uma string.
- `ft_strmapi(char const *s, char (*f)(unsigned int, char))` - Aplica uma função a cada caractere de uma string.
- `ft_striteri(char *s, void (*f)(unsigned int, char*))` - Aplica uma função a cada caractere de uma string (modifica a original).

### 3. **Manipulação de Memória**
- `ft_memset(void *b, int c, size_t len)` - Preenche um bloco de memória com um valor específico.
- `ft_bzero(void *s, size_t n)` - Preenche um bloco de memória com zero.
- `ft_memcpy(void *dst, const void *src, size_t n)` - Copia um bloco de memória de uma área para outra.
- `ft_memmove(void *dst, const void *src, size_t len)` - Move um bloco de memória de uma área para outra.
- `ft_memchr(const void *s, int c, size_t n)` - Encontra a primeira ocorrência de um caractere em um bloco de memória.
- `ft_memcmp(const void *s1, const void *s2, size_t n)` - Compara dois blocos de memória.
- `ft_calloc(size_t count, size_t size)` - Aloca memória para um número de elementos e inicializa-os a zero.

### 4. **Manipulação de Arquivos**
- `ft_putchar_fd(char c, int fd)` - Escreve um caractere no descritor de arquivo.
- `ft_putendl_fd(char *s, int fd)` - Escreve uma string seguida por uma nova linha no descritor de arquivo.
- `ft_putstr_fd(char *s, int fd)` - Escreve uma string no descritor de arquivo.
- `ft_putnbr_fd(int n, int fd)` - Escreve um número inteiro no descritor de arquivo.

### 5. **Funções Auxiliares**
- `ft_split(char const *s, char c)` - Divide uma string em um array de strings, com base em um delimitador.
  
## Como Usar

1. **Clone o repositório:**
   ```bash
   
   git clone https://github.com/rubens-maldonado/LIBFT.git

2. **Compile a biblioteca:**
   ```bash
   
    cd libft
    make

3. **Inclua no seu projeto:** Adicione a biblioteca ao seu código incluindo o arquivo 'libft.h' e fazendo o link com o arquivo estático 'libft.a'.
  Exemplo:
    ```c

    #include "libft.h"

4. **Limpeza:** Para remover arquivos temporários e a biblioteca compilada:
    ```bash
    
    make clean

5. **Para remover todos os arquivos**, incluindo o arquivo 'libft.a':
    ```bash
    
    make fclean

6. **Recompilar:** Para recompilar o projeto:
    ```bash
    
    make re
