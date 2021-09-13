---
title: Utilize a API de comunicações em nuvem para criar ou participar de reuniões online
description: Você terá a flexibilidade de criar uma reunião que acontecerá no futuro ou instantaneamente
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
ms.openlocfilehash: d8e084b148e91a4400a8367d47caa7b57b7fe890
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59136156"
---
# <a name="use-the-cloud-communications-api-to-create-or-join-online-meetings"></a>Utilize a API de comunicações em nuvem para criar ou participar de reuniões online

As reuniões online fornecem a capacidade de especificar determinados detalhes, como o assunto da reunião e quem são todos os participantes. Você também pode definir a data e a hora para quando a reunião é iniciada e terminada.

As reuniões online oferecem flexibilidade para criar uma reunião que ocorre no futuro ou instantaneamente. A capacidade de configurar uma reunião que começa imediatamente após sua criação é ideal para problemas inesperados e outros incidentes que exigem a atenção imediata dos participantes.

> **Observação** Esse conjunto de APIs permite a flexibilidade e a integração mais rica com Microsoft Teams ou Skype recursos; ele não atualiza ou cria qualquer evento em um calendário. Para uma abordagem conveniente para adicionar uma reunião online a um calendário Outlook, use a API de calendário. Consulte [Escolha uma API no Microsoft Graph para criar e participar de reuniões online](choose-online-meeting-api.md) para obter mais informações.

## <a name="create-an-online-meeting"></a>Criar uma reunião online

Ao criar uma reunião online, você receberá [coordenadas](/graph/api/resources/onlinemeeting) para a reunião. Quando os participantes ins juntam-se à reunião usando essas coordenadas de reunião, uma chamada de grupo é criada.

Quando todos os participantes sairem da chamada de grupo, a chamada de grupo terminará. Os participantes ainda podem voltar à reunião depois usando as mesmas coordenadas de reunião, mas isso criará outra chamada de grupo.

>**Observação:** As reuniões criadas não aparecem em calendários.

## <a name="join-an-online-meeting"></a>Participar de uma reunião online
Depois que uma reunião online é criada, os usuários podem participar de duas maneiras:

1. Por meio do navegador, usando **o joinWebURL** retornado como parte das [coordenadas de reunião](/graph/api/resources/onlinemeeting).

2. Por meio [da API de](/graph/api/application-post-calls#example-5-join-scheduled-meeting-with-service-hosted-media)chamada de criação , que exige que você forneça as [coordenadas](/graph/api/resources/onlinemeeting)da reunião , ([organizermeetinginfo](/graph/api/resources/organizermeetinginfo)e [chatInfo](/graph/api/resources/chatinfo)).

## <a name="see-also"></a>Confira também

- [Permissões de reunião online](./permissions-reference.md#online-meetings-permissions)
- [Escolha uma API do Microsoft Graph para criar e participar de reuniões online](choose-online-meeting-api.md)
