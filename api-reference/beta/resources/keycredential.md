---
title: Tipo de recurso keyCredential
description: Contém uma credencial de chave associada a um aplicativo ou uma entidade de serviço. A **propriedade keyCredentials** das entidades application and servicePrincipal é uma coleção de **keyCredential**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 8095ea20d6c7dcef94e9f9cf2e42fca6087c58d8
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58265971"
---
# <a name="keycredential-resource-type"></a>Tipo de recurso keyCredential

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém uma credencial de chave associada a um aplicativo ou uma entidade de serviço. A **propriedade keyCredentials** das entidades [application](application.md) and [servicePrincipal](serviceprincipal.md) é uma coleção **de keyCredential**.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|customKeyIdentifier|Binário| Identificador de chave personalizada |
| displayName | Cadeia de caracteres | Nome amigável para a chave. Opcional. |
|endDateTime|DateTimeOffset|A data e a hora em que a credencial expira. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|chave|Binário| Valor para a credencial de chave. Deve ser um valor codificado base 64. |
|keyId|Guid|O identificador exclusivo da chave.|
|startDateTime|DateTimeOffset|A data e a hora em que a credencial se torna válida. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|type|Cadeia de caracteres|O tipo de credencial de chave; por exemplo, `Symmetric` .|
|usage|Cadeia de caracteres|Uma cadeia de caracteres que descreve a finalidade para a qual a chave pode ser usada; por exemplo, `Verify` .|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyCredential"
}-->

```json
{
  "@odata.type": "#microsoft.graph.keyCredential",
  "customKeyIdentifier": "Binary",
  "displayName": "String",
  "endDateTime": "String (timestamp)",
  "key": "Binary",
  "keyId": "Guid",
  "startDateTime": "String (timestamp)",
  "type": "String",
  "usage": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "keyCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


