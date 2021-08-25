---
title: tipo de recurso term
description: Define uma entidade de termo em um armazenamento de termos.
author: vishriv
localization_priority: Normal
ms.prod: taxonomy
doc_type: resourcePageType
ms.openlocfilehash: 5a8c429a20ed533c6de8fb11bb13aa877e2c41be
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514853"
---
# <a name="term-resource-type"></a>tipo de recurso term

Namespace: microsoft.graph.termStore

Representa um termo usado em um armazenamento de [termos.] Um termo pode ser usado para representar um objeto que pode ser usado como metadados para marcar conteúdo. Vários termos podem ser organizados de maneira hierárquica dentro de um [conjunto].

Herda da [entidade](../resources/entity.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar filhos](../api/termstore-term-list-children.md)|[coleção microsoft.graph.termStore.term](../resources/termstore-term.md)|Obter os filhos de primeiro nível de um termo em um armazenamento de [termos.]|
|[Listar relações](../api/termstore-term-list-relations.md)|[coleção microsoft.graph.termStore.relation](../resources/termstore-relation.md)|Obter as relações de um termo em um armazenamento de [termos.]|
|[Criar relação](../api/termstore-relation-post.md)|[microsoft.graph.termStore.relation](../resources/termstore-relation.md)|Crie uma nova relação para um termo ou [um conjunto] em um armazenamento de [termos.]|
|[Criar termo](../api/termstore-term-post.md)|[microsoft.graph.termStore.term](../resources/termstore-term.md)|Criar um novo objeto de termo em um armazenamento de [termos.]|
|[Obter termo](../api/termstore-term-get.md)|[microsoft.graph.termStore.term](../resources/termstore-term.md)|Leia as propriedades e as relações de um objeto term em um armazenamento de [termos.]|
|[Termo de atualização](../api/termstore-term-update.md)|[microsoft.graph.termStore.term](../resources/termstore-term.md)|Atualize as propriedades de um objeto term em um armazenamento de [termos.]|
|[Excluir termo](../api/termstore-term-delete.md)|Nenhuma|Excluir um objeto term em um armazenamento de [termos.]|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Data e hora da criação do termo. Somente leitura.|
|descriptions|[coleção microsoft.graph.termStore.localizedDescription](../resources/termstore-localizeddescription.md)|Descrição sobre o termo que depende do languageTag.|
|id|Cadeia de caracteres|Identificador exclusivo do termo. Somente Leitura.|
|labels|[coleção microsoft.graph.termStore.localizedLabel](../resources/termstore-localizedlabel.md)|Rotular metadados para um termo.|
|lastModifiedDateTime|DateTimeOffset|Última data e hora da modificação do termo. Somente leitura.|
|properties|[coleção microsoft.graph.keyValue](../resources/keyvalue.md)|Coleção de propriedades no termo.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|filhos|[coleção microsoft.graph.termStore.term](../resources/termstore-term.md)|Filhos do termo atual.|
|relations|[coleção microsoft.graph.termStore.relation](../resources/termstore-relation.md)|Para indicar quais termos estão relacionados ao termo atual como fixado ou reutilizado.|
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

[store]: ../resources/termstore-store.md
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


