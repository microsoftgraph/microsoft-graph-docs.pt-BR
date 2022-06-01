---
title: Usar a API do Microsoft To Do
description: Você pode usar a API do Microsoft Graph criada no todoTask para criar um aplicativo que se conecta com as tarefas no Microsoft To Do.
author: avijityadav
ms.localizationpriority: high
ms.prod: outlook
doc_type: conceptualPageType
ms.openlocfilehash: e20b6102eb94e05b62b701026fa6958b895739d3
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820382"
---
# <a name="use-the-microsoft-to-do-api"></a>Usar a API do Microsoft To Do

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Use a API de Tarefas Pendentes do Microsoft Graph criada em [todoTask](todotask.md) para criar um aplicativo que se conecta a tarefas em todos os clientes do Microsoft To Do. Compilar uma variedade de experiências com tarefas, tais como as seguintes:

* Crie tarefas a partir do fluxo de trabalho do seu aplicativo, por exemplo, por email ou notificações, e salve-as no To Do. Use a entidade [linkedResource](linkedresource.md) para armazenar o link de volta ao seu aplicativo.
* Sincronize as tarefas existentes de seu aplicativo com o To Do e crie uma única exibição de tarefa para melhor priorização e gerenciabilidade.
* Gerenciar tarefas To Do em aplicações comerciais personalizadas.

Atualmente, a API suporta apenas as permissões delegadas pelo usuário conectado.

Antes de começar com a API To Do, dê uma olhada nos recursos e como eles se relacionam entre si.

![Captura de tela realçando entidades de To Do API pendentes. A captura de tela mostra uma lista de listas de tarefas à esquerda, tarefas dentro de uma lista de tarefas específica no centro e, à direita, itens de lista de verificação e recursos vinculados junto com outras propriedades de tarefas.](/graph/images/tasks-api-entities.png)

## <a name="task-list"></a>Lista de tarefas

Neste conjunto de APIs, uma lista de tarefas é representada por [todoTaskList](./todotasklist.md), que é um recipiente lógico de recursos do [todoTask](./todotask.md). Atualmente, você só pode criar tarefas em uma lista de tarefas. Para [obter todas as suas listas de tarefas](../api/todotasklist-get.md), faça a seguinte solicitação HTTP:

``` http
GET /me/todo/lists
```

## <a name="task"></a>Tarefas

Neste conjunto de APIs, uma tarefa é representada por um recurso [todoTask](./todotask.md) que é uma peça de trabalho ou item pessoal que pode ser rastreado e concluído. Para obter suas tarefas de uma lista de tarefas, faça a seguinte solicitação HTTP:
``` http
GET /me/todo/lists/{todoTaskListId}/tasks
```

## <a name="checklist-item"></a>Item da lista de verificação 

Um [checklistItem](checklistitem.md) representa uma subtarefa em um [todoTask](./todotask.md) maior. **ChecklistItem** permite dividir uma tarefa complexa em tarefas menores e mais acionáveis. Para obter um **checklistItem** de uma tarefa, faça a seguinte solicitação HTTP:
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{todoTaskId}/checklistItems/{checklistItems}
```

## <a name="linked-resource"></a>Recurso vinculado

O [linkedResource](linkedresource.md) representa qualquer item de um aplicativo de parceiro relacionado à tarefa, por exemplo, um item como o email de onde uma tarefa foi criada. Você pode usá-la para armazenar informações e o link de volta para o item relacionado em seu aplicativo. Para obter um recurso vinculado de uma tarefa, faça a seguinte solicitação HTTP:
``` http
GET /me/todo/lists/{todoTaskListId}/tasks/{todoTaskId}/linkedresources/{linkedResourceId}
```

## <a name="track-changes-using-delta-query"></a>Acompanhar alterações usando a consulta delta

Por motivos de desempenho, talvez você queira manter um cache local de objetos e sincronizar periodicamente o cache local com o servidor, usando uma [consulta delta](/graph/delta-query-overview).

Os seguintes recursos da API To Do oferecem suporte à consulta delta:
* Coleção [toTask](./todotask.md) em uma lista de tarefas
* [todoTaskList](./todotasklist.md)

## <a name="whats-new"></a>O que há de novo
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.

