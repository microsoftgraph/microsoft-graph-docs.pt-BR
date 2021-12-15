---
title: API de retransmissão de dispositivos no Microsoft Graph (prévia)
description: 'Hoje, as pessoas interagem com vários dispositivos diariamente. Os usuários geralmente iniciam tarefas de produtividade e atividades de entretenimento em um dispositivo e continuam em outro. Para atender às necessidades de seus clientes, seus aplicativos precisam abranger dispositivos e plataformas. '
ms.localizationpriority: medium
author: FaithOmbongi
ms.prod: cross-device-experiences
ms.openlocfilehash: 38a90e2cbdb5357190edbf3f8d3ea6f234414902
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61524571"
---
# <a name="device-relay-api-in-microsoft-graph-preview"></a>API de retransmissão de dispositivos no Microsoft Graph (prévia)

Hoje, as pessoas interagem com vários dispositivos diariamente. Os usuários geralmente iniciam tarefas de produtividade e atividades de entretenimento em um dispositivo e continuam em outro. Para atender às necessidades de seus clientes, seus aplicativos precisam abranger dispositivos e plataformas. 

Você pode usar as APIs de retransmissão de dispositivos para fornecer experiências perfeitas para seus usuários. Você pode permitir que eles transfiram ativamente uma experiência de um dispositivo para outro ou a aprimorem usando vários dispositivos ao mesmo tempo. Isso é feito por meio de ações no aplicativo (um botão ou seleção no aplicativo) que chama a API de retransmissão de dispositivos para descobrir os dispositivos dos usuários e permitir que eles iniciem e enviem mensagens ao seu aplicativo nesses outros dispositivos.

## <a name="why-integrate-with-device-relay"></a>Por que integrar-se com a retransmissão de dispositivos?

A API de retransmissão de dispositivos permite que seu aplicativo se registre e descubra, comande e envie mensagens para seu aplicativo nos dispositivos do usuário. Ao fazer isso, você pode tornar as tarefas nas quais seus clientes trabalham no tema central. Eles podem trabalhar no dispositivo que for mais conveniente para eles, descobrindo-o e transferindo tarefas para ele. Eles também podem aprimorar uma experiência em andamento com o aplicativo usando outros dispositivos disponíveis.

Você pode usar a API de retransmissão de dispositivos para dispositivos complementares ou cenários de controle remoto. Use os recursos de mensagens para criar um canal de aplicativos entre dois dispositivos para enviar e receber mensagens personalizadas. Por exemplo, você pode permitir que seus clientes usem o telefone para controlar a reprodução em uma TV. Em um cenário de produtividade, você também pode oferecer um aplicativo complementar exibindo ações comumente usadas baseadas em contexto em um telefone enquanto os usuários trabalham na visualização principal do aplicativo no PC.

Seus clientes também podem transferir ativamente uma experiência de um dispositivo para outro executando uma ação no seu aplicativo. Por exemplo, uma usuária pode estar assistindo a uma transmissão ao vivo no telefone enquanto está no ônibus, mas, ao chegar em casa, poderá transferir a reprodução para o PC em sua sala de estar. Os cenários de produtividade também são compatíveis com a retransmissão de dispositivos. 

### <a name="extend-the-experience"></a>Estender a experiência

Estenda seu aplicativo oferecendo uma experiência do usuário para descobrir dispositivos e iniciar seu aplicativo nesses dispositivos. Por exemplo, o usuário poderia estar trabalhando em um pedido de compra no telefone, descobrir o PC no escritório e iniciar o aplicativo para terminar de inserir o pedido de compra.  

### <a name="augment-the-experience"></a>Aumente a experiência

Crie uma experiência complementar para seu aplicativo em outro dispositivos do usuário. Por exemplo, o aplicativo pode incluir uma experiência do usuário para iniciar em outros dispositivos. Em um jogo, o usuário poderia iniciar o aplicativo em um dispositivo com uma tela maior (por exemplo, de um computador para um Xbox). O Xbox poderia apresentar uma visão completa do jogo (uma visão em primeira pessoa), enquanto o dispositivo com a tela menor poderia apresentar uma visão diferente com contexto adicional (uma visão de nível superior do nível do jogo mostrando o jogador e as localizações dos adversários).  

### <a name="enrich-the-experience"></a>Aprimorar a experiência

Adicione mais habilidades de controle ao seu aplicativo. Por exemplo, forneça habilidades de controle remoto para o aplicativo principal de um dispositivo complementar. Quando o usuário iniciasse um aplicativo de um dispositivo para outro, o dispositivo de destino poderia mostrar a experiência completa (por exemplo, um modelo 3D em um aplicativo de design), enquanto o dispositivo de origem poderia mostrar uma lista das ações mais comuns dependendo do estado do aplicativo no dispositivo de destino (por exemplo, girar, redimensionar, paleta de cores).

## <a name="see-also"></a>Confira também

- [Experiências entre dispositivos no Microsoft Graph](cross-device-concept-overview.md)
- [Saiba mais sobre a API de retransmissão de dispositivos](/graph/api/resources/project-rome-overview?view=graph-rest-beta)
- [Saiba mais sobre o Project Rome](/windows/project-rome/)
