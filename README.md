# 🌐 Laboratório de Redes — Cisco Packet Tracer

<p align="center">
  <strong>Comunicação entre 3 Redes Distintas</strong>
</p>

<p align="center">
  Projeto prático desenvolvido durante meus estudos de Redes de Computadores e Cibersegurança.
</p>

---

## 📌 Sobre o projeto

Este projeto foi desenvolvido utilizando o **Cisco Packet Tracer** com o objetivo de simular a comunicação entre **três redes distintas**.

A topologia utiliza um **roteador Cisco 2911**, três **switches Cisco 2960** e seis computadores, permitindo praticar conceitos fundamentais de redes e comunicação entre diferentes segmentos.

---

## 🎯 Objetivo

O principal objetivo foi:

- Criar uma topologia com três redes distintas;
- Configurar os endereços IPv4 dos dispositivos;
- Configurar as interfaces do roteador;
- Definir o gateway padrão dos computadores;
- Conectar os dispositivos por meio de switches;
- Testar a comunicação entre as redes.

---

## 🖥️ Topologia da rede

### Equipamentos utilizados

| Equipamento | Quantidade |
|---|---:|
| Roteador Cisco 2911 | 1 |
| Switch Cisco 2960 | 3 |
| Computadores | 6 |

### Organização das redes

**🔵 Rede A**
- PC A1
- PC A2
- Switch A

**🟢 Rede B**
- PC B1
- PC B2
- Switch B

**🟠 Rede C**
- PC C1
- PC C2
- Switch C

### 📷 Topologia

![Topologia da rede](Captura%20de%20tela%202026-09-14%20150453.png)

---

## 🌐 Endereçamento IPv4

### Rede A

| Dispositivo | Endereço IP | Máscara | Gateway |
|---|---|---|---|
| PC A1 | 10.0.0.2 | 255.0.0.0 | 10.0.0.1 |
| PC A2 | 10.0.0.3 | 255.0.0.0 | 10.0.0.1 |

### Rede B

| Dispositivo | Endereço IP | Máscara | Gateway |
|---|---|---|---|
| PC B1 | 172.16.0.2 | 255.255.0.0 | 172.16.0.1 |
| PC B2 | 172.16.0.3 | 255.255.0.0 | 172.16.0.1 |

### Rede C

| Dispositivo | Endereço IP | Máscara | Gateway |
|---|---|---|---|
| PC C1 | 192.168.1.2 | 255.255.255.0 | 192.168.1.1 |
| PC C2 | 192.168.1.3 | 255.255.255.0 | 192.168.1.1 |

---

## 🔀 Configuração do roteador

O roteador Cisco 2911 foi configurado com uma interface para cada rede:

| Interface | Endereço IP |
|---|---|
| GigabitEthernet0/0 | 10.0.0.1 |
| GigabitEthernet0/1 | 172.16.0.1 |
| GigabitEthernet0/2 | 192.168.1.1 |

Esses endereços foram utilizados como **gateways padrão** dos computadores de cada rede.

---

## 🔌 Conexões

As conexões utilizadas na topologia foram:

- Roteador → Switch A
- Roteador → Switch B
- Roteador → Switch C
- Switch A → PC A1 e PC A2
- Switch B → PC B1 e PC B2
- Switch C → PC C1 e PC C2

Foi utilizado o cabo **Copper Straight-Through** para as conexões da atividade.

---

## 🧪 Testes de conectividade

Após a configuração dos dispositivos, foram realizados testes utilizando o comando:

```text
ping
```

O objetivo dos testes foi verificar se os dispositivos conseguiam se comunicar entre redes diferentes por meio do roteador.

### ✅ Resultado esperado

A comunicação entre as redes deve ocorrer através das interfaces configuradas no roteador.

---

## 📚 Principais aprendizados

Durante o desenvolvimento deste laboratório, pratiquei:

- 🌐 Endereçamento IPv4
- 📐 Máscara de sub-rede
- 🚪 Gateway padrão
- 🔀 Comunicação entre redes distintas
- 🖧 Configuração básica de roteador Cisco
- 🔌 Conexão entre roteador, switches e computadores
- 🧪 Testes de conectividade com `ping`
- 🗺️ Montagem de uma topologia de rede
- 💻 Utilização do Cisco Packet Tracer

---

## 🛠️ Ferramenta utilizada

**Cisco Packet Tracer**

---

## 📂 Arquivos do projeto

O repositório contém o arquivo da simulação desenvolvida no Cisco Packet Tracer:

📄 **Cisco Packet Tracer Comunicação de redes.pkt**

O arquivo pode ser aberto utilizando o **Cisco Packet Tracer**.

---

## 👩‍💻 Sobre o projeto

Este laboratório faz parte da minha jornada de estudos em **Tecnologia, Redes de Computadores e Cibersegurança**, com foco na construção de conhecimentos práticos em infraestrutura e comunicação de redes.

---

⭐ Projeto desenvolvido para fins de estudo e aprendizado.
