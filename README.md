# Voo.java
public class Voo {
    private int numeroVoo;
    private String origem;
    private String destino;
    private String dataPartida;
    private String HoraPartida;
    private int totalAssentos;
    private int assentosDisponiveis;

    public Voo(int numeroVoo, String origem, String destino, String dataPartida, String HoraPartida, int totalAssentos) {
        this.numeroVoo = NumeroVoo;
        this.origem = origem;
        this.destino = destino;
        this.dataPartida = DataPartida;
        this.HoraPartida = HoraPartida;
        this.totalAssentos = TotalAssentos;
        this.assentosDisponiveis = TotalAssentos;
    }

    public boolean reservarAssento() {
        if (assentosDisponiveis > 0) {
            assentosDisponiveis--;
            return true;
        } else {
            return false;
        }
    }

    public void exibirInformacoes() {
        System.out.println("Numero do Voo:" + numeroVoo);
        System.out.println("Origem: " + origem);
        System.out.println("Destino: " + destino);
        System.out.println("Data: " + dataPartida);
        System.out.println("HoraPartida:" + HoraPartida);
        System.out.println("Total de Assentos: " + totalAssentos);
        System.out.println("Assentos Disponiveis: " + assentosDisponiveis);
    }
}
