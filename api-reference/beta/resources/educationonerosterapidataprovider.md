---
title: recurso educationOneRosterApiDataProvider
description: Usado para configurar o perfil de sincronização de dados da escola quando a API OneRoster é usada como a fonte de entrada.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 540a508ae3ac7d2b2ecf0f4cec2862b1331e4958
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501525"
---
# <a name="educationonerosterapidataprovider-resource"></a>recurso educationOneRosterApiDataProvider

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado para configurar o perfil de sincronização de dados da escola quando a [API OneRoster](https://www.imsglobal.org/activity/onerosterlis) é usada como a fonte de entrada.

Derivado de [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-|:-|:-|
| **connectionUrl** | String | A URL de conexão para a instância do OneRoster. |
| **schoolsIds** | String collection |  A lista de sourcedIds escolar a ser sincronizada. |
| **providerName** | String | O nome do provedor de serviços do OneRoster conforme definido pela [especificação OneRoster](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA). |
| **connectionSettings** | [Microsoft. Graph. educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md) | Configurações de conexão para a instância do OneRoster. Deve ser do tipo [Microsoft. Graph. educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) ou [Microsoft. Graph. educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md). |
| **personalizações** | [Microsoft. Graph. educationSynchronizationCustomizations](educationsynchronizationcustomizations.md) | Personalização opcional a ser aplicada ao perfil de sincronização.|

## <a name="json-representation"></a>Representação JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationoneRosterApiDataProvider"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationoneRosterApiDataProvider",
    "connectionUrl": "String",
    "providerName": "String",
    "schoolsIds": [
        "String"
    ],
    "connectionSettings": {
        "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
        "clientId": "String",
        "clientSecret": "String",
    },
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
