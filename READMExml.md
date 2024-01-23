# **Introdução ao XML: Formato Original vs. Simplificado**

O XML (Extensible Markup Language) é uma linguagem de marcação amplamente utilizada para representar dados de forma hierárquica e estruturada. Neste contexto, exploraremos as diferenças entre o formato original e o formato simplificado do XML, fornecendo exemplos práticos e demonstrando como realizar a leitura desses formatos usando a linguagem de programação Java.

## **Formato Original do XML**

O formato original do XML é caracterizado pela presença de tags aninhadas e explícitas, contendo informações encapsuladas entre tags de abertura e fechamento. Abaixo está um exemplo de XML original representando informações sobre filmes, livros e comidas:

```xml
<?xml version ="1.0" encoding="utf-8" standalone="yes"?>
<minhasPreferencias>
    <filmes>
        <filme id="1">
            <titulo>O Jogo da Imitação</titulo>
            <ano_lancamento>2014</ano_lancamento>
            <elenco_principal>Benedict Cumberbatch, Keira Knightley</elenco_principal>
            <tipo>Drama</tipo>
            <sinopse>A história de Alan Turing, matemático e pioneiro da computação, durante a Segunda Guerra Mundial.</sinopse>
        </filme>
        <filme id="2">  
             <titulo>O Poderoso Chefão</titulo>
            <ano_lancamento>1972</ano_lancamento>
            <elenco_principal>Marlon Brando, Al Pacino</elenco_principal>
            <tipo>Drama</tipo>
            <sinopse>Um épico sobre a família Corleone e seu império do crime organizado.</sinopse>
        </filme>
        <filme id="3">
             <titulo>Piratas do Vale do Silício</titulo>
            <ano_lancamento>1999</ano_lancamento>
            <elenco_principal>Noah Wyle, Anthony Michael Hall</elenco_principal>
            <tipo>Drama</tipo>
            <sinopse>A história da rivalidade entre as empresas de tecnologia Apple e Microsoft nos primórdios da revolução da computação pessoal.</sinopse>
        </filme>
        </filme>        
    </filmes>
    <livros>
        <livro id="1">
            <titulo>O Senhor dos Anéis</titulo>
            <autor>J.R.R. Tolkien</autor>
            <ano_lancamento>1954</ano_lancamento>
            <tipo>Fantasia</tipo>
            <numero_paginas>1178</numero_paginas>
        </livro>
        <livro id="2">
            <titulo>Orgulho e Preconceito</titulo>
            <autor>Jane Austen</autor>
            <ano_lancamento>1813</ano_lancamento>
            <tipo>Romance</tipo>
            <numero_paginas>432</numero_paginas>
        </livro>
        <livro id="3">
            <titulo>Cem Anos de Solidão</titulo>
            <autor>Gabriel García Márquez</autor>
            <ano_lancamento>1967</ano_lancamento>
            <tipo>Ficção Mágica</tipo>
            <numero_paginas>448</numero_paginas>
        </livro>
    </livros>
    <comidas>
        <comida id="1">
            <nome>Pizza Margherita</nome>
            <ingredientes>Massa de pizza, molho de tomate, mussarela, tomate, manjericão</ingredientes>
        </comida>
        <comida id="2">
            <nome>Sushi</nome>
            <ingredientes>Arroz, alga nori, peixe fresco, abacate</ingredientes>
        </comida>
        <comida id="3">
            <nome>Lasanha</nome>
            <ingredientes>Massa de lasanha, carne moída, molho de tomate, queijo</ingredientes>
        </comida>
    </comidas>
</minhasPreferencias>
```
## **Formato Simplificado do XML**

O formato simplificado do XML visa reduzir a verbosidade, utilizando atributos diretamente nas tags principais. Aqui está um exemplo simplificado baseado no XML original:

```xml
<minhasPreferencias>
    <filmes>
        <filme id="1" titulo="O Jogo da Imitação" ano_lancamento="2014" elenco_principal="Benedict Cumberbatch, Keira Knightley" tipo="Drama" sinopse="História de Alan Turing durante a Segunda Guerra Mundial." />
        <filme id="2" titulo="O Poderoso Chefão" ano_lancamento="1972" elenco_principal="Marlon Brando, Al Pacino" tipo="Drama" sinopse="Épico sobre a família Corleone no crime organizado." />
        <filme id="3" titulo="Piratas do Vale do Silício" ano_lancamento="1999" elenco_principal="Noah Wyle, Anthony Michael Hall" tipo="Drama" sinopse="Rivalidade entre Apple e Microsoft na revolução da computação pessoal." />
    </filmes>
    <livros>
        <livro id="1" titulo="O Senhor dos Anéis" autor="J.R.R. Tolkien" ano_lancamento="1954" tipo="Fantasia" numero_paginas="1178" />
        <livro id="2" titulo="Orgulho e Preconceito" autor="Jane Austen" ano_lancamento="1813" tipo="Romance" numero_paginas="432" />
        <livro id="3" titulo="Cem Anos de Solidão" autor="Gabriel García Márquez" ano_lancamento="1967" tipo="Ficção Mágica" numero_paginas="448" />
    </livros>
    <comidas>
        <comida id="1" nome="Pizza Margherita" ingredientes="Massa de pizza, molho de tomate, mussarela, tomate, manjericão" />
        <comida id="2" nome="Sushi" ingredientes="Arroz, alga nori, peixe fresco, abacate" />
        <comida id="3" nome="Lasanha" ingredientes="Massa de lasanha, carne moída, molho de tomate, queijo" />
    </comidas>
</minhasPreferencias>
```
### Versão Original:

- **Legibilidade:** Mais legível e intuitiva para quem está familiarizado com a estrutura XML tradicional.
- **Hierarquia Explícita:** A hierarquia de elementos é explicitamente definida, útil para compreensão detalhada.

### Versão Simplificada:

- **Menos Verbosa:** Reduz a verbosidade do XML, tornando-o mais compacto e fácil de entender em uma única visualização.
- **Facilidade de Processamento:** Pode ser mais fácil de processar em situações onde a estrutura precisa ser manipulada por máquinas.

