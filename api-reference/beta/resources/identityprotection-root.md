---
title: Usar as APIs de proteção de identidade do Azure AD
description: Você pode usar o Microsoft Graph para consultar as APIs do Identity Protection para receber informações sobre o risco detectado pelo Azure AD Identity Protection.
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 712aa53234f8917fec334c52234db8155f1e913e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129384"
---
# <a name="use-the-azure-ad-identity-protection-api"></a>Usar a API de proteção de identidade do Azure AD

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O Identity Protection é uma ferramenta que permite que as organizações descubram, investiguem e remediam riscos baseados em identidade em seu ambiente. Você pode usar as seguintes APIs do Microsoft Graph para consultar os riscos detectados pelo Identity Protection: 

* [riskDetection](riskdetection.md) - Consulte o Microsoft Graph para obter uma lista de detecções de risco vinculado de usuário e de login e informações associadas sobre a detecção. As detecções de risco no Azure AD Identity Protection incluem ações suspeitas identificadas relacionadas a contas de usuário no diretório.

* [riskyUsers](riskyuser.md) - Consulte o Microsoft Graph para obter informações sobre usuários que a Proteção de Identidade detectou como arriscadas. O risco do usuário representa a probabilidade de que uma determinada identidade ou conta seja comprometida. Esses riscos são calculados offline usando as fontes de inteligência contra ameaças internas e externas da Microsoft, incluindo pesquisadores de segurança, profissionais de aplicação da lei, equipes de segurança da Microsoft e outras fontes confiáveis.

* [signIn](signin.md) - Consulte o Microsoft Graph para obter informações sobre as instalações do Azure AD com propriedades específicas relacionadas ao estado, detalhes e nível de risco. Um risco de login representa a probabilidade de que uma determinada solicitação de autenticação não seja autorizada pelo proprietário da identidade. Esses riscos podem ser calculados em tempo real ou offline usando as fontes de inteligência contra ameaças internas e externas da Microsoft, incluindo pesquisadores de segurança, profissionais da lei, equipes de segurança da Microsoft e outras fontes confiáveis.

* [identityRiskEvents](identityriskevent.md) - Consulte o Microsoft Graph para obter uma lista de detecções de risco e informações associadas. Essa API foi preterida; em vez disso, recomendamos que você use **riskDetections.**

>[!CAUTION]
>A API **identityRiskEvents** foi preterida e interromperá o retorno de dados em 10 de janeiro de 2020. Para obter detalhes, [consulte Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).

## <a name="see-also"></a>Confira também

* [Sobre o Azure Active Directory Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection)
* [Começar a trabalhar com a proteção de identidade do Azure Active Directory e o Microsoft Graph](/azure/active-directory/identity-protection/howto-identity-protection-graph-api)
