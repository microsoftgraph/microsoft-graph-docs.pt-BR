---
title: tipo de recurso de notificação (preterido)
description: 'Representa uma notificação publicada por um servidor de aplicativos destinado a um usuário especificado. A notificação é armazenada no Microsoft Graph e é distribuída para diferentes pontos de extremidade de dispositivo pertencentes ao usuário. '
ms.localizationpriority: medium
ms.prod: notifications
doc_type: resourcePageType
author: merzink
ms.openlocfilehash: c2b8c64ca775c0e57d44a5735133b55984fbe193
ms.sourcegitcommit: 7a0f9f1a535795c6f77c80e02fd97581c36f1273
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/27/2021
ms.locfileid: "61608749"
---
# <a name="notification-resource-type-deprecated"></a>tipo de recurso de notificação (preterido)

Namespace: microsoft.graph

> [!IMPORTANT]
> A API Graph de notificações da Microsoft está preterida e interromperá o retorno de dados até o final de janeiro de 2022. Para obter uma experiência de notificação alternativa, [consulte Microsoft Azure Hubs](/azure/notification-hubs)de Notificação e confira [esta postagem de blog](https://devblogs.microsoft.com/microsoft365dev/retiring-microsoft-graph-notifications/) para obter mais informações.

Representa uma notificação publicada por um servidor de aplicativos destinado a um usuário especificado. A notificação é armazenada no Microsoft Graph e é distribuída para diferentes pontos de extremidade de dispositivo pertencentes ao usuário. 

Uma notificação pode ser uma carga de notificação visual que pode ser interpretada pelo sistema operacional (Windows, Android e plataformas iOS). Também pode ser uma carga de dados (rawContent) que é entregue e manipulada por clientes de aplicativo (incluindo a Web), que determina a experiência do usuário correspondente em cada dispositivo.  Geralmente, essa é uma interface do usuário de notificação visual, gerada localmente, que corresponde ao conteúdo na carga de dados original. 

Quando um usuário age em uma notificação visual, o cliente de aplicativo pode usar o SDK de notificações do lado do cliente para atualizar o estado do feed de notificação correspondente no Microsoft Graph - por exemplo, marcando uma notificação como descartada. Em seguida, a atualização será distribuída para todos os outros pontos de extremidade do cliente de aplicativo e os clientes lidam com a alteração de acordo, por exemplo, descartando a notificação para impedir que o usuário veja informações redundantes. Os clientes de aplicativos podem acessar o mesmo recurso de notificação posteriormente antes de expirar (mesmo depois de marcado como ignorado), como histórico de notificação, por meio do [SDK de notificação.](https://aka.ms/GNSDK) 

> [!NOTE]
> As atualizações de estado de notificação, como leitura ou descartada, não serão descartadas para os pontos de extremidade da Web. Isso porque os pushs da Web em vários navegadores exigem que as notificações visuais do sistema sejam exibidas para um usuário. Como as alterações de estado não têm conteúdo visual correspondente, elas serão disponibilizadas apenas para notificações que direcionam Windows, iOS ou plataformas Android.

## <a name="methods"></a>Métodos
|Método | Tipo de retorno | Descrição|
|:------|:------------|:-----------|
|[Criar notificação](../api/user-post-notifications.md) | [notification](projectrome-notification.md) |Crie e envie uma notificação. |

## <a name="properties"></a>Propriedades
|Nome | Tipo | Descrição|
|:----|:-----|:-----------|
| targetHostName | Cadeia de caracteres | Representa o nome de host do aplicativo para o qual o serviço de chamada deseja postar a notificação, para o usuário determinado. Se direcionar pontos de extremidade da Web (consulte **targetPolicy.platformTypes**), verifique se **targetHostName** é o mesmo que o nome usado ao criar uma assinatura no lado do cliente dentro da propriedade JSON do aplicativo. |
| appNotificationId | Cadeia de caracteres | A ID exclusiva definida pelo servidor de aplicativos de uma notificação usada para identificar e direcionar uma notificação individual. |
| groupName | Cadeia de caracteres | O nome do grupo ao que essa notificação pertence. Ele é definido pelo desenvolvedor com o objetivo de agrupar notificações. |
| targetPolicy | [targetPolicyEndpoints](targetpolicyendpoints.md) | O objeto de política de destino lida com a política de entrega de notificação para tipos de ponto de extremidade que devem ser direcionados (Windows, iOS, Android e WebPush) para o usuário específico. |
| payload | [payloadTypes](payloadtypes.md)| Esse é o conteúdo de dados de uma notificação de usuário bruta ou visual que será entregue e consumida pelo cliente de aplicativo que recebe essa notificação. |
| displayTimeToLive | Int32 | Define por quanto tempo (em segundos) esse conteúdo de notificação ficará no visualizador de notificação de cada plataforma. Por exemplo, quando a notificação é entregue a um dispositivo Windows, o valor dessa propriedade é passado para ToastNotification.ExpirationTime, que determina por quanto tempo a notificação do notificação de notificação do Windows do usuário. |
| expirationDateTime | DateTimeOffset | Define uma data e hora de expiração UTC em uma notificação de usuário usando o formato ISO 8601 (por exemplo, meia-noite UTC em 1º de janeiro de 2019 teria esta aparência: `'2019-01-01T00:00:00Z'` ). Quando o tempo acabou, a notificação é removida do armazenamento de feed de notificação do Microsoft Graph completamente e não faz mais parte do histórico de notificação. O valor máximo é 30 dias. |
| prioridade | cadeia de caracteres | Indica a prioridade de uma notificação de usuário bruta. As notificações visuais são enviadas com alta prioridade por padrão. Os valores válidos são `None`, `High` e `Low`. |
| fallbackPolicy | [fallbackpolicy](fallbackpolicy.md) | O objeto de política de fallback opcional lida com a política de fallback de notificação apenas para pontos de extremidade do iOS e foi projetado para ser usado para notificações brutas de alta prioridade que podem não ser entregues a dispositivos devido a restrições específicas da plataforma (por exemplo, modo de economia de bateria). |


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
  "fallbackPolicy": {"@odata.type": "microsoft.graph.fallbackpolicy"} 
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


