# ataques-ransomware--notebooklm

# Contexto e objetivos
**Tema escolhido: Ataques Ransomware**
**Objetivo: Compreender como os ataques de ransomware funcionam**

## Curadoria de fontes 
1. https://www.fortinet.com/br/resources/cyberglossary/recent-ransomware-settlements
2. https://www.ibm.com/br-pt/think/topics/ransomware
3. https://www.microsoft.com/pt-br/security/business/security-101/what-is-ransomware
4. https://www.tempest.com.br/blog/ataque-ransomware
5. https://cloud.google.com/security/resources/insights/what-ransomware?hl=pt-BR

## Engenharia de Prompts e "Cicatrizes"

1.**Como acontece o ataque de ransomware? Existe um padrão ou há variações?**
   
Um ataque de ransomware segue um padrão geral de ciclo de vida, mas apresenta diversas variações significativas em suas táticas, tecnologias e modelos de extorsão.
   
Como Acontece um Ataque de Ransomware (O Padrão Geral)

A maioria dos ataques desdobra-se em etapas bem definidas:
 
1. Acesso Inicial (Infecção): Os cibercriminosos obtêm entrada no sistema por meio de métodos como e-mails de phishing e engenharia social, exploração de vulnerabilidades de softwares ou sistemas operacionais (incluindo falhas de dia zero), roubo de credenciais de acesso (como via RDP) ou downloads automáticos ao visitar sites maliciosos.

2. Pós-Exploração e Movimento Lateral: Após conseguir a entrada inicial, os invasores expandem o ataque para outras máquinas, servidores e domínios da rede conectada.

3. Coleta e Exfiltração de Dados: Os invasores identificam e copiam (roubam) dados confidenciais e valiosos, como credenciais, propriedade intelectual ou informações pessoais de clientes.

4. Criptografia ou Bloqueio de Sistemas: O malware é executado para codificar os arquivos da vítima ou bloquear o acesso ao dispositivo/sistema operacional. Além disso, os invasores frequentemente desativam recursos de restauração e apagam ou criptografam backups conectados à rede para impedir a recuperação rápida.

5. Notificação e Exigência de Resgate: É exibida uma mensagem de resgate (via arquivo de texto, pop-ups ou tela bloqueada) com instruções e prazos para o pagamento, geralmente exigido em criptomoedas, em troca da chave de descriptografia ou restauração.

### As Variações no Ataque

Embora o fluxo acima seja a estrutura padrão, existem variações marcantes:

1. Variações pelo Tipo de Malware
   
* Ransomware de Criptografia: Codifica dados e arquivos sensíveis, exigindo o pagamento para liberação da chave.
* Ransomware de Bloqueio: Bloqueia a tela ou as funções do dispositivo (bastante comum em dispositivos móveis), impedindo o uso da máquina sem necessariamente criptografar os arquivos.

2. Variações nos Modelos de Extorsão
* Extorsão Simples: Cobrança de resgate apenas em troca da chave de descriptografia dos dados.
* Dupla Extorsão (Leakware / Doxware): Além de criptografar os dados, os atacantes exfiltram dados sigilosos e ameaçam publicá-los na internet se o resgate não for pago.
* Tripla Extorsão: Acrescenta a ameaça de usar os dados roubados para extorquir ou atacar diretamente os clientes e parceiros de negócios da vítima.
* Wipers (Limpadores / Destrutivos): Malware projetado para apagar permanentemente os dados, sem garantia ou intenção de recuperação mesmo após o pagamento.
* Scareware: Utiliza táticas de intimidação (falsificando mensagens de autoridades policiais ou falsos alertas de vírus) para induzir o pagamento de taxas.

3. Variações nos Modelos Operacionais
* Ransomware Operado por Humanos: Grupos de invasores que investigam ativamente as vulnerabilidades e os documentos financeiros de uma organização específica antes de infectá-la.
* Ransomware como Serviço (RaaS): Modelo de negócios em que desenvolvedores alugam o código malicioso para "afiliados" executarem os ataques e dividirem os lucros.
* Ataques sem Criptografia (Infostealers): Algumas gangues roubam dados confidenciais e exigem resgates sem a necessidade de criptografar ou bloquear os sistemas da vítima.

2. **Qual variação de ataque é mais perigoso: por humanos ou RaaS?**

As fontes não definem uma modalidade como estritamente "mais perigosa" que a outra, pois ambas representam um salto na gravidade das ameaças contra empresas e grandes organizações.
Na verdade, a principal razão de serem tão devastadoras é que elas frequentemente atuam juntas no mesmo ataque.

A diferença entre elas está na natureza do perigo que cada uma traz:

## Ransomware Operado por Humanos

* Qual é o perigo? A sofisticação e o direcionamento customizado.

* Como funciona: Em vez de disparar um malware genérico e automatizado, um grupo de invasores humanos utiliza inteligência coletiva para navegar manualmente pela rede da vítima. Eles pesquisam a empresa, identificam vulnerabilidades específicas e chegam a investigar documentos financeiros internos para definir o valor máximo de resgate que a organização pode pagar.
  
## Ransomware como Serviço (RaaS)

* Qual é o perigo? A escala e a democratização do cibercrime.

* Como funciona: Trata-se de um modelo de negócios em que desenvolvedores de malware licenciam suas ferramentas para "afiliados" executarem as invasões e dividirem os lucros do resgate.
Isso reduz a barreira técnica, permitindo que criminosos com habilidades limitadas lancem ataques complexos, o que multiplica exponencialmente a quantidade de ameaças ativas.

### A Combinação dos Dois

A maior ameaça atual surge do cruzamento dessas duas modalidades: grupos de invasores operados por humanos usam a infraestrutura e os softwares fornecidos por plataformas de RaaS (como ocorreu com variantes conhecidas como LockBit, REvil ou DarkSide) para realizar invasões focadas e altamente lucrativas.

# Miniguia de Estudo

# Resumo

A maioria dos ataques ransomware possuem etapas definidas. Os cibercriminosos entram no sistema das vítimas através de e-mails de phishing, engenharia social, entre outros. Os invasores roubam dados confidenciais, em seguida, o malware é executado para bloquear o acesso ao dispositivo/ sistema e para a vítima é apresentada uma mensagem de resgate com instruções para o pagamento em troca da chave de descriptografia. 
Existem outras variações por tipo de malware, modelos de extorsão e modelos operacionais.
Por fim, os ataques ransomware podem ser operados por humanos ou serviços (RaaS). No entanto, ambos os ataques apresentam o mesmo perigo. 

# Glossário

- A maioria dos ataques ransomware seguem o mesmo padrão;
- Existem variações para a extorsão, por exemplo, aém de criptografar os dados, os atacantes exfiltram dados sigilosos e ameaçam publicá-los na internet se o resgate não for pago.

# Conjunto de prompts

* Como acontece o ataque de ransomware? Existe um padrão ou há variações?
* Qual variação de ataque é mais perigoso: por humanos ou RaaS?
