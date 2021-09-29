---
title: Visão geral da API de relatórios para treinamento de simulação de ataque como parte do Microsoft Defender para Office 365
description: Esta seção descreve as APIs que acessam os relatórios de segurança que fazem parte do Microsoft Defender para Office 365.
ms.localizationpriority: high
author: Gopal-MSFT
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 6b2fbce1924da4f15762e93df7e16fe670fbd328
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979504"
---
# <a name="reports-api-overview-for-attack-simulation-training-as-part-of-microsoft-defender-for-office-365"></a>Visão geral da API de relatórios para treinamento de simulação de ataque como parte do Microsoft Defender para Office 365

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Esta seção descreve os recursos de relatórios do Microsoft Defender para Office 365, especificamente APIs que acessam relatórios sobre a participação de um locatário no treinamento de simulação de ataque. Os treinamentos de simulação de ataque configuram simulações de ataque cibernético benigno para treinar usuários no locatário para aumentar sua conscientização e ajudar a identificar usuários vulneráveis.

## <a name="what-role-do-the-attack-simulation-reports-play-in-enterprise-defense"></a>Qual é a função dos relatórios de simulação de ataque na defesa corporativa?

Os relatórios de simulação de ataque ajudam os administradores de locatários a identificarem as lacunas de conhecimento de segurança, para que possam treinar ainda mais seus usuários para diminuir sua suscetibilidade a ataques. O serviço de treinamento de simulação de ataque faz parte do [Microsoft Defender para Office 365](/microsoft-365/security/office-365-security/defender-for-office-365?view=o365-worldwide&preserve-view=true), que protege sua organização contra ameaças mal-intencionadas causadas por mensagens de email, links (URLs) e ferramentas de colaboração.

O Microsoft Defender para Office 365 pertence ao pacote [Microsoft 365 Defender](/microsoft-365/security/defender/microsoft-365-defender?view=o365-worldwide&preserve-view=true) que inclui os seguintes serviços:

- [Microsoft Defender para Ponto de Extremidade](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint)
- [Microsoft Defender para Office 365](/microsoft-365/security/office-365-security/overview)
- [Microsoft Defender para Identidade](https://docs.microsoft.com/defender-for-identity/)
- [Microsoft Cloud App Security](/cloud-app-security/)

O Microsoft 365 Defender é um pacote unificado de defesa corporativa que ajuda a detectar riscos de segurança, investigar ataques a uma organização e evitar atividades prejudiciais automaticamente. Ele fornece um portal central de administradores ([https://security.microsoft.com/](https://security.microsoft.com)) que combina proteção, detecção, investigação e resposta contra ameaças para _email_, _colaboração_, _identidade_ e _dispositivos_.

Para acessar o treinamento de simulação de ataque, abra o portal do Microsoft 365 Defender, vá para **Email e colaboração** > **Treinamento de simulação de ataque**.


## <a name="authorization"></a>Autorização

O Microsoft Graph controla o acesso aos recursos utilizando permissões. Você deve especificar as permissões necessárias para acessar os recursos dos relatórios. Para obter mais informações, consulte [Referência de permissões do Microsoft Graph](/graph/permissions-reference) e [permissões de relatórios](/graph/permissions-reference#reports-permissions).

## <a name="what-kinds-of-data-do-the-reports-return"></a>Que tipos de dados os relatórios retornam?

| Tipos de dados          | Recurso                                | API         |
|:---------------------- |:--------------------------------------- |:------------|
| Reincidentes vulneráveis em um locatário | [attackSimulationRepeatOffender](attacksimulationrepeatoffender.md) | [getAttackSimulationRepeatOffenders](../api/reportroot-getattacksimulationrepeatoffenders.md) |
| Dados e resultados de simulação para cada usuário em um locatário | [attackSimulationSimulationUserCoverage](attacksimulationsimulationusercoverage.md) | [getAttackSimulationSimulationUserCoverage](../api/reportroot-getattacksimulationsimulationusercoverage.md) |
| Cobertura de treinamento para cada usuário em um locatário | [attackSimulationTrainingUserCoverage](attacksimulationtrainingusercoverage.md) | [getAttackSimulationTrainingUserCoverage](../api/reportroot-getattacksimulationtrainingusercoverage.md) |

## <a name="next-steps"></a>Próximas etapas

APIs e recursos de relatório podem criar novas maneiras de se relacionar com os usuários e gerenciar as experiências deles com o Microsoft Graph. Para saber mais:

- Examine os métodos e as propriedades dos recursos mais úteis para o seu cenário.
- Experimente a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).

