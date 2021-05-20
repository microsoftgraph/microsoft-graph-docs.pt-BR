---
title: Tipo de recurso accessReviewInactiveUsersQueryScope
description: Um tipo de accessReviewQueryScope que permite que apenas usuários inativos sejam selecionados no escopo de uma revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 80d415125679ddbb44a08fe75f33b115e4ba1f04
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579743"
---
# <a name="accessreviewinactiveusersqueryscope-resource-type"></a>Tipo de recurso accessReviewInactiveUsersQueryScope

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Um tipo de [accessReviewQueryScope](../resources/accessreviewqueryscope.md) que permite que apenas usuários inativos sejam selecionados no escopo de uma revisão de acesso. A duração da inatividade é calculada com base na última data de entrada do usuário em relação à data de início da instância de revisão de acesso, conforme definido na propriedade **settings** [de accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md).

Herda de [accessReviewQueryScope](../resources/accessreviewqueryscope.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|inactiveDuration|Duration|Define a duração da inatividade. A inatividade é baseada na última data de entrada do usuário em comparação com a data de início da instância de revisão de acesso. Se essa propriedade não for especificada, ela será atribuída ao valor padrão `PT0S` .|
|consulta|String|Herdado [de accessReviewQueryScope](../resources/accessreviewqueryscope.md).|
|queryRoot|String|Herdado [de accessReviewQueryScope](../resources/accessreviewqueryscope.md).|
|queryType|String|Herdado [de accessReviewQueryScope](../resources/accessreviewqueryscope.md).|

Você também deve especificar a **propriedade @odata.type com** o valor `#microsoft.graph.accessReviewInactiveUsersQueryScope` . Para obter mais  informações sobre opções de configuração para escopo usando **accessReviewInactiveUsersQueryScope**, consulte Configure the scope of your [access review definition using the Microsoft Graph API](/graph/accessreviews-scope-concept).

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInactiveUsersQueryScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String",
  "inactiveDuration": "String (duration)"
}
```
