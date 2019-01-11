---
title: Usar a API do Microsoft Graph para trabalhar com o Project Roma
description: Project Roma é uma iniciativa da Microsoft para criar uma referência cruzada de dispositivo experiências de plataforma. Project Roma permite que um aplicativo em um cliente local ou serviço interagir com aplicativos e serviços em um host remoto quando o usuário entra com a mesma conta da Microsoft que eles usam para entrar no dispositivo do cliente. Isso permite que você programa entre dispositivos plataforma cruzada experiências e que são centralizadas em torno de tarefas do usuário, em vez dos dispositivos.
localization_priority: Normal
ms.openlocfilehash: d103bb68560a39cc4491460969a36bb81bb6da44
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840961"
---
# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a>Usar a API do Microsoft Graph para trabalhar com o Project Roma

[Project Roma](https://developer.microsoft.com/en-us/windows/project-rome) é uma iniciativa da Microsoft para criar uma referência cruzada de dispositivo experiências de plataforma. Project Roma permite que um aplicativo em um cliente local ou serviço interagir com aplicativos e serviços em um host remoto quando o usuário entra com a mesma conta da Microsoft que eles usam para entrar no dispositivo do cliente. Isso permite que você programa entre dispositivos plataforma cruzada experiências e que são centralizadas em torno de tarefas do usuário, em vez dos dispositivos.

Um componente-chave é exposto por meio do Microsoft Graph para habilitar essas experiências: atividades.

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

