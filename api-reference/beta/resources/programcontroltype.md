---
title: Tipo de recurso programControlType
description: 'No recurso de revisões de acesso do Azure AD, o tipo de controle de programa é usado ao associar um controle a um programa, para indicar o tipo de revisão de acesso para o qual o controle se trata.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 58c9ee3ade6e3969de9653f54c5181a66f087ea5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960359"
---
# <a name="programcontroltype-resource-type"></a>Tipo de recurso programControlType

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No recurso de revisões de acesso do Azure [AD,](accessreviews-root.md) o tipo de controle de programa é usado ao associar um controle a um programa, para indicar o tipo de revisão de acesso para o qual o controle se trata.  

Os objetos do tipo de controle do programa são gerados automaticamente quando o administrador global inscarda o locatário para usar o recurso de críticas de acesso.  Nenhum tipo de controle de programa adicional pode ser criado.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar programControlTypes](../api/programcontroltype-list.md) | [Coleção programControlType](programcontroltype.md)| Listar tipos de controle de programa. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| id                     |Cadeia de caracteres                | O identificador atribuído ao recurso do tipo de controle do programa                                      |
| displayName            |Cadeia de caracteres                | O nome do tipo de controle do programa                                                             |


## <a name="relationships"></a>Relações

Nenhum


## <a name="see-also"></a>Ver também

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar programControl](../api/programcontrol-create.md) |     [programControl](programcontrol.md) |   Adicione um programControl a um programa.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.programControlType"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "programControlType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


