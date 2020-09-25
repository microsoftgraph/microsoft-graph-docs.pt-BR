---
title: tipo de recurso Term
description: Define uma entidade Term em um repositório de termos.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 71c22c86d2ebbb02587a20355adb1d461479297d
ms.sourcegitcommit: 3c0fa2d13ede0fdfa66d966d4ec32cb468c3befa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/25/2020
ms.locfileid: "48273569"
---
# <a name="term-resource-type"></a>tipo de recurso Term

Namespace: Microsoft. Graph. termos

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um termo usado em um [repositório]de termos. Um termo pode ser usado para representar um objeto que pode ser usado como metadados para marcar o conteúdo. Vários termos podem ser organizados de maneira hierárquica dentro de um [conjunto].

Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar filhos](../api/termstore-term-list-children.md)|coleção [Microsoft. Graph. termos. Term](../resources/termstore-term.md)|Obter os filhos de primeiro nível de um termo em um [repositório]de termos.|
|[Listar relações](../api/termstore-term-list-relations.md)|coleção [Microsoft. Graph. termos. relation](../resources/termstore-relation.md)|Obter as relações de um termo em um [repositório]de termos.|
|[Criar relação](../api/termstore-relation-post.md)|[Microsoft. Graph. termos. relation](../resources/termstore-relation.md)|Crie uma nova relação para um termo ou um [conjunto] em um [repositório]de termos.|
|[Criar termo](../api/termstore-term-post.md)|[Microsoft. Graph. termos. Term](../resources/termstore-term.md)|Criar um novo objeto Term em um [repositório]de termos.|
|[Obter termo](../api/termstore-term-get.md)|[Microsoft. Graph. termos. Term](../resources/termstore-term.md)|Leia as propriedades e os relacionamentos de um objeto Term em um  [repositório]de termos.|
|[Atualizar termo](../api/termstore-term-update.md)|[Microsoft. Graph. termos. Term](../resources/termstore-term.md)|Atualizar as propriedades de um objeto Term em um [repositório]de termos.|
|[Excluir termo](../api/termstore-term-delete.md)|Nenhum|Excluir um objeto Term em um [repositório]de termos.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Data e hora da criação do termo. Somente leitura|
|descrições|coleção [Microsoft. Graph. termos. localizedDescription](../resources/termstore-localizeddescription.md)|Descrição sobre o termo que é dependente do languageTag|
|id|String|Identificador exclusivo do termo. Somente leitura|
|Legendas|coleção [Microsoft. Graph. termos. localizedLabel](../resources/termstore-localizedlabel.md)||Metadados de rótulo para um termo|
|lastModifiedDateTime|DateTimeOffset|Data e hora da última modificação do termo. Somente leitura|
|properties|coleção [Microsoft. Graph. KeyValue](../resources/keyvalue.md)|Coleção de propriedades no termo|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|filhos|coleção [Microsoft. Graph. termos. Term](../resources/termstore-term.md)|Filhos do termo atual|
|Relations|coleção [Microsoft. Graph. termos. relation](../resources/termstore-relation.md)|Para indicar quais termos estão relacionados ao termo atual como fixado ou reutilizado|
|set|[Microsoft. Graph. termos. Set](../resources/termstore-set.md)|O [conjunto] em que o termo é criado|

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

[Guarde]: ../resources/termstore-store.md
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
    "Resources/termstore-term": "#"
  },
  "suppressions": []
}
-->


