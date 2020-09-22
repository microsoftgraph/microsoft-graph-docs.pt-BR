---
title: recurso educationOneRosterApiDataProvider
description: Usado para configurar o perfil de sincronização de dados da escola quando a API OneRoster é usada como a fonte de entrada.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5b96322cdb408069136a46aa9c83cf363cc1b6f2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998842"
---
# <a name="educationonerosterapidataprovider-resource"></a>recurso educationOneRosterApiDataProvider

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado para configurar o perfil de sincronização de dados da escola quando a [API OneRoster](https://www.imsglobal.org/activity/onerosterlis) é usada como a fonte de entrada.

Derivado de [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).

## <a name="properties"></a>Propriedades

| Propriedade           | Tipo                                         | Descrição                                                                                           |
| :----------------- | :------------------------------------------- | :---------------------------------------------------------------------------------------------------- |
| connectionUrl      | String                                       | A URL de conexão para a instância do OneRoster.                                                         |
| providerName       | String                                       | O nome do provedor de serviços do OneRoster conforme definido pela [especificação OneRoster][oneroster].           |
| schoolsIds         | Coleção de cadeias de caracteres                            | A lista de [escolas/org][orgs] `sourcedId` a ser sincronizada.                                                   |
| termIds            | Coleção de cadeias de caracteres                            | A lista de [sessões acadêmicas][terms] a serem sincronizadas.                                                       |
| connectionSettings | [educationSynchronizationConnectionSettings] | As configurações do [oauth 1,0][onerosteroauth1] ou [OAuth 2,0][onerosteroauth2] para a instância do OneRoster. |
| personalizações     | [educationSynchronizationCustomizations])    | Personalização opcional a ser aplicada ao perfil de sincronização.                                  |

> [!IMPORTANT]
> O OneRoster usa sessões acadêmicas em vez de um único ano escolar para segmentar seus dados. Essa segmentação é dissociada na interface de usuário de sincronização de dados da escola, mas não esta API. Você precisará chamar o ponto de `/terms` extremidade do OneRoster para obter a coleção de IDs de sessão acadêmica a fim de preencher a `termIds` coleção.

[educationsynchronizationconnectionsettings]: educationsynchronizationconnectionsettings.md
[educationsynchronizationcustomizations]: educationsynchronizationcustomizations.md
[oneroster]: https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA
[onerosteroauth2]: educationsynchronizationoauth2clientcredentialsconnectionsettings.md
[onerosteroauth1]: educationsynchronizationoauth1connectionsettings.md
[terms]: https://www.imsglobal.org/oneroster-v11-final-specification#_Toc480452034
[orgs]: https://www.imsglobal.org/oneroster-v11-final-specification#_Toc480452016

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
  "schoolsIds": ["String"],
  "termIds": ["String"],
  "connectionSettings": {
    "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
    "clientId": "String",
    "clientSecret": "String"
  },
  "customizations": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomizations"
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2020-05-06 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOneRosterApiDataProvider resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
      "Error: microsoft.graph.educationoneRosterApiDataProvider/connectionSettings:\r\n      Referenced type microsoft.graph.educationSynchronizationConnectionSettings is not defined in the doc set! Potential suggestion: microsoft.graph.settings"
  ]
}-->


