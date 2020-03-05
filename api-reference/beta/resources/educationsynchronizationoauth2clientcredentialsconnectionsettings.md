---
title: recurso educationSynchronizationOAuth2ClientCredentialsConnectionSettings
description: Quando a concessão de credenciais de cliente do OAuth2 for usada para se conectar ao provedor de dados, esse tipo de configuração de conexão deverá ser usado para configurar o perfil.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d38853e40d8f88bf4aa8323395848185793cc42c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500090"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a>recurso educationSynchronizationOAuth2ClientCredentialsConnectionSettings

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Quando a [concessão de credenciais de cliente do OAuth2](https://tools.ietf.org/html/rfc6749#section-4.4) for usada para se conectar ao provedor de dados, esse tipo de configuração de conexão deverá ser usado para configurar o perfil.

Derivado de [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-|:-|:-|
| **tokenUrl** | String | A URL para obter tokens de acesso para o provedor de dados. |
| **scope** | String | [O escopo da solicitação de acesso](https://tools.ietf.org/html/rfc6749#section-3.3). |

## <a name="json-representation"></a>Representação JSON
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings",
    "clientId": "String",
    "clientSecret": "String",
    "tokenUrl": "String",
    "scope": "String"
}
```
