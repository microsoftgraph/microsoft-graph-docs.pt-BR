---
title: tipo de recurso relation
description: Representa a relação entre termos em um repositório de termos.
author: mohitpcad
ms.localizationpriority: medium
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 18753cf6cb246eea25f9a497ebebc197ac23cb93
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66732657"
---
# <a name="relation-resource-type"></a>tipo de recurso relation

Namespace: microsoft.graph.termStore

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a relação entre [termos em](../resources/termstore-term.md) um repositório de [termos]. Atualmente, há suporte para dois tipos de relações: fixar e reutilizar. 

Em uma relação de pino, um termo pode ser fixado em um termo diferente em um conjunto de termos diferente. Em uma relação fixada, novos filhos ao termo só podem ser adicionados no conjunto de termos no qual o termo foi criado. Qualquer alteração na hierarquia sob o termo é refletida nos conjuntos em que o termo foi fixado. 

A relação de reutilização é semelhante à relação fixada, exceto que as alterações no termo reutilizado podem ser feitas de qualquer hierarquia na qual o termo seja reutilizado. Além disso, uma alteração na hierarquia feita no termo reutilizada não é refletida nos outros conjuntos de termos nos quais o termo é reutilizados.

Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar relações](../api/termstore-term-list-relations.md)|[coleção microsoft.graph.termstore.relation](../resources/termstore-relation.md)|Recuperar uma lista de **objetos de** relação.|
|[Criar relação](../api/termstore-relation-post.md)|[microsoft.graph.termstore.relation](../resources/termstore-relation.md)|Crie um novo **objeto de** relação.|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A ID da relação.|
|relação|String|O tipo de relação. Os valores possíveis são: `pin`, `reuse`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|fromTerm|[microsoft.graph.termStore.term](../resources/termstore-term.md)|O termo [de] origem da relação. O termo do qual a relação é definida. Um valor nulo indicaria que a relação está diretamente com o [conjunto]. |
|set|[microsoft.graph.termStore.set](../resources/termstore-set.md)|O [conjunto] no qual a relação é relevante.|
|toTerm|[microsoft.graph.termStore.term](../resources/termstore-term.md)|O termo [a] ser da relação. O termo para o qual a relação é definida.|

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
[Termo]: ../resources/termstore-term.md
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


