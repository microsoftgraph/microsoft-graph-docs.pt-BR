---
title: Visão geral de mídia
description: Habilite seus bots para enviar e receber conteúdo relacionado a áudio e vídeo.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 74738233915f0a0731790ee8b0646f437585cb67
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522423"
---
# <a name="media-overview"></a>Visão geral de mídia

As APIs de comunicação em nuvem no Microsoft Graph adicionam uma nova dimensão a como seus aplicativos e serviços interagem com os usuários por meio de vários recursos relacionados a comunicações, como chamadas e reuniões online. Você pode habilitar seus bots para enviar e receber conteúdo relacionado a áudio e vídeo. Ao fazer uso da mídia, você pode criar uma experiência mais interativa entre seus bots e usuários.

Este artigo irá ajudá-lo a descobrir qual opção de Hospedagem de mídia é adequada para você com base em suas necessidades.

## <a name="service-hosted-media-remote-hosting"></a>Mídia hospedado pelo serviço (hospedagem remota)
Se você quiser que o bot execute um aviso personalizado quando um cliente discar o número de sua empresa ou para detectar toques de telefone, gravar pequenos clipes de voz ou executar qualquer um dos vários cenários de[IVR](/graph/api/resources/calls-api-ivr-overview)(resposta interativa de voz), considere usar as [APIs de mídia hospedadas pelo serviço](/graph/api/resources/communications-api-overview).

**Se suas necessidades de mídia forem mais simples, explore esta opção primeiro**. Como o processamento de mídia intensa é descarregado remotamente, esta é uma solução de peso mais leve que permite que você crie seu bot de maneira mais flexível.

Para obter um exemplo que mostra como criar um bot que usa mídia de host de serviço, consulte os [exemplos de bot de chamada de mídia remota](https://github.com/microsoftgraph/microsoft-graph-comms-samples/tree/master/Samples/BetaSamples/RemoteMediaSamples).

![Diagrama de hospedagem remota](images/communications-remote-media.PNG)

## <a name="application-hosted-media-local-hosting"></a>Mídia hospedada por aplicativo (hospedagem local)
Se você quiser que o bot acesse um fluxo ativo de áudio e vídeo de seus clientes para usar para gravação, transcrever, traduzir ou remediar a análise por meio de um serviço de processamento de idioma natural, considere hospedar sua mídia localmente.

>**Observação:** Você **não pode** usar a API de acesso à mídia para registrar ou manter o conteúdo de mídia de chamadas ou reuniões que seu aplicativo acessa, ou dados derivados desse conteúdo de mídia ("Record" ou "Recording"), sem primeiro chamar a [API updateRecordingStatus](/graph/api/call-updaterecordingstatus) para indicar que a gravação foi iniciada e receber uma resposta de êxito dessa API. Se o aplicativo começar a gravar qualquer reunião/chamada, ele deverá finalizar a gravação antes de chamar a API updateRecordingStatus para indicar que a gravação foi concluída. Certifique-se de que você está em conformidade com as leis e regulamentos de sua área em relação à proteção de dados e à confidencialidade das comunicações. Confira os [Termos de Uso](/legal/microsoft-apis/terms-of-use) e converse com sua assessoria jurídica para saber mais.

**Se você quiser mais controle sobre sua mídia, escolha essa opção**. Você terá acesso direto aos fluxos de mídia e poderá usar o compartilhamento de tela baseado em vídeo. Você poderá criar cenários IVR mais sofisticados que estão habilitados para fala. Esta é uma solução ponderada mais complicada que oferece maior flexibilidade na forma como você deseja programar a mídia.

Confira também os [requisitos e considerações](/microsoftteams/platform/concepts/calls-and-meetings/requirements-considerations-application-hosted-media-bots) para bots de mídia hospedados por aplicativos.

Para obter um exemplo que mostra como criar um bot que usa mídia hospedada no aplicativo, consulte os [exemplos de mídia local](https://github.com/microsoftgraph/microsoft-graph-comms-samples/tree/master/Samples/V1.0Samples/LocalMediaSamples).

![Diagrama de hospedagem local](images/communications-local-media.PNG)

## <a name="see-also"></a>Confira também

- [Permissões de chamadas](./permissions-reference.md#calls-permissions)
