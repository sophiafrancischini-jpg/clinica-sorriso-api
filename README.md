# DR. Roberto
Objetivo do Sistema: Otimizar a
gestão clínica e o fluxo de recepção
por meio do cadastro unificado de
pacientes, acompanhamento do status
das consultas em tempo real e
disponibilização de um prontuário
digital com foco estritamente clínico
(sem exibição de dados financeiros).
O software possui regra de restrição
de agenda que bloqueia consultas aos
sábados de manhã para clientes sem a
classificação VIP, operando sob uma
interface de alta performance nas
cores Azul Marinho e Prata.

# MER - Modelo Entidade-Relacionamento

## Entidades e Atributos

PACIENTE

 id_paciente (PK)**
nome
 e_vip

DENTISTA

id_dentista (PK)**
 nome

AGENDAMENTO

id_agendamento (PK)**
 data_hora
status
id_paciente (FK)**
id_dentista (FK)**

PRONTUARIO

**id_prontuario (PK)**
registro_clinico
 **id_agendamento (FK)**

![Diagrama DER](./database/Diagrama%20sem%20nome.drawio.png)