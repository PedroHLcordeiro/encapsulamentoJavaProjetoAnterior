# encapsulamentoJavaProjetoAnterior
import br.com.alura.screenmatch.modelos.Ficha;

public class musica {
    public static void main(String[] args) {
        Ficha pessoal = new Ficha();

        pessoal.setTitulo("Anônimo");
        pessoal.setArtista("Bob Odenkirk");
        pessoal.setAnoDeLnaçamento(2021);

        pessoal.exibeFichaTecnica();
        pessoal.avalia(9);
        pessoal.avalia(10);
        pessoal.avalia(9);
        pessoal.avalia(10);
        pessoal.avalia(10);
        pessoal.avalia(10);
        pessoal.avalia(9);
        pessoal.avalia(10);
        pessoal.avalia(10);
        pessoal.avalia(10);
        pessoal.avalia(10);
        pessoal.avalia(10);

        System.out.println("Média de avaliações do filme: " + pessoal.pegaMedia());
    }
}
package br.com.alura.screenmatch.modelos;

public class Ficha {
    private String Titulo;
    private String Artista;
    private int AnoDeLnaçamento;
    private double somaDasAvaliacoes;
    private int totalDeAvaliacoes;

    public void exibeFichaTecnica() {
        System.out.println("Nome do filme: " + Titulo);
        System.out.println("Nome Do Artista: " + Artista);
        System.out.println("Ano de lançamento: " + AnoDeLnaçamento);
    }

    public String getTitulo() {
        return Titulo;
    }

    public void setTitulo(String titulo) {
        this.Titulo = titulo;
    }

    public String getArtista() {
        return Artista;
    }

    public void setArtista(String artista) {
        this.Artista = artista;
    }

    public int getAnoDeLnaçamento() {
        return AnoDeLnaçamento;
    }

    public void setAnoDeLnaçamento(int anoDeLnaçamento) {
        this.AnoDeLnaçamento = anoDeLnaçamento;
    }

    public void avalia(double nota) {
        somaDasAvaliacoes += nota;
        totalDeAvaliacoes++;
    }

    public double pegaMedia() {
        return somaDasAvaliacoes / totalDeAvaliacoes;
    }
}
// aprendendo sobre segurança no código para restringir a vizualização ou modificação de informações
