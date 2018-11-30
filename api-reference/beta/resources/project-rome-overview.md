---
title: 'Usar a API do Microsoft Graph para trabalhar com o Project Roma '
description: 'Project Roma é uma iniciativa da Microsoft para criar uma plataforma que permite que os desenvolvedores de aplicativos criar ótimas experiências de referência cruzada de dispositivo. Project Roma habilita recursos diferentes que se conectam a diferentes serviços e pontos de extremidade do cliente quando a usuário se conecta com a Microsoft a mesma conta ou trabalha ou escola conta. Isso permite que você implemente experiências entre dispositivos e plataforma cruzada que são centralizadas em torno de tarefas do usuário, em vez dos dispositivos. '
ms.openlocfilehash: f779c04a76331d27fdcae6436e758bacfc052f8e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035444"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a>Usar a API do Microsoft Graph para trabalhar com o Project Roma 

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

[Project Roma](https://developer.microsoft.com/en-us/windows/project-rome) é uma iniciativa da Microsoft para criar uma plataforma que permite que os desenvolvedores de aplicativos criar ótimas experiências de referência cruzada de dispositivo. Project Roma habilita recursos diferentes que se conectam a diferentes serviços e pontos de extremidade do cliente quando a usuário se conecta com a Microsoft a mesma conta ou trabalha ou escola conta. Isso permite que você implemente experiências entre dispositivos e plataforma cruzada que são centralizadas em torno de tarefas do usuário, em vez dos dispositivos. 

Três principais recursos de projeto Roma são expostos por meio do Microsoft Graph para ajudá-lo a habilitar ótimas experiências de referência cruzada de dispositivo: atividades, dispositivos e notificações. 

## <a name="activities"></a>Atividades

Atividades no Microsoft Graph habilitar compromisso do usuário de unidade com seus aplicativos em plataformas e dispositivos. Uma atividade é a unidade de compromisso do usuário e consiste em três componentes:

- Um link profundo
- Uma representação visual
- Metadados do conteúdo que descreve a atividade, usando o [https://schema.org/](https://schema.org/) shared vocabulário

Quando uma sessão é criada por um aplicativo, um item de histórico é adicionado à atividade para refletir o período de participação do usuário. Cada vez que um usuário reengages com uma atividade, um novo item de histórico é adicionado à atividade acumular compromisso do usuário.

Quando um aplicativo publica objetos de atividade do usuário, o objeto será mostrada no algumas das novas superfícies de interface do usuário no Windows; Por exemplo, Cortana notificações e linha do tempo. Você pode especificar metadados sofisticados (para permitir atividades a serem apresentados no contexto certo) e o ricas visuais (usando marcação [Cartão adaptável](https://adaptivecards.io/) ) em seus objetos de atividade.

Você pode usar as seguintes APIs do Microsoft Graph para criar e recuperar as atividades do usuário:

- [Criar ou substituir atividade](../api/projectrome-put-activity.md)
- [Obter atividades](../api/projectrome-get-activities.md)
- [Obter atividades recentes](../api/projectrome-get-recent-activities.md)
- [Excluir uma atividade](../api/projectrome-delete-activity.md)
- [Criar ou substituir um item do histórico](../api/projectrome-put-historyitem.md)
- [Excluir um item do histórico](../api/projectrome-delete-historyitem.md)

## <a name="devices"></a>Dispositivos

Você pode usar o Project Roma APIs no Microsoft Graph:

- Descobrir e se conectar a dispositivos do usuário
- Início remotamente apps nesses dispositivos
- Enviar mensagens para seus aplicativos nesses dispositivos

Com essas APIs, você pode criar aplicativos que criam experiências fora de um único dispositivo. Por exemplo, você pode estender seu aplicativo de inicialização em uma tela maior. Ou você pode criar uma experiência de complementares para um aplicativo em outro dos dispositivos do usuário.

Você pode usar as seguintes APIs do Microsoft Graph para se comunicar com outros dispositivos do Windows:

- [Listar os dispositivos do usuário](../api/user-list-devices.md)
- [Enviar um comando para um dispositivo](../api/send-device-command.md)
- [Obter o status de comando](../api/get-device-command-status.md)

## <a name="notifications"></a>Notifications

Você pode usar as APIs de notificações no Microsoft Graph para fornecer notificações entre vários pontos de extremidade que o mesmo usuário tiver entrado em. É possível direcionar um usuário diretamente ao lançar notificações, em vez de se preocupar como endereços/canais de dispositivo. Dessa forma, você pode focalizar Projetando os cenários de notificação direita em uma humanos centrada, em vez de uma maneira centralizada no dispositivo. 

Você pode publicar uma notificação de dados brutos ou uma notificação visual direta. Quando uma notificação de dados brutos é entregue para um ponto de extremidade do dispositivo, você pode, em seguida, usar o [SDK do cliente](https://github.com/Microsoft/project-rome) (notificações de Microsoft Graph SDK para Windows, Roma SDK do Project para iOS e Android) para receber e gerenciar notificações. Quando uma notificação visual direta é entregue para um ponto de extremidade do dispositivo, ela mostra específicos de plataforma nativa notificação ao usuário. 

Para obter detalhes, consulte [criar e enviar uma notificação](../api/projectrome-notification-post.md).

