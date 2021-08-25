---
title: tipo de recurso relation
description: Representa a relação entre termos em um armazenamento de termos.
author: vishriv
localization_priority: Normal
ms.prod: taxonomy
doc_type: resourcePageType
ms.openlocfilehash: 9b4ccd5ed062fa36cdb16dbec0d8b2631f991b12
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514876"
---
# <a name="relation-resource-type"></a>tipo de recurso relation

Namespace: microsoft.graph.termStore

Representa a relação entre [termos](../resources/termstore-term.md) em um armazenamento de [termos.] Atualmente, há suporte para dois tipos de relações: **pin** e **reutilização.** 

Em uma relação de pino, um termo pode ser fixado em um termo diferente em um conjunto de termos diferente. Em uma relação fixada, novos filhos ao termo só podem ser adicionados no conjunto de termos no qual o termo foi criado. Qualquer alteração na hierarquia sob o termo é refletida nos conjuntos nos quais o termo foi fixado. 

A relação de reutilização é semelhante à relação fixada, exceto que as alterações no termo reutilizado podem ser feitas de qualquer hierarquia na qual o termo seja reutilizado. Além disso, uma alteração na hierarquia feita ao termo reutilizado não se reflete nos outros conjuntos de termos nos quais o termo é reutilizado.

Herda da [entidade](../resources/entity.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar relações](../api/termstore-term-list-relations.md)|[coleção microsoft.graph.termStore.relation](../resources/termstore-relation.md)|Recupere uma lista de **objetos relacionais.**|
|[Criar relação](../api/termstore-relation-post.md)|[microsoft.graph.termStore.relation](../resources/termstore-relation.md)|Crie um novo **objeto relation.**|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID da relação.|
|relação|microsoft.graph.termStore.relationType|O tipo de relação. Os valores possíveis são: `pin`, `reuse`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|fromTerm|[microsoft.graph.termStore.term](../resources/termstore-term.md)|O termo [from] da relação. O termo a partir do qual a relação é definida. Um *valor* nulo indicaria que a relação está diretamente com o [conjunto]. |
|set|[microsoft.graph.termStore.set](../resources/termstore-set.md)|O [conjunto] no qual a relação é relevante.|
|toTerm|[microsoft.graph.termStore.term](../resources/termstore-term.md)|O termo [para] a relação. O termo para o qual a relação é definida.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termStore.relation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.relation",
  "id": "String (identifier)",
  "relationship": "String"
}
```

[microsoft.graph.termStore.term]: termstore-term.md
[microsoft.graph.termStore.set]: termstore-set.md
[microsoft.graph.termStore.relations]: termstore-relation.md
[microsoft.graph.termStore.relation]: termstore-relation.md
[store]: ../resources/termstore-store.md
[term]: ../resources/termstore-term.md
[set]: ../resources/termstore-set.md

<!--
{
  "type": "#page.annotation",
  "description": "TermRelation is the entity for mapping relations between different terms",
  "keywords": "termRelation,facet,resource",
  "section": "documentation",
  "tocPath": "TermRelation",
  "tocBookmarks": {
    "Resources/termStore.relation&quot;: &quot;#"
  },
  "suppressions": []
}
-->


