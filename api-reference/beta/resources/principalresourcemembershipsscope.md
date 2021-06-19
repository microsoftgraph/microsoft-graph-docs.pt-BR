---
title: Tipo de recurso principalResourceMembershipsScope
description: Permite que a seleção do escopo de revisão de acesso revise o acesso das entidades selecionadas aos recursos selecionados.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d2706246089bcc6a26e2ec8ca3cd115edd18e10a
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030842"
---
# <a name="principalresourcemembershipsscope-resource-type"></a>Tipo de recurso principalResourceMembershipsScope

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

O principalResourceMembershipsScope é um tipo de [accessReviewScope](accessreviewscope.md) que permite selecionar uma coleção de escopos principais e uma coleção de escopos de recursos e revisar o acesso de entidades selecionadas aos recursos selecionados. Ele é usado para configurar a propriedade **scope** de [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md).

Herda de [accessReviewScope](../resources/accessreviewscope.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|principalScopes|[Coleção accessReviewScope](../resources/accessreviewscope.md)|Define os escopos das entidades cujo acesso aos recursos é revisado na revisão de acesso.|
|resourceScopes|[Coleção accessReviewScope](../resources/accessreviewscope.md)|Define os escopos dos recursos para os quais o acesso é revisado.|

Você também deve especificar a **propriedade @odata.type com** o valor `#microsoft.graph.principalResourceMembershipsScope` . Para obter mais  informações sobre opções de configuração para escopo usando **o principalResourceMembershipsScope,** consulte Configure the scope of your [access review definition using the Microsoft Graph API](/graph/accessreviews-scope-concept).

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.principalResourceMembershipsScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
  "principalScopes": [
    {
      "@odata.type": "microsoft.graph.accessReviewScope"
    }
  ],
  "resourceScopes": [
    {
      "@odata.type": "microsoft.graph.accessReviewScope"
    }
  ]
}
```
