---
title: 'Usar a API Graph Microsoft para trabalhar com Project Rome '
description: 'Project Roma é uma iniciativa da Microsoft para criar uma plataforma que permite que os desenvolvedores de aplicativos criem ótimas experiências entre dispositivos. Project Rome habilita diferentes recursos que conectam diferentes serviços e pontos de extremidade do cliente quando o usuário se conecta com a mesma conta da Microsoft ou conta de trabalho ou de estudante. Isso permite que você implemente experiências entre dispositivos e plataformas centralizadas em torno de tarefas do usuário, em vez de dispositivos. '
ms.localizationpriority: medium
doc_type: conceptualPageType
author: ailae
ms.prod: project-rome
ms.openlocfilehash: d8dafd71d02a49080b9070254415b3b59d2ffd8a
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/01/2022
ms.locfileid: "62291426"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a>Usar a API Graph Microsoft para trabalhar com Project Rome

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Project Roma é](https://developer.microsoft.com/windows/project-rome) uma iniciativa da Microsoft para criar uma plataforma que permite que os desenvolvedores de aplicativos criem ótimas experiências entre dispositivos. Project Rome habilita diferentes recursos que conectam diferentes serviços e pontos de extremidade do cliente quando o usuário se conecta com a mesma conta da Microsoft ou conta de trabalho ou de estudante. Isso permite que você implemente experiências entre dispositivos e plataformas centralizadas em torno de tarefas do usuário, em vez de dispositivos.

Três principais Project de Roma são expostos por meio do Microsoft Graph para ajudá-lo a habilitar ótimas experiências entre dispositivos: atividades, dispositivos e notificações.

## <a name="activities"></a>Atividades

As atividades no Microsoft Graph permitem que você conduza o envolvimento do usuário com seus aplicativos em dispositivos e plataformas. Uma atividade é a unidade de envolvimento do usuário e consiste em três componentes:

- Um link profundo
- Uma representação visual
- Metadados de conteúdo que descrevem a atividade usando o [https://schema.org/](https://schema.org/) vocabulário compartilhado

Quando uma sessão é criada por um aplicativo, um item de histórico é adicionado à atividade para refletir o período de envolvimento do usuário. Sempre que um usuário reaja com uma atividade, um novo item de histórico é adicionado à atividade para acumular o envolvimento do usuário.

Quando um aplicativo publica objetos de atividade do usuário, o objeto aparece em algumas das novas superfícies da interface do usuário no Windows; por exemplo, Cortana Notificações e Linha do Tempo. Você pode especificar metadados ricos (para permitir que atividades sejam apresentadas apenas no contexto correto) e elementos visuais ricos ([](https://adaptivecards.io/)usando marcação de Cartão Adaptável) em seus objetos de atividade.

Você pode usar as seguintes APIs Graph Microsoft para criar e recuperar atividades do usuário:

- [Criar ou substituir atividade](../api/projectrome-put-activity.md)
- [Obter atividades](../api/projectrome-get-activities.md)
- [Obter atividades recentes](../api/projectrome-get-recent-activities.md)
- [Excluir uma atividade](../api/projectrome-delete-activity.md)
- [Criar ou substituir um item do histórico](../api/projectrome-put-historyitem.md)
- [Excluir um item do histórico](../api/projectrome-delete-historyitem.md)

## <a name="devices-deprecated"></a>Dispositivos (preterido)

Você pode usar Project APIs de Roma no Microsoft Graph para:

- Descobrir e conectar-se aos dispositivos do usuário
- Iniciar remotamente aplicativos nesses dispositivos
- Enviar mensagens para seus aplicativos nesses dispositivos

Com essas APIs, você pode criar aplicativos que criam experiências ricas que transcendem um único dispositivo. Por exemplo, você pode estender seu aplicativo para iniciar em uma tela maior. Ou você pode criar uma experiência de companhia para um aplicativo em outro dispositivo do usuário.

Você pode usar as seguintes APIs Graph Microsoft para se comunicar com outros Windows dispositivos:

- [Listar os dispositivos do usuário](../api/user-list-devices.md)
- [Enviar um comando para um dispositivo](../api/send-device-command.md)
- [Obter status do comando](../api/get-device-command-status.md)

## <a name="whats-new"></a>Novidades
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.

