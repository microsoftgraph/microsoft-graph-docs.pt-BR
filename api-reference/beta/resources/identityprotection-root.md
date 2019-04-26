---
title: Usar a API de proteção de identidade do Azure AD (versão prévia)
description: Você pode usar o Microsoft Graph para consultar o recurso identityRiskEvent para cada tipo de evento de risco detectado pela proteção de identidade do Azure AD. Esses eventos estão disponíveis para clientes com o Azure AD Premium P2. Um subconjunto de eventos está disponível para clientes com o Azure AD Premium P1.
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 892387c3149f7492b5494a02bbd5e4200cc7757c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340258"
---
# <a name="use-the-azure-ad-identity-protection-api-preview"></a>Usar a API de proteção de identidade do Azure AD (versão prévia)

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode usar o Microsoft Graph para consultar o recurso [identityRiskEvent](identityriskevent.md) para cada tipo de evento de risco detectado pela [proteção de identidade do Azure ad](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection). Esses eventos estão disponíveis para clientes com o Azure AD Premium P2. Um subconjunto de eventos está disponível para clientes com o Azure AD Premium P1.

* [entradas de endereços IP anônimos](anonymousipriskevent.md)
* [entradas de dispositivos infectados por malware](malwareriskevent.md)
* [impossível viajar para locais atypical](impossibletravelriskevent.md)
* [usuários com credenciais vazadas](leakedcredentialsriskevent.md)
* [entradas de endereços IP suspeitos](suspiciousipriskevent.md)
* [entradas de locais desconhecidos](unfamiliarlocationriskevent.md)

Use as operações a seguir para obter estes eventos e informações associadas:

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar identityRiskEvent](../api/identityriskevent-get.md) |[identityRiskEvent](identityriskevent.md)| Obtém a coleção identityRiskEvent. |
|[Obter identityRiskEvent](../api/identityriskevent-get.md) |[identityRiskEvent](identityriskevent.md)| Obtém o objeto identityRiskEvent. |
|[Listar anonymousIpRiskEvent](../api/anonymousipriskevent-get.md) |[anonymousIpRiskEvent](anonymousipriskevent.md)| Obtém a coleção anonymousIpRiskEvent. |
|[Obter anonymousIpRiskEvent](../api/anonymousipriskevent-get.md) |[anonymousIpRiskEvent](anonymousipriskevent.md)| Obtém o objeto anonymousIpRiskEvent. |
|[Listar impossibleTravelRiskEvent](../api/impossibletravelriskevent-get.md) |[impossibleTravelRiskEvent](impossibletravelriskevent.md)| Obtém a coleção impossibleTravelRiskEvent. |
|[Obter impossibleTravelRiskEvent](../api/impossibletravelriskevent-get.md) |[impossibleTravelRiskEvent](impossibletravelriskevent.md)| Obtém o objeto impossibleTravelRiskEvent. |
|[Listar leakedCredentialsRiskEvent](../api/leakedcredentialsriskevent-get.md) |[leakedCredentialsRiskEvent](leakedcredentialsriskevent.md)| Obtém a coleção leakedCredentialsRiskEvent. |
|[Obter leakedCredentialsRiskEvent](../api/leakedcredentialsriskevent-get.md) |[leakedCredentialsRiskEvent](leakedcredentialsriskevent.md)| Obtém o objeto leakedCredentialsRiskEvent. |
|[Listar malwareRiskEvent](../api/malwareriskevent-get.md) |[malwareRiskEvent](malwareriskevent.md)| Obtém a coleção malwareRiskEvent. |
|[Obter malwareRiskEvent](../api/malwareriskevent-get.md) |[malwareRiskEvent](malwareriskevent.md)| Obtém o objeto malwareRiskEvent. |
|[Listar suspiciousIpRiskEvent](../api/suspiciousipriskevent-get.md) |[suspiciousIpRiskEvent](suspiciousipriskevent.md)| Obtém a coleção suspiciousIpRiskEvent. |
|[Obter suspiciousIpRiskEvent](../api/suspiciousipriskevent-get.md) |[suspiciousIpRiskEvent](suspiciousipriskevent.md)| Obtém o objeto suspiciousIpRiskEvent. |
|[Listar unfamiliarLocationRiskEvent](../api/unfamiliarlocationriskevent-get.md) |[unfamiliarLocationRiskEvent](unfamiliarlocationriskevent.md)| Obtém a coleção unfamiliarLocationRiskEvent. |
|[Obter unfamiliarLocationRiskEvent](../api/unfamiliarlocationriskevent-get.md) |[unfamiliarLocationRiskEvent](unfamiliarlocationriskevent.md)| Obtém o objeto unfamiliarLocationRiskEvent. |

# <a name="see-also"></a>Confira também

* [Sobre a proteção de identidade do Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection)
* [Introdução à proteção de identidade do Azure Active Directory e ao Microsoft Graph](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection-graph-getting-started)
