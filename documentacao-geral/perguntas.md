# Possíveis Questionamentos Técnicos: Startup Ilítia

Este documento consolida as principais frentes de sabatina técnica para uma HealthTech que atua com monitoramento de dados sensíveis e suporte à decisão clínica.

## 1. Segurança e Privacidade (Conformidade LGPD)
Como a plataforma lida com dados de saúde (dados sensíveis), a segurança será o ponto mais questionado:
* **Gestão de Dados:** "Como é feita a gestão das chaves de criptografia para dados em repouso e em trânsito?"
* **Hospedagem:** "Os dados são armazenados em servidores locais ou em nuvem (Cloud)? Existe redundância geográfica?"
* **Direitos do Titular:** "Como o sistema operacionaliza tecnicamente o direito ao esquecimento e a portabilidade dos dados, conforme a LGPD?"

## 2. Algoritmos e Validação Clínica
Sobre a inteligência por trás da triagem ativa:
* **Protocolos Médicos:** "Quais protocolos clínicos (Ex: Ministério da Saúde, OMS) fundamentam as regras do algoritmo de triagem?"
* **Acurácia:** "Como vocês mitigam o risco de 'fadiga de alertas' (excesso de falsos positivos) e garantem a detecção de casos críticos (falsos negativos)?"
* **Natureza do Algoritmo:** "O sistema utiliza IA/Machine Learning para predição de riscos ou baseia-se em árvores de decisão determinísticas?"

## 3. Arquitetura e Engenharia (Stack FastAPI/React)
Questões sobre a robustez da solução:
* **Escalabilidade:** "Como a arquitetura em FastAPI lida com alta concorrência em cenários de implementação B2G (ex: uma capital inteira utilizando o sistema)?"
* **Sincronização Offline:** "Qual a estratégia técnica para o armazenamento local e a resolução de conflitos de dados quando o dispositivo recupera a conectividade?"
* **Interoperabilidade:** "A plataforma suporta padrões de intercâmbio de dados em saúde, como o HL7 FHIR, para integração com prontuários eletrônicos (PEP) existentes?"

## 4. Experiência do Usuário (UX) e Acessibilidade
* **Inclusão Digital:** "Como a interface foi otimizada para gestantes com dispositivos de baixo desempenho ou baixa literacia digital?"
* **Desempenho:** "Qual é o tempo médio de resposta (latência) entre a detecção de um sintoma crítico e o alerta chegar ao profissional de saúde?"
