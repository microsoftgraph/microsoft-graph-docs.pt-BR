---
title: Usar o Microsoft API do Graph para trabalhar com o Project Rome
description: Project Roma é uma iniciativa da Microsoft para criar uma plataforma de experiências entre dispositivos. o Project Rome permite que um aplicativo em um cliente ou serviço local interaja com aplicativos e serviços em um host remoto quando o usuário entra com a mesma conta da Microsoft que ele usa para entrar no dispositivo cliente. Isso permite que você programe experiências entre dispositivos e plataformas que são centralizadas em torno de tarefas do usuário em vez de dispositivos.
ms.localizationpriority: medium
author: ailae
ms.prod: project-rome
doc_type: conceptualPageType
ms.openlocfilehash: 30e0c2049a5c4ef0b9aea79ebe2d420f5a341c87
ms.sourcegitcommit: 423e698a580c3b902f2816b0216ab9d5b91e6d20
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2022
ms.locfileid: "66034457"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a>Usar o Microsoft API do Graph para trabalhar com o Project Rome

[Project Roma é](https://developer.microsoft.com/en-us/windows/project-rome) uma iniciativa da Microsoft para criar uma plataforma de experiências entre dispositivos. o Project Rome permite que um aplicativo em um cliente ou serviço local interaja com aplicativos e serviços em um host remoto quando o usuário entra com a mesma conta da Microsoft que ele usa para entrar no dispositivo cliente. Isso permite que você programe experiências entre dispositivos e plataformas que são centralizadas em torno de tarefas do usuário em vez de dispositivos.

Um componente-chave é exposto por meio do Microsoft Graph para habilitar essas experiências: atividades.

## <a name="activities"></a>Atividades

As atividades no Microsoft Graph permitem que você conduza o envolvimento do usuário com seus aplicativos entre dispositivos e plataformas. Uma atividade é a unidade de envolvimento do usuário e consiste em três componentes:

- Um link profundo
- Uma representação visual
- Metadados de conteúdo que descrevem a atividade, usando o [https://schema.org/](https://schema.org/) vocabulário compartilhado

Quando uma sessão é criada por um aplicativo, um item de histórico é adicionado à atividade para refletir o período de envolvimento do usuário. Sempre que um usuário se reangaja com uma atividade, um novo item de histórico é adicionado à atividade para acumular o envolvimento do usuário.

Quando um aplicativo publica objetos de atividade do usuário, o objeto aparecerá em algumas das novas superfícies de interface do usuário no Windows; por exemplo, Cortana Notificações e Linha do Tempo. Você pode especificar metadados avançados (para permitir que as atividades sejam apresentadas apenas no contexto certo) e visuais avançados (usando marcação de Cartão [Adaptável](https://adaptivecards.io/) ) em seus objetos de atividade.

Você pode usar as seguintes APIs do Microsoft Graph para criar e recuperar atividades do usuário:

- [Criar ou substituir atividade](../api/projectrome-put-activity.md)
- [Obter atividades](../api/projectrome-get-activities.md)
- [Obter atividades recentes](../api/projectrome-get-recent-activities.md)
- [Excluir uma atividade](../api/projectrome-delete-activity.md)
- [Criar ou substituir um item do histórico](../api/projectrome-put-historyitem.md)
- [Excluir um item do histórico](../api/projectrome-delete-historyitem.md)

## <a name="whats-new"></a>Novidades
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.
