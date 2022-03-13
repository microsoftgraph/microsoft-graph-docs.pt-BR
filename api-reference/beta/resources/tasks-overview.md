---
title: Usar a API To Do no Microsoft Graph
description: Você pode usar a API Microsoft Graph para criar um aplicativo que se conecta a tarefas e listas de tarefas no Microsoft To Do.
author: avijityadav
ms.localizationpriority: high
ms.prod: outlook
doc_type: conceptualPageType
ms.openlocfilehash: 5db7dbb8a853fa7a2752d3b4931a22b5ae1e1b4b
ms.sourcegitcommit: 6950d15d8cce5e04733738b8debb92cd8c1d63fe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2022
ms.locfileid: "63451126"
---
# <a name="use-the-to-do-api-in-microsoft-graph"></a>Usar a API To Do no Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usar a API do Microsoft Graph To Do para criar um aplicativo que se conecta à tarefa dos usuários em suas caixas de correio. Compilar uma variedade de experiências com tarefas, tais como as seguintes:

* Crie tarefas a partir do fluxo de trabalho do seu aplicativo, por exemplo, por email ou notificações, e salve-as no To Do. Use a entidade [linkedResource](linkedresource.md) para armazenar o link de volta ao seu aplicativo.
* Sincronize as tarefas existentes de seu aplicativo com o To Do e crie uma única exibição de tarefa para melhor priorização e gerenciabilidade.
* Gerenciar tarefas To Do em aplicações comerciais personalizadas.
* Crie [checklistItems](checklistitem.md) em uma tarefa para dividir tarefas complexas em etapas menores.

Atualmente, a API suporta apenas as permissões delegadas pelo usuário conectado.

Antes de começar com a API To Do, dê uma olhada nos recursos e como eles se relacionam entre si.

![Captura de tela realçando entidades de To Do API pendentes. A captura de tela mostra uma lista de listas de tarefas à esquerda, tarefas dentro de uma lista de tarefas específica no centro e, à direita, itens de lista de verificação e recursos vinculados junto com outras propriedades de tarefas.](/graph/images/tasks-api-entities.png)

## <a name="task-list"></a>Lista de tarefas

Uma [taskList](./basetasklist.md) representa um contêiner lógico de [tarefa](./basetask.md) recursos. Atualmente, você só pode criar tarefas em uma lista de tarefas. As tarefas criadas sem especificar a lista são criadas na lista de Tarefas padrão. Para [obter todas as suas listas de tarefas](../api/basetasklist-get.md), faça a seguinte solicitação HTTP:

``` http
GET /me/tasks/lists
```

## <a name="task"></a>Tarefas

Uma [tarefa](./basetask.md) representa uma tarefa, ou seja, um trabalho ou item pessoal que pode ser rastreado e concluído. Para obter suas tarefas de uma lista de tarefas, faça a seguinte solicitação HTTP:
``` http
GET /me/tasks/lists/{taskListId}/tasks
```

## <a name="checklist-item"></a>Item da lista de verificação 

Um [checklistItem](checklistitem.md) representa um item que ajuda a dividir tarefas complexas em etapas muito menores. Para obter um **checklistItem** de uma tarefa, faça a seguinte solicitação HTTP:
``` http
GET /me/tasks/lists/{taskListId}/tasks/{taskId}/checklistItems/{checklistItems}
```

## <a name="linked-resource"></a>Recurso vinculado

Um [linkedResource](linkedresource_v2.md) representa qualquer item de um aplicativo parceiro relacionado à tarefa; por exemplo, um email de onde uma tarefa foi criada. Você pode usá-la para armazenar informações e o link de volta para o item relacionado em seu aplicativo. Para obter um recurso vinculado de uma tarefa, faça a seguinte solicitação HTTP:
``` http
GET /me/tasks/lists/{taskListId}/tasks/{taskId}/linkedresources/{linkedResourceId}
```

## <a name="track-changes-using-delta-query"></a>Acompanhar alterações usando a consulta delta

Por motivos de desempenho, talvez você queira manter um cache local de objetos e sincronizar periodicamente o cache local com o servidor, usando uma [consulta delta](/graph/delta-query-overview).

Os seguintes recursos da API To Do oferecem suporte à consulta delta:
* [Coleção](./basetask.md) tarefa em uma lista de tarefas
* [TaskList](./basetasklist.md)

## <a name="whats-new"></a>Novidades
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.
