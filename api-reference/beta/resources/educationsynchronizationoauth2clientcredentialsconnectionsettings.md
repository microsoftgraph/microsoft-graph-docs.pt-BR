---
title: recurso educationSynchronizationOAuth2ClientCredentialsConnectionSettings
description: Quando a concessão de credenciais de cliente do OAuth2 for usada para se conectar ao provedor de dados, esse tipo de configuração de conexão deverá ser usado para configurar o perfil.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 00e1e531ff33f28a2e63f76925cd0b4e7759696b
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434904"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a>recurso educationSynchronizationOAuth2ClientCredentialsConnectionSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Quando a [concessão de credenciais de cliente do OAuth2](https://tools.ietf.org/html/rfc6749#section-4.4) for usada para se conectar ao provedor de dados, esse tipo de configuração de conexão deverá ser usado para configurar o perfil.

Derivado de [educationSynchronizationConnectionSettings].

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   | Descrição                                                                                                                |
| :----------- | :----- | :------------------------------------------------------------------------------------------------------------------------- |
| clientId     | Cadeia de caracteres | ID do cliente usada para se conectar ao provedor. Herdado de [educationSynchronizationConnectionSettings].                    |
| clientSecret | Cadeia de caracteres | Segredo do cliente para autenticar a conexão com o provedor. Herdado de [educationSynchronizationConnectionSettings]. |
| tokenUrl     | Cadeia de caracteres | A URL para obter tokens de acesso para o provedor de dados.                                                                        |
| escopo        | String | O escopo da solicitação de acesso (consulte [RFC6749](https://tools.ietf.org/html/rfc6749#section-3.3)).                          |

[educationsynchronizationconnectionsettings]: educationsynchronizationconnectionsettings.md

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
