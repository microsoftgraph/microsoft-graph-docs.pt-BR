---
title: Tipo de recurso programControlType (preterido)
description: 'No recurso Azure AD revisões de acesso, o tipo de controle de programa é usado ao associar um controle a um programa, para indicar o tipo de revisão de acesso para o qual o controle se aplica.  '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 2dcb4c5e00b4c3b5ea0cf9283dadaa9b2c89cd12
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2022
ms.locfileid: "65819734"
---
# <a name="programcontroltype-resource-type-deprecated"></a>Tipo de recurso programControlType (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

No recurso Azure AD [revisões](accessreviews-root.md) de acesso, o tipo de controle de programa é usado ao associar um controle a um programa, para indicar o tipo de revisão de acesso para o qual o controle se aplica.  

Os objetos de tipo de controle de programa são gerados automaticamente quando o administrador global integra o locatário para usar o recurso de revisões de acesso.  Nenhum tipo de controle de programa adicional pode ser criado.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar programControlTypes](../api/programcontroltype-list.md) | [coleção programControlType](programcontroltype.md)| Listar tipos de controle de programa. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| id                     |String                | O identificador atribuído ao recurso do tipo de controle de programa                                      |
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


