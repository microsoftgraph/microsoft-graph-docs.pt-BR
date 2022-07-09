---
title: Tipo de recurso accessReviewReviewerScope
description: Representa quem examinará uma revisão de acesso.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5374d68318349a9ae4fa7cb36c54e0aa8efe8870
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66696529"
---
# <a name="accessreviewreviewerscope-resource-type"></a>Tipo de recurso accessReviewReviewerScope

Namespace: microsoft.graph

O accessReviewReviewerScope define quem examinará as instâncias de [um accessReviewScheduleDefinition](accessreviewscheduledefinition.md). É uma consulta OData que permite que os revisores sejam especificados como uma lista estática de usuários (ou seja, usuários específicos, proprietários de grupos e membros do grupo) ou dinamicamente em que cada usuário é examinado por seu gerente ou por proprietários de grupo. Para criar uma auto-revisão (em que os usuários examinam seu próprio acesso), não forneça revisores na criação [de accessReviewScheduleDefinition](accessreviewscheduledefinition.md) .

Herda de [accessReviewScope](../resources/accessreviewscope.md).

## <a name="properties"></a>Propriedades
| Propriedade | Tipo | Descrição |
| :-------------------------| :---------- | :---------- |
| consulta | Cadeia de caracteres | A consulta que especifica quem será o revistor. Consulte a tabela para obter exemplos. |
| queryType | Cadeia de caracteres | O tipo de consulta. Os exemplos incluem `MicrosoftGraph` e `ARM`. |
| queryRoot | Cadeia de caracteres | No cenário em que os revisores precisam ser especificados dinamicamente, essa propriedade é usada para indicar a origem relativa da consulta. Essa propriedade só será necessária se uma consulta relativa, por exemplo, `./manager`for especificada. Valor possível: `decisions`. |

Para obter mais informações sobre as opções de configuração para **revisores**, consulte [Atribuir revisores à sua definição de revisão de acesso usando o Microsoft API do Graph](/graph/accessreviews-reviewers-concept).


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
