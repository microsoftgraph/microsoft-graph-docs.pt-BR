---
title: Tipo de recurso educationResource
description: Uma classe base para todos os objetos de recurso no sistema.
ms.localizationpriority: medium
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e5da9bdd3a9c1046949c5be36b6c7f1ccc79709a
ms.sourcegitcommit: 0a312d63934cdf9789a5648c2b3f348f48542ff4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/07/2021
ms.locfileid: "60219776"
---
# <a name="educationresource-resource-type"></a>Tipo de recurso educationResource

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma classe base para [educationExcelResource](../resources/educationexcelresource.md), [educationFileResource](../resources/educationfileresource.md), [educationLinkResource](../resources/educationlinkresource.md), [educationPowerPointResource](../resources/educationpowerpointresource.md), [educationWordResource](../resources/educationwordresource.md), [educationMediaResource](../resources/educationmediaresource.md) e [educationExternalResource](../resources/educationexternalresource.md).

Um educationResource está associado [a](educationassignment.md) uma atribuição e/ou [envio](educationsubmission.md), que representa o objeto de aprendizagem que está sendo entregue ou entregue. Não é possível instaurá-lo diretamente; você deve fazer uma subclasse que representará o tipo de recurso que está sendo usado.

Esse recurso armazena as propriedades comuns em todos os tipos de recursos.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|createdBy|[identitySet](identityset.md)|Who criou o recurso.|
|createdDateTime|Momento no tempo em que o recurso foi criado.  DateTimeOffset|O tipo de carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|displayName|Cadeia de caracteres|Nome de exibição do recurso.|
|lastModifiedBy|[identitySet](identityset.md)|Who foi o último usuário a modificar o recurso.|
|lastModifiedDateTime|DateTimeOffset|Momento no tempo em que o recurso foi modificado pela última vez.  O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationResource"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


