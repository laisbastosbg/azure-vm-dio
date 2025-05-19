## ✅ **O que pode ser configurado ao criar uma Máquina Virtual na Azure**

### 🔹 **1. Sistema Operacional**

- Escolha entre Windows, Linux (Ubuntu, Debian, CentOS, etc.)
    
- Pode escolher imagens padrão ou personalizadas (do marketplace ou da sua própria galeria)
    

---

### 🔹 **2. Região e Zona de Disponibilidade**

- **Região**: Localização geográfica onde a VM será criada (ex: Brazil South, East US).
    
- **Zona**: Subdivisão dentro da região; garante alta disponibilidade (ex: Zona 1, 2, 3).
    

---

### 🔹 **3. Tamanho da VM**

- Define quantidade de **vCPUs**, **memória RAM**, **armazenamento temporário** e **desempenho de rede**.
    
- Tipos comuns:
    
    - **B** (baixo custo)
        
    - **D** (uso geral)
        
    - **E** (memória otimizada)
        
    - **F** (processamento otimizado)
        
    - **NV** (GPU, gráficos)
        
    - **HB/HC** (alta performance computacional)
        

---

### 🔹 **4. Configurações de Rede**

- **VNet (rede virtual)**
    
- **Sub-rede**
    
- **IP público ou privado**
    
- **Grupos de segurança de rede (NSG)**: controla portas abertas (por ex., RDP 3389, SSH 22)
    

---

### 🔹 **5. Configurações de Acesso**

- **Usuário e senha** OU
    
- **Chave pública SSH** (para acesso seguro sem senha, comum em servidores Linux)
    

> 💡 _SSH é um protocolo seguro para acesso remoto à linha de comando._

---

### 🔹 **6. Configurações de Disco**

- **Disco do sistema operacional**
    
- Discos adicionais (dados, temporários)
    
- Tipo: **HDD, SSD padrão ou SSD premium**
    
- Capacidade e desempenho podem ser ajustados.
    

---

### 🔹 **7. Configurações de Segurança**

- **Microsoft Defender for Cloud** (proteção contra ameaças)
    
- **Política de atualizações** e **aplicação de patches automáticos**
    
- **Desligamento automático programado**
    
- **Autenticação multifator** (geralmente via Azure AD)
    
- **Firewalls e controle de tráfego**
    

---

### 🔹 **8. Monitoramento e Diagnóstico**

- **Diagnóstico de inicialização**
    
- **Métricas de integridade**
    
- **Logs e alertas**
    
- **Monitoramento com Azure Monitor, Log Analytics, Application Insights**
    

---

### 🔹 **9. Configurações Avançadas**

- **Extensões**: pequenos scripts ou agentes que podem ser instalados automaticamente (por ex., antivírus, scripts de automação, agente do Azure Monitor)
    
- **Script de inicialização (custom data)**: comandos executados na primeira inicialização da VM
    
- **Aceleração de disco NVMe** (disco local de alta performance, útil para VMs que exigem I/O intenso)
    
- **Grupos de proximidade**: garantem que VMs estejam fisicamente próximas no datacenter, reduzindo latência
    

---

### 🔹 **10. Marcas (Tags)** ❗

- **Tags** = pares **nome/valor** (ex: `Ambiente = Produção`, `Departamento = Financeiro`)
    
- Servem para:
    
    - **Organizar recursos**
        
    - **Controlar custos por equipe, projeto ou cliente**
        
    - **Filtrar e buscar recursos facilmente**
        
    - **Aplicar políticas de governança**
        

> 💡 _Imagine que sua empresa tem 100 VMs para projetos diferentes. Com tags, você pode agrupar por projeto, cliente ou equipe e saber quanto cada grupo está gastando._

## ✅ **Situações comuns para criar uma Máquina Virtual em Nuvem**

### 1. **Ambientes de desenvolvimento e teste (Dev/Test)**

- Criar VMs temporárias para desenvolver ou testar software sem afetar o ambiente de produção.
    
- Testar novas configurações, atualizações ou integrações sem risco.
    

> 🧠 _Vantagem:_ Pode ser descartada após o uso, evitando custo permanente.

---

### 2. **Hospedagem de aplicações web**

- Servidores para hospedar sites, APIs, backends de aplicativos ou serviços de e-commerce.
    
- Ideal quando se precisa de controle total sobre o sistema operacional e configuração.
    

> 🧠 _Exemplo:_ Lojas virtuais personalizadas, aplicações corporativas sob demanda.

---

### 3. **Servidores de banco de dados**

- Executar SGBDs como MySQL, PostgreSQL, SQL Server, Oracle, etc., em um ambiente controlado.
    
- Necessário quando se deseja configurações específicas de desempenho, segurança ou backup.
    

> 💡 _Obs:_ Há serviços gerenciados de banco de dados (PaaS), mas alguns preferem controle total via VM.

---

### 4. **Servidores de arquivos e compartilhamento interno**

- Armazenamento e compartilhamento de arquivos internos da empresa com controle por usuário.
    
- Útil em empresas distribuídas, com filiais ou trabalho remoto.
    

---

### 5. **Execução de scripts e tarefas agendadas**

- Máquinas configuradas para executar rotinas de automação, integração ou coleta de dados.
    

> 🛠️ _Exemplo:_ Uma VM que roda um script Python diariamente para gerar relatórios.

---

### 6. **Ambientes de treinamento e laboratório**

- Usado por instituições de ensino ou equipes de TI para simular ambientes de rede, segurança, servidores etc.
    

> 🎓 _Exemplo:_ Criar um laboratório virtual para treinamento em Linux, Active Directory, segurança ofensiva, etc.

---

### 7. **Backup e recuperação de desastres (DR)**

- VMs configuradas para entrar em operação apenas em caso de falha no sistema principal local.
    
- Suporte a planos de continuidade de negócios.
    

---

### 8. **Acesso remoto e uso como desktop virtual (VDI)**

- Máquinas na nuvem acessadas por usuários remotos, com ambiente configurado sob medida.
    
- Alternativa a computadores físicos, com mais segurança e mobilidade.
    

> 🖥️ _Exemplo:_ Uma equipe de suporte que acessa um desktop corporativo de qualquer lugar.

---

### 9. **Execução de software legado**

- Rodar aplicações antigas que exigem versões específicas de SO ou bibliotecas.
    
- Evita migração forçada e reduz impacto em sistemas que ainda funcionam bem.
    

---

### 10. **Alta demanda e escalabilidade**

- Lançamento de novos produtos ou campanhas que exigem aumento temporário de capacidade computacional.
    
- VMs podem ser criadas rapidamente para suportar o tráfego.
    

> 📈 _Exemplo:_ Black Friday, campanhas publicitárias, eventos esportivos com transmissão ao vivo.

---

## ✅ **Vantagens de usar VMs na nuvem**

- Escalabilidade sob demanda
    
- Pagar apenas pelo tempo de uso
    
- Backup e snapshots fáceis
    
- Disponibilidade global
    
- Integração com outros serviços (como balanceadores de carga, banco de dados gerenciado, etc.)
