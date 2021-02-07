---
title: APIs de Proteção de Identidade
description: Tipo de recurso identityProtectionRoot
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 344dc8073ee33d028943c803eb560f94a4ecdc86
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129741"
---
# <a name="identityprotectionroot-resource-type"></a>Tipo de recurso identityProtectionRoot

Namespace: microsoft.graph

O Identity Protection é uma ferramenta que permite que as organizações descubram, investiguem e remediam riscos baseados em identidade em seu ambiente. Você pode usar as seguintes APIs do Microsoft Graph para consultar os riscos detectados pelo Identity Protection: 

* [riskDetection](riskdetection.md) - Consulte o Microsoft Graph para obter uma lista de detecções de risco vinculado de usuário e de login e informações associadas sobre a detecção. As detecções de risco no Azure AD Identity Protection incluem ações suspeitas identificadas relacionadas a contas de usuário no diretório.

* [riskyUsers](riskyuser.md) - Consulte o Microsoft Graph para obter informações sobre usuários que a Proteção de Identidade detectou como arriscadas. O risco do usuário representa a probabilidade de que uma determinada identidade ou conta seja comprometida. Esses riscos são calculados offline usando as fontes de inteligência contra ameaças internas e externas da Microsoft, incluindo pesquisadores de segurança, profissionais de aplicação da lei, equipes de segurança da Microsoft e outras fontes confiáveis.

* [signIn](signin.md) - Consulte o Microsoft Graph para obter informações sobre as instalações do Azure AD com propriedades específicas relacionadas ao estado, detalhes e nível de risco. Um risco de login representa a probabilidade de que uma determinada solicitação de autenticação não seja autorizada pelo proprietário da identidade. Esses riscos podem ser calculados em tempo real ou offline usando as fontes de inteligência contra ameaças internas e externas da Microsoft, incluindo pesquisadores de segurança, profissionais de aplicação da lei, equipes de segurança da Microsoft e outras fontes confiáveis.

## <a name="what-can-i-do-with-identity-protection-apis-in-microsoft-graph"></a>O que posso fazer com as APIs de Proteção de Identidade no Microsoft Graph?

As seguintes solicitações são populares para trabalhar com dados de log de auditoria:

Operation | URL
:----------|:----
OBTER usuários arriscados | [OBTER https://graph.microsoft.com/v1.0/identityProtection/riskyUsers](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskyUsers&version=v1.0)
OBTER detecções de risco | [OBTER https://graph.microsoft.com/v1.0/identityProtection/riskDetections](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskDetections&version=v1.0)
OBTER o histórico de riscos de um usuário | [OBTER https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/{riskyUserId}/history](https://developer.microsoft.com/graph/graph-explorer?request=identityProtection/riskyUsers/{riskyUserId}/history&version=v1.0)
CONFIRMAR um usuário como comprometido | [POST https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/confirmCompromised](https://developer.microsoft.com/graph/graph-explorer?request=/identityProtection/riskyUsers/confirmCompromised&version=v1.0)
DESCARTAR um usuário arriscado | [POST https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/dismiss](https://developer.microsoft.com/graph/graph-explorer?request=/identityProtection/riskyUsers/dismiss&version=v1.0)

## <a name="what-licenses-do-i-need"></a>De quais licenças eu preciso?

O Azure AD Identity Protection é um recurso premium. Você precisa de uma licença P1 ou P2 do Azure AD Premium para acessar a API riskDetection (observação: as licenças P1 recebem informações de risco limitadas). A API riskyUsers só está disponível para licenças do Azure AD Premium P2.

## <a name="see-also"></a>Confira também

* [Sobre o Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection)
* [Começar a trabalhar com a proteção de identidade do Azure Active Directory e o Microsoft Graph](/azure/active-directory/identity-protection/howto-identity-protection-graph-api)
