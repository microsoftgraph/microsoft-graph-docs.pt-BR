---
title: tipo de recurso educationResource
description: Uma superclasse para todos os objetos de recurso no sistema. Um recurso é associado a uma **atribuição** e/ou **envio**, que representa o objeto de aprendizado que está sendo
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: dc2c1c4ecd6ce7b57992637bfdcf9a1523265f90
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501091"
---
# <a name="educationresource-resource-type"></a>tipo de recurso educationResource

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma superclasse para todos os objetos de recurso no sistema. Um recurso é associado a uma **atribuição** e/ou **envio**, que representa o objeto de aprendizado que está sendo entregue ou entregue. Você não pode criar uma instância de um recurso diretamente; Você deve criar uma subclasse que representará o tipo de recurso que está sendo usado.

Esse recurso armazena as propriedades comuns em todos os tipos de recurso.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|createdBy|[identitySet](identityset.md)|Quem criou o recurso.|
|createdDateTime|Momento no momento em que o recurso foi criado.  DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|displayName|String|Exibe o nome do recurso.|
|lastModifiedBy|[identitySet](identityset.md)|Quem foi o último usuário a modificar o recurso.|
|lastModifiedDateTime|DateTimeOffset|Momento no momento em que o recurso foi modificado pela última vez.  O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|

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
