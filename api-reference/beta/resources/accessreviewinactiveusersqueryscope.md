---
title: Tipo de recurso accessReviewInactiveUsersQueryScope
description: Um tipo de accessReviewQueryScope que permite que somente usuários inativos sejam selecionados no escopo de uma revisão de acesso.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: c313352b0b9ef43bbf37fff78c99322fffa86a87
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697891"
---
# <a name="accessreviewinactiveusersqueryscope-resource-type"></a>Tipo de recurso accessReviewInactiveUsersQueryScope

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Um tipo de [accessReviewQueryScope](../resources/accessreviewqueryscope.md) que permite que somente usuários inativos sejam selecionados no escopo de uma revisão de acesso. A duração da inatividade é calculada com base na data de última entrada do usuário em relação à data de início da instância de revisão de acesso, conforme definido na propriedade **settings** [de accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md).

Herda de [accessReviewQueryScope](../resources/accessreviewqueryscope.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|inactiveDuration|Duração|Define a duração da inatividade. A inatividade é baseada na data de entrada do último usuário em comparação com a data de início da instância de revisão de acesso. Se essa propriedade não for especificada, ela será atribuída ao valor padrão `PT0S`.|
|consulta|Cadeia de caracteres|Herdado [de accessReviewQueryScope](../resources/accessreviewqueryscope.md).|
|queryRoot|Cadeia de caracteres|Herdado [de accessReviewQueryScope](../resources/accessreviewqueryscope.md).|
|queryType|Cadeia de Caracteres|Herdado [de accessReviewQueryScope](../resources/accessreviewqueryscope.md).|

Você também deve especificar a **propriedade @odata.type** com o valor `#microsoft.graph.accessReviewInactiveUsersQueryScope`. Para obter mais informações sobre as  opções de configuração para escopo usando **accessReviewInactiveUsersQueryScope**, consulte Configurar o escopo de sua definição de revisão de acesso usando o [Microsoft API do Graph](/graph/accessreviews-scope-concept).

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
