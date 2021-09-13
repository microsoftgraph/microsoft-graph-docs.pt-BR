---
title: Visão geral de chamadas
description: Saiba mais sobre os tipos de chamada com suporte e como eles são usados para o processo de sinalização.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
ms.openlocfilehash: 34b7e2e507576333df36f7eae9185785872d24ec
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59137487"
---
# <a name="calls-overview"></a>Visão geral de chamadas

As APIs de comunicações na nuvem na Microsoft Graph adicionar uma nova dimensão à forma como seus aplicativos e serviços interagem com os usuários por meio de vários recursos relacionados à comunicação, como chamadas e reuniões online. Este artigo descreve os tipos de chamada com suporte e como eles são usados para o processo de sinalização.

## <a name="peer-to-peer-calls"></a>Chamadas ponto a ponto
Uma chamada é ponto a ponto (P2P) quando um participante está chamando diretamente outro participante. Se um bot chamar um usuário e o usuário for o único destino de chamada especificado, este será um exemplo de uma chamada P2P.

![Diagrama de chamada P2P](images/communications-p2p-call.PNG)

Se um usuário quiser chamar um bot, o bot não precisará de permissões adicionais para responder à chamada P2P. Para que um bot chame um usuário, ele deve ter a Calls.Initiate. Todas as permissões para uma chamada P2P.

## <a name="group-calls"></a>Chamadas de grupo

Uma chamada de grupo ocorrerá se houver três ou mais participantes na chamada ou se as coordenadas de reunião foram [especificadas](/graph/api/resources/onlinemeeting) quando a chamada foi criada inicialmente. 

Você pode criar uma chamada de grupo Microsoft Teams, por exemplo.

![Diagrama de chamada de grupo](images/communications-group-call.PNG)

Atualmente, os bots são capazes de:
- Criar chamadas de grupo
- Participar de chamadas de grupo de exisiting
- Convidar outros participantes para uma chamada de grupo existente
- Ser convidado para chamadas de grupo existentes

## <a name="see-also"></a>Confira também

- [Visão geral da API de comunicações na nuvem](cloud-communications-concept-overview.md)
- [Permissões para chamadas](./permissions-reference.md#calls-permissions)
