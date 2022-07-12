---
title: definir tipo de recurso
description: Representa um conjunto em um repositório de termos.
author: mohitpcad
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: b9374c1d41ef713b6edfeb3dd0ec4614b5562c2a
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66734225"
---
# <a name="set-resource-type"></a>definir tipo de recurso

Namespace: microsoft.graph.termStore

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o conjunto usado em um repositório de [termos]. O conjunto representa uma unidade que contém uma coleção de termos hierárquicos. Um [grupo] pode conter vários conjuntos.

Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Conjuntos de listas](../api/termstore-group-list-sets.md)|collection [microsoft.graph.termStore.set] | Retorna a lista de conjuntos contidos em [um grupo] de um repositório de [termos] |
|[Criar conjunto](../api/termstore-set-post.md)|[microsoft.graph.termStore.set](../resources/termstore-set.md)|Crie um novo objeto set em um repositório de [termos].|
|[Criar termo](../api/termstore-term-post.md)|[microsoft.graph.termStore.term](../resources/termstore-term.md)|Crie um novo [objeto de] termo em um repositório de [termos].|
|[Obter conjunto](../api/termstore-set-get.md)|[microsoft.graph.termStore.set](../resources/termstore-set.md)| Obter um objeto set em um repositório de [termos].|
|[Obter termo](../api/termstore-term-get.md)|[microsoft.graph.termStore.term](../resources/termstore-term.md)| Obter um [objeto de] termo em um repositório de [termos].|
|[Conjunto de atualizações](../api/termstore-set-update.md)|[microsoft.graph.termStore.set](../resources/termstore-set.md)|Atualize as propriedades de um objeto set em um repositório de [termos].|
|[Excluir conjunto](../api/termstore-set-delete.md)|Nenhum|Exclui um objeto set em um repositório de [termos].|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Data e hora da criação do conjunto. Somente leitura.|
|description|String|Descrição fornecendo detalhes sobre o uso do termo.|
|id|String|Identificador exclusivo. Somente leitura.|
|localizedNames|[coleção microsoft.graph.termStore.localizedName](../resources/termstore-localizedname.md)|Nome do conjunto para cada languageTag.|
|properties|[coleção microsoft.graph.keyValue](../resources/keyvalue.md)|Propriedades personalizadas para o conjunto.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|filhos|[coleção microsoft.graph.termStore.term](../resources/termstore-term.md)|Termos filhos de conjunto no repositório de [termos].|
|parentGroup|[microsoft.graph.termStore.group](../resources/termstore-group.md)|O grupo [pai] que contém o conjunto.|
|Relações|[coleção microsoft.graph.termStore.relation](../resources/termstore-relation.md)|Indica quais termos foram fixados ou reutilizados diretamente no conjunto.|
|Termos|[coleção microsoft.graph.termStore.term](../resources/termstore-term.md)|Todos os termos sob o conjunto.|

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
[loja]: ../resources/termstore-store.md
[group]: ../resources/termstore-group.md
[set]: ../resources/termstore-set.md
[Termo]: ../resources/termstore-term.md


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


