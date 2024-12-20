# Tema do Trabalho: **Formas Geométricas em 3D**

![image](https://github.com/user-attachments/assets/63607b16-1a0c-43be-813e-cf573bbd597b)

### Link da aplicação:
https://ailtonleite.github.io/formasgeometricascg/public/geometriacgabc-3.html

### Integrantes do projeto:
- Ailton Leite Manoel Santana Junior - RA: 11201811049
- Mariana Vieira Santos - RA: 11201811863
- Pedro Henrique Garcez Silva - RA: 11202130642

# Introdução
Este trabalho foi desenvolvido para atender às necessidades de professores de matemática e geometria no ensino de formas geométricas tridimensionais na educação básica. O ensino de geometria, especialmente de formas tridimensionais, enfrenta diversos desafios significativos. A visualização e a compreensão espacial são habilidades complexas, e muitos alunos têm dificuldade em desenvolvê-las a partir de representações bidimensionais.

Um programa de computação gráfica pode ser uma ferramenta poderosa para superar essas dificuldades. Ele permite a visualização interativa de formas geométricas em três dimensões, facilitando a compreensão de conceitos espaciais. Os alunos podem rotacionar, ampliar e examinar os objetos de diferentes ângulos, enriquecendo a experiência de aprendizado e tornando o processo mais intuitivo e envolvente.

Além disso, tal programa pode auxiliar os professores ao oferecer recursos visuais que complementam a teoria, tornando as aulas mais dinâmicas e interessantes. A possibilidade de criar simulações e animações transforma conceitos abstratos em experiências concretas, promovendo um entendimento mais profundo e duradouro nos alunos.


# Objetivo
Este projeto visa melhorar a qualidade do ensino de geometria, tornando o aprendizado mais acessível e eficaz para todos os alunos. Busca atender às demandas e desafios enfrentados pelos educadores, fornecendo uma ferramenta prática para o ensino de formas geométricas tridimensionais.

Além disso, o projeto foi testado por professores do ensino fundamental, garantindo que sua aplicação atende às necessidades reais do ambiente educacional e colhendo feedbacks e ideias sobre o projeto.

# Guia de utilização
A aplicação possui uma interface contendo: uma lista de seleção de objetos, uma lista de seleção de shaders (Iluminação modelo “Blinn Phong”, Texturização e reflexão de ambiente) e uma seleção de cores para o objeto.

O objeto é renderizado no centro da tela e pode ser movimentado tridimensionalmente por meio do botão esquerdo do mouse e a iluminação ou ambiente por meio do botão direito do mouse, além da possibilidade de zoom pelo botão de rolagem.

A interface também conta com uma descrição mostrando o número de vértices, arestas e faces do objeto selecionado.

# Projeto e desenvolvimento
Todo o projeto foi desenvolvido em linguagem C++ e utilizando o framework ABCg (desenvolvida pelo professor Harlen Batagelo) que utiliza funções da API gráfica OpenGL.

Para o projeto foram utilizados renderização de gráficos tridimensionais por meio do OpenGL (função OnPaint() da classe Window e LoadObj() da classe Model), Interação a partir de seleção de objetos, shaders e cor (função OnPaintUI() da classe Window), movimentação por meio de TrackBall (Classe TrackBall) e iluminação, texturização e mapeamento de ambiente por meio dos Shaders (função loadDiffuseTexture() da classe Model e createSkyBox() da classe Window).

Um dos maiores problemas enfrentados ao longo do desenvolvimento foi a otimização da aplicação, onde foi identificado que o objeto era renderizado a cada frame, ajustamos o código para que o objeto seja renderizado uma única vez ao selecioná-lo na interface.

# Resultado e análises:
A aplicação foi finalizada com um ótimo desempenho e uma interface simples e prática para uso educacional. O professor Thiago Reis da Escola técnica estadual Visconde de Mauá, utilizou a aplicação gráfica, segundo o mesmo, um dos pontos que mais chamou a atenção da aplicação foi a interatividade e o uso visual, podendo ser usado em sala de aula e não se limitando apenas de desenhos projetados no quadro. O professor também deu sugestões de melhorias futuras para o projeto, como demonstrar as fórmulas geométricas e traçados nos objetos indicando a altura, raio, etc.

# Conclusão
O diferencial dessa aplicação além da interatividade com as formas geométricas, é a funcionalidade de iluminação e reflexão, o que melhora ainda mais a experiência do usuário, podendo prender a atenção dos alunos em sala de aula e contribuindo para o ensino básico. Como trabalhos futuros, continuaremos atualizando a aplicação para uso, atendendo a sugestões e feedbacks coletados pelos professores e alunos.

# Referências
https://hbatagelo.github.io/cg/abcg.html
