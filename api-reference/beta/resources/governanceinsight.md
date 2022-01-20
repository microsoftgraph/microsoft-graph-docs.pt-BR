---
title: Tipo de recurso governanceInsight
description: Representa informações apresentadas ao revisor para um accessReviewInstanceDecisionItem.
author: shubhamguptacal
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: fdbe8aa65487e1d872e7f0943ae5582958fcaaec
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137234"
---
# <a name="governanceinsight-resource-type"></a>Tipo de recurso governanceInsight

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Representa informações apresentadas ao revisor para [um accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md). Insights recomendações aos revisadores para ajudá-los a concluir as análises de acesso.

Esse recurso é um tipo abstrato para o tipo derivado [userSignInInsight.](usersignininsight.md)

## <a name="properties"></a>Propriedades
| Propriedade    | Tipo   | Descrição |
| :---------------| :---------- | :---------- |
| id | Cadeia de caracteres | Identificador do insight. Somente leitura. |
| insightCreatedDateTime | DateTimeOffset | Indica quando o insight foi criado. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.governanceInsight",
  "keyProperty": "id"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.governanceinsight",
  "id": "String",
  "insightCreatedDateTime": "DateTimeOffset"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "governanceinsight resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
