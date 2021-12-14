---
title: Usar a API de Tarefas Pendentes da Microsoft
description: Você pode usar a API Microsoft Graph para criar um aplicativo que se conecta a tarefas e listas de tarefas no Microsoft To Do.
author: avijityadav
ms.localizationpriority: high
ms.prod: outlook
doc_type: conceptualPageType
ms.openlocfilehash: 1151b52f94c4458f500abb5a767674cf19aa5f5a
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/13/2021
ms.locfileid: "61424821"
---
# <a name="use-the-microsoft-to-do-api"></a>Usar a API do Microsoft To Do

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Use a API de Tarefas Pendentes do Microsoft Graph para criar um aplicativo que se conecta às tarefas dos usuários em suas caixas de correio. Compilar uma variedade de experiências com tarefas, tais como as seguintes:

* Crie tarefas a partir do fluxo de trabalho do seu aplicativo, por exemplo, por email ou notificações, e salve-as no To Do. Use a entidade [linkedResource](linkedresource.md) para armazenar o link de volta ao seu aplicativo.
* Sincronize as tarefas existentes de seu aplicativo com o To Do e crie uma única exibição de tarefa para melhor priorização e gerenciabilidade.
* Gerenciar tarefas To Do em aplicações comerciais personalizadas.
* Crie [checklistItems](checklistitem.md) em uma tarefa para dividir tarefas complexas em etapas menores.

Atualmente, a API suporta apenas as permissões delegadas pelo usuário conectado.

Antes de começar com a API de Tarefas Pendentes, dê uma olhada nos recursos e como eles se relacionam entre si.

![Captura de tela que destaca as entidades da API de Tarefas Pendentes. A captura de tela mostra a lista de listas de tarefas à esquerda, tarefas dentro de uma lista de tarefas específica no centro e, à direita, itens de lista de verificação e recurso vinculado junto com outras propriedades da tarefa.](/graph/images/tasks-api-entities.png)

## <a name="task-list"></a>Lista de tarefas

Uma [TaskList](./basetasklist.md) representa um contêiner lógico de recursos [Tarefa](./basetask.md). Atualmente, você só pode criar tarefas em uma lista de tarefas. As tarefas criadas sem especificar a lista são criadas na lista de Tarefas padrão. Para [obter todas as suas listas de tarefas](../api/todotasklist-get.md), faça a seguinte solicitação HTTP:

``` http
GET /me/tasks/lists
```

## <a name="task"></a>Tarefas

Uma [Tarefa](./basetask.md) representa uma tarefa, ou seja, um trabalho ou item pessoal que pode ser rastreado e concluído. Para obter suas tarefas de uma lista de tarefas, faça a seguinte solicitação HTTP:
``` http
GET /me/tasks/lists/{taskListId}/tasks
```

## <a name="checklist-item"></a>Item da Lista de Verificação 

Um [ChecklistItem](linkedresource_v2.md) um item que ajuda a dividir tarefas complexas em etapas muito menores. Para obter um checklistItems de uma tarefa, faça a seguinte solicitação HTTP:
``` http
GET /me/todo/lists/{taskListId}/tasks/{taskId}/checklistItems/{checklistItems}
```

## <a name="linked-resource"></a>Recurso vinculado

O [linkedResource](linkedresource_v2.md) representa qualquer item de um aplicativo de parceiro relacionado à tarefa, por exemplo, um item como o email de onde uma tarefa foi criada. Você pode usá-la para armazenar informações e o link de volta para o item relacionado em seu aplicativo. Para obter um recurso vinculado de uma tarefa, faça a seguinte solicitação HTTP:
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
