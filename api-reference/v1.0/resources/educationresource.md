---
title: Tipo de recurso educationResource
description: Uma superclasse para todos os objetos de recurso no sistema.
ms.localizationpriority: medium
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e13ce13fd6bba8a67b1b10103d0c5225736b8360
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59036603"
---
# <a name="educationresource-resource-type"></a>Tipo de recurso educationResource

Namespace: microsoft.graph

Uma superclasse para todos os objetos de recurso no sistema. Um recurso é associado a um **Assignment** and/or **Submission**, que representa o objeto de aprendizagem que está sendo entregue ou entregue. Não é possível instaurá-lo diretamente; você deve fazer uma subclasse que representará o tipo de recurso que está sendo usado.

Esse recurso armazena as propriedades comuns em todos os tipos de recursos.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|createdBy|[identitySet](identityset.md)|O indivíduo que criou o recurso.|
|createdDateTime|DateTimeOffset|Momento no tempo em que o recurso foi criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|displayName|Cadeia de caracteres|Nome de exibição do recurso.|
|lastModifiedBy|[identitySet](identityset.md)|O último usuário a modificar o recurso.|
|lastModifiedDateTime|DateTimeOffset|Momento no tempo em que o recurso foi modificado pela última vez.  O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|

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


