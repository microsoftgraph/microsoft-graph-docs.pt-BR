---
title: Tipos de chamada com suporte na API de comunicações na nuvem
description: Saiba mais sobre os tipos de chamada com suporte na API de comunicações na nuvem no Microsoft Graph e como eles são usados para o processo de sinalização.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
ms.openlocfilehash: 21b220b75e4d78286a7455fc042066ca50b67c45
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66441017"
---
# <a name="supported-call-types"></a>Tipos de chamada com suporte

Este artigo descreve os tipos de chamada com suporte na API de comunicações na nuvem no Microsoft Graph e como eles são usados para o processo de sinalização.

## <a name="peer-to-peer-calls"></a>Chamadas ponto a ponto

Uma chamada é P2P (ponto a ponto) quando um participante está chamando diretamente outro participante. Se um bot chamar um usuário e o usuário for o único destino de chamada especificado, este será um exemplo de uma chamada P2P.

![Diagrama de chamada P2P](images/communications-p2p-call.PNG)

Se um usuário quiser chamar um bot, o bot não precisará de permissões adicionais para responder à chamada P2P. Para que um bot chame um usuário, ele deve ter a permissão Calls.Initiate.All para uma chamada P2P.

## <a name="group-calls"></a>Chamadas de grupo

Uma chamada de grupo ocorrerá se houver três ou mais participantes na chamada ou se as coordenadas da reunião foram [especificadas](/graph/api/resources/onlinemeeting) quando a chamada foi criada inicialmente. 

Você pode criar uma chamada em grupo por meio do Microsoft Teams, por exemplo.

![Diagrama de chamada de grupo](images/communications-group-call.PNG)

Atualmente, os bots são capazes de:
- Criar chamadas de grupo
- Ingressar em chamadas de grupo de saída
- Convidar outros participantes para uma chamada de grupo existente
- Ser convidado para chamadas de grupo existentes

## <a name="see-also"></a>Confira também

- [Visão geral da API de comunicações na nuvem](cloud-communications-concept-overview.md)
- [Permissões para chamadas](./permissions-reference.md#calls-permissions)
