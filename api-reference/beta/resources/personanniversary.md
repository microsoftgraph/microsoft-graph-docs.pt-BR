---
title: tipo de recurso personAnniversary
description: tipo de recurso personAnniversary
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 7dad5536eb78b2d7119ace63eb0f7ce16880e85f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521922"
---
# <a name="personanniversary-resource-type"></a>tipo de recurso personAnniversary

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de datas significativas associadas a uma pessoa em um [perfil](profile.md)de usuário.

Herda de [Myfacet](itemFacet.md).

## <a name="methods"></a>Métodos

| Método                                                   | Tipo de retorno                               | Descrição                                                    |
|:---------------------------------------------------------|:------------------------------------------|:---------------------------------------------------------------|
| [Obter personAnniversary](../api/personanniversary-get.md) | [personAnniversary](personanniversary.md) | Leia as propriedades e os relacionamentos de um objeto **personAnniversary** . |
| [Update](../api/personanniversary-update.md)             | [personAnniversary](personanniversary.md) | Atualizar um objeto **personAnniversary** .                               |
| [Delete](../api/personanniversary-delete.md)             | None                                      | Excluir um objeto **personAnniversary** .                               |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição                                                      |
|:-------------|:------------|:-----------------------------------------------------------------|
|data          |Data         | Contém a data associada ao tipo de aniversário.         |
|type          |cadeia de caracteres       | Os valores possíveis são: `birthday`, `wedding`, `unknownFutureValue`.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso. 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personAnniversary",
  "baseType": ""
}-->

```json
{
  "date": "String (timestamp)",
  "type": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personAnniversary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
