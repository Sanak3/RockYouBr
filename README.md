# RockYouBr

# 🇧🇷 RockYouBR - Brazilian Wordlist for Pentesting

Uma wordlist otimizada, limpa e unificada com foco no contexto brasileiro, criada especialmente para testes de penetração e auditorias de segurança. 

Este repositório fornece uma base de dados robusta e higienizada, livre de linhas em branco e espaços indesejados, pronta para ser utilizada sem erros nas principais ferramentas de brute-force.

## 🚀 Diferenciais

* **Otimizada para Ferramentas:** Sanitizada (remoção de `whitespaces` invisíveis nas bordas e linhas vazias), garantindo 100% de compatibilidade com ferramentas de quebra de hash que leem arquivos de forma literal.
* **Livre de Duplicatas:** Mesclada a partir de várias fontes e higienizada, removendo completamente qualquer senha repetida para otimizar o tempo de processamento.
* **Ordem Alfabética:** Organizada para facilitar a navegação, auditoria e o particionamento do arquivo, se necessário.
* **Senhas Comuns Injetadas:** Conta com a adição das senhas mais populares no cenário nacional atual (times de futebol, sequências numéricas clássicas, etc.).

## 📊 Estatísticas do Arquivo

O arquivo final foi compilado e filtrado a partir da fusão das seguintes listas:

* `rockyoubr.txt`: 569.437 linhas
* `rockyoubr2.txt`: 6.140.275 linhas
* **Total no arquivo final (`rockyoubrf.txt`): 6.190.103 senhas únicas**

*Nota: A diferença entre a soma dos arquivos originais e o arquivo final prova a eficiência da remoção de milhares de senhas duplicadas e linhas inválidas.*

## 🛠️ Como Usar

Baixe o arquivo `rockyoubrf.txt` e utilize em suas suítes favoritas de segurança ofensiva.

**Exemplo com Aircrack-ng (Wi-Fi WPA/WPA2):**
```bash
aircrack-ng -w rockyoubrf.txt -b [MAC_DO_ROTEADOR] captura.cap
```

**Exemplo com John the Ripper:**
```bash
john --wordlist=rockyoubrf.txt hashes.txt
```

**Exemplo com Hashcat:**
```bash
hashcat -m 1000 -a 0 hashes.txt rockyoubrf.txt
```

## ⚠️ Aviso Legal

Este projeto foi criado estritamente para **fins educacionais** e para uso em **auditorias de segurança autorizadas**. O autor não se responsabiliza pelo mau uso dos dados aqui disponibilizados. Utilize este material com responsabilidade para fortalecer a segurança da informação.

---
*Criado por Sanak3*
