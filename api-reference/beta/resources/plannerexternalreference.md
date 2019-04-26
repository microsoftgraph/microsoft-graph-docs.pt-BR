---
title: tipo de recurso plannerExternalReference
description: O recurso **plannerExternalReference** representa os metadados de uma referência (anexos como arquivo, URL). É o valor dos pares propriedade-valor no objeto externalReferences.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 6d2bce70afbeee3848f3055530daf732afe8a2b5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344820"
---
# <a name="plannerexternalreference-resource-type"></a>tipo de recurso plannerExternalReference

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **plannerExternalReference** representa os metadados de uma referência (anexos como arquivo, URL). É o valor dos pares propriedade-valor no [objeto externalReferences](plannerexternalreferences.md).



## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|alias|Cadeia de caracteres|Um alias de nome para descrever a referência.|
|lastModifiedBy|[identitySet](identityset.md)|Somente leitura. ID de usuário pela qual esta foi modificada pela última vez.|
|lastModifiedDateTime|DateTimeOffset|Somente leitura. Data e hora da última modificação. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|previewPriority|String|Usado para definir a ordem de prioridade relativa na qual a referência será mostrada como uma visualização na tarefa.|
|type|String|Usado para descrever o tipo da referência. Os tipos incluem `PowerPoint`: `Word`, `Excel`, `Other`,.|

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
<!--
{
  "type": "#page.annotation",
  "description": "plannerExternalReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
