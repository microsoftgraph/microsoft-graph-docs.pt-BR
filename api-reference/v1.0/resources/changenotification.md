---
title: Tipo de recurso changeNotification
description: Representa a notificação de alteração enviada ao assinante.
ms.localizationpriority: medium
author: Jumaodhiss
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: 2d0563a77710b5553f9ace2d58a8c695259a81cf
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59104247"
---
# <a name="changenotification-resource-type"></a>Tipo de recurso changeNotification

Namespace: microsoft.graph

Representa a notificação enviada ao assinante.

Para obter detalhes, confira [Usar a API do Microsoft Graph para receber notificações de alteração](webhooks.md).

## <a name="methods"></a>Métodos

Nenhum.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
| changeType | changeType | Indica o tipo de alteração que levantará a notificação de alteração. Os valores com suporte são: `created`, `updated`, `deleted`. Obrigatório. |
| clientState | string | Valor da **propriedade clientState** enviada na solicitação de assinatura (se alguma). O tamanho máximo é de 255 caracteres. O cliente pode verificar se a notificação de alteração veio do serviço comparando os valores da **propriedade clientState.** O valor da **propriedade clientState** enviado com a assinatura é comparado com o valor da **propriedade clientState** recebida com cada notificação de alteração. Opcional. |
| encryptedContent | [changeNotificationEncryptedContent](changenotificationencryptedcontent.md) | (Visualização) Conteúdo criptografado anexado com a notificação de alteração. Somente fornecido se **encryptionCertificate** e **includeResourceData** foram definidos durante a solicitação de assinatura e se o recurso oferece suporte a ela. Opcional. |
| id | cadeia de caracteres | ID exclusiva da notificação. Opcional. |
| lifecycleEvent | lifecycleEventType| O tipo de notificação do ciclo de vida se a notificação atual for uma notificação do ciclo de vida. Opcional. Os valores suportados `missed` são `subscriptionRemoved` , , `reauthorizationRequired` . |
| recurso | cadeia de caracteres | O URI do recurso que emitiu a notificação de alteração em relação a `https://graph.microsoft.com` . Obrigatório. |
| resourceData | [resourceData](resourcedata.md) | O conteúdo dessa propriedade depende do tipo de recurso que está sendo assinado. Obrigatório. |
| subscriptionExpirationDateTime | DateTimeOffset | O tempo de expiração da assinatura. Obrigatório. |
| subscriptionId | GUID | O identificador exclusivo da assinatura que gerou a notificação. |
| tenantId | GUID | O identificador exclusivo do locatário do qual a notificação de alteração se originou. |

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

