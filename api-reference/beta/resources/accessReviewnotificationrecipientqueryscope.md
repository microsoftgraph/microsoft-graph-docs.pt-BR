---
title: Tipo de recurso accessReviewnotificationrecipientqueryscope
description: Representa os usuários que receberão notificações para avaliações de acesso.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 19b619b7479212e5fc055f5ab19b025d8d512dc1
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896730"
---
# <a name="accessreviewnotificationrecipientqueryscope-resource-type"></a>Tipo de recurso accessReviewnotificationrecipientqueryscope

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Especifica uma lista estática de destinatários (por exemplo, usuários específicos, proprietários de grupo ou membros do grupo) para receber notificações de revisão de acesso.

Herda de [accessReviewNotificationRecipientScope](../resources/accessreviewnotificationrecipientscope.md).

## <a name="properties"></a>Propriedades
| Propriedade | Tipo | Descrição |
| :-------------------------| :---------- | :---------- |
| consulta | Cadeia de caracteres | Isso representa a consulta para quem são os destinatários. Por exemplo, `/groups/{group id}/members` para membros do grupo e para um usuário `/users/{user id}` específico. |
| queryType | Cadeia de caracteres | Indica o tipo de consulta. O valor permitido é `MicrosoftGraph` . |
| queryRoot | Cadeia de caracteres | No cenário em que os revisadores precisam ser especificados dinamicamente, essa propriedade é usada para indicar a fonte relativa da consulta. Essa propriedade só será necessária se uma consulta relativa, ou seja, `./manager` ) for especificada. |


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
