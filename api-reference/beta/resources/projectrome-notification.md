---
title: tipo de recurso de notificação
description: 'Representa uma notificação que é publicada por um servidor de aplicativo que tem como destino um usuário especificado. A notificação é armazenada no Microsoft Graph e é distribuída aos pontos de extremidade de dispositivo diferente pertencentes ao usuário. '
localization_priority: Normal
ms.openlocfilehash: cc68b95e01452e657187e42aa5f92bfec07f396a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869535"
---
# <a name="notification-resource-type"></a>tipo de recurso de notificação
> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa uma notificação que é publicada por um servidor de aplicativo que tem como destino um usuário especificado. A notificação é armazenada no Microsoft Graph e é distribuída aos pontos de extremidade de dispositivo diferente pertencentes ao usuário. 

Uma notificação pode ser uma carga de notificação visual que possa ser interpretada por um sistema operacional, incluindo as plataformas Windows, Android e iOS. Ele também pode ser uma carga de dados que tem entregues e manipulados pelos clientes app, que, em seguida, determine o usuário correspondente experiência em cada dispositivo – em geral, uma notificação visual da interface do usuário que corresponde ao conteúdo a carga de dados original que seja gerada localmente. 

Quando um usuário atua em uma notificação visual, o cliente app pode usar, em seguida, Roma SDK do lado do cliente Project para atualizar o estado da notificação correspondente feed no Microsoft Graph - por exemplo, marcando uma notificação conforme descartado. A atualização, em seguida, será distribuída para todos os outros pontos de cliente app e os clientes manipular a alteração apropriadamente, por exemplo, descarte a notificação para impedir que o usuário ver informações redundantes. Clientes de aplicativo podem acessar o mesmo recurso de notificação em um momento posterior antes que ela expire (mesmo depois que ela é marcada como descartado), como histórico de notificação, por meio do [SDK do Project Roma](https://github.com/Microsoft/project-rome). 

## <a name="methods"></a>Métodos
|Método | Tipo de retorno | Descrição|
|:------|:------------|:-----------|
|[Criar notificação](../api/projectrome-notification-post.md) | [notificação](projectrome-notification.md) |Criar e enviar uma notificação. |

## <a name="properties"></a>Propriedades
|Nome | Tipo | Descrição|
|:----|:-----|:-----------|
| targetHostName | Cadeia de caracteres | Representa o nome de host do aplicativo ao qual o serviço de chamada deseja postar a notificação, para um determinado usuário. |
| appNotificationId | Cadeia de caracteres | A id exclusiva definida pelo servidor de aplicativo de uma notificação que é usado para identificar e uma notificação individual de destino. |
| expirationDateTime | DateTimeOffset | Define um tempo de expiração de UTC em uma notificação de usuário - quando o tempo é para cima, a notificação é removida do repositório de feed de notificação do Microsoft Graph completamente e não está mais parte do histórico de notificação. Valor máximo é 30 dias. |
| payload | Edm.ComplexType, o objeto JSON | Esse é o conteúdo de dados de uma notificação de usuário brutos ou visual que serão entregues e consumido pelo cliente app receber essa notificação. |
| payload.rawContent | Cadeia de caracteres | O conteúdo de notificação de uma notificação de usuário brutos que serão entregues e consumido pelo cliente app receber essa notificação. Pelo menos uma das Payload.RawContent e Payload.VisualContent precisa ser válida para uma solicitação de notificação de POSTAGEM. |
| payload.Visual | Edm.ComplexType, o objeto JSON | O conteúdo visual de uma notificação de usuário visual, que será consumida pela plataforma de notificação em cada plataforma móvel e renderizado para os usuários. Pelo menos um dos conteúdo e VisualContent precisa ser válida para uma solicitação de notificação de POSTAGEM. |
| payload.Visual.Title | Cadeia de caracteres | O título de uma notificação de usuário visual. Deve ter o título ou corpo. |
| payload.Visual.body | Cadeia de caracteres | O corpo de uma notificação de usuário visual. Deve ter o título ou corpo. |
| displayTimeToLive | Int | Define quanto tempo (em segundos) esse conteúdo notificação permanecerão no Visualizador de notificação da cada plataforma. Por exemplo, quando a notificação é entregue a um dispositivo do Windows, o valor dessa propriedade é passado para ToastNotification.ExpirationTime, que determina quanto tempo a notificação de proposta permanecerão na Central de ações do Windows do usuário. |
| prioridade | EnumType | Indica a prioridade de uma notificação de usuário brutos. Por padrão, notificações visuais são enviadas com alta prioridade. Valores válidos são de alta e baixa. |
| groupName | Cadeia de caracteres | O nome do grupo ao qual essa notificação pertence. Ela é definida pelo desenvolvedor para fins de agrupamento de notificações. |
| targetPolicy | Edm.ComplexType, o objeto JSON | Política de entrega da notificação em dois níveis diferentes - tipos de ponto de extremidade (Windows, iOS e Android) que devem ser direcionados e pontos de extremidade específicos (identificados por ids de inscrição) que devem ser direcionados lida com o objeto de diretiva de destino. |
| targetPolicy.platformTypes | Edm.ComplexType, a coleção (EnumType) | Use para filtrar a distribuição de notificação para uma plataforma específica ou plataformas. Por padrão, todos os tipos de ponto de extremidade de push (iOS, Windows e Android) estão habilitados. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
A seguir está uma representação JSON do recurso quando você publica uma notificação visual direta que será enviada para o sistema operacional de destino.

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

A seguir está uma representação JSON do recurso quando você publica uma notificação de dados brutos é entregue aos clientes app.
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
