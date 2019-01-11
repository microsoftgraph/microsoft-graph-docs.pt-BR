---
title: recurso de educationSynchronizationOAuth2ClientCredentialsConnectionSettings
description: Quando OAuth2 Grant de credenciais de cliente será usado para se conectar ao provedor de dados, esse tipo de configurações de conexão deve ser usado para configurar o perfil.
localization_priority: Normal
ms.openlocfilehash: 49a0a267ddb3a8f3a954888679806ea7913e24f0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822579"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a>recurso de educationSynchronizationOAuth2ClientCredentialsConnectionSettings

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Quando [OAuth2 Grant de credenciais de cliente](https://tools.ietf.org/html/rfc6749#section-4.4) será usado para se conectar ao provedor de dados, esse tipo de configurações de conexão deve ser usado para configurar o perfil.

Derivado do [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-|:-|:-|
| **tokenUrl** | Cadeia de caracteres | A URL para obter tokens de acesso para o provedor de dados. |
| **scope** | Cadeia de caracteres | [O escopo da solicitação de acesso](https://tools.ietf.org/html/rfc6749#section-3.3). |

## <a name="json-representation"></a>Representação JSON
<!-- {
  "blockType": "resource",
  "@odata.type": "#microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings"
}-->

```json
"connectionSettings": {
    "@odata.type": "#microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings",
    "clientId": "String",
    "clientSecret": "String",
    "tokenUrl": "String",
    "scope": "String"
}
```
