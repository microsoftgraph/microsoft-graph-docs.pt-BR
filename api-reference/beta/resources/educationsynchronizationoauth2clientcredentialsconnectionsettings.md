---
title: recurso educationSynchronizationOAuth2ClientCredentialsConnectionSettings
description: Quando a concessão de credenciais de cliente do OAuth2 for usada para se conectar ao provedor de dados, esse tipo de configuração de conexão deverá ser usado para configurar o perfil.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ffc3af93a90ba0d6991007a64d24b9fb776e8bc8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972366"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a>recurso educationSynchronizationOAuth2ClientCredentialsConnectionSettings

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
