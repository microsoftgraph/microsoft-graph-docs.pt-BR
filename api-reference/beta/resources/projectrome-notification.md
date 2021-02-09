---
title: tipo de recurso de notificação
description: 'Representa uma notificação publicada por um servidor de aplicativos destinado a um usuário especificado. A notificação é armazenada no Microsoft Graph e distribuída para pontos de extremidade de dispositivo diferentes pertencentes ao usuário. '
localization_priority: Normal
ms.prod: notifications
doc_type: resourcePageType
author: merzink
ms.openlocfilehash: abd17119e80e4e8a7967197356811ee519d813ba
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159448"
---
# <a name="notification-resource-type"></a>tipo de recurso de notificação

Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma notificação publicada por um servidor de aplicativos destinado a um usuário especificado. A notificação é armazenada no Microsoft Graph e distribuída para pontos de extremidade de dispositivo diferentes pertencentes ao usuário. 

Uma notificação pode ser uma carga de notificação visual que pode ser interpretada pelo sistema operacional (plataformas Windows, Android e iOS). Também pode ser uma carga de dados (rawContent) entregue e manipulada por clientes de aplicativo (incluindo a Web), que determina a experiência do usuário correspondente em cada dispositivo.  Isso geralmente é uma interface do usuário de notificação visual, gerada localmente, que corresponde ao conteúdo na carga de dados original. 

Quando um usuário atua em uma notificação visual, o cliente do aplicativo pode então usar o SDK de notificações do lado do cliente para atualizar o estado do feed de notificação correspondente no Microsoft Graph, por exemplo, marcando uma notificação como descartada. A atualização será então distribuída a todos os outros pontos de extremidade do cliente do aplicativo, e os clientes lidarão com a alteração de acordo, por exemplo, descartando a notificação para impedir que o usuário veja informações redundantes. Os clientes do aplicativo podem acessar o mesmo recurso de notificação posteriormente antes de expirar (mesmo depois de ser marcado como ignorado), como histórico de notificações, por meio do [SDK de notificação.](https://aka.ms/GNSDK) 

> [!NOTE]
> As atualizações de estado de notificação, como lidas ou descartadas, não serão fan-out para pontos de extremidade da Web. Isso porque os pushs da Web em vários navegadores exigem que as notificações do sistema visual sejam exibidas para um usuário. Como as alterações de estado não têm conteúdo visual correspondente, elas só terão fan-out para notificações para as plataformas Windows, iOS ou Android.

## <a name="methods"></a>Métodos
|Método | Tipo de retorno | Descrição|
|:------|:------------|:-----------|
|[Criar notificação](../api/user-post-notifications.md) | [notificação](projectrome-notification.md) |Crie e envie uma notificação. |

## <a name="properties"></a>Propriedades
|Nome | Tipo | Descrição|
|:----|:-----|:-----------|
| targetHostName | String | Representa o nome de host do aplicativo para o qual o serviço de chamada deseja postar a notificação para o usuário determinado. Se estiver direcionando pontos de extremidade da Web (consulte **targetPolicy.platformTypes**), verifique se **targetHostName** é o mesmo nome usado ao criar uma assinatura no lado do cliente dentro da propriedade JSON do aplicativo. |
| appNotificationId | String | A ID exclusiva definida pelo servidor de aplicativo de uma notificação que é usada para identificar e direcionar uma notificação individual. |
| groupName | String | O nome do grupo ao que essa notificação pertence. Ele é definido pelo desenvolvedor para agrupar as notificações. |
| targetPolicy | [targetPolicyEndpoints](targetpolicyendpoints.md) | O objeto de política de destino lida com a política de entrega de notificação para tipos de ponto de extremidade que devem ser direcionados (Windows, iOS, Android e WebPush) para o usuário específico. |
| payload | [payloadTypes](payloadtypes.md)| Esse é o conteúdo de dados de uma notificação bruta ou visual do usuário que será entregue e consumida pelo cliente de aplicativo que recebe essa notificação. |
| displayTimeToLive | Int32 | Define por quanto tempo (em segundos) esse conteúdo de notificação ficará no visualizador de notificações de cada plataforma. Por exemplo, quando a notificação é entregue a um dispositivo Windows, o valor dessa propriedade é passado para ToastNotification.ExpirationTime, que determina por quanto tempo a notificação do sistema ficará na Central de Ações do Windows do usuário. |
| expirationDateTime | DateTimeOffset | Define uma data e hora de expiração UTC em uma notificação do usuário usando o formato ISO 8601 (por exemplo, meia-noite em UTC no dia 1º de janeiro de 2019 teria esta aparência: `'2019-01-01T00:00:00Z'` ). Quando o tempo acaba, a notificação é removida do armazenamento de feeds de notificação do Microsoft Graph completamente e não faz mais parte do histórico de notificações. O valor máximo é de 30 dias. |
| prioridade | string | Indica a prioridade de uma notificação de usuário bruta. As notificações visuais são enviadas com alta prioridade por padrão. Os valores válidos são `None`, `High` e `Low`. |
| fallbackPolicy | [fallbackpolicy](fallbackpolicy.md) | O objeto de política de fallback opcional lida com a política de fallback de notificação somente para pontos de extremidade do iOS e foi projetado para ser usado para notificações brutas de alta prioridade que podem não ser entregues a dispositivos devido a restrições específicas da plataforma (por exemplo, modo de economia de bateria). |


## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.notification",
  "keyProperty": "id"
}-->

```json
{
  "targetHostName": "String",
  "appNotificationid": "String (identifier)",
  "groupName": "String", 
  "targetPolicy": {"@odata.type": "microsoft.graph.targetPolicyEndpoints"},
  "payload": {"@odata.type": "microsoft.graph.payloadTypes"},
  "displayTimeToLive": 1024,
  "expirationDateTime": "String (timestamp)",
  "priority": "string",
  "fallbackPolicy": {"@odata.type": "microsoft.graph.fallbackpolicy"},  
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


