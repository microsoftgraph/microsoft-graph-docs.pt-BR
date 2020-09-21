---
title: recurso educationSynchronizationOAuth1ConnectionSettings
description: Quando o OAuth1 é usado para se conectar ao provedor de dados, esse tipo de configuração de conexão deve ser usado para configurar o perfil.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a73876185469ab762a08f409028880a4f7234d45
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989624"
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


