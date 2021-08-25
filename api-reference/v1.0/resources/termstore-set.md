---
title: definir tipo de recurso
description: Representa um conjunto em um armazenamento de termos.
author: vishriv
localization_priority: Normal
ms.prod: taxonomy
doc_type: resourcePageType
ms.openlocfilehash: d56bc436dca1c645d7e5d24face75a9bf5acd957
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514855"
---
# <a name="set-resource-type"></a>definir tipo de recurso

Namespace: microsoft.graph.termStore

Representa o conjunto usado em um armazenamento de [termos.] O conjunto representa uma unidade que contém uma coleção de termos hierárquicos. Um [grupo] pode conter vários conjuntos.

Herda da [entidade](../resources/entity.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Conjuntos de listas](../api/termstore-group-list-sets.md)|coleção [microsoft.graph.termStore.set] | Retorna uma lista de conjuntos contidos em [um grupo] de um armazenamento de [termos.] |
|[Criar conjunto](../api/termstore-set-post.md)|[microsoft.graph.termStore.set](../resources/termstore-set.md)|Crie um novo objeto set em um armazenamento de [termos.]|
|[Criar termo](../api/termstore-term-post.md)|[microsoft.graph.termStore.term](../resources/termstore-term.md)|Criar um novo [objeto de] termo em um armazenamento de [termos.]|
|[Obter conjunto](../api/termstore-set-get.md)|[microsoft.graph.termStore.set](../resources/termstore-set.md)| Obter um objeto set em um armazenamento de [termos.]|
|[Obter termo](../api/termstore-term-get.md)|[microsoft.graph.termStore.term](../resources/termstore-term.md)| Obter um [objeto term] em um armazenamento de [termos.]|
|[Conjunto de atualizações](../api/termstore-set-update.md)|[microsoft.graph.termStore.set](../resources/termstore-set.md)|Atualize as propriedades de um objeto set em um armazenamento de [termos.]|
|[Excluir conjunto](../api/termstore-set-delete.md)|Nenhuma|Exclui um objeto set em um armazenamento de [termos.]|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Data e hora da criação do conjunto. Somente leitura.|
|description|Cadeia de caracteres|Descrição que fornece detalhes sobre o uso do termo.|
|id|Cadeia de caracteres|Identificador exclusivo. Somente leitura.|
|localizedNames|[coleção microsoft.graph.termStore.localizedName](../resources/termstore-localizedname.md)|Nome do conjunto para cada languageTag.|
|properties|[coleção microsoft.graph.keyValue](../resources/keyvalue.md)|Propriedades personalizadas para o conjunto.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|filhos|[coleção microsoft.graph.termStore.term](../resources/termstore-term.md)|Termos filhos de conjunto no armazenamento de [termos.]|
|parentGroup|[microsoft.graph.termStore.group](../resources/termstore-group.md)|O grupo [pai] que contém o conjunto.|
|relations|[coleção microsoft.graph.termStore.relation](../resources/termstore-relation.md)|Indica quais termos foram fixados ou reutilizados diretamente sob o conjunto.|
|termos|[coleção microsoft.graph.termStore.term](../resources/termstore-term.md)|Todos os termos sob o conjunto.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termStore.set",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.set",
  "id": "String (identifier)",
  "localizedNames": [
    {
      "@odata.type": "microsoft.graph.termStore.localizedName"
    }
  ],
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "properties": [
    {
      "@odata.type": "microsoft.graph.termStore.keyValue"
    }
  ]
}
```

[microsoft.graph.termStore.term]: termstore-term.md
[microsoft.graph.termStore.set]: termstore-set.md
[microsoft.graph.termStore.group]: termstore-group.md
[microsoft.graph.termStore.relation]: termstore-relation.md
[microsoft.graph.termStore.store]: termstore-store.md
[microsoft.graph.termStore.localizedName]: termstore-localizedname.md
[store]: ../resources/termstore-store.md
[group]: ../resources/termstore-group.md
[set]: ../resources/termstore-set.md
[term]: ../resources/termstore-term.md


<!--
{
  "type": "#page.annotation",
  "description": "TermSet is the entity containing the particular taxonomy for a tenant",
  "keywords": "termSet,facet,resource",
  "section": "documentation",
  "tocPath": "TermSet",
  "tocBookmarks": {
    "Resources/termStore.set&quot;: &quot;#"
  },
  "suppressions": []
}
-->


