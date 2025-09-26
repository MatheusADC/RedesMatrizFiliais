# <img src="https://github.com/user-attachments/assets/caabfdf0-0f9e-44a3-8200-c6579fe87887" alt="Ícone de descrição" width="28"> Descrição
A atividade tem como intuito representar redes interligadas entre diferentes localidades usando o software **Cisco Packet Tracer**.

# <sub><img src="https://img.icons8.com/?size=100&id=kqyQaZS6Rp1n&format=png&color=000000" alt="Ícone de fluxograma" width="32"></sub>  Caso de Uso
Uma empresa possui três localidades principais: uma **matriz** e duas **filiais**.  
A matriz está localizada em **Vitória**, enquanto as filiais estão nas cidades de **Rio de Janeiro** e **São Paulo**.  

- Cada local possui dois departamentos: **Vendas** e **TI**, e cada departamento deve ter sua própria **sub-rede**.  
- A empresa possui o endereço IP classe B **192.168.0.0/16**, que deve ser dividido para atender o cenário.  
- A matriz, localizada em Vitória, possui a única **saída para a internet**, e os roteadores das filiais devem encaminhar o tráfego destinado à internet para o roteador da matriz.  
- A divisão das sub-redes deve ser feita de forma a **minimizar o número de rotas** configuradas em cada roteador, utilizando **agregação de rotas** sempre que possível.  

# <sub><img src="https://img.icons8.com/?size=100&id=jL3NncSLLzPF&format=png&color=000000" alt="Ícone de requisitos" width="34"></sub> Requisitos
### Endereçamento IP
- O endereço IP **192.168.0.0/16** deve ser dividido para criar sub-redes que atendam os requisitos:
  - Cada sub-rede deve suportar **30 dispositivos** (incluindo os 2 computadores configurados inicialmente e espaço para crescimento futuro).  
  - A divisão dos endereços deve permitir **agregação de rotas**, minimizando o número de rotas estáticas configuradas em cada roteador.  

### Dispositivos por localidade
Cada local (Vitória, Rio de Janeiro e São Paulo) possui:
- **Roteador:** Conectado à internet e entre os departamentos.  
- **Switches:** Dois switches, um para cada sub-rede (Vendas e TI).  
- **Computadores:** Dois PCs em cada sub-rede (Vendas e TI).  

### Roteamento Estático
- Configurar **rotas estáticas** nos roteadores para garantir a comunicação entre todas as sub-redes.  
- Configurar os roteadores das **filiais** para encaminhar o tráfego destinado à internet para o roteador da **matriz** em Vitória.  

### Simulação
Após a configuração, realizar testes de conectividade com o comando `ping`:
- Entre computadores de diferentes sub-redes e localidades.  
- Entre computadores e um **servidor fictício** configurado para representar a internet (simulado na matriz).  

### Ferramenta
O trabalho deve ser realizado utilizando o **Cisco Packet Tracer**, que pode ser baixado gratuitamente no site oficial da Cisco Networking Academy:

🔗 [Download Packet Tracer](https://www.netacad.com/resources/lab-downloads?courseLang=pt-BR)

# <img src="https://img.icons8.com/?size=100&id=0wmdU4RVIEp7&format=png&color=000000" alt="Ícone de roteador" width="32"> Redes
<img width="1842" height="584" alt="image" src="https://github.com/user-attachments/assets/bb94890c-0e8b-477d-84fe-901722e127af" />
