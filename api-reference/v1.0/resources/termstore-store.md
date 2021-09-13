---
title: tipo de recurso de armazenamento
description: Representa um armazenamento de termos de taxonomia.
author: vishriv
ms.localizationpriority: medium
ms.prod: taxonomy
doc_type: resourcePageType
ms.openlocfilehash: c94c0edb6589bd467676ac42294ead8416e829df
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084038"
---
# <a name="store-resource-type"></a>tipo de recurso de armazenamento

Namespace: microsoft.graph.termStore

Representa um armazenamento de termos de taxonomia.

Herda da [entidade](../resources/entity.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar grupos](../api/termstore-list-groups.md)|[coleção microsoft.graph.termStore.group](../resources/termstore-group.md)| Obter os grupos disponíveis no objeto de armazenamento de termos.|
|[Obter loja](../api/termstore-store-get.md) | [microsoft.graph.termStore.store](../resources/termstore-store.md) | Leia as propriedades e as relações de um objeto de armazenamento de termos.|
|[Armazenamento de atualizações](../api/termstore-store-update.md) | [microsoft.graph.termStore.store](../resources/termstore-store.md) | Atualize as propriedades de um objeto de armazenamento de termos.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|defaultLanguageTag | Cadeia de caracteres | Idioma padrão do armazenamento de termos.|
|id|Cadeia de caracteres | Identificador exclusivo do armazenamento de termos. Somente leitura.|
|languageTags | Coleção String | Lista de idiomas para o armazenamento de termos.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|grupos |[coleção microsoft.graph.termStore.group](../resources/termstore-group.md) | Coleção de todos os grupos disponíveis no armazenamento de termos.|
|sets | [coleção microsoft.graph.termStore.set](../resources/termstore-set.md) | Coleção de todos os conjuntos disponíveis no armazenamento de termos.|


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



