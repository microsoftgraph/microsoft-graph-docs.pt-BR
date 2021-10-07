---
title: Usar as APIs de proteção de identidade do Azure AD
description: Você pode usar o Microsoft Graph para consultar as APIs de Proteção de Identidade para receber informações sobre o risco detectado pela Proteção de Identidade do Azure AD.
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: conceptualPageType
ms.openlocfilehash: 37fef748455df6511eedd631332d453a5feaaf77
ms.sourcegitcommit: 0a312d63934cdf9789a5648c2b3f348f48542ff4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/07/2021
ms.locfileid: "60220651"
---
# <a name="use-the-azure-ad-identity-protection-api"></a>Usar a API de proteção de identidade do Azure AD

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A Proteção de Identidade é uma ferramenta que permite que as organizações descubram, investiguem e correção de riscos baseados em identidade em seu ambiente. Você pode usar as seguintes APIs Graph Microsoft para consultar os riscos detectados pela Proteção de Identidade: 

* [riskDetection](riskdetection.md) - Consulte a Microsoft Graph para obter uma lista de detecções de risco vinculadas de usuário e de login e informações associadas sobre a detecção. As detecções de risco na Proteção de Identidade do Azure AD incluem quaisquer ações suspeitas identificadas relacionadas a contas de usuário no diretório.

* [riskyUsers](riskyuser.md) - Consulte o Microsoft Graph informações sobre usuários que a Proteção de Identidade detectou como arriscada. O risco do usuário representa a probabilidade de que uma determinada identidade ou conta seja comprometida. Esses riscos são calculados offline usando as fontes internas e externas de inteligência contra ameaças da Microsoft, incluindo pesquisadores de segurança, profissionais de aplicação da lei, equipes de segurança na Microsoft e outras fontes confiáveis.

* [signIn](signin.md) - Consulte o Microsoft Graph informações sobre as instalações do Azure AD com propriedades específicas relacionadas ao estado de risco, detalhes e nível. Um risco de entrar representa a probabilidade de que uma determinada solicitação de autenticação não seja autorizada pelo proprietário da identidade. Esses riscos podem ser calculados em tempo real ou calculados offline usando as fontes de inteligência de ameaças internas e externas da Microsoft, incluindo pesquisadores de segurança, profissionais de aplicação da lei, equipes de segurança na Microsoft e outras fontes confiáveis.


>[!CAUTION]
>A **API identityRiskEvents** está preterida e interromperá o retorno de dados em 10 de janeiro de 2020. Para obter detalhes, [consulte Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).

## <a name="see-also"></a>Confira também

* [Sobre Azure Active Directory Proteção de Identidade](/azure/active-directory/identity-protection/overview-identity-protection)
* [Começar a Azure Active Directory proteção de identidade e o Microsoft Graph](/azure/active-directory/identity-protection/howto-identity-protection-graph-api)
