---
title: Usar as APIs Graph proteção de identidade do Microsoft Graph
description: Use o Microsoft Graph para consultar e receber informações sobre os riscos detectados pelo Azure AD Identity Protection.
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 2fc391e49d9d177c8487e23b752bdfdc276c186d
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2022
ms.locfileid: "65059903"
---
# <a name="use-the-microsoft-graph-identity-protection-apis"></a>Usar as APIs Graph proteção de identidade do Microsoft Graph

Namespace: microsoft.graph

Azure Active Directory (Azure AD) [Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection) é uma ferramenta que permite que as organizações descubram, investiguem e corrijam riscos baseados em identidade em sua organização do Azure AD. Você pode usar as seguintes APIs do Microsoft Graph para consultar os riscos detectados pelo Azure AD Identity Protection:

* [riskDetection](riskdetection.md) – Consulte o Microsoft Graph para obter uma lista de detecções de risco vinculados de usuário e entrada e informações associadas sobre a detecção. As detecções de risco no Azure AD Identity Protection incluem todas as ações suspeitas identificadas relacionadas a contas de usuário no diretório.

* [riskyUsers](riskyuser.md) – Consulte o Microsoft Graph para obter informações sobre usuários que o Azure AD Identity Protection detectou como arriscado. O risco do usuário representa a probabilidade de uma determinada identidade ou conta ser comprometida. Esses riscos são calculados offline usando fontes internas e externas de inteligência contra ameaças da Microsoft, incluindo pesquisadores de segurança, profissionais de aplicação da lei, equipes de segurança da Microsoft e outras fontes confiáveis.

* [signIn](signin.md) – Consulte o Microsoft Graph para obter informações sobre entradas do Azure AD com propriedades específicas relacionadas ao estado de risco, detalhes e nível. Um risco de entrada representa a probabilidade de que uma determinada solicitação de autenticação não seja autorizada pelo proprietário da identidade. Esses riscos podem ser calculados em tempo real ou calculados offline usando fontes de inteligência contra ameaças internas e externas da Microsoft, incluindo pesquisadores de segurança, profissionais de aplicação da lei, equipes de segurança da Microsoft e outras fontes confiáveis.


## <a name="what-can-i-do-with-identity-protection-apis-in-microsoft-graph"></a>O que posso fazer com APIs de proteção de identidade no Microsoft Graph?

As seguintes solicitações são populares para trabalhar com dados de log de auditoria:

Operation | URL
:----------|:----
OBTER usuários arriscados | [OBTER https://graph.microsoft.com/v1.0/identityProtection/riskyUsers](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskyUsers&version=v1.0)
Obter detecções de risco | [OBTER https://graph.microsoft.com/v1.0/identityProtection/riskDetections](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskDetections&version=v1.0)
OBTER o histórico de risco de um usuário | [OBTER https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/{riskyUserId}/history](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskyUsers/{riskyUserId}/history&version=v1.0)
CONFIRMAR um usuário como comprometido | [POSTAR https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/confirmCompromised](https://developer.microsoft.com/graph/graph-explorer?request=/identityProtection/riskyUsers/confirmCompromised&version=v1.0)
IGNORAR um usuário arriscado | [POSTAR https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/dismiss](https://developer.microsoft.com/graph/graph-explorer?request=/identityProtection/riskyUsers/dismiss&version=v1.0)

Para obter diretrizes específicas e informações adicionais, consulte Identificar e corrigir riscos usando [APIs do Microsoft Graph](/graph/tutorial-riskdetection-api).

## <a name="what-licenses-do-i-need"></a>De quais licenças eu preciso?

O Azure AD Identity Protection é um recurso premium. Você precisa de uma Azure AD Premium P1 ou P2 para acessar a [API riskDetection](riskdetection.md) do Microsoft Graph (observação: as licenças P1 recebem informações de risco limitadas). A [API riskyUsers](riskyuser.md) só está disponível com uma licença Azure AD Premium P2 usuário.

## <a name="how-much-data-is-available"></a>Quantos dados estão disponíveis?

A disponibilidade de dados de risco é governada pelas políticas de retenção de dados do [Azure AD](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data).

## <a name="see-also"></a>Confira também

* [Sobre o Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection)
* [Introdução com o Azure Active Directory Identity Protection e o Microsoft Graph](/azure/active-directory/identity-protection/howto-identity-protection-graph-api)
