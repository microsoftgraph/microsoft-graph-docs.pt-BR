---
title: Utilize a API de comunicações em nuvem para criar ou participar de reuniões online
description: Você terá a flexibilidade de criar uma reunião que acontecerá no futuro ou instantaneamente
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 08d7195f3eb91ba896e8045b4576e46f12aaf795
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2020
ms.locfileid: "48289348"
---
# <a name="use-the-cloud-communications-api-to-create-or-join-online-meetings"></a>Utilize a API de comunicações em nuvem para criar ou participar de reuniões online

As reuniões online oferecem a capacidade de especificar determinados detalhes, como o assunto da reunião e todos os participantes. Você também pode definir a data e a hora de início e término da reunião.

As reuniões online oferecem a flexibilidade para criar uma reunião que ocorra no futuro ou instantaneamente. A capacidade de configurar uma reunião que inicia imediatamente após sua criação é ideal para problemas inesperados e outros incidentes que exigem a atenção imediata dos participantes.

> **Observação** Esse conjunto de APIs permite a flexibilidade e a integração mais rica com o Microsoft Teams ou recursos do Skype; Ele não atualiza ou cria nenhum evento em um calendário. Para obter uma abordagem conveniente para adicionar uma reunião online a um calendário do Outlook, use a API de calendário. Consulte [Escolha uma API no Microsoft Graph para criar e participar de reuniões online](choose-online-meeting-api.md) para obter mais informações.

## <a name="create-an-online-meeting"></a>Criar uma reunião online

Ao criar uma reunião online, você receberá as [coordenadas](/graph/api/resources/onlinemeeting) da reunião. Quando os participantes ingressam na reunião usando essas coordenadas de reunião, uma chamada de grupo é criada.

Quando todos os participantes saírem da chamada de grupo, a chamada do grupo será finalizada. Os participantes ainda podem reingressar na reunião posteriormente usando as mesmas coordenadas de reunião, mas isso criará outra chamada de grupo.

>**Observação:** As reuniões criadas não aparecem em calendários.

## <a name="join-an-online-meeting"></a>Ingressar em uma reunião online
Após a criação de uma reunião online, os usuários podem participar de duas maneiras:

1. Por meio do navegador, usando o **joinWebURL** que foi retornado como parte das [coordenadas da reunião](/graph/api/resources/onlinemeeting).

2. Por meio da [API Create Call](/graph/api/application-post-calls#example-5-join-scheduled-meeting-with-service-hosted-media), que requer que você forneça as [coordenadas da reunião](/graph/api/resources/onlinemeeting), ([organizermeetinginfo](/graph/api/resources/organizermeetinginfo)e [chatInfo](/graph/api/resources/chatinfo)).

## <a name="see-also"></a>Confira também

- [Permissões de reunião online](./permissions-reference.md#online-meetings-permissions)
- [Escolha uma API do Microsoft Graph para criar e participar de reuniões online](choose-online-meeting-api.md)