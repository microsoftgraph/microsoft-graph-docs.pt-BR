---
title: recurso educationOneRosterApiDataProvider
description: Usado para configurar o perfil de sincronização de dados escolares quando a API do OneRoster é usada como a fonte de entrada.
author: mmast-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 538f3740fafc3c0debe6dacd8b0a76c81c14a228
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695703"
---
# <a name="educationonerosterapidataprovider-resource"></a>recurso educationOneRosterApiDataProvider

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado para configurar o perfil de sincronização de dados escolares quando a [API do OneRoster](https://www.imsglobal.org/activity/onerosterlis) é usada como a fonte de entrada.

Derivado de [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).

## <a name="properties"></a>Propriedades

| Propriedade           | Tipo                                         | Descrição                                                                                           |
| :----------------- | :------------------------------------------- | :---------------------------------------------------------------------------------------------------- |
| connectionUrl      | String                                       | A URL da conexão com a instância do OneRoster.                                                         |
| providerName       | String                                       | O nome do Provedor de Serviços do OneRoster conforme definido pela [especificação do OneRoster][oneroster].           |
| schoolsIds         | Coleção de cadeias de caracteres                            | A lista de [Escola/Organização a][orgs] `sourcedId` ser sincronizada.                                                   |
| termIds            | Coleção de cadeias de caracteres                            | A lista de [sessões acadêmicas][terms] a sincronizar.                                                       |
| connectionSettings | [educationSynchronizationConnectionSettings] | As [configurações OAuth 1.0][onerosteroauth1] ou [OAuth 2.0][onerosteroauth2] para a instância do OneRoster. |
| personalizações     | [educationSynchronizationCustomizations]    | Personalização opcional a ser aplicada ao perfil de sincronização.                                  |

> [!IMPORTANT]
> O OneRoster usa sessões acadêmicas em vez de um único ano escolar para segmentar seus dados. Essa segmentação é abstraida dentro School Data Sync interface do usuário, mas não essa API. Você precisará chamar o ponto de extremidade do OneRoster para obter a coleção de IDs de sessão acadêmica para preencher `/terms` a `termIds` coleção.

[educationSynchronizationConnectionSettings]: educationsynchronizationconnectionsettings.md
[educationsynchronizationcustomizations]: educationsynchronizationcustomizations.md
[oneroster]: https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA
[onerosteroauth2]: educationsynchronizationoauth2clientcredentialsconnectionsettings.md
[onerosteroauth1]: educationsynchronizationoauth1connectionsettings.md
[terms]: https://www.imsglobal.org/oneroster-v11-final-specification#_Toc480452034
[orgs]: https://www.imsglobal.org/oneroster-v11-final-specification#_Toc480452016

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  truncated: true,
  "optionalProperties": [

  ],
  "@odata.type&quot;: &quot;microsoft.graph.educationoneRosterApiDataProvider"
}-->

```json
{
  "@odata.type": "microsoft.graph.educationoneRosterApiDataProvider",
  "connectionUrl": "String",
  "providerName": "String",
  "schoolsIds": ["String"],
  "termIds": ["String"],
  "connectionSettings": {
    "@odata.type": "microsoft.graph.educationSynchronizationConnectionSettings",
    "clientId": "String",
    "clientSecret&quot;: &quot;String"
  },
  "customizations": {
    "@odata.type&quot;: &quot;microsoft.graph.educationSynchronizationCustomizations"
  }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2020-05-06 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  truncated: true,
  "description": "educationOneRosterApiDataProvider resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
      "Error: microsoft.graph.educationoneRosterApiDataProvider/connectionSettings:\r\n      Referenced type microsoft.graph.educationSynchronizationConnectionSettings is not defined in the doc set! Potential suggestion: microsoft.graph.ediscovery.settings"
  ]
}-->


