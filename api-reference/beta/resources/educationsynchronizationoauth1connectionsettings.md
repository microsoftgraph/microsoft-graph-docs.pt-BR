---
title: recurso educationSynchronizationOAuth1ConnectionSettings
description: Quando o OAuth1 é usado para se conectar ao provedor de dados, esse tipo de configuração de conexão deve ser usado para configurar o perfil.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 525809121b07616c6eb5077f1b12d5b736586065
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434918"
---
# <a name="educationsynchronizationoauth1connectionsettings-resource"></a>recurso educationSynchronizationOAuth1ConnectionSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Quando o OAuth1 é usado para se conectar ao provedor de dados, esse tipo de configuração de conexão deve ser usado para configurar o perfil.

Derivado de [educationSynchronizationConnectionSettings].

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   | Descrição                                                                                                                |
| :----------- | :----- | :------------------------------------------------------------------------------------------------------------------------- |
| clientId     | Cadeia de caracteres | ID do cliente usada para se conectar ao provedor. Herdado de [educationSynchronizationConnectionSettings].                    |
| clientSecret | Cadeia de caracteres | Segredo do cliente para autenticar a conexão com o provedor. Herdado de [educationSynchronizationConnectionSettings]. |

[educationsynchronizationconnectionsettings]: educationsynchronizationconnectionsettings.md

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings"
}-->

```json
{
  "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
  "clientId": "String",
  "clientSecret": "String"
}
```
