---
title: tipo de recurso externalItem
description: Um item indexado por meio de uma conexão de pesquisa da Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 900cf61536204ff5924aea0de268befad6626b37
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704168"
---
# <a name="externalitem-resource-type"></a>tipo de recurso externalItem

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um item indexado por meio de uma [conexão](externalconnection.md)de pesquisa da Microsoft.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>Métodos

| Método                                                        | Tipo de retorno                     | Descrição |
|:--------------------------------------------------------------|:--------------------------------|:--|
| [Criar externalItem](../api/externalconnection-put-items.md) | [externalItem](externalitem.md) | Criar um externalItem. |
| [Atualizar externalItem](../api/externalitem-update.md)          | [externalItem](externalitem.md) | Atualizar um externalItem. |
| [Excluir externalItem](../api/externalitem-delete.md)          | Nenhum                            | Excluir um externalItem. |

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo                     | Descrição                          |
|:-----------|:-------------------------|:-------------------------------------|
| ACL        | coleção [ACL](acl.md) | Uma matriz de entradas de controle de acesso. Cada entrada especifica o acesso concedido a um usuário ou grupo. Obrigatório. |
| content    | Cadeia de caracteres                   | Uma representação de texto simples do conteúdo do item. O texto nessa propriedade é indexado de texto completo. Opcional. |
| id         | String                   | ID exclusiva fornecida pelo desenvolvedor do item dentro do [externalConnection](externalconnection.md)que contém o. Deve ser alfanumérico e um máximo de 128 caracteres. Obrigatório. |
| properties | Objeto                   | Um recipiente de propriedades com as propriedades do item. As propriedades devem estar em conformidade com o [esquema](schema.md) definido para o [externalConnection](externalconnection.md). Obrigatório. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalItem",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "acl": [{"@odata.type": "microsoft.graph.acl"}],
  "content": "String",
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
