---
title: Tipo de recurso accessReviewReviewerScope
description: Representa quem revisará uma revisão de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 573e6934250ab6a932922185776b20af92f6f0615f8ede33e87d26e1944386c4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54121428"
---
# <a name="accessreviewreviewerscope-resource-type"></a>Tipo de recurso accessReviewReviewerScope

Namespace: microsoft.graph

O accessReviewReviewerScope define quem revisará instâncias de [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md). É uma consulta OData que permite que os revisadores sejam especificados como uma lista estática de usuários (ou seja, usuários específicos, proprietários de grupos e membros do grupo) ou dinamicamente em que cada usuário é revisado por seu gerente ou por proprietários de grupo. Para criar uma auto-revisão (onde os usuários analisam seu próprio acesso), não forneça aos revisores sobre a criação [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md)

Herda de [accessReviewScope](../resources/accessreviewscope.md).

## <a name="properties"></a>Propriedades
| Propriedade | Tipo | Descrição |
| :-------------------------| :---------- | :---------- |
| consulta | Cadeia de caracteres | A consulta especificando quem será o revistor. Consulte tabela para exemplos. |
| queryType | Cadeia de caracteres | O tipo de consulta. Exemplos incluem `MicrosoftGraph` `ARM` e . |
| queryRoot | Cadeia de caracteres | No cenário em que os revisadores precisam ser especificados dinamicamente, essa propriedade é usada para indicar a fonte relativa da consulta. Essa propriedade só será necessária se uma consulta relativa, por exemplo, `./manager` , for especificada. Valor possível: `decisions` . |

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
