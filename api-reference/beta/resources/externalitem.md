---
title: Tipo de recurso externalItem
description: Um item adicionado a uma conexão Graph Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 7c570a7e4754724ca4239b7e3dbe128d09db9d75
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366524"
---
# <a name="externalitem-resource-type"></a>Tipo de recurso externalItem

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um item adicionado a uma conexão microsoft Graph [.](externalconnection.md) 

## <a name="methods"></a>Métodos

| Método                                                        | Tipo de retorno                     | Descrição |
|:--------------------------------------------------------------|:--------------------------------|:--|
| [Criar externalItem](../api/externalconnection-put-items.md) | [externalItem](externalitem.md) | Crie um externalItem. |
| [Obter externalItem](../api/externalitem-get.md)                | [externalItem](externalitem.md) | Obter um externalItem.    |
| [Atualizar externalItem](../api/externalitem-update.md)          | [externalItem](externalitem.md) | Atualize um externalItem. |
| [Excluir externalItem](../api/externalitem-delete.md)          | Nenhum                            | Exclua um externalItem. |

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo                     | Descrição                          |
|:-----------|:-------------------------|:-------------------------------------|
| acl        | [Coleção acl](acl.md) | Uma matriz de entradas de controle de acesso. Cada entrada especifica o acesso concedido a um usuário ou grupo. Obrigatório. |
| conteúdo    | [externalItemContent](externalitemcontent.md) | Uma representação em texto sem texto do conteúdo do item. O texto nesta propriedade é indexado em texto completo. Opcional. |
| id         | String                   | ID exclusiva fornecida pelo desenvolvedor do item dentro do [externalConnection](externalconnection.md). Deve ser alfanumérico e um máximo de 128 caracteres. Obrigatório. |
| properties | Objeto                   | Um pacote de propriedades com as propriedades do item. As propriedades DEVEM estar em conformidade [com o esquema](schema.md) definido para [externalConnection](externalconnection.md). Obrigatório. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalItem",
  "keyProperty": "id"
}-->

```json
{
  "acl": [{"@odata.type": "microsoft.graph.acl"}],
  "content": {"@odata.type": "microsoft.graph.externalItemContent"},
  "id": "String (identifier)",
  "properties": "Object"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: microsoft.graph.externalItem/properties:\r\n      Referenced type microsoft.graph.object is not defined in the doc set! Potential suggestion: microsoft.graph.directoryObject"
  ]
}-->
