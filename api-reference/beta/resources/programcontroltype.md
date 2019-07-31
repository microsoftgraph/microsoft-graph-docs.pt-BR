---
title: tipo de recurso programControlType
description: 'No recurso de revisões do Azure AD Access, o tipo de controle do programa é usado ao associar um controle a um programa, para indicar o tipo de revisão do Access para o qual o controle é.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: c7b4360ffa22711c9af9961fbb9f48cee7d29424
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965625"
---
# <a name="programcontroltype-resource-type"></a>tipo de recurso programControlType

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No recurso de revisões do Azure AD [Access](accessreviews-root.md) , o tipo de controle do programa é usado ao associar um controle a um programa, para indicar o tipo de revisão do Access para o qual o controle é.  

Os objetos de tipo de controle do programa são gerados automaticamente quando o administrador global embuti o locatário para usar o recurso de revisões do Access.  Nenhum tipo de controle de programa adicional pode ser criado.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar programControlTypes](../api/programcontroltype-list.md) | coleção [programControlType](programcontroltype.md)| Listar tipos de controle de programa. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| `id`                     |`String`                | O identificador atribuído ao recurso do tipo de controle do programa                                      |
| `displayName`            |`String`                | O nome do tipo de controle do programa                                                             |


## <a name="relationships"></a>Relações

Nenhum


## <a name="see-also"></a>Ver também

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar programControl](../api/programcontrol-create.md) |     [programControl](programcontrol.md) |   Adicionar um programControl a um programa.|


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
