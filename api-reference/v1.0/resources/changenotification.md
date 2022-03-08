---
title: Tipo de recurso changeNotification
description: Representa a notificação de alteração enviada ao assinante.
ms.localizationpriority: medium
author: Jumaodhiss
doc_type: resourcePageType
ms.prod: change-notifications
ms.openlocfilehash: 7ce05497382eb23d3137dd1e1bf2867b38e0095a
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337149"
---
# <a name="changenotification-resource-type"></a>Tipo de recurso changeNotification

Namespace: microsoft.graph

Representa a notificação enviada ao assinante. Todas as propriedades desse recurso são somente leitura.

Para obter detalhes, confira [Usar a API do Microsoft Graph para receber notificações de alteração](webhooks.md).

## <a name="methods"></a>Métodos

Nenhum.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
| changeType | changeType | Indica o tipo de alteração que levantará a notificação de alteração. Os valores com suporte são: `created`, `updated`, `deleted`. Obrigatório. |
| clientState | string | Valor da **propriedade clientState** enviada na solicitação de assinatura (se alguma). O tamanho máximo é de 255 caracteres. O cliente pode verificar se a notificação de alteração veio do serviço comparando os valores da **propriedade clientState** . O valor da **propriedade clientState** enviado com a assinatura é comparado com o valor da **propriedade clientState** recebida com cada notificação de alteração. Opcional. |
| encryptedContent | [changeNotificationEncryptedContent](changenotificationencryptedcontent.md) | (Visualização) Conteúdo criptografado anexado com a notificação de alteração. Somente fornecido se **encryptionCertificate** e **includeResourceData** foram definidos durante a solicitação de assinatura e se o recurso oferece suporte a ela. Opcional. |
| id | cadeia de caracteres | ID exclusiva da notificação. Opcional. |
| lifecycleEvent | lifecycleEventType| O tipo de notificação do ciclo de vida se a notificação atual for uma notificação do ciclo de vida. Opcional. Os valores suportados são `missed`, `subscriptionRemoved`, `reauthorizationRequired`. Opcional.|
| recurso | Cadeia de caracteres | O URI do recurso que emitiu a notificação de alteração em relação a `https://graph.microsoft.com`. Obrigatório. |
| resourceData | [resourceData](resourcedata.md) | O conteúdo dessa propriedade depende do tipo de recurso que está sendo assinado. Opcional. |
| subscriptionExpirationDateTime | DateTimeOffset | O tempo de expiração da assinatura. Obrigatório. |
| subscriptionId | Guid | O identificador exclusivo da assinatura que gerou a notificação. Necessário. |
| tenantId | Guid | O identificador exclusivo do locatário do qual a notificação de alteração se originou. Obrigatório. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.changeNotification"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.changeNotification",
  "id": "String (identifier)",
  "subscriptionId": "Guid",
  "subscriptionExpirationDateTime": "String (timestamp)",
  "clientState": "String",
  "changeType": "String",
  "resource": "String",
  "tenantId": "Guid",
  "encryptedContent": {
    "@odata.type": "microsoft.graph.changeNotificationEncryptedContent"
  },
  "lifecycleEvent": "String",
  "resourceData": {
    "@odata.type": "microsoft.graph.resourceData"
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

