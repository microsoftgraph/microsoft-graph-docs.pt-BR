---
title: APIs de Proteção de Identidade
description: Tipo de recurso identityProtectionRoot
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: d4eee47b1503b8c37eb0551817725b966d492866
ms.sourcegitcommit: 9eeb056f311044aaa40654cdb3ae5ae61f1c4d04
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/09/2021
ms.locfileid: "52854121"
---
# <a name="identityprotectionroot-resource-type"></a>Tipo de recurso identityProtectionRoot

Namespace: microsoft.graph

A Proteção de Identidade é uma ferramenta que permite que as organizações descubram, investiguem e correção de riscos baseados em identidade em seu ambiente. Você pode usar as seguintes APIs Graph Microsoft para consultar os riscos detectados pela Proteção de Identidade: 

* [riskDetection](riskdetection.md) - Consulte a Microsoft Graph para obter uma lista de detecções de risco vinculadas de usuário e de login e informações associadas sobre a detecção. As detecções de risco na Proteção de Identidade do Azure AD incluem quaisquer ações suspeitas identificadas relacionadas a contas de usuário no diretório.

* [riskyUsers](riskyuser.md) - Consulte o Microsoft Graph informações sobre usuários que a Proteção de Identidade detectou como arriscada. O risco do usuário representa a probabilidade de que uma determinada identidade ou conta seja comprometida. Esses riscos são calculados offline usando as fontes internas e externas de inteligência contra ameaças da Microsoft, incluindo pesquisadores de segurança, profissionais de aplicação da lei, equipes de segurança na Microsoft e outras fontes confiáveis.

* [signIn](signin.md) - Consulte o Microsoft Graph informações sobre as instalações do Azure AD com propriedades específicas relacionadas ao estado de risco, detalhes e nível. Um risco de entrar representa a probabilidade de que uma determinada solicitação de autenticação não seja autorizada pelo proprietário da identidade. Esses riscos podem ser calculados em tempo real ou calculados offline usando as fontes de inteligência de ameaças internas e externas da Microsoft, incluindo pesquisadores de segurança, profissionais de aplicação da lei, equipes de segurança na Microsoft e outras fontes confiáveis.

## <a name="what-can-i-do-with-identity-protection-apis-in-microsoft-graph"></a>O que posso fazer com APIs de Proteção de Identidade no Microsoft Graph?

As seguintes solicitações são populares para trabalhar com dados de log de auditoria:

Operation | URL
:----------|:----
OBTER usuários arriscados | [OBTER https://graph.microsoft.com/v1.0/identityProtection/riskyUsers](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskyUsers&version=v1.0)
OBTER detecções de risco | [OBTER https://graph.microsoft.com/v1.0/identityProtection/riskDetections](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskDetections&version=v1.0)
OBTER o histórico de riscos de um usuário | [OBTER https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/{riskyUserId}/history](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskyUsers/{riskyUserId}/history&version=v1.0)
CONFIRMAR um usuário como comprometido | [Postar https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/confirmCompromised](https://developer.microsoft.com/graph/graph-explorer?request=/identityProtection/riskyUsers/confirmCompromised&version=v1.0)
DESCARTAR um usuário arriscado | [Postar https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/dismiss](https://developer.microsoft.com/graph/graph-explorer?request=/identityProtection/riskyUsers/dismiss&version=v1.0)

Para obter orientações específicas e informações adicionais, consulte Identificar e correção de riscos usando as [APIs Graph Microsoft.](/graph/tutorial-riskdetection-api)

## <a name="what-licenses-do-i-need"></a>De quais licenças eu preciso?

A Proteção de Identidade do Azure AD é um recurso premium. Você precisa de uma licença do Azure AD Premium P1 ou P2 para acessar a API riskDetection (observação: as licenças P1 recebem informações de risco limitados). A API riskyUsers só está disponível para licenças do Azure AD Premium P2.

## <a name="see-also"></a>Confira também

* [Sobre Azure Active Directory Proteção de Identidade](/azure/active-directory/identity-protection/overview-identity-protection)
* [Começar a Azure Active Directory proteção de identidade e o Microsoft Graph](/azure/active-directory/identity-protection/howto-identity-protection-graph-api)
