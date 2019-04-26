---
title: Como trabalhar com a API de chamadas e reuniões online no Microsoft Graph
description: A API de reuniões online e chamadas do Microsoft Graph adiciona uma nova dimensão à forma como seus aplicativos e serviços podem interagir com usuários e permitir recursos de voz e vídeo. A API permite que você crie chamadas e receba chamadas de usuários e aplicativos no Microsoft Teams. Você pode usar essas APIs para criar um aplicativo de serviço (bot) que possa atuar como participante de uma chamada ou reunião.
author: VinodRavichandran
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: ab01bc71ccb4f7490a60c47712198f72032fc157
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543834"
---
# <a name="working-with-the-calls-and-online-meetings-api-in-microsoft-graph"></a>Como trabalhar com a API de chamadas e reuniões online no Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A API de reuniões online e chamadas do Microsoft Graph adiciona uma nova dimensão à forma como seus aplicativos e serviços podem interagir com usuários e permitir recursos de voz e vídeo. A API permite que você crie chamadas e receba chamadas de usuários e aplicativos no Microsoft Teams. Você pode usar essas APIs para criar um aplicativo de serviço (bot) que possa atuar como participante de uma chamada ou reunião.

## <a name="call-types"></a>Tipos de chamadas

As chamadas são categorizadas como chamadas de ponto a ponto ou com vários participantes. Um usuário pode iniciar uma chamada de ponto a ponto com seu bot ou convidar seu bot para uma conferência existente com vários participantes. Não são necessárias permissões quando o usuário convida o bot para uma chamada de ponto a ponto. Para seu bot participar de uma chamada com vários participantes, o bot precisa ter permissão do administrador do locatário para participar de uma chamada em grupo.

![Uma imagem mostrando chamadas de ponto a ponto ou com vários participantes](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/call-types.png)

Se seu bot estiver criando a chamada, ele precisará ter a permissão de iniciar ou iniciar chamada em grupo. O bot tem a opção para criar uma chamada de ponto a ponto ou uma chamada com vários participantes.

- No caso de uma chamada de ponto a ponto, o bot só precisa especificar um destino e nenhuma coordenada para a reunião. 
- Se o bot iniciar uma chamada com vários participantes, uma reunião ad hoc será configurada nos bastidores e todos ingressarão na conferência. Se as coordenadas para a reunião forem especificadas, uma chamada com vários participantes será configurada mesmo se houver apenas um destino.

Uma chamada ser iniciada como uma chamada de a ponto a ponto e ser escalonada para uma chamada com vários participantes. Uma conferência será automaticamente provisionada e a mídia redirecionada para a conferência. Seu bot pode iniciar o escalonamento convidando outras pessoas, desde que seu bot tenha a permissão de iniciar chamada em grupo. Se escalonamento for iniciado por outro participante e o bot não tiver permissão de ingressar na chamada em grupo, o bot será retirado da chamada.

> **Importante:** quando uma chamada é passada de ponto a ponto para com vários participantes, nem todos os recursos com vários participantes estão disponíveis. Especificamente, o bot não receberá atualizações da lista de participantes.

## <a name="signaling"></a>Sinalização

### <a name="incoming-call"></a>Chamada de entrada

Para receber uma chamada de entrada, registre o bot de chamada. Quando o bot receber a notificação de entrada, terá as seguintes opções.

| Método                              | Descrição                                  |
|:------------------------------------|:---------------------------------------------|
| [Resposta](../api/call-answer.md)     | Responda a chamada de entrada.                    |
| [Reject](../api/call-reject.md)     | Rejeite e desligue a chamada.                  |
| [Redirecionar](../api/call-redirect.md) | Redirecione a chamada.                           |

O bot pode redirecionar a chamada para outro usuário ou um bot. O bot também pode redirecioná-la para a caixa postal do usuário.

![Imagem mostrando um bot redirecionando uma chamada para uma caixa postal](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/call-handling.png)

> **Importante:** o redirecionamento ou a realização de chamadas de saída para o PSTN não tem suporte atualmente.

### <a name="in-call"></a>Na chamada

As operações para o bot estão disponíveis no objeto call. Elas afetam o bot como participante na chamada.

| Método                                                            | Descrição                                  |
|:------------------------------------------------------------------|:---------------------------------------------|
| [Mute](../api/call-mute.md)                                       | Ative o mudo automaticamente na chamada.                       |
| [Unmute](../api/call-unmute.md)                                   | Desative o mudo automaticamente na chamada.                     |
| [UpdateMetadata](../api/call-updatemetadata.md)                   | Atualize metadados automaticamente na lista de participantes.          |
| [ChangeScreenSharingRole](../api/call-changescreensharingrole.md) | Inicie e interrompa a tela de compartilhamento na chamada.   |

Para interagir com outros participantes na chamada, use o objeto participants.

| Método                                                            | Descrição                                  |
|:------------------------------------------------------------------|:---------------------------------------------|
| [List participants](../api/call-list-participants.md)             | Obtenha uma coleção de objetos participant.         |
| [Invite Participants](../api/participant-invite.md)               | Convide participantes para a chamada ativa.      |
| [Mute All Participants](../api/participant-muteall.md)            | Ative o mudo para todos os participantes em uma chamada.           |

## <a name="media"></a>Mídia

O processamento de mídia é gerenciado pelo Microsoft RealTime Media Platform. O RealTime Media Platform ajuda no envolvimento dos bots em reuniões e chamadas de áudio/vídeo do Microsoft Teams. Permite que bots em tempo real participem em chamadas de ponto a ponto e com vários participantes.

Quando o bot responde a uma chamada recebida, ou se junta a uma chamada nova ou existente, ele precisa informar o RealTime Media Platform como a mídia será tratada. Se você estiver criando um sistema IVR (Resposta de voz interativa), poderá descarregar o caro processamento de áudio para os componentes de mídia hospedados pelo serviço da Microsoft. Se seu bot exigir acesso direto aos fluxos de mídia, oferecemos uma opção de mídia hospedada pelo aplicativo usando o SDK do RealTime Media.

### <a name="service-hosted-media"></a>Mídia hospedada pelo serviço

Os bots podem gerenciar o fluxo de trabalho e descarregar o processamento de áudio para o Microsoft RealTime Media Platform. Com mídia hospedada pelo serviço, você tem várias opções para implementar e hospedar seu bot. Considere usar um dos [SDKs](https://developer.microsoft.com/graph/code-samples-and-sdks) disponíveis. Um bot mídia hospedada pelo serviço pode ser implementado como um serviço sem estado já que não processa mídia localmente.

| Método                                                        | Descrição                                             |
|:--------------------------------------------------------------|:--------------------------------------------------------|
| [PlayPrompt](../api/call-playprompt.md)                       | Reproduza um clipe de áudio para o usuário.                         |
| [Record](../api/call-record.md)                               | Opcionalmente, reproduza um prompt e grave um clipe de áudio.      |
| [SubscribeToTone](../api/call-subscribetotone.md)             | Inscreva-se nos Tons DTMF a partir do usuário.                  |
| [CancelMediaProcessing](../api/call-cancelmediaprocessing.md) | Cancele qualquer processamento de mídia que já estiver na fila.             |

### <a name="application-hosted-media"></a>Mídia hospedada pelo aplicativo

Para que o bot tenha acesso direto à mídia, o bot precisa da permissão do Access-Media. A biblioteca do RealTime Media e o SDK com estado ajudam na compilação de bots de chamadas do RealTime Media. Um bot hospedado pelo aplicativo deve estar hospedado em um ambiente Windows. Os [exemplos de mídias hospedadas pelo aplicativo](https://github.com/microsoftgraph/microsoft-graph-comms-samples) mostram como criar um bot em várias Plataformas Azure (incluindo o Cloud Services e o Service Fabric).

Você pode usar o [SDK de Chamadas do Microsoft Graph](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/index.html) para simplificar a criação de bots. O SDK fornece a funcionalidade para gerenciar os estados dos recursos na memória e fazer pull na pilha de mídia dos desenvolvedores de bots.

O SDK do Media permite que o bot envie e receba conteúdo de compartilhamento de tela de áudio, vídeo e baseado em vídeo. O compartilhamento de tela baseado em vídeo é modelado como um canal de vídeo. O bot pode se inscrever no canal de áudio misto e em vários canais de vídeo. Para o canal de vídeo, o bot tem a opção de enviar e receber vídeo como um fluxo H.264 codificado ou como quadros brutos decodificados.

> **Observação:** você não pode usar a API Microsoft.Graph.Calls.Media para gravar ou persistir conteúdo de mídia de chamadas ou reuniões que seu bot acessar.

## <a name="see-also"></a>Confira também

[Exemplos de chamadas e reuniões online API](https://github.com/microsoftgraph/microsoft-graph-comms-samples/)

[Problemas conhecidos](/graph/known-issues#calls-and-online-meetings)
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/calls-api-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
