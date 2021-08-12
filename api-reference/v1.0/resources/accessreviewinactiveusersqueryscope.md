---
title: Tipo de recurso accessReviewInactiveUsersQueryScope
description: Um tipo de accessReviewQueryScope que permite que apenas usuários inativos sejam selecionados no escopo de uma revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: c7c0fcfb14041888ba760492bcfe6a2a224eb8656fdab8d7fee922f3e86b2af9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54230820"
---
# <a name="accessreviewinactiveusersqueryscope-resource-type"></a>Tipo de recurso accessReviewInactiveUsersQueryScope

Namespace: microsoft.graph

Um tipo de [accessReviewQueryScope](../resources/accessreviewqueryscope.md) que permite que apenas usuários inativos sejam selecionados no escopo de uma revisão de acesso. A duração da inatividade é calculada com base na última data de entrada do usuário em relação à data de início da instância de revisão de acesso, conforme definido na propriedade **settings** [de accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md).

Herda de [accessReviewQueryScope](../resources/accessreviewqueryscope.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|inactiveDuration|Duration|Define a duração da inatividade. A inatividade é baseada na última data de entrada do usuário em comparação com a data de início da instância de revisão de acesso. Se essa propriedade não for especificada, ela será atribuída ao valor padrão `PT0S` .|
|consulta|Cadeia de caracteres|Herdado [de accessReviewQueryScope](../resources/accessreviewqueryscope.md).|
|queryRoot|String|Herdado [de accessReviewQueryScope](../resources/accessreviewqueryscope.md).|
|queryType|Cadeia de caracteres|Herdado [de accessReviewQueryScope](../resources/accessreviewqueryscope.md).|

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
