---
title: Tipo de recurso plannerExternalReference
description: O **recurso plannerExternalReference** representa os metadados de uma referência (anexos como arquivo, URL). É o valor de pares de valor de propriedade no objeto externalReferences.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 536e7b6a933ffdad610bf6cce561b2546d60e5d2
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722311"
---
# <a name="plannerexternalreference-resource-type"></a>Tipo de recurso plannerExternalReference

Namespace: microsoft.graph

O **recurso plannerExternalReference** representa os metadados de uma referência (anexos como arquivo, URL). É o valor de pares de valor de propriedade no [objeto externalReferences](plannerexternalreferences.md).



## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|alias|Cadeia de caracteres|Um alias de nome para descrever a referência.|
|lastModifiedBy|[identitySet](identityset.md)|Somente leitura. ID do usuário pela qual foi modificada pela última vez.|
|lastModifiedDateTime|DateTimeOffset|Somente leitura. Data e hora em que isso foi modificado pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|previewPriority|Cadeia de caracteres|Usado para definir a ordem de prioridade relativa na qual a referência será mostrada como uma visualização na tarefa.|
|tipo|Cadeia de caracteres|Usado para descrever o tipo da referência. Os tipos `PowerPoint` incluem: `Word` , , , `Excel` `Other` .|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerExternalReference"
}-->

```json
{
  "alias": "String",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "previewPriority": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerExternalReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

