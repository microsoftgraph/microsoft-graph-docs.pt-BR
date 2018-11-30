---
title: Trabalhando com a API de reuniões online no Microsoft Graph e de chamadas
description: O Microsoft Graph chama e reuniões online API adiciona uma nova dimensão a como seus aplicativos e serviços podem interagir com os usuários, permitindo que os recursos de vídeos e voz. A API permite criar chamadas e receber chamadas de usuários e aplicativos no Microsoft Teams. Você pode usar essas APIs para criar um aplicativo de serviço (bot) que possa atuar como um participante de uma chamada ou reunião.
ms.openlocfilehash: fcb1d69e204f5bba7c1ece01bcd61ae21f6ca6b4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033476"
---
# <a name="working-with-the-calls-and-online-meetings-api-in-microsoft-graph"></a>Trabalhando com a API de reuniões online no Microsoft Graph e de chamadas

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

O Microsoft Graph chama e reuniões online API adiciona uma nova dimensão a como seus aplicativos e serviços podem interagir com os usuários, permitindo que os recursos de vídeos e voz. A API permite criar chamadas e receber chamadas de usuários e aplicativos no Microsoft Teams. Você pode usar essas APIs para criar um aplicativo de serviço (bot) que possa atuar como um participante de uma chamada ou reunião.

## <a name="call-types"></a>Tipos de chamada

As chamadas são classificadas como chamadas ponto a ponto ou mais participantes. Um usuário pode iniciar uma chamada ponto a ponto com sua bot ou convidar sua bot em uma conferência com vários participantes existente. Não há permissões são necessárias quando o usuário está convidando o bot para uma chamada ponto a ponto. Para o seu bot participar de uma chamada com vários participantes, o bot precisa ter a permissão do administrador de locatário para ingressar em uma chamada do grupo.

![Uma imagem mostrando as chamadas ponto a ponto e multipontos](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/call-types.png)

Se seu bot está criando a chamada, ele precisa ter a permissão de chamada do grupo de iniciar ou o iniciar. Sua bot tem a opção para criar uma chamada ponto a ponto ou uma chamada com vários participantes.

- Para uma chamada ponto a ponto, o bot deve especificar apenas um destino e nenhum coordenadas de reunião. 
- Se seu bot inicia uma chamada com vários participantes, uma reunião ad hoc está configurada em segundo plano e everyone ingressa conferência. Se a reunião coordenadas forem especificadas, uma chamada com vários participantes está configurada, mesmo se não houver apenas um destino.

Uma chamada pode iniciar como ponto a ponto e escale para com vários participantes. Uma conferência é provisionada automaticamente e a mídia é redirecionada para a conferência. Sua bot pode iniciar o escalonamento convidando outras pessoas, desde que sua bot tem a permissão de chamada do grupo de iniciar. Se o escalonamento é iniciado por outro participante e o bot não tem permissão de associação de grupo de chamada, sua bot será eliminado da chamada.

> **Importante:** Quando uma chamada será escalonada de ponto a ponto com vários participantes, nem todos os recursos com vários participantes estão disponíveis. Especificamente, o bot não receberão atualizações da lista de participação.

## <a name="signaling"></a>Sinalização

### <a name="incoming-call"></a>Chamada de entrada

Para receber uma chamada de entrada, você precisa registrar o bot de chamada. Quando o bot recebe a notificação de entrada, ela possui as seguintes opções.

| Método                              | Descrição                                  |
|:------------------------------------|:---------------------------------------------|
| [Resposta](../api/call-answer.md)     | Atenda a chamada de entrada.                    |
| [Reject](../api/call-reject.md)     | Rejeitar e desligar a chamada.                  |
| [Redirecionar](../api/call-redirect.md) | Redirecione a chamada.                           |

O bot pode redirecionar a chamada para outro usuário ou um bot. O bot também poderá redirecioná-la para a caixa postal de um usuário.

![Imagem mostrando um bot redirecionar uma chamada para uma caixa postal](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/call-handling.png)

> **Importante:** Redirecionando ou fazer chamadas de saída para PSTN atualmente não é suportado.

### <a name="in-call"></a>Chamada

Operações para o bot estão disponíveis no objeto de chamada. Eles afetam o bot como participante na chamada.

| Método                                                            | Descrição                                  |
|:------------------------------------------------------------------|:---------------------------------------------|
| [Sem áudio](../api/call-mute.md)                                       | Ativar Mudo self na chamada.                       |
| [Desativar Mudo](../api/call-unmute.md)                                   | Desativar o mudo self na chamada.                     |
| [UpdateMetadata](../api/call-updatemetadata.md)                   | Atualize os metadados para self na lista de participação.          |
| [ChangeScreenSharingRole](../api/call-changescreensharingrole.md) | Iniciar e interromper o compartilhamento de tela na chamada.   |

Para interagir com outros participantes na chamada, use o objeto de participantes.

| Método                                                            | Descrição                                  |
|:------------------------------------------------------------------|:---------------------------------------------|
| [Participantes da lista](../api/call-list-participants.md)             | Obtenha uma coleção de objetos dos participantes.         |
| [Convidar participantes](../api/participant-invite.md)               | Convide participantes à chamada ativa.      |
| [Ativar Mudo de todos os participantes](../api/participant-muteall.md)            | Ativar Mudo de todos os participantes na chamada.           |

## <a name="media"></a>Mídia

Processamento de mídia é gerenciado por meio da plataforma de mídia em tempo real da Microsoft. A plataforma de mídia em tempo real ajuda bots participar de reuniões e chamadas de áudio/vídeo Teams da Microsoft. Ele permite bots em tempo real participar de chamadas ponto a ponto e multipontos.

Quando o bot atende uma chamada de entrada ou ingressa em uma chamada de nova ou existente, ele precisa saber a plataforma de mídia em tempo real como mídia será tratada. Se você estiver criando um sistema de resposta de voz interativa (IVR), você pode descarregam o áudio caro componentes de processamento de mídia do serviço hospedado Microsoft. Se seu bot requer acesso direto aos fluxos de mídia, oferecemos uma opção de mídia de aplicativo hospedado por meio do SDK de mídia em tempo real.

### <a name="service-hosted-media"></a>Serviço hospedado de mídia

Bots pode gerenciar o fluxo de trabalho e descarregamento de processamento de áudio para a plataforma de mídia em tempo real Microsoft. Com o serviço hospedado de mídia, você tem enfatizam opções para implementar e hospedar seu bot. Considere o uso de um dos [SDKs](https://developer.microsoft.com/graph/code-samples-and-sdks)disponíveis. Um bot de serviço hospedado mídia pode ser implementado como um serviço sem estado conforme ele não processará a mídia localmente.

| Método                                                        | Descrição                                             |
|:--------------------------------------------------------------|:--------------------------------------------------------|
| [PlayPrompt](../api/call-playprompt.md)                       | Reproduza um clipe de áudio para o usuário.                         |
| [Record](../api/call-record.md)                               | Opcionalmente, reproduzir um prompt e registre um clipe de áudio.      |
| [SubscribeToTone](../api/call-subscribetotone.md)             | Assine os tons DTMF do usuário.                  |
| [CancelMediaProcessing](../api/call-cancelmediaprocessing.md) | Cancele qualquer mídia já processamento na fila.             |

### <a name="application-hosted-media"></a>Aplicativo hospedado de mídia

Para o bot obter acesso direto à mídia, o bot precisa a permissão de acesso de mídia. A biblioteca de mídia em tempo real e o SDK com estado ajuda você a criar a mídia avançada em tempo real, chamar bots. Um bot de aplicativo hospedado deve ser hospedado em um ambiente Windows. [Aplicativo hospedado amostras de mídia](https://github.com/microsoftgraph/microsoft-graph-comms-samples) mostram como criar o bot em diversas plataformas do Windows Azure (incluindo os serviços em nuvem e malha de serviço).

Você pode usar o [SDK do Microsoft Graph chamadas](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/index.html) para simplificar a criação de bots. O SDK fornece funcionalidade para gerenciar os estados dos recursos na memória e coloque na pilha de mídia dos desenvolvedores bot.

O Media SDK permite que o bot enviar e receber o compartilhamento de tela de áudio, vídeo e vídeo com base no conteúdo. Compartilhamento de tela com base em vídeo é modelado como um canal de vídeo. O bot pode assinar o canal de áudio misto e vários canais de vídeos. Para o canal de vídeo, o bot tem uma opção para enviar e receber vídeo como um fluxo de h. 264 codificado ou decodificados quadros brutos.

> **Observação:** Você não pode usar a API de Microsoft.Graph.Calls.Media para registrar ou caso contrário, conteúdo de mídia de chamadas ou reuniões que acessa seu bot de persistência.

## <a name="see-also"></a>Confira também

[Chamadas e reuniões online exemplos de API](https://github.com/microsoftgraph/microsoft-graph-comms-samples/)

[Problemas conhecidos](/graph/known-issues#calls-and-online-meetings)