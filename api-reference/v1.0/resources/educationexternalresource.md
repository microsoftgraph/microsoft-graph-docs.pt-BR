---
title: Tipo de recurso educationExternalResource
description: Uma subclasse de educationResource. Esse é o serviço padrão de atribuições de tipo de recurso usado para mapear todos os recursos que não expomos ao grafo. Isso permite que todos os chamadores do SDK funcionem perfeitamente.
ms.localizationpriority: medium
author: cristobal-buenrostro
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a692ff228b8df5543b94acb340d215b57912762a
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/06/2022
ms.locfileid: "64684869"
---
# <a name="educationexternalresource-resource-type"></a>Tipo de recurso educationExternalResource

Namespace: microsoft.graph

Representa um tipo genérico para mapear recursos não expostos no Microsoft Graph.

Herda de [educationResource](educationresource.md).

Esse tipo complexo permite que todos os chamadores do SDK funcionem perfeitamente.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|webUrl|String|Local do recurso. Obrigatório|
|createdBy|Cadeia de caracteres|O nome de exibição do usuário que criou esse objeto.|
|createdDateTime|DateTimeOffset|Data em que a reordenação foi adicionada.|
|displayName|string|O nome de exibição do recurso.|
|lastModifiedBy|[identitySet](identityset.md)|O último usuário a modificar o recurso.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que o recurso foi modificado pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.educationExternalResource"
}-->

```json
{
  "webUrl": "String",
  "createdBy": "String (User)",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "lastModifiedBy": "String (User)",
  "lastModifiedDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2021-09-21 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationExternalResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
