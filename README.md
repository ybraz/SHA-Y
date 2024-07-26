# SHA-Y: O Algoritmo de Hash Místico

Bem-vindo ao repositório de **SHA-Y**, um algoritmo de hash que mergulha nas profundezas das constantes matemáticas e das propriedades universais. Desenvolvido por um cientista excêntrico e genial, este algoritmo é uma ode à beleza matemática e à complexidade do universo.

## Sumário

- [Introdução](#introdução)
- [Instalação](#instalação)
- [Uso](#uso)
- [Como Funciona](#como-funciona)
- [Contribuição](#contribuição)
- [Licença](#licença)

## Introdução

SHA-Y é um algoritmo de hash customizado que utiliza 13 variáveis de hash, 240 rodadas de compressão e funções de rotação personalizadas, inspiradas em propriedades matemáticas profundas e constantes transcendentais. Este projeto é um experimento em criptografia e um tributo às maravilhas da matemática.

## Instalação

Para utilizar o SHA-Y, você precisará ter o Python instalado em seu sistema. Clone este repositório e navegue até o diretório do projeto:

```bash
git clone https://github.com/seuusuario/shay.git
cd shay
```

## Uso

SHA-Y pode ser utilizado para gerar hashes customizados de mensagens. Veja um exemplo básico de uso:

```python
from shay import custom_sha

mensagem = b"Hello, World!"
hash_resultado = custom_sha(mensagem)
print(f"Custom SHA Hash: {hash_resultado}")
```

## Como Funciona

SHA-Y é construído em torno de conceitos matemáticos fascinantes:

1. **Constantes Matemáticas**: Utiliza valores iniciais derivados de constantes como π (pi), e (número de Euler), φ (número áureo) e outras.
2. **Funções de Rotação Customizadas**: Combina rotações para a esquerda e para a direita, criando uma função de rotação única.
3. **Expansão de Palavras**: Expande as palavras da mensagem para 240 palavras de 32 bits, usando propriedades de XOR e rotação.
4. **Compressão Principal**: Realiza 240 iterações de compressão, utilizando funções de mistura baseadas em AND, OR e XOR.

### Exemplo de Função de Rotação

```python
def custom_rotate(n, b, c):
    """
    Função de rotação customizada que combina rotações para a esquerda e para a direita.

    Args:
        n (int): O valor a ser rotacionado.
        b (int): Número de bits para a rotação para a esquerda.
        c (int): Número de bits para a rotação para a direita.

    Returns:
        int: O valor rotacionado.
    """
    return ((n << b) | (n >> (32 - b)) | (n >> c) | (n << c)) & 0xffffffff
```

## Contribuição

Contribuições são bem-vindas! Se você é um entusiasta da criptografia ou um amante da matemática, sinta-se à vontade para enviar pull requests, reportar problemas ou sugerir melhorias.

## Licença

Este projeto é licenciado sob a Licença MIT. Veja o arquivo `LICENSE` para mais detalhes.

---

Mergulhe no código e explore a beleza mística das constantes matemáticas e da criptografia personalizada. Que a jornada seja tão fascinante quanto as equações que a compõem!
