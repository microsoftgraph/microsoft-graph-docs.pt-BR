---
title: Tipo de recurso accessReviewReviewerScope
description: Representa quem revisará uma revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7c8a0644699daf7e204226d89bdd6cab6048888d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133487"
---
# <a name="accessreviewreviewerscope-resource-type"></a>Tipo de recurso accessReviewReviewerScope

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O accessReviewReviewerScope define quem revisará instâncias de um [accessReviewScheduleDefinition](accessreviewscheduledefinition.md). Isso é expresso como uma consulta OData, que permite que os revisadores sejam especificados como uma lista estática de usuários (ou seja, usuários específicos, proprietários de grupos, membros do grupo) ou dinamicamente (ou seja, o caso em que cada usuário é revisado por seu gerente). Para criar uma auto-revisão (onde os usuários revisam seu próprio acesso), não forneça aos revisores sobre a criação [de accessReviewScheduleDefinition.](accessreviewscheduledefinition.md)


## <a name="properties"></a>Propriedades
| Propriedade | Tipo | Descrição |
| :-------------------------| :---------- | :---------- |
| consulta | String | A consulta especificando quem será o revistor. Consulte a tabela para ver exemplos. |
| queryType | String | O tipo de consulta. Exemplos incluem `MicrosoftGraph` e `ARM` . |
| queryRoot | String | No cenário em que os revisadores precisam ser especificados dinamicamente, essa propriedade é usada para indicar a fonte relativa da consulta. Essa propriedade só será necessária se uma consulta relativa (ou seja, ./manager) for especificada. |

### <a name="supported-queries-for-accessreviewreviewerscope"></a>Consultas com suporte para accessReviewReviewerScope

|Cenário| consulta | queryType | queryRoot |
|--|--|--|--|
| Proprietário do grupo como revistor | /groups/{group id}/owners |MicrosoftGraph||
| Usuário específico como revistor | /users/{user id} |MicrosoftGraph||
| Gerente do usuário que está sendo revisado como revistor | ./manager | MicrosoftGraph |decisões|

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
