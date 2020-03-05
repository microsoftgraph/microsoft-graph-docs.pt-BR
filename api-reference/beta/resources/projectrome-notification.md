---
title: tipo de recurso de notificação
description: 'Representa uma notificação publicada por um servidor de aplicativos que se destina a um usuário especificado. A notificação é armazenada no Microsoft Graph e é distribuída para diferentes pontos de extremidade do dispositivo de Propriedade do usuário. '
localization_priority: Normal
ms.prod: notifications
doc_type: resourcePageType
author: merzink
ms.openlocfilehash: 2b72c55d7159f44fbc368acda9c431ef96be3905
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521401"
---
# <a name="notification-resource-type"></a>tipo de recurso de notificação

Namespace: Microsoft. Graph[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma notificação publicada por um servidor de aplicativos que se destina a um usuário especificado. A notificação é armazenada no Microsoft Graph e é distribuída para diferentes pontos de extremidade do dispositivo de Propriedade do usuário. 

Uma notificação pode ser uma carga de notificação visual que pode ser interpretada pelo sistema operacional (Windows, Android e plataformas iOS). Também pode ser uma carga de dados (rawContent) que é entregue e manipulada por clientes de aplicativos (incluindo Web), que, em seguida, determinam a experiência do usuário correspondente em cada dispositivo.  Isso geralmente é uma interface do usuário de notificação Visual, gerada localmente, que corresponde ao conteúdo da carga de dados original. 

Quando um usuário atua em uma notificação Visual, o cliente do aplicativo pode usar o SDK de notificações do lado do cliente para atualizar o estado do feed de notificação correspondente no Microsoft Graph, por exemplo, marcando uma notificação como descartada. A atualização será distribuída para todos os outros pontos de extremidade do cliente de aplicativos, e os clientes cuidam da alteração de acordo, por exemplo, descartando a notificação para impedir que o usuário veja informações redundantes. Os clientes de aplicativos podem acessar o mesmo recurso de notificação mais tarde antes de expirar (mesmo depois de ser marcado como ignorado), como histórico de notificações, por meio do [SDK de notificação](https://aka.ms/GNSDK). 

> [!NOTE]
> As atualizações de estado de notificação, como lidas ou ignoradas, não serão fanned para os pontos de extremidade da Web. Isso ocorre porque os envios da Web em vários navegadores exigem que as notificações visuais de torradeira sejam exibidas para um usuário. Como as alterações de estado não possuem conteúdo visual correspondente, elas só serão fanneddas para notificações direcionadas a plataformas Windows, iOS ou Android.

## <a name="methods"></a>Métodos
|Método | Tipo de retorno | Descrição|
|:------|:------------|:-----------|
|[Criar notificação](../api/user-post-notifications.md) | [Notifica](projectrome-notification.md) |Criar e enviar uma notificação. |

## <a name="properties"></a>Propriedades
|Nome | Tipo | Descrição|
|:----|:-----|:-----------|
| targetHostName | String | Representa o nome do host do aplicativo para o qual o serviço de chamada deseja postar a notificação para o usuário específico. Se estiver direcionando pontos de extremidade da Web (consulte **targetPolicy. platformTypes**), certifique-se de que **targetHostName** é igual ao nome usado ao criar uma assinatura no lado do cliente dentro da propriedade JSON do aplicativo. |
| appNotificationId | String | A ID exclusiva definida pelo servidor de aplicativos de uma notificação que é usada para identificar e direcionar uma notificação individual. |
| Nome_do_grupo | String | O nome do grupo ao qual essa notificação pertence. Ele é definido pelo desenvolvedor com o objetivo de agrupar notificações. |
| targetPolicy | [targetPolicyEndpoints](targetpolicyendpoints.md) | O objeto de política de destino manipula a política de entrega de notificação para tipos de ponto de extremidade que devem ser direcionados (Windows, iOS, Android e webpush) para o usuário fornecido. |
| payload | [payloadTypes](payloadtypes.md)| Este é o conteúdo de dados de uma notificação de usuário bruto ou Visual que será entregue e consumido pelo cliente do aplicativo que está recebendo esta notificação. |
| displayTimeToLive | Int32 | Define por quanto tempo (em segundos) esse conteúdo de notificação permanecerá no Visualizador de notificação de cada plataforma. Por exemplo, quando a notificação é entregue a um dispositivo do Windows, o valor dessa propriedade é passado para ToastNotification. ExpirationTime, que determina por quanto tempo a notificação de notificação de falha permanecerá na central de ações do Windows do usuário. |
| expirationDateTime | DateTimeOffset | Define uma data e hora de vencimento UTC em uma notificação de usuário usando o formato ISO 8601 (por exemplo, meia-noite UTC em 1º de janeiro de `'2019-01-01T00:00:00Z'`2019 teria a seguinte aparência:). Quando o tempo é concluído, a notificação é removida do repositório de feeds de notificação do Microsoft Graph completamente e não faz mais parte do histórico de notificações. O valor máximo é 30 dias. |
| prioridade | string | Indica a prioridade de uma notificação de usuário bruto. As notificações visuais são enviadas com alta prioridade por padrão. Os valores válidos são `None`, `High` e `Low`. |
| fallbackPolicy | [fallbackPolicy](fallbackpolicy.md) | O objeto de política de fallback opcional trata da política de fallback de notificação para pontos de extremidade iOS somente e é projetado para ser usado para notificações brutas de alta prioridade que podem não ser entregues aos dispositivos devido a restrições específicas de plataforma (por exemplo, modo economia de bateria). |


## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.notification",
  "baseType": "",
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
