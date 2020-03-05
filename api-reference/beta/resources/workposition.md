---
title: tipo de recurso workPosition
description: tipo de recurso workPosition
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 086273e54d923054ce8e71ef1c67fb2bb4f7002a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519061"
---
# <a name="workposition-resource-type"></a>tipo de recurso workPosition

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações detalhadas sobre posições de trabalho associadas ao [perfil](profile.md)de um usuário.

Esse tipo de recurso herda de [Myfacet](itemfacet.md).

## <a name="methods"></a>Métodos

| Método                                         | Tipo de retorno                     | Descrição                                               |
|:-----------------------------------------------|:--------------------------------|:----------------------------------------------------------|
| [Obter workPosition](../api/workposition-get.md) | [workPosition](workposition.md) | Leia as propriedades e os relacionamentos de um objeto **workPosition** . |
| [Atualizar workPosition](../api/workposition-update.md)        | [workPosition](workposition.md) | Atualizar um objeto **workPosition** .                               |
| [Excluir workPosition](../api/workposition-delete.md)        | Nenhum                            | Excluir um objeto **workPosition** .                               |

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo                               | Descrição                                                                                                |
|:---------------------|:-----------------------------------|:-----------------------------------------------------------------------------------------------------------|
|categories            |String collection                   | Contém categorias que um usuário associou à posição (por exemplo, transformação digital, pessoas). |
|detalhada                |[positionDetail](positiondetail.md) | Contém detalhes sobre as posições de emprego atuais e anteriores do usuário.                                 |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workPosition",
  "baseType": ""
}-->

```json
{
  "categories": ["String"],
  "detail": {"@odata.type": "microsoft.graph.positionDetail"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workPosition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
