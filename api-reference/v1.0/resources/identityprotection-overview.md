---
title: Usar as APIs Graph proteção de identidade da Microsoft
description: Use o Microsoft Graph para consultar e receber informações sobre riscos detectados pela Proteção de Identidade do Azure AD.
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: b170326d51361643c8f9335a601b0f26a73fd35e
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/21/2022
ms.locfileid: "62161603"
---
# <a name="use-the-microsoft-graph-identity-protection-apis"></a>Usar as APIs Graph proteção de identidade da Microsoft

Namespace: microsoft.graph

Azure Active Directory (Azure AD) [Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection) é uma ferramenta que permite às organizações descobrir, investigar e correção de riscos baseados em identidade em sua organização do Azure AD. Você pode usar as seguintes APIs Graph Microsoft para consultar os riscos detectados pela Proteção de Identidade do Azure AD:

* [riskDetection](riskdetection.md) - Consulte a Microsoft Graph para obter uma lista de detecções de risco vinculadas de usuário e de login e informações associadas sobre a detecção. As detecções de risco na Proteção de Identidade do Azure AD incluem quaisquer ações suspeitas identificadas relacionadas a contas de usuário no diretório.

* [riskyUsers](riskyuser.md) - Consulte o Microsoft Graph informações sobre usuários que a Proteção de Identidade do Azure AD detectou como arriscada. O risco do usuário representa a probabilidade de que uma determinada identidade ou conta seja comprometida. Esses riscos são calculados offline usando as fontes internas e externas de inteligência contra ameaças da Microsoft, incluindo pesquisadores de segurança, profissionais de aplicação da lei, equipes de segurança na Microsoft e outras fontes confiáveis.

* [signIn](signin.md) - Consulte o Microsoft Graph informações sobre as instalações do Azure AD com propriedades específicas relacionadas ao estado de risco, detalhes e nível. Um risco de entrar representa a probabilidade de que uma determinada solicitação de autenticação não seja autorizada pelo proprietário da identidade. Esses riscos podem ser calculados em tempo real ou calculados offline usando as fontes de inteligência de ameaças internas e externas da Microsoft, incluindo pesquisadores de segurança, profissionais de aplicação da lei, equipes de segurança na Microsoft e outras fontes confiáveis.


## <a name="what-can-i-do-with-identity-protection-apis-in-microsoft-graph"></a>O que posso fazer com APIs de proteção de identidade no Microsoft Graph?

As seguintes solicitações são populares para trabalhar com dados de log de auditoria:

Operation | URL
:----------|:----
OBTER usuários arriscados | [OBTER https://graph.microsoft.com/v1.0/identityProtection/riskyUsers](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskyUsers&version=v1.0)
OBTER detecções de risco | [OBTER https://graph.microsoft.com/v1.0/identityProtection/riskDetections](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskDetections&version=v1.0)
OBTER o histórico de riscos de um usuário | [OBTER https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/{riskyUserId}/history](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskyUsers/{riskyUserId}/history&version=v1.0)
CONFIRMAR um usuário como comprometido | [POSTAR https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/confirmCompromised](https://developer.microsoft.com/graph/graph-explorer?request=/identityProtection/riskyUsers/confirmCompromised&version=v1.0)
DESCARTAR um usuário arriscado | [POSTAR https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/dismiss](https://developer.microsoft.com/graph/graph-explorer?request=/identityProtection/riskyUsers/dismiss&version=v1.0)

Para obter orientações específicas e informações adicionais, consulte Identificar e correção de riscos usando as [APIs Graph Microsoft.](/graph/tutorial-riskdetection-api)

## <a name="what-licenses-do-i-need"></a>De quais licenças eu preciso?

A Proteção de Identidade do Azure AD é um recurso premium. Você precisa de uma Azure AD Premium P1 ou P2 para acessar a [API Graph riskDetection](riskdetection.md) da Microsoft (observação: as licenças P1 recebem informações de risco limitados). A [API riskyUsers](riskyuser.md) só está disponível com uma Azure AD Premium P2 de usuário.

## <a name="see-also"></a>Confira também

* [Sobre Azure Active Directory Proteção de Identidade](/azure/active-directory/identity-protection/overview-identity-protection)
* [Começar a Azure Active Directory Identity Protection e o Microsoft Graph](/azure/active-directory/identity-protection/howto-identity-protection-graph-api)
