[![Waffle.io - Issues in progress](https://badge.waffle.io/phoenixproject/sistemasdistribuidos.svg?label=in%20progress&title=In%20Progress)](http://waffle.io/phoenixproject/sistemasdistribuidos)
[![Codacy Badge](https://api.codacy.com/project/badge/Grade/b7f7f3c927ef4770911df44bb8fde04d)](https://www.codacy.com/app/phoenixproject.erp/sistemasdistribuidos?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=phoenixproject/sistemasdistribuidos&amp;utm_campaign=Badge_Grade)
<br>
[![Throughput Graph](https://graphs.waffle.io/phoenixproject/sistemasdistribuidos/throughput.svg)](https://waffle.io/phoenixproject/sistemasdistribuidos/metrics/throughput)
<br><br>

1. [Laboratório de Sockets]<br/>
 1.1 [Exemplo de Sockets](http://www.cs.rpi.edu/%7Emoorthy/Courses/os98/Pgms/socket.html)<br/>
 1.2 Altere o programa acima para implementar um chat entre dois nós (cliente e servidor) da rede, ou seja, que permita a troca de múltiplas mensagens entre os dois usuários.
O número de mensagens enviada por um dos usuários deve ser INDEPENDENTE do número de mensagens enviada pelo outro -- DICA: USE UMA THREAD ADICIONAL.
A conexão deve ser finalizada apenas quando um dos usuários digitar "bye" -- neste caso, TODAS as threads devem ser encerradas (DICA: USE PTHREAD_CANCEL) e o SOCKET DEVE SER ENCERRADO - liberando os recursos do sistema.<br/>

2. [Laboratório de Threads]<br/>
 2.1 Altere o programa [thread_integral.c](https://github.com/phoenixproject/sistemasdistribuidos/tree/master/_THREAD/_LAB) para descobrir o número de processadores (núcleos) do sistema e criar automaticamente o mesmo número de threads para calcular a integral.
O programa deve garantir a exclusão mútua através de um semáforo quando acessar a variável global 'integral'.

  Dica: Crie um vetor de threads e um vetor de argumentos. Faça um for para criar as threads e outro para o join.

  DICA: cheque os comandos: pthread_mutex_lock, pthread_mutex_unlock, get_nproc.


  Em seguida, faça um breve relatório explicativo do funcionamento do seu programa e envie em um arquivo único (zip) contendo o relatório (.ODT) e o seu programa (.C).
  Dentro de seu programa (.C), informe como proceder para compilar e rodar seu programa e qual a plataforma utilizada.<br/>

3. [Laboratório de MPI]<br/>
 3.1 Neste laboratório vamos utilizar o padrão MPI (3.1) -- que é uma interface de troca de mensagens -- para implementar uma versão paralela do programa concorrente Integral utilizado no Laboratório de threads.<br/>

	 Para isso, escolhemos a implementação da biblioteca OpenMPI (https://www.open-mpi.org).
 

# Cálculo do Speedup

###### Onde S é Speedup e E é a eficácia do tempo.

![Modelo Lógico](https://github.com/phoenixproject/sistemasdistribuidos/blob/master/_MEDIA/05_aula.jpg)


##### Links para consulta

https://github.com/racorretjer/Parallel-Merge-Sort-with-MPI/blob/master/merge-mpi.c

https://github.com/racorretjerhttps://github.com/racorretjer

https://github.com/racorretjerv

https://pdfs.semanticscholar.org/c036/849884c34973c1dc4afb90f9fc05c9893553.pdf

https://link.springer.com/book/10.1007/978-3-642-03770-2

http://penguin.ewu.edu/~trolfe/ParallelMerge/ParallelMerge.html

##### Termos para pesquisa:

parallel merge sort with mpi mege-mpi.c

[Powered by Phoenix Project](https://github.com/phoenixproject/sistemasdistribuidos)<br/>

