---
title: Tipo de recurso accessReviewReviewerScope
description: Representa quem revisará uma revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 58abda6c89e484336b34d546edc68ebbfe432162
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579250"
---
# <a name="accessreviewreviewerscope-resource-type"></a>Tipo de recurso accessReviewReviewerScope

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

O accessReviewReviewerScope define quem revisará instâncias de [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md). É uma consulta OData que permite que os revisadores sejam especificados como uma lista estática de usuários (ou seja, usuários específicos, proprietários de grupos e membros do grupo) ou dinamicamente em que cada usuário é revisado por seu gerente ou por proprietários de grupo. Para criar uma auto-revisão (onde os usuários analisam seu próprio acesso), não forneça aos revisores sobre a criação [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md)

Herda de [accessReviewScope](../resources/accessreviewscope.md).

## <a name="properties"></a>Propriedades
| Propriedade | Tipo | Descrição |
| :-------------------------| :---------- | :---------- |
| consulta | String | A consulta especificando quem será o revistor. Consulte tabela para exemplos. |
| queryType | String | O tipo de consulta. Exemplos incluem `MicrosoftGraph` `ARM` e . |
| queryRoot | String | No cenário em que os revisadores precisam ser especificados dinamicamente, essa propriedade é usada para indicar a fonte relativa da consulta. Essa propriedade só será necessária se uma consulta relativa, por exemplo, `./manager` , for especificada. Valor possível: `decisions` . |

Para obter mais informações sobre opções de configuração para revisadores, consulte Atribuir revisadores à sua definição de revisão de acesso [usando a API do Microsoft Graph](/graph/accessreviews-reviewers-concept).


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewReviewerScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewReviewerScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewReviewerScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
