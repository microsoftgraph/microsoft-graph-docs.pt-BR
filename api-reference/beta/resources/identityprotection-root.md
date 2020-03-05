---
title: Usar as APIs de proteção de identidade do Azure AD (versão prévia)
description: Você pode usar o Microsoft Graph para consultar as APIs de proteção de identidade para receber informações sobre o risco detectado pela proteção de identidade do Azure AD.
author: cloudhandler
localization_priority: Normal
ms.prod: security
doc_type: conceptualPageType
ms.openlocfilehash: 9f2e1dbdd20645768a4cb3e14c2de9f9d9a98b7e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496758"
---
# <a name="use-the-azure-ad-identity-protection-api-preview"></a>Usar a API de proteção de identidade do Azure AD (versão prévia)

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A proteção de identidade é uma ferramenta que permite às organizações detectar, investigar e corrigir riscos baseados em identidade em seu ambiente. Você pode usar as seguintes APIs do Microsoft Graph para consultar os riscos detectados pela proteção de identidade: 

* [riskDetection](riskdetection.md) -consulta o Microsoft Graph para obter uma lista de detecções de riscos vinculados de usuário e de entrada e informações associadas sobre a detecção. As detecções de risco na proteção de identidade do Azure AD incluem qualquer ação suspeita identificada relacionada às contas de usuário no diretório.

* [riskyUsers](riskyuser.md) – consulta o Microsoft Graph para obter informações sobre os usuários que a proteção de identidade detectou como arriscado. O risco do usuário representa a probabilidade de que uma determinada identidade ou conta seja comprometida. Esses riscos são calculados offline usando fontes de inteligência de ameaças internas e externas da Microsoft, incluindo pesquisadores de segurança, profissionais de imposição de leis, equipes de segurança da Microsoft e outras fontes confiáveis.

* [Sign](signin.md) -in – consultar o Microsoft Graph para obter informações sobre as entradas do Azure AD com propriedades específicas relacionadas ao estado, detalhes e nível do risco. Um risco de entrada representa a probabilidade de que uma determinada solicitação de autenticação não seja autorizada pelo proprietário da identidade. Esses riscos podem ser calculados em tempo real ou calculados offline usando fontes de inteligência de ameaças internas e externas da Microsoft, incluindo pesquisadores de segurança, profissionais de imposição de leis, equipes de segurança da Microsoft e outras fontes confiáveis.

* [identityRiskEvents](identityriskevent.md) – consulta o Microsoft Graph para obter uma lista de detecções de risco e informações associadas. Essa API foi preterida; Recomendamos que você use **riskDetections** em vez disso.

>[!NOTE]
>A API **identityRiskEvents** foi preterida e interromperá o retorno de dados em 10 de janeiro de 2020. Para obter detalhes, consulte [Preterition of the IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).

## <a name="see-also"></a>Confira também

* [Sobre a proteção de identidade do Azure Active Directory](https://docs.microsoft.com/azure/active-directory/identity-protection/overview-identity-protection)
* [Introdução à proteção de identidade do Azure Active Directory e ao Microsoft Graph](https://docs.microsoft.com/azure/active-directory/identity-protection/howto-identity-protection-graph-api)
