---
title: Visão geral das chamadas
description: Saiba mais sobre os tipos de chamadas compatíveis e como eles são usados para o processo de sinalização.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 2a91e37dd04cf6067cae253eb19b6afee7c799b9
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2020
ms.locfileid: "48289453"
---
# <a name="calls-overview"></a>Visão geral das chamadas

As APIs de comunicação em nuvem no Microsoft Graph adicionam uma nova dimensão a como seus aplicativos e serviços interagem com os usuários por meio de vários recursos relacionados a comunicações, como chamadas e reuniões online. Este artigo descreve os tipos de chamadas compatíveis e como eles são usados para o processo de sinalização.

## <a name="peer-to-peer-calls"></a>Chamadas ponto a ponto
Uma chamada é ponto a ponto (P2P) quando um participante está ligando diretamente para outro participante. Se um bot chamar um usuário e o usuário for o único destino de chamada especificado, este é um exemplo de uma chamada P2P.

![Diagrama de chamada P2P](images/communications-p2p-call.PNG)

Se um usuário quiser chamar um bot, o bot não precisará de nenhuma permissão adicional para responder à chamada P2P. Para que um bot chame um usuário, ele deve ter o Calls.Initiate. Todas as permissões para uma chamada P2P.

## <a name="group-calls"></a>Chamadas de grupo

Uma chamada de grupo ocorrerá se houver três ou mais participantes na chamada ou se as [coordenadas da reunião](/graph/api/resources/onlinemeeting) foram especificadas quando a chamada foi criada inicialmente. 

Você pode criar uma chamada de grupo pelo Microsoft Teams, por exemplo.

![Diagrama de chamada de grupo](images/communications-group-call.PNG)

No momento, os bots podem:
- Criar chamadas em grupo
- Ingressar em chamadas de grupo existentes
- Convidar outros participantes para uma chamada de grupo existente
- Ser convidado para chamadas de grupo existentes

## <a name="see-also"></a>Confira também

- [Visão geral da API de comunicações em nuvem](cloud-communications-concept-overview.md)
- [Permissões para chamadas](./permissions-reference.md#calls-permissions)