---
title: Usar a API do Microsoft To Do
description: Você pode usar a API do Microsoft Graph para criar um aplicativo que se conecta com tarefas no Microsoft To Do.
author: avijityadav
localization_priority: Priority
ms.prod: outlook
doc_type: conceptualPageType
ms.openlocfilehash: e5e28602f2a8c3b057984af75d06e5f8cbde20de822f39dca146ccc1e6dc981e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189174"
---
# <a name="use-the-microsoft-to-do-api"></a>Usar a API do Microsoft To Do

Use a API To Do no Microsoft Graph para criar um aplicativo que se conecta com tarefas através do Microsoft To Do. Compilar uma variedade de experiências com tarefas, tais como as seguintes:

* Crie tarefas a partir do fluxo de trabalho do seu aplicativo, por exemplo, por email ou notificações, e salve-as no To Do. Use a entidade [linkedResource](linkedresource.md) para armazenar o link de volta ao seu aplicativo.
* Sincronize as tarefas existentes de seu aplicativo com o To Do e crie uma única exibição de tarefa para melhor priorização e gerenciabilidade.
* Gerenciar tarefas To Do em aplicações comerciais personalizadas.

Atualmente, a API suporta apenas as permissões delegadas pelo usuário conectado.
 
Antes de começar com a API To Do, dê uma olhada nos recursos e como eles se relacionam entre si.

![Entidades da API To Do](/graph/images/todo-api-entities.png)

## <a name="task-list"></a>Lista de tarefas

O [todoTaskList](./todotasklist.md) representa um contêiner lógico dos recursos [todoTask](./todotask.md). Atualmente, você só pode criar tarefas em uma lista de tarefas. Para [obter todas as suas listas de tarefas](../api/todotasklist-get.md), faça a seguinte solicitação HTTP:

``` http
GET /me/todo/lists
```

## <a name="task"></a>Tarefas

O [todoTask](./todotask.md) representa uma tarefa, ou seja, um trabalho ou um item pessoal que pode ser acompanhado e concluído. Para obter suas tarefas de uma lista de tarefas, faça a seguinte solicitação HTTP:
``` http
GET /me/todo/lists/{todoTaskListId}/tasks
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

