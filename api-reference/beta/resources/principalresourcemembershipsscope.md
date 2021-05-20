---
title: Tipo de recurso principalResourceMembershipsScope
description: Permite que os escopos de seleção revisem o acesso das entidades selecionadas aos recursos selecionados.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b22c52c0bf71f1a1169d51e2e6fd3e8ac10e99d9
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579890"
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
|principalScopes|[Coleção accessReviewScope](../resources/accessreviewscope.md)|Define os escopos das entidades a serem incluídas em uma revisão de acesso.|
|resourceScopes|[Coleção accessReviewScope](../resources/accessreviewscope.md)|Define os escopos dos recursos para os quais o acesso será revisado.|

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
