---
title: Tipo de recurso accessReviewNotificationRecipientItem
description: Define usuários ou grupos que receberão notificações de revisão de acesso.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 34b6f56f166fa972171467f89c06ac0090523fc1
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698377"
---
# <a name="accessreviewnotificationrecipientitem-resource-type"></a>Tipo de recurso accessReviewNotificationRecipientItem

Namespace: microsoft.graph

Representa um Azure AD [de notificação de revisão](accessreviewsv2-overview.md) de acesso em uma instância de uma revisão. Este item contém um tipo de modelo de email e propriedades de destinatário para habilitar o envio de determinado tipo de notificações para uma determinada instância [de revisão de acesso](accessreviewinstance.md).

## <a name="properties"></a>Propriedades

| Propriedade                     | Tipo     | Descrição                          |
| :--------------------------- | :------  | :----------                          |
| notificationTemplateType  |Cadeia de Caracteres  | Indica o tipo de email de revisão de acesso a ser enviado. O tipo de modelo com suporte é `CompletedAdditionalRecipients`, que envia notificações de conclusão de revisão para os destinatários.|
| notificationRecipientScope |[accessReviewNotificationRecipientScope](../resources/accessreviewnotificationrecipientscope.md)  | Determina o destinatário do email de notificação.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewNotificationRecipientItem",
  "openType": true
}
-->

```json
{
  "@odata.type":"#microsoft.graph.accessReviewNotificationRecipientItem",
  "notificationRecipientScope": {
      "@odata.type":"#microsoft.graph.accessReviewNotificationRecipientQueryScope"                
    },
  "notificationTemplateType": "String"
}
```
