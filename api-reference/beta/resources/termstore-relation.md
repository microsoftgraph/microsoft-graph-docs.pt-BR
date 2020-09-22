---
title: tipo de recurso relation
description: Representa a relação entre os termos em um repositório de termos.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 2e8f4dc8b82c496909f5b150829d9fb4e114ba59
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973586"
---
# <a name="relation-resource-type"></a>tipo de recurso relation

Namespace: Microsoft. Graph. termos

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a relação entre os [termos](../resources/termstore-term.md) em um [repositório]de termos. Atualmente, dois tipos de relações têm suporte: PIN e reutilização. 

Em um relacionamento de PIN, um termo pode ser fixado em um termo diferente em um conjunto de termos diferente. Em uma relação fixa, só é possível adicionar novos filhos ao termo no conjunto de termos em que o termo foi criado. Qualquer alteração na hierarquia sob o termo é refletida nos conjuntos em que o termo foi fixado. 

A relação de reutilização é semelhante à relação fixa, exceto que as alterações no termo reutilizado podem ser feitas de qualquer hierarquia na qual o termo é reutilizado. Além disso, uma alteração na hierarquia feita no termo reutilizado não é refletida nos outros conjuntos de termos nos quais o termo é reutilizado.

Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar relações](../api/termstore-term-list-relations.md)|coleção [Microsoft. Graph. termos. relation](../resources/termstore-relation.md)|Recupere uma lista de objetos **relation** .|
|[Criar relação](../api/termstore-relation-post.md)|[Microsoft. Graph. termos. relation](../resources/termstore-relation.md)|Criar um novo objeto **relation** .|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A ID da relação.|
|relação|String|O tipo de relação. Os valores possíveis são: `pin`, `reuse`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|fromTerm|[Microsoft. Graph. termos. Term](../resources/termstore-term.md)|O [termo] de da relação. O termo a partir do qual a relação é definida. Um valor nulo indicaria que a relação é diretamente com o [conjunto]. |
|set|[Microsoft. Graph. termos. Set](../resources/termstore-set.md)|O [conjunto] em que a relação é relevante.|
|toterm|[Microsoft. Graph. termos. Term](../resources/termstore-term.md)|O [termo] to da relação. O termo para o qual o realtionship está definido.|

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
[loja]: ../resources/termstore-store.md
[terminal]: ../resources/termstore-term.md
[set]: ../resources/termstore-set.md

<!--
{
  "type": "#page.annotation",
  "description": "TermRelation is the entity for mapping relations between different terms",
  "keywords": "termRelation,facet,resource",
  "section": "documentation",
  "tocPath": "TermRelation",
  "tocBookmarks": {
    "Resources/termStore.relation": "#"
  },
  "suppressions": []
}
-->


