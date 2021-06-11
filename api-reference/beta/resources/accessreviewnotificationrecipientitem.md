---
title: Tipo de recurso accessReviewNotificationRecipientItem
description: Define usuários ou grupos que receberão notificações de acesso a notificações de revisão.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3d6ed767f1350f3e4a43a1b31363920ffb58a9b5
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896729"
---
# <a name="accessreviewnotificationrecipientitem-resource-type"></a>Tipo de recurso accessReviewNotificationRecipientItem

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]


Representa um evento de notificação de revisão [de](accessreviewsv2-root.md) acesso do Azure AD em uma instância de uma revisão. Este item contém um tipo de modelo de email e propriedades de destinatário para habilitar o envio de determinado tipo de notificações para uma determinada instância de revisão [de acesso.](accessreviewinstance.md)

## <a name="properties"></a>Propriedades

| Propriedade                     | Tipo     | Descrição                          |
| :--------------------------- | :------  | :----------                          |
| notificationTemplateType  |Cadeia de caracteres  | Indica o tipo de email de revisão de acesso a ser enviado. O tipo de modelo com suporte é o que envia notificações de conclusão `CompletedAdditionalRecipients` de revisão aos destinatários.|
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
