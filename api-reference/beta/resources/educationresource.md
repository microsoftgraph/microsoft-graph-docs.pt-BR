---
title: Tipo de recurso educationResource
description: Uma classe base para todos os objetos de recurso no sistema.
ms.localizationpriority: medium
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 1af5cb6ae12eb435b6335d902430fdbc717fcd25
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461363"
---
# <a name="educationresource-resource-type"></a>Tipo de recurso educationResource

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma classe base para [educationExcelResource](../resources/educationexcelresource.md), [educationFileResource](../resources/educationfileresource.md), [educationLinkResource](../resources/educationlinkresource.md), [educationPowerPointResource](../resources/educationpowerpointresource.md), [educationWordResource](../resources/educationwordresource.md), [educationMediaResource](../resources/educationmediaresource.md), [educationExternalResource](../resources/educationexternalresource.md) e [educationTeamsAppResource](../resources/educationteamsappresource.md).

Um educationResource está [associado a uma](educationassignment.md) tarefa e/ou [envio, que](educationsubmission.md) representa o objeto de aprendizado que está sendo entregue ou entregue. Você não pode instanciar um recurso diretamente; você deve criar uma subclasse que representará o tipo de recurso que está sendo usado.

Esse recurso armazena as propriedades comuns em todos os tipos de recursos.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|createdBy|[identitySet](identityset.md)|Who criou o recurso.|
|createdDateTime|Momento no tempo em que o recurso foi criado.  DateTimeOffset|O tipo de carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|displayName|String|Nome de exibição do recurso.|
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


