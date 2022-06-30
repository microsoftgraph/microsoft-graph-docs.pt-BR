---
title: Criar ou ingressar em reuniões online usando a API de comunicações na nuvem
description: Use a API de comunicações na nuvem no Microsoft Graph para criar ou ingressar em reuniões online. Crie uma reunião que ocorra no futuro ou instantaneamente.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
ms.openlocfilehash: 41d823f384cb9682c90be22982b3d676e5652912
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440968"
---
# <a name="create-or-join-online-meetings"></a>Criar ou ingressar em reuniões online

Use a API de comunicações na nuvem no Microsoft Graph para criar ou ingressar em reuniões online. As reuniões online fornecem a capacidade de especificar determinados detalhes, como o assunto da reunião e quem são todos os participantes. Você também pode definir a data e a hora de quando a reunião começa e termina.

As reuniões online fornecem a flexibilidade para criar uma reunião que ocorre no futuro ou instantaneamente. A capacidade de configurar uma reunião que começa imediatamente após sua criação é ideal para problemas inesperados e outros incidentes que exigem a atenção imediata dos participantes.

> [!NOTE]
> Esse conjunto de APIs permite a flexibilidade e a integração mais avançada com os recursos do Microsoft Teams ou do Skype; ele não atualiza nem cria nenhum evento em um calendário. Para obter uma abordagem conveniente para adicionar uma reunião online a um calendário do Outlook, use a API de calendário. Consulte [Escolha uma API no Microsoft Graph para criar e participar de reuniões online](choose-online-meeting-api.md) para obter mais informações.

## <a name="create-an-online-meeting"></a>Criar uma reunião online

Ao criar uma reunião online, você receberá [coordenadas](/graph/api/resources/onlinemeeting) para a reunião. Quando os participantes ingressam na reunião usando essas coordenadas de reunião, uma chamada de grupo é criada.

Quando todos os participantes saírem da chamada de grupo, a chamada de grupo terminará. Os participantes ainda podem reingressar na reunião posteriormente usando as mesmas coordenadas de reunião, mas isso criará outra chamada de grupo.

> [!NOTE]
> As reuniões criadas não aparecem em calendários.

## <a name="join-an-online-meeting"></a>Ingressar em uma reunião online

Depois que uma reunião online é criada, os usuários podem ingressar de duas maneiras:

1. Por meio do navegador, usando **o joinWebURL** que foi retornado como parte das [coordenadas da reunião](/graph/api/resources/onlinemeeting).

2. Por meio [da API de criação](/graph/api/application-post-calls#example-5-join-scheduled-meeting-with-service-hosted-media) de chamada, que exige que você forneça as [coordenadas](/graph/api/resources/onlinemeeting) da reunião ([organizermeetinginfo](/graph/api/resources/organizermeetinginfo) e [chatInfo](/graph/api/resources/chatinfo)).

## <a name="see-also"></a>Confira também

- [Permissões de reunião online](./permissions-reference.md#online-meetings-permissions)
- [Escolha uma API do Microsoft Graph para criar e participar de reuniões online](choose-online-meeting-api.md)
- [Visão geral da API de comunicações na nuvem](cloud-communications-concept-overview.md)
