---
title: Tipo de recurso accessReviewnotificationrecipientqueryscope
description: Representa os usuários que receberão notificações para revisões de acesso.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: fae6a904f06424f79ea96ce4750efa67f6cf1cd4
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697950"
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
| consulta | Cadeia de caracteres | Isso representa a consulta para quem são os destinatários. Por exemplo, para `/groups/{group id}/members` membros do grupo e `/users/{user id}` para um usuário específico. |
| queryType | Cadeia de caracteres | Indica o tipo de consulta. O valor permitido é `MicrosoftGraph`. |
| queryRoot | Cadeia de Caracteres | No cenário em que os revisores precisam ser especificados dinamicamente, essa propriedade é usada para indicar a origem relativa da consulta. Essa propriedade só será necessária se uma consulta relativa, ou seja, `./manager`) for especificada. |


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
