---
title: tipo de recurso changeNotification
description: Representa a notificação de alteração enviada ao Assinante.
localization_priority: Normal
author: baywet
doc_type: resourcePageType
ms.prod: non-product-specific
ms.openlocfilehash: 5aa207fba6293db3ca1d0de4879639a4ea1c1b76
ms.sourcegitcommit: 41a5bd5868685c10181f6285d5ac91c6dad556e2
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 07/04/2020
ms.locfileid: "45038519"
---
# <a name="changenotification-resource-type"></a>tipo de recurso changeNotification

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a notificação enviada ao Assinante.

Para obter detalhes, consulte [usar a API do Microsoft Graph para obter notificações de alteração](webhooks.md).

## <a name="methods"></a>Métodos

Nenhum.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
| changeType | string | Indica o tipo de alteração que irá gerar a notificação de alteração. Os valores com suporte são: `created`, `updated`, `deleted`. Obrigatório. |
| clientState | string | O valor da propriedade **ClientState** enviado especificado na solicitação de assinatura (se houver). O tamanho máximo é de 255 caracteres. O cliente pode verificar se a notificação de alteração veio do serviço, comparando os valores da propriedade **ClientState** . O valor da propriedade **ClientState** enviada com a assinatura é comparado com o valor da propriedade **ClientState** recebida com cada notificação de alteração. Opcional. |
| encryptedContent | [Microsoft. Graph. changeNotificationEncryptedContent](changenotificationencryptedcontent.md) | Prever Conteúdo criptografado anexado à notificação de alteração. Só é fornecido se **encryptionCertificate** e **includeResourceData** foram definidos durante a solicitação de assinatura e se o recurso oferecer suporte a ele. Opcional |
| lifecycleEvent | string | O tipo de notificação de ciclo de vida se a notificação atual é uma notificação de ciclo de vida. Opcional. Os valores com suporte são `missed` , `removed` , `reauthorizationRequired` . |
| id | cadeia de caracteres | ID exclusiva da notificação. Opcional. |
| recurso | string | O URI do recurso que emitiu a notificação de alteração relativa a `https://graph.microsoft.com` . Obrigatório. |
| resourceData | [Microsoft. Graph. resourceData](resourcedata.md) | O conteúdo dessa propriedade depende do tipo de recurso que está sendo assinado. Obrigatório. |
| subscriptionExpirationDateTime | [dateTime](https://tools.ietf.org/html/rfc3339) | O tempo de expiração da assinatura. Obrigatório. |
| subscriptionId | string | O identificador exclusivo da assinatura que gerou a notificação. |
| tenantId | #c0 | O identificador exclusivo do locatário do qual a notificação de alteração se originou. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.changeNotification"
}-->

```json
{
  "subscriptionId": "76222963-cc7b-42d2-882d-8aaa69cb2ba3",
  "changeType": "created",
  "clientState": "client state provided when creating subscription",
  "id": "15ee1d1f-af7b-42d9-885b-9d00db065dd9",
  "tenantId": "2c937fad-a8a7-496c-b0e4-bf77dcc7eb2a",
  "subscriptionExpirationDateTime": "2020-04-12T23:20:50.52Z",
  "resource": "teams('d29828b8-c04d-4e2a-b2f6-07da6982f0f0')/channels('19:f127a8c55ad949d1a238464d22f0f99e@thread.skype')/messages('1565045424600')/replies('1565047490246')",
  "resourceData": {
    "id": "1565293727947",
    "@odata.type": "#Microsoft.Graph.ChatMessage",
    "@odata.id": "teams('88cbc8fc-164b-44f0-b6a6-b59b4a1559d3')/channels('19:8d9da062ec7647d4bb1976126e788b47@thread.tacv2')/messages('1565293727947')/replies('1565293727947')"
  }
}
```

<!-- uuid: 15ee1d1f-af7b-42d9-885b-9d00db065dd9
2020-05-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "change notification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
