---
title: Escolha uma opção de hospedagem de mídia usando a API de comunicações na nuvem
description: Use a API de comunicações na nuvem no Microsoft Graph para escolher uma opção de hospedagem de mídia que permite que seus bots enviem e recebam conteúdo relacionado a áudio e vídeo.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
ms.openlocfilehash: d0178fe09668c2199ec2a985ff7df89d36d1d02f
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440996"
---
# <a name="choose-a-media-hosting-option"></a>Escolher uma opção de hospedagem de mídia

Use a API de comunicações na nuvem no Microsoft Graph para permitir que seus bots enviem e recebam conteúdo relacionado a áudio e vídeo. Ao usar a mídia, você pode criar uma experiência mais interativa entre seus bots e usuários.

Este artigo ajuda você a determinar qual opção de hospedagem de mídia é ideal para você com base em suas necessidades: mídia hospedada pelo serviço ou mídia hospedada pelo aplicativo.

## <a name="service-hosted-media-remote-hosting"></a>Mídia hospedada pelo serviço (hospedagem remota)

Se você quiser que o bot reproduza um prompt personalizado quando um cliente disca o número da sua empresa ou para detectar tons de telefone, gravar clipes de voz curtos ou executar qualquer um dos vários cenários de [IVR](/graph/api/resources/calls-api-ivr-overview) (Resposta interativa de voz), considere usar as [APIs](/graph/api/resources/communications-api-overview) de mídia hospedadas pelo serviço.

**Se suas necessidades de mídia forem mais simples, explore essa opção primeiro**. Como o processamento de mídia pesada é descarregado remotamente, essa é uma solução de peso mais leve que permite criar seu bot de uma maneira mais flexível.

Para obter um exemplo que mostra como criar um bot que usa mídia hospedada pelo serviço, consulte os [exemplos de bot](https://github.com/microsoftgraph/microsoft-graph-comms-samples/tree/master/Samples/V1.0Samples/RemoteMediaSamples) de chamada de mídia remota.

![Diagrama de hospedagem remota](images/communications-remote-media.PNG)

## <a name="application-hosted-media-local-hosting"></a>Mídia hospedada pelo aplicativo (hospedagem local)

Se você quiser que o bot acesse uma transmissão ao vivo do áudio e vídeo de seus clientes para usar para gravação, transcrição, tradução ou análise de sentimento por meio de um serviço de processamento de idioma natural, considere hospedar sua mídia localmente.

> [!IMPORTANT]
> Você  não pode usar a API de Acesso à Mídia para gravar ou persistir conteúdo de mídia de chamadas ou reuniões que seu aplicativo acessa ou dados derivados desse conteúdo de mídia ("registro" ou "gravação"), sem primeiro chamar a [API updateRecordingStatus](/graph/api/call-updaterecordingstatus) para indicar que a gravação começou e receber uma resposta bem-sucedida dessa API.
>
> Se o aplicativo começar a gravar qualquer reunião/chamada, ele deverá encerrar a gravação antes de chamar a API updateRecordingStatus para indicar que a gravação foi encerrada. Verifique se você está em conformidade com as leis e regulamentos da sua área em relação à proteção de dados e à confidencialidade das comunicações. Consulte os [Termos de Uso e](/legal/microsoft-apis/terms-of-use) consulte seu advogado jurídico para obter mais informações.

**Se você quiser ter mais controle sobre a mídia, escolha esta opção**. Você terá acesso direto a fluxos de mídia e poderá usar o compartilhamento de tela baseado em vídeo. Você poderá criar cenários de IVR mais sofisticados habilitados para fala. Essa é uma solução de peso mais pesada que oferece mais flexibilidade em como você deseja programar sua mídia.

Confira também os [requisitos e considerações para bots](/microsoftteams/platform/concepts/calls-and-meetings/requirements-considerations-application-hosted-media-bots) de mídia hospedados pelo aplicativo.

Para obter um exemplo que mostra como criar um bot que usa mídia hospedada pelo aplicativo, consulte os [exemplos de mídia local](https://github.com/microsoftgraph/microsoft-graph-comms-samples/tree/master/Samples/V1.0Samples/LocalMediaSamples).

![Diagrama de hospedagem local](images/communications-local-media.PNG)

## <a name="see-also"></a>Confira também

- [Permissões de chamadas](./permissions-reference.md#calls-permissions)
- [Visão geral da API de comunicações na nuvem](cloud-communications-concept-overview.md)