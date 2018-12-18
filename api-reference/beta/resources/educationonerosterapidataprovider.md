---
title: recurso de educationOneRosterApiDataProvider
description: Usado para configurar o perfil de sincronização de dados da escola quando a API OneRoster é usada como a fonte de entrada.
author: mmast-msft
ms.openlocfilehash: 66c79c5e5d5ced4efcd635d2976e83887e545a9f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309566"
---
# <a name="educationonerosterapidataprovider-resource"></a>recurso de educationOneRosterApiDataProvider

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Usado para configurar o perfil de sincronização de dados da escola quando a [API OneRoster](https://www.imsglobal.org/activity/onerosterlis) é usado como a fonte de entrada.

Derivado do [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:-|:-|:-|
| **URL de conexão** | String | A URL da conexão para a instância de OneRoster. |
| **schoolsIds** | String collection |  A lista de sourcedIds escola para sincronizar. |
| **providerName** | String | O nome do provedor de serviços de OneRoster conforme definido pela [especificação OneRoster](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA). |
| **connectionSettings** | [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md) | Configurações de Conexão para a instância de OneRoster. Deve ser do tipo [educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) ou [educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md). |
| **personalizações** | [educationSynchronizationCustomizations](educationsynchronizationcustomizations.md) | Personalização opcional a ser aplicado ao perfil de sincronização.|

## <a name="json-representation"></a>Representação JSON
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationoneRosterApiDataProvider"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationoneRosterApiDataProvider",
    "connectionUrl": "String",
    "providerName": "String",
    "schoolsIds": [
        "String"
    ],
    "connectionSettings": {
        "@odata.type": "#microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
        "clientId": "String",
        "clientSecret": "String",
    },
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
