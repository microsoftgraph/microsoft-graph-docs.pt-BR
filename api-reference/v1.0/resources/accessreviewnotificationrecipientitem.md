---
title: Tipo de recurso accessReviewNotificationRecipientItem
description: Define usuários ou grupos que receberão notificações de acesso a notificações de revisão.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7f63f9cfe3e1233407d0aaf966d9e2c0d933da26
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2021
ms.locfileid: "61649686"
---
# <a name="accessreviewnotificationrecipientitem-resource-type"></a>Tipo de recurso accessReviewNotificationRecipientItem

Namespace: microsoft.graph

Representa um evento de notificação de revisão [de](accessreviewsv2-overview.md) acesso do Azure AD em uma instância de uma revisão. Este item contém um tipo de modelo de email e propriedades de destinatário para habilitar o envio de determinado tipo de notificações para uma determinada instância de revisão [de acesso.](accessreviewinstance.md)

## <a name="properties"></a>Propriedades

| Propriedade                     | Tipo     | Descrição                          |
| :--------------------------- | :------  | :----------                          |
| notificationTemplateType  |String  | Indica o tipo de email de revisão de acesso a ser enviado. O tipo de modelo com suporte é , que envia notificações de `CompletedAdditionalRecipients` conclusão de revisão aos destinatários.|
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
