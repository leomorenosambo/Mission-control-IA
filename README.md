# Mission Control AI - Pensamento Computacional e Automação com Python

## 📋 Descrição do Projeto
O **Mission Control AI** é um sistema inteligente de monitoramento de missões espaciais desenvolvido em Python para a Global Solution 2026.1 da FIAP. O software analisa dados de telemetria em tempo real, identifica riscos operacionais e gera recomendações automáticas para apoiar a tomada de decisão da equipe de controle.

## 🚀 Funcionalidades
- ✅ Análise automática de 5 parâmetros vitais (temperatura, comunicação, bateria, oxigênio, estabilidade)
- ✅ Geração de alertas em 3 níveis: NORMAL, ATENÇÃO, CRÍTICO
- ✅ Cálculo de pontuação de risco por ciclo (0 a 10 pontos)
- ✅ Classificação de ciclos: MISSÃO ESTÁVEL, EM ATENÇÃO ou CRÍTICA
- ✅ Análise de tendência (melhora, piora ou estabilidade)
- ✅ Identificação da área mais afetada
- ✅ Relatório final completo no terminal

## 📊 Regras de Negócio

| Parâmetro | NORMAL (0 pts) | ATENÇÃO (1 pt) | CRÍTICO (2 pts) |
| :--- | :--- | :--- | :--- |
| **Temperatura** | 18°C a 30°C | < 18°C ou 31°C a 35°C | > 35°C |
| **Comunicação** | ≥ 60% | 30% a 59% | < 30% |
| **Bateria** | ≥ 50% | 20% a 49% | < 20% |
| **Oxigênio** | ≥ 90% | 80% a 89% | < 80% |
| **Estabilidade** | ≥ 70% | 40% a 69% | < 40% |

**Classificação do Ciclo:**
- 0 a 2 pontos: **MISSÃO ESTÁVEL**
- 3 a 5 pontos: **MISSÃO EM ATENÇÃO**
- 6 a 10 pontos: **MISSÃO CRÍTICA**

## 💻 Como Executar

### Pré-requisitos
- Python 3.x instalado

### Passos
1. Clone o repositório:
```bash
   git clone https://github.com/SEU_USUARIO/mission-control-ai.git
   cd mission-control-ai
