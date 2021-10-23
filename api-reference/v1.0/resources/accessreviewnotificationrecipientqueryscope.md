---
title: Tipo de recurso accessReviewnotificationrecipientqueryscope
description: Especifica uma lista de usuários que receberão notificações para avaliações de acesso.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 82d1cbffd3e51ee8aff5dee3bdefd3196d004243
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60562108"
---
# <a name="accessreviewnotificationrecipientqueryscope-resource-type"></a>Tipo de recurso accessReviewnotificationrecipientqueryscope

Namespace: microsoft.graph

Especifica uma lista estática de destinatários (por exemplo, usuários específicos, proprietários de grupo ou membros do grupo) para receber notificações de revisão de acesso.

Herda de [accessReviewNotificationRecipientScope](../resources/accessreviewnotificationrecipientscope.md).

## <a name="properties"></a>Propriedades
| Propriedade | Tipo | Descrição |
| :-------------------------| :---------- | :---------- |
| consulta | Cadeia de Caracteres | Representa a consulta para quem são os destinatários. Por exemplo, `/groups/{group id}/members` para membros do grupo e para um usuário `/users/{user id}` específico. |
| queryType | Cadeia de Caracteres | Indica o tipo de consulta. O valor permitido é `MicrosoftGraph` . |
| queryRoot | Cadeia de Caracteres | No cenário em que os revisadores precisam ser especificados dinamicamente, indica a origem relativa da consulta. Essa propriedade só será necessária se uma consulta relativa (ou seja, `./manager` ) for especificada. |


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewNotificationRecipientQueryScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewNotificationRecipientQueryScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String"
}
```
