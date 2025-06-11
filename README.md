# 🛠️ Projeto Oficina Mecânica

**Projeto utilizando MySQL - Diagrama EER**

## 📄 Descrição do Projeto

Modelo **controle e gerenciamento de ordens de serviço em uma oficina mecânica**.  
Desenvolvido com base em uma narrativa que simula o atendimento a clientes, execução de serviços e uso de peças para consertos e revisões de veículos.

---

## 📊 Diagrama EER

![Diagrama EER](https://github.com/NatyAnalytcs-1/Projeto-Oficina/blob/main/Projeto%20Oficina.png)

---

## 🔗 Descrição do Modelo Oficina Mecânica

### Cliente → Veículo  
**1 : N**  
Um cliente pode ter vários veículos.  
Cada veículo pertence a apenas um cliente.

---

### Veículo → Ordem de Serviço (OS)  
**1 : N**  
Um veículo pode gerar várias ordens de serviço.  
Cada OS está associada a apenas um veículo.

---

### Ordem de Serviço ↔ Serviço  
**N : N** (via `os_servico`)  
Uma OS pode incluir vários serviços.  
Um mesmo serviço pode estar presente em várias OS.

---

### Ordem de Serviço ↔ Mecânico  
**N : N** (via `os_mecanico`)  
Uma OS pode ser executada por vários mecânicos.  
Um mecânico pode atuar em várias OS.

---

### Ordem de Serviço ↔ Peça  
**N : N** (via `os_peca`)  
Uma OS pode conter várias peças.  
Uma peça pode ser usada em várias OS.

---

## 🔧 Tecnologias

- MySQL Workbench  
- GitHub

---

Feito com 💻 por [NatyAnalytics-1](https://github.com/NatyAnalytics-1)
