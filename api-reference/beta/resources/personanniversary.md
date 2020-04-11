---
title: tipo de recurso personAnniversary
description: tipo de recurso personAnniversary
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: c8ea4e9bf7db268c5ec6bffad1c7d43cbbdd2439
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227726"
---
# <a name="personanniversary-resource-type"></a>tipo de recurso personAnniversary

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de datas significativas associadas a uma pessoa em um [perfil](profile.md)de usuário.

Herda de [Myfacet](itemFacet.md).

## <a name="methods"></a>Métodos

| Método                                                   | Tipo de retorno                               | Descrição                                                              |
|:---------------------------------------------------------|:------------------------------------------|:-------------------------------------------------------------------------|
| [Obter personAnniversary](../api/personanniversary-get.md) | [personAnniversary](personanniversary.md) | Leia as propriedades e os relacionamentos de um objeto **personAnniversary** . |
| [Update](../api/personanniversary-update.md)             | [personAnniversary](personanniversary.md) | Atualizar um objeto **personAnniversary** .                                   |
| [Delete](../api/personanniversary-delete.md)             | None                                      | Excluir um objeto **personAnniversary** .                                   |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição                                                      |
|:-------------|:------------|:-----------------------------------------------------------------|
|data          |Data         | Contém a data associada ao tipo de aniversário.          |
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
