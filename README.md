## Hi there 👋
# Portfólio Profissional

## Projeto: PortfolioGUI

Aplicativo Java Swing que exibe um portfólio profissional em uma janela gráfica, com informações sobre formação, experiência, habilidades, objetivos e contato.

### Descrição

- Interface simples usando `JFrame`, `JPanel`, `JLabel` e `JTextArea`.
- Texto formatado e rolável com `JScrollPane`.
- Ideal para demonstrar habilidades em Java GUI e apresentação de portfólio.

### Como executar

```bash
javac PortfolioGUI.java
java PortfolioGUI
```

### Código principal

```java
import javax.swing.*;
import java.awt.*;

public class PortfolioGUI extends JFrame {

    public PortfolioGUI() {
        setTitle("Portfólio Profissional");
        setSize(700, 500);
        setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        setLocationRelativeTo(null);

        JPanel painel = new JPanel();
        painel.setLayout(new BorderLayout());

        JLabel titulo = new JLabel("Meu Portfólio", SwingConstants.CENTER);
        titulo.setFont(new Font("Arial", Font.BOLD, 28));

        JTextArea conteudo = new JTextArea();
        conteudo.setEditable(false);
        conteudo.setFont(new Font("Arial", Font.PLAIN, 16));
        conteudo.setText(
                "SOBRE MIM\n\n"
                        + "Estudante de Programação Python e atualmente cursando o 4º semestre de Biomedicina.\n\n"
                        + "Tenho experiência em clínica odontológica e farmácia, com atuação em atendimento,\n"
                        + "organização de processos e suporte em ambientes de saúde e estética.\n\n"
                        + "HABILIDADES\n\n"
                        + "• Python\n"
                        + "• Java\n"
                        + "• Git e GitHub\n"
                        + "• Lógica de Programação\n"
                        + "• Atendimento ao Público\n"
                        + "• Organização e Trabalho em Equipe\n\n"
                        + "OBJETIVOS\n\n"
                        + "Unir tecnologia e saúde através do desenvolvimento de sistemas\n"
                        + "que contribuam para a melhoria dos processos e do atendimento.\n\n"
                        + "CONTATO\n\n"
                        + "GitHub: github.com/seuusuario\n"
                        + "LinkedIn: linkedin.com/in/seuperfil\n"
                        + "E-mail: geovannagd.nogueira@gmail.com"
        );

        JScrollPane scroll = new JScrollPane(conteudo);

        painel.add(titulo, BorderLayout.NORTH);
        painel.add(scroll, BorderLayout.CENTER);
        add(painel);
    }

    public static void main(String[] args) {
        SwingUtilities.invokeLater(() -> {
            PortfolioGUI portfolio = new PortfolioGUI();
            portfolio.setVisible(true);
        });
    }
}
```

---

Use esta entrada no seu portfólio para mostrar um projeto Java com interface gráfica e apresentação profissional.
<!--
**Nogueiragi/nogueiragi** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
