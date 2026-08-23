# Perfil de Engenharia de Sistemas

Perfil técnico público focado em arquitetura de software, sistemas embarcados, protocolos, backend e engenharia de confiabilidade.

## Áreas técnicas

- serviços backend distribuídos;
- contratos de API e compatibilidade;
- software embarcado e máquinas de estado determinísticas;
- pipelines de eventos e processamento concorrente;
- framing, validação e versionamento de protocolos;
- observabilidade, isolamento de falhas e recuperação;
- ambientes públicos com dados exclusivamente sintéticos;
- automação de infraestrutura e engenharia de deployment;
- CQRS, event sourcing e optimistic concurrency;
- backpressure, bulkheads, circuit breakers e retries limitados.

## Modelo de engenharia

```text
requisitos
   ↓
contratos / RFCs
   ↓
modelo de domínio
   ↓
implementação
   ↓
validação / testes
   ↓
observabilidade
   ↓
deployment
   ↓
feedback de incidentes
```

## Princípios técnicos

1. Interfaces possuem versionamento explícito.
2. Falhas são isoladas em domínios limitados.
3. Exemplos públicos usam somente dados sintéticos.
4. Segredos não pertencem ao controle de versão.
5. Transições de estado são determinísticas e auditáveis.
6. Chamadas externas possuem timeout e política explícita de retry.
7. Processamento de eventos considera idempotência desde o projeto.
8. Schemas são validados nas fronteiras do sistema.
9. Builds e testes devem ser reproduzíveis.
10. Comportamento operacional deve ser observável.
11. Concorrência possui ownership definido e encerramento controlado.
12. Mudanças incompatíveis exigem migração e rollback documentados.

## Política de código público

Os repositórios públicos podem conter algoritmos, estruturas de dados, protocolos sintéticos, simuladores, testes, benchmarks e documentação de arquitetura.

Não são publicados intencionalmente:

- nomes de empresas ou marcas privadas;
- dados pessoais;
- credenciais de produção;
- endpoints internos;
- topologia privada;
- dados reais de clientes;
- inventário real de dispositivos;
- interfaces operacionais de controle físico.
