---
title: Tipo de recurso principalResourceMembershipsScope
description: Permite que a seleção do escopo de revisão de acesso examine o acesso das entidades de segurança selecionadas aos recursos selecionados.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: be18d6711ea155d3c84c8aa1962319a6b8fa564f
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697600"
---
# <a name="principalresourcemembershipsscope-resource-type"></a>Tipo de recurso principalResourceMembershipsScope

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

O principalResourceMembershipsScope é um tipo de [accessReviewScope](accessreviewscope.md) que permite selecionar uma coleção de escopos de entidade de segurança e uma coleção de escopos de recursos e examinar o acesso das entidades de segurança selecionadas aos recursos selecionados. Ele é usado para configurar a **propriedade de** escopo de [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md).

Herda de [accessReviewScope](../resources/accessreviewscope.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|principalScopes|[coleção accessReviewScope](../resources/accessreviewscope.md)|Define os escopos das entidades de segurança cujo acesso aos recursos é revisado na revisão de acesso.|
|resourceScopes|[coleção accessReviewScope](../resources/accessreviewscope.md)|Define os escopos dos recursos para os quais o acesso é revisado.|

Você também deve especificar a **propriedade @odata.type** com o valor `#microsoft.graph.principalResourceMembershipsScope`. Para obter mais informações sobre as  opções de configuração para escopo usando **principalResourceMembershipsScope**, consulte Configurar o escopo da definição de revisão de acesso usando o [Microsoft API do Graph](/graph/accessreviews-scope-concept).

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
