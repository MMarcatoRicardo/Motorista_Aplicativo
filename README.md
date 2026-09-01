# 🚗 Rota Certa — Alugar ou usar o meu?

Calculadora web que mostra ao motorista de aplicativo se compensa mais **alugar um carro** ou **rodar com o próprio**, considerando os custos que normalmente ficam de fora da conta.

**[▶ Testar a aplicação](https://mmarcatoricardo.github.io/Motorista_Aplicativo/app/)** · **[Ver o site do projeto](https://mmarcatoricardo.github.io/Motorista_Aplicativo/)**

---

## O problema

Quem começa a dirigir por aplicativo enfrenta a mesma dúvida logo no início: alugar um carro por semana ou usar o que já tem. A escolha errada custa centenas de reais por mês.

A conta é difícil porque exige números que ninguém conhece de cabeça — custo por quilômetro, consumo real, depreciação. Por isso a decisão acaba sendo tomada no chute.

## A solução

O Rota Certa pergunta apenas o que o motorista já sabe:

- Quantos dias rodou na semana
- Quantas horas por dia
- Quantos quilômetros por dia
- Quanto recebeu
- Quanto gastou de combustível

A partir desses cinco fatos, o aplicativo **deriva sozinho** o ganho por hora, o consumo real do carro em km/litro e o custo de combustível por quilômetro. Em seguida compara os dois cenários e entrega o veredito em reais.

---

## Funcionalidades

| Recurso | O que faz |
|---|---|
| 🧮 Raio-X da semana | Calcula ganho por hora, ganho por km e consumo real do carro |
| ⚖️ Comparativo | Mostra entrada, saída e sobra de cada cenário com barra proporcional |
| 📈 Ponto de virada | Gráfico que revela a partir de quantas horas por dia a resposta muda |
| 🎚️ Simulação ao vivo | Controles que recalculam tudo ao mexer na jornada |
| 🏦 Projeção de patrimônio | Soma dinheiro guardado e valor do carro em 12 meses |
| 📵 Funciona offline | Roda no navegador, salva no aparelho, não envia dados |

---

## Como rodar localmente

O projeto não tem dependências nem etapa de build. Basta clonar e abrir:

```bash
git clone https://github.com/MMarcatoRicardo/Motorista_Aplicativo.git
cd Motorista_Aplicativo
```

Depois abra o arquivo `index.html` no navegador.

Se preferir servir por HTTP (recomendado, para os caminhos relativos funcionarem igual ao GitHub Pages):

```bash
python -m http.server 8000
```

E acesse `http://localhost:8000`.

---

## Estrutura do projeto

```
Motorista_Aplicativo/
├── index.html            # Hero e apresentação do projeto
├── funcionalidades.html  # Lista de recursos
├── equipe.html           # Mural da equipe
├── contato.html          # Links, tecnologias e formulário
├── app/
│   └── index.html        # A calculadora (aplicação principal)
├── assets/
│   └── style.css         # Estilos compartilhados do site
├── README.md
├── LICENSE
└── .gitignore
```

---

## Tecnologias utilizadas

- **HTML5** semântico
- **CSS3** com variáveis, grid e flexbox
- **JavaScript** puro, sem framework ou biblioteca
- **SVG** para o gráfico e a identidade visual
- **localStorage** para persistência no aparelho
- **Google Fonts** — Barlow e IBM Plex Mono
- **Git** e **GitHub** com branches e pull requests
- **GitHub Pages** para publicação

---

## Equipe

Os dados completos de cada integrante — nome, RGM e perfil do GitHub — estão na
página [Quem somos](equipe.html), preenchidos por cada um em seu próprio commit.

| Integrante | Função no projeto |
|---|---|
| Ricardo Marcato | Líder — apresentação do projeto |
| Vinícius Baliski | Funcionalidades |
| Davi Taniguchi | Mural da equipe |
| Erik Comegno | Contato e aplicação |
| Luiz Matheus | Documentação |

O histórico de contribuições de cada integrante está em [Insights › Contributors](https://github.com/MMarcatoRicardo/Motorista_Aplicativo/graphs/contributors).

---

## Fluxo de trabalho

Todo o desenvolvimento seguiu o mesmo fluxo, sem commits diretos na `main`:

1. Cada integrante criou uma branch própria para a sua seção
2. Fez os commits nessa branch, com a própria conta
3. Abriu um Pull Request descrevendo a entrega
4. Outro integrante revisou e aprovou antes do merge

---

## Licença

Distribuído sob a Licença MIT. Veja [LICENSE](LICENSE.txt) para mais informações.

---

## Aviso

Este é um **projeto acadêmico**. Os cálculos são estimativas baseadas nos dados informados pelo usuário e não consideram Imposto de Renda, INSS, multas ou variações regionais. Servem para comparar dois caminhos, não como garantia de ganho.
