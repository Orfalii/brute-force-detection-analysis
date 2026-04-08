# Incident Report – Brute Force Attack

## Data
10/04/2026

## Objetivo
Analisar logs de autenticação para identificar atividades suspeitas.

---

## Detecção
Foram identificadas múltiplas tentativas de login falhas seguidas de um login bem-sucedido para o usuário "admin".

---

## Evidências
- Tentativas repetidas de login
- IP de origem: 192.168.1.50
- Login bem-sucedido após falhas

Arquivo analisado: logs.txt

---

## Análise
O padrão indica tentativa de brute force, onde um atacante tentou diversas combinações de senha até obter acesso.

---

## Impacto
Possível comprometimento da conta "admin", com risco de acesso não autorizado ao sistema.

---

## Mitigações
- Bloqueio do IP no firewall
- Reset de credenciais
- Implementação de MFA
- Monitoramento contínuo
- Investigação da origem interna

---

## Conclusão
Foi identificado um ataque de brute force com sucesso, resultando em comprometimento de conta.
