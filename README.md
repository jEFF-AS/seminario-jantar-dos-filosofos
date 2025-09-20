# Relatório: Resolução do Problema do Jantar dos Filósofos

## Descrição Geral
Este repositório contém o relatório de um seminário sobre Computação Concorrente e Distribuída no Centro Universitário Atenas (Paracatu, 2025). O foco é resolver o problema clássico do Jantar dos Filósofos, proposto por Dijkstra, que ilustra desafios de sincronização e alocação de recursos em sistemas paralelos. O relatório analisa várias abordagens, com ênfase em mutex e semáforos implementados em Python para evitar deadlocks e condições de corrida.

**Autores:** Eduardo, Jéferson, Leicimara  
**Curso:** Sistemas de Informação  

## Resumo
O problema envolve 5 filósofos em uma mesa circular, compartilhando garfos para comer, com riscos de deadlock (bloqueio mútuo) e starvation (fome eterna). O relatório explora soluções como:
- **Abordagem Estatística:** Probabilística para quebrar ciclos de espera, simples mas não determinística.
- **Abordagem com Semáforos/Mutex:** Foco principal, usando locks em Python para exclusão mútua. Evita deadlocks com ordenação de aquisição.
- **Teoria dos Grafos:** Modela como grafo para detectar ciclos.
- **SAT/CSP:** Verificação formal de restrições para configurações sem deadlock.

Implementações em Python (código com mutex e semáforos) são apresentadas, com discussões sobre eficiência, robustez e escalabilidade. Testes mostram que semáforos oferecem melhor fairness (todos comem igualmente), com tempos de execução de 10-12s vs. 10-15s para mutex.

## Estrutura do Relatório
- **Introdução:** Objetivo e importância do problema.
- **Fundamentação Teórica:** Conceitos de sincronização, descrição do problema e abordagens.
- **Implementação:** Códigos em Python e tecnologias usadas (threading, time, random).
- **Discussão de Resultados:** Comparações práticas e teóricas entre mutex e semáforos.
- **Conclusão:** Eficiência da abordagem e sugestões para trabalhos futuros (ex.: ML para prioridades).

## Referências Principais
- Dijkstra (1965): Origem do problema.
- Lehmann e Rabin (1981): Solução simétrica.
- Silberschatz et al. (2018): Conceitos de SO.
- Tanenbaum e Bos (2016): Sistemas operacionais modernos.
- Várias fontes online (GeeksforGeeks, Stack Overflow, Medium) para implementações práticas.

Para detalhes completos, consulte o PDF no repositório. Este projeto é para fins acadêmicos.