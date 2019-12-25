---
title: Visão geral de reuniões online
description: Você terá a flexibilidade de criar uma reunião que ocorra no futuro ou instantaneamente
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: bd85c3be66890d4763e2c2b1910ee7049573d446
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871546"
---
# <a name="online-meetings-overview"></a>Visão geral de reuniões online

As reuniões online oferecem a capacidade de especificar determinados detalhes, como o assunto da reunião e todos os participantes. Você também pode definir a data e a hora de início e término da reunião.

As reuniões online oferecem a flexibilidade para criar uma reunião que ocorra no futuro ou instantaneamente. A capacidade de configurar uma reunião que inicia imediatamente após sua criação é ideal para problemas inesperados e outros incidentes que exigem a atenção imediata dos participantes.

## <a name="create-an-online-meeting"></a>Criar uma reunião online

Ao criar uma reunião online, você receberá as [coordenadas](/graph/api/resources/onlinemeeting) da reunião. Quando os participantes ingressam na reunião usando essas coordenadas de reunião, uma chamada de grupo é criada.

Quando todos os participantes saírem da chamada de grupo, a chamada do grupo será finalizada. Os participantes ainda podem reingressar na reunião posteriormente usando as mesmas coordenadas de reunião, mas isso criará outra chamada de grupo.

>**Observação:** As reuniões criadas não aparecem em calendários.

## <a name="join-an-online-meeting"></a>Ingressar em uma reunião online
Após a criação de uma reunião online, os usuários podem participar de duas maneiras:

1. Por meio do navegador, usando o **joinURL** que foi retornado como parte das [coordenadas da reunião](/graph/api/resources/onlinemeeting).

2. Por meio da [API Create Call](/graph/api/application-post-calls#example-5-join-scheduled-meeting-with-service-hosted-media), que requer que você forneça as [coordenadas da reunião](/graph/api/resources/onlinemeeting), ([organizermeetinginfo](/graph/api/resources/organizermeetinginfo)e [chatInfo](/graph/api/resources/chatinfo)).

## <a name="see-also"></a>Confira também

- [Permissões de reunião online](/graph/permissions-reference#online-meetings-permissions)
