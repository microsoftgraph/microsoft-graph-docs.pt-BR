---
title: Tipo de recurso accessReviewNotificationRecipientItem
description: Define usuários ou grupos que receberão notificações de acesso a notificações de revisão.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: aab29de91f37d04282b357e47d2fefdedf566a9f
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60562106"
---
# <a name="accessreviewnotificationrecipientitem-resource-type"></a>Tipo de recurso accessReviewNotificationRecipientItem

Namespace: microsoft.graph

Representa um evento de notificação de revisão [de](accessreviewsv2-root.md) acesso do Azure AD em uma instância de uma revisão. Este item contém um tipo de modelo de email e propriedades de destinatário para habilitar o envio de determinado tipo de notificações para uma determinada instância de revisão [de acesso.](accessreviewinstance.md)

## <a name="properties"></a>Propriedades

| Propriedade                     | Tipo     | Descrição                          |
| :--------------------------- | :------  | :----------                          |
| notificationTemplateType  |Cadeia de Caracteres  | Indica o tipo de email de revisão de acesso a ser enviado. O tipo de modelo com suporte é , que envia notificações de `CompletedAdditionalRecipients` conclusão de revisão aos destinatários.|
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
