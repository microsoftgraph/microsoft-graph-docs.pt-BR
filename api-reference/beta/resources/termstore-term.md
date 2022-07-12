---
title: tipo de recurso term
description: Define uma entidade de termo em um repositório de termos.
author: mohitpcad
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: 0207c740d52f7e7401ed6c741cf8d9134ec47eb1
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66730274"
---
# <a name="term-resource-type"></a>tipo de recurso term

Namespace: microsoft.graph.termStore

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um termo usado em um repositório de [termos]. Um termo pode ser usado para representar um objeto que pode ser usado como metadados para marcar o conteúdo. Vários termos podem ser organizados de maneira hierárquica dentro de um [conjunto].

Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Filhos de lista](../api/termstore-term-list-children.md)|[coleção microsoft.graph.termStore.term](../resources/termstore-term.md)|Obter os filhos de primeiro nível de um termo em um repositório de [termos].|
|[Listar relações](../api/termstore-term-list-relations.md)|[coleção microsoft.graph.termStore.relation](../resources/termstore-relation.md)|Obter as relações de um termo em um repositório de [termos].|
|[Criar relação](../api/termstore-relation-post.md)|[microsoft.graph.termStore.relation](../resources/termstore-relation.md)|Crie uma nova relação para um termo ou um [conjunto] em um repositório de [termos].|
|[Criar termo](../api/termstore-term-post.md)|[microsoft.graph.termStore.term](../resources/termstore-term.md)|Crie um novo objeto de termo em um repositório de [termos].|
|[Obter termo](../api/termstore-term-get.md)|[microsoft.graph.termStore.term](../resources/termstore-term.md)|Leia as propriedades e as relações de um objeto de termo em um repositório de  [termos].|
|[Atualizar termo](../api/termstore-term-update.md)|[microsoft.graph.termStore.term](../resources/termstore-term.md)|Atualize as propriedades de um objeto de termo em um repositório de [termos].|
|[Excluir termo](../api/termstore-term-delete.md)|Nenhum|Exclua um objeto de termo em um repositório de [termos].|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Data e hora da criação do termo. Somente leitura.|
|Descrições|[coleção microsoft.graph.termStore.localizedDescription](../resources/termstore-localizeddescription.md)|Descrição sobre o termo que depende da languageTag.|
|id|String|Identificador exclusivo do termo. Somente Leitura.|
|Rótulos|[coleção microsoft.graph.termStore.localizedLabel](../resources/termstore-localizedlabel.md)|Rotular metadados para um termo.|
|lastModifiedDateTime|DateTimeOffset|Última modificação de data e hora do termo. Somente leitura.|
|properties|[coleção microsoft.graph.keyValue](../resources/keyvalue.md)|Coleção de propriedades no termo.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|filhos|[coleção microsoft.graph.termStore.term](../resources/termstore-term.md)|Filhos do termo atual.|
|Relações|[coleção microsoft.graph.termStore.relation](../resources/termstore-relation.md)|Para indicar quais termos estão relacionados ao termo atual como fixados ou reutilizados.|
|set|[microsoft.graph.termStore.set](../resources/termstore-set.md)|O [conjunto] no qual o termo é criado.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termStore.term",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.term",
  "id": "String (identifier)",
  "labels": [
    {
      "@odata.type": "microsoft.graph.termStore.localizedLabel"
    }
  ],
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "descriptions": [
    {
      "@odata.type": "microsoft.graph.termStore.localizedDescription"
    }
  ],
  "properties": [
    {
      "@odata.type": "microsoft.graph.keyValue"
    }
  ]
}
```

[loja]: ../resources/termstore-store.md
[set]: ../resources/termstore-set.md
[term]: ../resources/termstore-term.md
[group]: ../resources/termstore-group.md

<!--
{
  "type": "#page.annotation",
  "description": "Term is the entity used for tagging in termStore",
  "keywords": "term,facet,resource",
  "section": "documentation",
  "tocPath": "Terms",
  "tocBookmarks": {
    "Resources/termstore-term&quot;: &quot;#"
  },
  "suppressions": []
}
-->


