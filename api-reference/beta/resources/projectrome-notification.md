---
title: tipo de recurso de notificação
description: 'Representa uma notificação publicada por um servidor de aplicativos que se destina a um usuário especificado. A notificação é armazenada no Microsoft Graph e é distribuída para diferentes pontos de extremidade do dispositivo de Propriedade do usuário. '
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: af130c9806511b0afbdaedb602790c7c40d3ca2e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563309"
---
# <a name="notification-resource-type"></a>tipo de recurso de notificação
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma notificação publicada por um servidor de aplicativos que se destina a um usuário especificado. A notificação é armazenada no Microsoft Graph e é distribuída para diferentes pontos de extremidade do dispositivo de Propriedade do usuário. 

Uma notificação pode ser uma carga de notificação visual que pode ser interpretada pelo sistema operacional, incluindo plataformas Windows, Android e iOS. Também pode ser uma carga de dados que é entregue e manipulado por clientes de aplicativos, que, em seguida, determinam a experiência do usuário correspondente em cada dispositivo – normalmente, uma interface de usuário de notificação visual que corresponde ao conteúdo da carga de dados original que é gerado localmente. 

Quando um usuário atua em uma notificação Visual, o cliente do aplicativo pode usar o SDK de projeto do lado do cliente Roma para atualizar o estado do feed de notificação correspondente no Microsoft Graph, por exemplo, marcando uma notificação como descartada. A atualização será distribuída para todos os outros pontos de extremidade do cliente de aplicativos, e os clientes cuidam da alteração de acordo, por exemplo, descartando a notificação para impedir que o usuário veja informações redundantes. Os clientes de aplicativos podem acessar o mesmo recurso de notificação mais tarde antes de expirar (mesmo depois de ser marcado como ignorado), como histórico de notificações, por meio do [SDK do Project Roma](https://github.com/Microsoft/project-rome). 

## <a name="methods"></a>Métodos
|Método | Tipo de retorno | Descrição|
|:------|:------------|:-----------|
|[Criar notificação](../api/projectrome-notification-post.md) | [Notifica](projectrome-notification.md) |Criar e enviar uma notificação. |

## <a name="properties"></a>Propriedades
|Nome | Tipo | Descrição|
|:----|:-----|:-----------|
| targetHostName | String | Representa o nome do host do aplicativo para o qual o serviço de chamada deseja postar a notificação para o usuário específico. |
| appNotificationId | String | A ID exclusiva definida pelo servidor de aplicativos de uma notificação que é usada para identificar e direcionar uma notificação individual. |
| expirationDateTime | DateTimeOffset | Define um horário de expiração UTC em uma notificação de usuário-quando o tempo for ativado, a notificação será removida do repositório de feed de notificação do Microsoft Graph completamente e não faz mais parte do histórico de notificações. O valor máximo é 30 dias. |
| payload | EDM. complexType, objeto JSON | Este é o conteúdo de dados de uma notificação de usuário bruto ou Visual que será entregue e consumido pelo cliente do aplicativo que está recebendo esta notificação. |
| Payload. rawContent | String | O conteúdo de notificação de uma notificação de usuário bruto que será entregue e consumido pelo cliente do aplicativo que está recebendo esta notificação. Pelo menos um dos payloads. RawContent e Payload. VisualContent precisam ser válidos para uma solicitação de notificação POST. |
| Payload. Visual | EDM. complexType, objeto JSON | O conteúdo visual de uma notificação de usuário visual, que será consumida pela plataforma de notificação em cada plataforma móvel e renderizada para os usuários. Pelo menos um dos conteúdos e VisualContent precisa ser válido para uma solicitação de notificação POST. |
| Payload. Visual. title | String | O título de uma notificação de usuário visual. Deve ter título ou corpo. |
| Payload. Visual. Body | String | O corpo de uma notificação de usuário visual. Deve ter título ou corpo. |
| displayTimeToLive | Limite | Define por quanto tempo (em segundos) esse conteúdo de notificação permanecerá no Visualizador de notificação de cada plataforma. Por exemplo, quando a notificação é entregue a um dispositivo do Windows, o valor dessa propriedade é passado para ToastNotification. ExpirationTime, que determina por quanto tempo a notificação de notificação de falha permanecerá na central de ações do Windows do usuário. |
| prioridade | EnumType | Indica a prioridade de uma notificação de usuário bruto. As notificações visuais são enviadas com alta prioridade por padrão. Os valores válidos são alto e baixo. |
| Nome_do_grupo | String | O nome do grupo ao qual essa notificação pertence. Ele é definido pelo desenvolvedor com o objetivo de agrupar notificações. |
| targetPolicy | EDM. complexType, objeto JSON | O objeto de política de destino trata a política de entrega de notificação em dois níveis diferentes-tipos de ponto de extremidade (Windows, iOS e Android) que devem ser direcionados e pontos de extremidade específicos (identificados por IDs de assinatura) que devem ser direcionados. |
| targetPolicy. platformTypes | EDM. complexType, coleção (EnumType) | Use para filtrar a distribuição de notificação para uma plataforma ou plataformas específicas. Por padrão, todos os tipos de ponto de extremidade de envio (iOS, Windows e Android) estão habilitados. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso quando você publica uma notificação Visual direta que é entregue ao sistema operacional de destino.

```json
{   
  "targetHostName": "String",
  "appNotificationId": "String",
  "expirationDateTime": "DateTimeOffset",
  "payload":  
  {
    "visualContent": 
    {
      "title": "String",
      "body": "String"
    },
  },
  "displayTimeToLive": "Int",
  "priority": "Enum",
  "groupName": "String",
  "targetPolicy":
  {
    "platformTypes": [ 
      "Enum"
    ]
  }
}
```

Veja a seguir uma representação JSON do recurso quando você publica uma notificação de dados brutos entregue a clientes de aplicativos.
```json
{   
  "targetHostName": "String",
  "appNotificationId": "String",
  "expirationDateTime": "DateTimeOffset",
  "payload":  
  {
    "rawContent": "String"
  },
  "displayTimeToLive": "Int",
  "priority": "Enum",
  "groupName": "String",
  "targetPolicy":
  {
    "platformTypes": [ 
      "Enum"
    ]
  }
}
```
