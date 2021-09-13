---
title: Tipo de recurso principalResourceMembershipsScope
description: Permite que a seleção do escopo de revisão de acesso revise o acesso das entidades selecionadas aos recursos selecionados.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7d4e30ccccedb5dda72c4d0bb168655e1a8aedfd
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019213"
---
# <a name="principalresourcemembershipsscope-resource-type"></a>Tipo de recurso principalResourceMembershipsScope

Namespace: microsoft.graph

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
