---
title: 'Usar a API do Microsoft Graph para trabalhar com o Project Roma '
description: 'O Project Roma é uma iniciativa da Microsoft para criar uma plataforma que permite aos desenvolvedores de aplicativos criar grandes experiências entre dispositivos. O Project Roma permite diferentes recursos que conectam diferentes serviços e pontos de extremidade do cliente quando o usuário entra com a mesma conta da Microsoft ou conta corporativa ou de estudante. Isso permite que você implemente experiências entre dispositivos e várias plataformas centradas em tarefas do usuário, em vez de dispositivos. '
localization_priority: Normal
doc_type: conceptualPageType
ms.prod: ''
author: ''
ms.openlocfilehash: fd3608c458b7e1f1fe3e39fdd35e1ba03a9f531e
ms.sourcegitcommit: ef9e0fd8fb6047fa9272e98310eaed2c4e0a2660
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/23/2020
ms.locfileid: "44353662"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a>Usar a API do Microsoft Graph para trabalhar com o Project Roma 

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O [Project Roma](https://developer.microsoft.com/en-us/windows/project-rome) é uma iniciativa da Microsoft para criar uma plataforma que permite aos desenvolvedores de aplicativos criar grandes experiências entre dispositivos. O Project Roma permite diferentes recursos que conectam diferentes serviços e pontos de extremidade do cliente quando o usuário entra com a mesma conta da Microsoft ou conta corporativa ou de estudante. Isso permite que você implemente experiências entre dispositivos e várias plataformas centradas em tarefas do usuário, em vez de dispositivos. 

Três principais recursos de Roma do projeto são expostos pelo Microsoft Graph para ajudá-lo a habilitar excelentes experiências entre dispositivos: atividades, dispositivos e notificações. 

## <a name="activities"></a>Atividades

As atividades no Microsoft Graph permitem que você direcionar o compromisso do usuário com seus aplicativos entre dispositivos e plataformas. Uma atividade é a unidade de contrato de usuário e consiste em três componentes:

- Um link profundo
- Uma representação visual
- Metadados de conteúdo que descrevem a atividade, usando o [https://schema.org/](https://schema.org/) vocabulário compartilhado

Quando uma sessão é criada por um aplicativo, um item de histórico é adicionado à atividade para refletir o período de envolvimento do usuário. Cada vez que um usuário reparticipa de uma atividade, um novo item de histórico é adicionado à atividade para acumular o envolvimento do usuário.

Quando um aplicativo publica objetos de atividade do usuário, o objeto aparecerá em algumas das novas superfícies de interface de usuário no Windows; por exemplo, notificações e cronograma da Cortana. Você pode especificar tanto metadados avançados (para permitir que as atividades sejam apresentadas no contexto certo) e Visual ricos (usando a marcação de [cartão adaptável](https://adaptivecards.io/) ) em seus objetos de atividade.

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

## <a name="whats-new"></a>Novidades
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.