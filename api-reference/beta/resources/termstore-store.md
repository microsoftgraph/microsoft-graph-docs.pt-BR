---
title: tipo de recurso de armazenamento
description: Representa um repositório de termos de taxonomia.
author: mohitpcad
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: f1b38c9fb826ce430614d44a7b41ed1712523481
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66735933"
---
# <a name="store-resource-type"></a>tipo de recurso de armazenamento

Namespace: microsoft.graph.termStore

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um repositório de termos de taxonomia.

Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição
|:---|:---|:---
|[Listar grupos](../api/termstore-list-groups.md)|[coleção microsoft.graph.termStore.group](../resources/termstore-group.md)| Obtenha os grupos disponíveis no objeto de repositório de termos.|
|[Obter repositório](../api/termstore-store-get.md) | [microsoft.graph.termStore.store](../resources/termstore-store.md) | Leia as propriedades e as relações de um objeto de repositório de termos.
|[Atualizar repositório](../api/termstore-store-update.md) | [microsoft.graph.termStore.store](../resources/termstore-store.md) | Atualize as propriedades de um objeto de repositório de termos.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição
|:---|:---|:---
|defaultLanguageTag | Cadeia de caracteres | Idioma padrão do repositório de termos.
|id|String | Identificador exclusivo do repositório de termos. Somente leitura.
|languageTags | Conjunto de cadeias de caracteres | Lista de idiomas para o repositório de termos.

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição
|:---|:---|:---
|grupos |[coleção microsoft.graph.termStore.group](../resources/termstore-group.md) | Coleção de todos os grupos disponíveis no repositório de termos.
|Define | [coleção microsoft.graph.termStore.set](../resources/termstore-set.md) | Coleção de todos os conjuntos disponíveis no repositório de termos.


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termStore.store",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.store",
  "id": "String (identifier)",
  "defaultLanguageTag": "String",
  "languageTags": [
    "String"
  ]  
}
```

<!--
{
  "type": "#page.annotation",
  "description": "TermStore is the top-level entity used for managing taxonomy for a client",
  "keywords": "termStore,facet,resource",
  "section": "documentation",
  "tocPath": "TermStore",
  "tocBookmarks": {
    "Resources/termStore.store": "#"
  },
  "suppressions": []
}
-->



