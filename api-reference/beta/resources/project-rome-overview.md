---
title: 'Usar a API do Microsoft Graph para trabalhar com o Project Roma '
description: 'O Project Roma é uma iniciativa da Microsoft para criar uma plataforma que permite aos desenvolvedores de aplicativos criar grandes experiências entre dispositivos. O Project Roma permite diferentes recursos que conectam diferentes serviços e pontos de extremidade do cliente quando o usuário entra com a mesma conta da Microsoft ou conta corporativa ou de estudante. Isso permite que você implemente experiências entre dispositivos e várias plataformas centradas em tarefas do usuário, em vez de dispositivos. '
localization_priority: Normal
ms.openlocfilehash: 57c5189f3caf64ec048d000d5e9108811bd88145
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563350"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a>Usar a API do Microsoft Graph para trabalhar com o Project Roma 

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O [Project Roma](https://developer.microsoft.com/en-us/windows/project-rome) é uma iniciativa da Microsoft para criar uma plataforma que permite aos desenvolvedores de aplicativos criar grandes experiências entre dispositivos. O Project Roma permite diferentes recursos que conectam diferentes serviços e pontos de extremidade do cliente quando o usuário entra com a mesma conta da Microsoft ou conta corporativa ou de estudante. Isso permite que você implemente experiências entre dispositivos e várias plataformas centradas em tarefas do usuário, em vez de dispositivos. 

Três principais recursos de Roma do projeto são expostos pelo Microsoft Graph para ajudá-lo a habilitar excelentes experiências entre dispositivos: atividades, dispositivos e notificações. 

## <a name="activities"></a>Atividades

As atividades no Microsoft Graph permitem que você direcionar o compromisso do usuário com seus aplicativos entre dispositivos e plataformas. Uma atividade é a unidade de contrato de usuário e consiste em três componentes:

- Um link profundo
- Uma representação visual
- Metadados de conteúdo que descrevem a atividade, usando [https://schema.org/](https://schema.org/) o vocabulário compartilhado

Quando uma sessão é criada por um aplicativo, um item de histórico é adicionado à atividade para refletir o período de envolvimento do usuário. Cada vez que um usuário reparticipa de uma atividade, um novo item de histórico é adicionado à atividade para acumular o envolvimento do usuário.

Quando um aplicativo publica objetos de atividade do usuário, o objeto aparecerá em algumas das novas superfícies de interface de usuário no Windows; por exemplo, notificações e cronograma da corTana. Você pode especificar tanto metadados avançados (para permitir que as atividades sejam apresentadas no contexto certo) e Visual ricos (usando a marcação de [cartão adaptável](https://adaptivecards.io/) ) em seus objetos de atividade.

Você pode usar as seguintes APIs do Microsoft Graph para criar e recuperar atividades do usuário:

- [Criar ou substituir atividade](../api/projectrome-put-activity.md)
- [Obter atividades](../api/projectrome-get-activities.md)
- [Obter atividades recentes](../api/projectrome-get-recent-activities.md)
- [Excluir uma atividade](../api/projectrome-delete-activity.md)
- [Criar ou substituir um item do histórico](../api/projectrome-put-historyitem.md)
- [Excluir um item do histórico](../api/projectrome-delete-historyitem.md)

## <a name="devices"></a>Dispositivos

Você pode usar as APIs do Project Roma no Microsoft Graph para:

- Descobrir e conectar a dispositivos do usuário
- Iniciar remotamente aplicativos nesses dispositivos
- Enviar mensagens para seus aplicativos nesses dispositivos

Com essas APIs, você pode criar aplicativos que criam experiências ricas que transcendem um único dispositivo. Por exemplo, você pode estender seu aplicativo para iniciar em uma tela maior. Ou você pode criar uma experiência complementar para um aplicativo em outro dispositivo do usuário.

Você pode usar as seguintes APIs do Microsoft Graph para se comunicar com outros dispositivos do Windows:

- [Listar os dispositivos do usuário](../api/user-list-devices.md)
- [Enviar um comando para um dispositivo](../api/send-device-command.md)
- [Obter status do comando](../api/get-device-command-status.md)

## <a name="notifications"></a>Notificações

Você pode usar as APIs de notificações no Microsoft Graph para entregar notificações entre vários pontos de extremidade nos quais o mesmo usuário está conectado. Você pode direcionar um usuário diretamente ao postar notificações em vez de se preocupar com endereços/canais de dispositivos. Dessa forma, você pode se concentrar no design dos cenários de notificação adequados em uma forma centrada no homem, e não em um dispositivo. 

Você pode publicar uma notificação de dados brutos ou uma notificação Visual direta. Quando uma notificação de dados brutos é entregue a um ponto de extremidade do dispositivo, você pode usar o SDK do [cliente](https://github.com/Microsoft/project-rome) (SDK de notificações do Microsoft Graph para Windows, SDK do Project Roma para IOS e Android) para receber e gerenciar notificações. Quando uma notificação Visual direta é entregue a um ponto de extremidade do dispositivo, ela mostra a notificação nativa específica da plataforma para o usuário. 

Para obter detalhes, consulte [criar e enviar uma notificação](../api/projectrome-notification-post.md).

