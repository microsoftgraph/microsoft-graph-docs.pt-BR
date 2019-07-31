---
title: tipo de recurso plannerPlanContextDetailsCollection
description: " o valor é o objeto plannerPlanContextDetails."
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: b8adf130dc925a4d9eb17819acf7b2a670a6c7b9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965898"
---
# <a name="plannerplancontextdetailscollection-resource-type"></a>tipo de recurso plannerPlanContextDetailsCollection

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


O recurso **plannerPlanContextDetailsCollection** representa a coleção de contextos externos aos quais um plano está vinculado. Esse recurso é um tipo aberto e faz parte do objeto [plannerPlanDetails](plannerplandetails.md) . O nome da propriedade no par propriedade-valor é um identificador específico do aplicativo do contexto; o valor é o objeto [plannerPlanContextDetails](plannerplancontextdetails.md) .


## <a name="properties"></a>Propriedades
As propriedades de um tipo aberto podem ser definidas pelo cliente. Nesse caso, o cliente deve usar um identificador distintivo que representa o contexto externo como o nome da propriedade. Os valores de propriedade devem ser objetos [plannerPlanContextDetails](plannerplancontextdetails.md) . Com base em OData, os nomes de propriedade em tipos abertos não podem conter `.`os `:`seguintes `@`caracteres `%`:,,,. Esses caracteres precisam ser codificados com o formato de codificação de URL. Para remover um item da lista favoritos, o valor precisa ser removido da coleção [plannerPlanContextCollection](plannerplancontextcollection.md) , o que removerá automaticamente a entrada desse objeto.

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContextDetailsCollection"
}-->

```json
{
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContextDetailsCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
