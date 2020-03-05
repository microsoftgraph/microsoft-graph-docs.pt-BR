---
title: tipo de recurso de Tel.
description: tipo de recurso de Tel.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 48c585a05043b4f17e5e7406eb44b9150b5e5bdc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523062"
---
# <a name="itemphone-resource-type"></a>tipo de recurso de Tel.

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações detalhadas sobre números de telefone associados a um usuário em vários serviços.

## <a name="methods"></a>Métodos

| Método                                     | Tipo de retorno               | Descrição                                            |
|:-------------------------------------------|:--------------------------|:-------------------------------------------------------|
| [Obter o número de telefone](../api/itemphone-get.md)   | [Número de telefone](itemphone.md) | Leia as propriedades e os relacionamentos de um objeto **MyPhone** . |
| [Atualizar o número de telefone](../api/itemphone-update.md)       | [Número de telefone](itemphone.md) | Atualize um objeto **MyPhone** .                               |
| [Excluir o número de telefone](../api/itemphone-delete.md)       | Nenhum                      | Excluir um objeto **MyPhone** .                               |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição                                                                                                                     |
|:-------------|:------------|:--------------------------------------------------------------------------------------------------------------------------------|
|displayName   |Cadeia de caracteres       | Contém um nome amigável para o número de telefone.                                                                                  |
|number        |String       | Contém o número de telefone.                                                                                                       |
|type          |string       | Os valores possíveis são: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.itemPhone",
  "baseType": ""
}-->

```json
{
  "displayName": "String",
  "number": "String",
  "type": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemPhone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
