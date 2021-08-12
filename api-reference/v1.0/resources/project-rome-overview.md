---
title: Usar a API Graph Microsoft para trabalhar com Project Rome
description: Project Roma é uma iniciativa da Microsoft para criar uma plataforma de experiências entre dispositivos. Project Roma permite que um aplicativo em um cliente ou serviço local interaja com aplicativos e serviços em um host remoto quando o usuário entrar com a mesma conta da Microsoft usada para entrar no dispositivo cliente. Isso permite que você programe experiências entre dispositivos e plataformas centralizadas em torno de tarefas do usuário, em vez de dispositivos.
localization_priority: Normal
author: ailae
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: 4b011f217d4ef3f55afdafa6880e60a8cd38bf53cecadee70f4355dafbdb7642
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54152310"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a>Usar a API Graph Microsoft para trabalhar com Project Rome

[Project Roma é](https://developer.microsoft.com/en-us/windows/project-rome) uma iniciativa da Microsoft para criar uma plataforma de experiências entre dispositivos. Project Roma permite que um aplicativo em um cliente ou serviço local interaja com aplicativos e serviços em um host remoto quando o usuário entrar com a mesma conta da Microsoft usada para entrar no dispositivo cliente. Isso permite que você programe experiências entre dispositivos e plataformas centralizadas em torno de tarefas do usuário, em vez de dispositivos.

Um componente chave é exposto por meio do Microsoft Graph para habilitar essas experiências: atividades.

## <a name="activities"></a>Atividades

As atividades no Microsoft Graph permitem que você conduza o envolvimento do usuário com seus aplicativos em dispositivos e plataformas. Uma atividade é a unidade de envolvimento do usuário e consiste em três componentes:

- Um link profundo
- Uma representação visual
- Metadados de conteúdo que descrevem a atividade usando o [https://schema.org/](https://schema.org/) vocabulário compartilhado

Quando uma sessão é criada por um aplicativo, um item de histórico é adicionado à atividade para refletir o período de envolvimento do usuário. Sempre que um usuário reaja com uma atividade, um novo item de histórico é adicionado à atividade para acumular o envolvimento do usuário.

Quando um aplicativo publica objetos de atividade do usuário, o objeto aparece em algumas das novas superfícies da interface do usuário no Windows; por exemplo, Cortana Notificações e Linha do Tempo. Você pode especificar metadados ricos (para permitir que atividades sejam apresentadas [](https://adaptivecards.io/) apenas no contexto correto) e elementos visuais ricos (usando marcação de Cartão Adaptável) em seus objetos de atividade.

Você pode usar as seguintes APIs Graph Microsoft para criar e recuperar atividades do usuário:

- [Criar ou substituir atividade](../api/projectrome-put-activity.md)
- [Obter atividades](../api/projectrome-get-activities.md)
- [Obter atividades recentes](../api/projectrome-get-recent-activities.md)
- [Excluir uma atividade](../api/projectrome-delete-activity.md)
- [Criar ou substituir um item do histórico](../api/projectrome-put-historyitem.md)
- [Excluir um item do histórico](../api/projectrome-delete-historyitem.md)

## <a name="whats-new"></a>Novidades
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.
