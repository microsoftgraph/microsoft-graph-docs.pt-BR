---
title: Use a proteção de identidade do Windows Azure AD API (preview)
description: Você pode usar o Microsoft Graph para consultar o recurso de identityRiskEvent para cada tipo de evento de risco detectado pelo proteção de identidade do Windows Azure AD. Esses eventos estão disponíveis para clientes com o Windows Azure AD Premium P2. Um subconjunto de eventos está disponível para clientes com o Windows Azure AD Premium P1.
author: cloudhandler
ms.openlocfilehash: 8afee9685d22dfaeea43a01f70a8b2834c8d4ff9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310371"
---
# <a name="use-the-azure-ad-identity-protection-api-preview"></a>Use a proteção de identidade do Windows Azure AD API (preview)

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Você pode usar o Microsoft Graph para consultar o recurso de [identityRiskEvent](identityriskevent.md) para cada tipo de evento de risco detectado pelo [proteção de identidade do Windows Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection). Esses eventos estão disponíveis para clientes com o Windows Azure AD Premium P2. Um subconjunto de eventos está disponível para clientes com o Windows Azure AD Premium P1.

* [entradas de endereços IP anônimos](anonymousipriskevent.md)
* [entradas de dispositivos infectados por malware](malwareriskevent.md)
* [Impossível viajar para locais atípicos](impossibletravelriskevent.md)
* [usuários com credenciais perdidas](leakedcredentialsriskevent.md)
* [entradas de endereços IP suspeitos](suspiciousipriskevent.md)
* [entradas de familiarizado locais](unfamiliarlocationriskevent.md)

Use as operações a seguir para obter essas informações associadas e eventos:

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Lista identityRiskEvent](../api/identityriskevent-get.md) |[identityRiskEvent](identityriskevent.md)| Obter a coleção de identityRiskEvent. |
|[Obter identityRiskEvent](../api/identityriskevent-get.md) |[identityRiskEvent](identityriskevent.md)| Obtenha o objeto identityRiskEvent. |
|[Lista anonymousIpRiskEvent](../api/anonymousipriskevent-get.md) |[anonymousIpRiskEvent](anonymousipriskevent.md)| Obter a coleção de anonymousIpRiskEvent. |
|[Obter anonymousIpRiskEvent](../api/anonymousipriskevent-get.md) |[anonymousIpRiskEvent](anonymousipriskevent.md)| Obtenha o objeto anonymousIpRiskEvent. |
|[Lista impossibleTravelRiskEvent](../api/impossibletravelriskevent-get.md) |[impossibleTravelRiskEvent](impossibletravelriskevent.md)| Obter a coleção de impossibleTravelRiskEvent. |
|[Obter impossibleTravelRiskEvent](../api/impossibletravelriskevent-get.md) |[impossibleTravelRiskEvent](impossibletravelriskevent.md)| Obtenha o objeto impossibleTravelRiskEvent. |
|[Lista leakedCredentialsRiskEvent](../api/leakedcredentialsriskevent-get.md) |[leakedCredentialsRiskEvent](leakedcredentialsriskevent.md)| Obter a coleção de leakedCredentialsRiskEvent. |
|[Obter leakedCredentialsRiskEvent](../api/leakedcredentialsriskevent-get.md) |[leakedCredentialsRiskEvent](leakedcredentialsriskevent.md)| Obtenha o objeto leakedCredentialsRiskEvent. |
|[Lista malwareRiskEvent](../api/malwareriskevent-get.md) |[malwareRiskEvent](malwareriskevent.md)| Obter a coleção de malwareRiskEvent. |
|[Obter malwareRiskEvent](../api/malwareriskevent-get.md) |[malwareRiskEvent](malwareriskevent.md)| Obtenha o objeto malwareRiskEvent. |
|[Lista suspiciousIpRiskEvent](../api/suspiciousipriskevent-get.md) |[suspiciousIpRiskEvent](suspiciousipriskevent.md)| Obter a coleção de suspiciousIpRiskEvent. |
|[Obter suspiciousIpRiskEvent](../api/suspiciousipriskevent-get.md) |[suspiciousIpRiskEvent](suspiciousipriskevent.md)| Obtenha o objeto suspiciousIpRiskEvent. |
|[Lista unfamiliarLocationRiskEvent](../api/unfamiliarlocationriskevent-get.md) |[unfamiliarLocationRiskEvent](unfamiliarlocationriskevent.md)| Obter a coleção de unfamiliarLocationRiskEvent. |
|[Obter unfamiliarLocationRiskEvent](../api/unfamiliarlocationriskevent-get.md) |[unfamiliarLocationRiskEvent](unfamiliarlocationriskevent.md)| Obtenha o objeto unfamiliarLocationRiskEvent. |

# <a name="see-also"></a>Confira também

* [Sobre a proteção de identidade do Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection)
* [Noções básicas sobre proteção de identidade do Windows Azure Active Directory e do Microsoft Graph](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection-graph-getting-started)
