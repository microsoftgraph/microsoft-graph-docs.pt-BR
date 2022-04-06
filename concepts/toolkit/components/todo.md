---
title: To Do componente no microsoft Graph Toolkit
description: O To Do permite que o usuário exibir, adicionar, remover, concluir ou editar todas as tarefas. Ele funciona com qualquer tarefa no Microsoft To-Do.
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 6a77d75609cbff22fbaccefe45cd1f8b9e5355ca
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589244"
---
# <a name="to-do-component-in-the-microsoft-graph-toolkit"></a>To Do componente no microsoft Graph Toolkit

O componente To Do é usado para permitir que o usuário inscreveu para exibir, adicionar, remover, concluir e/ou editar tarefas do Microsoft To Do usando a API To Do no Microsoft Graph.

## <a name="example"></a>Exemplo

O exemplo a seguir exibe as tarefas de Microsoft To Do do usuário Microsoft To Do usando o `mgt-todo` componente. Você pode usar o editor de código para ver como as [propriedades](#properties) alteram o comportamento do componente.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-todo--tasks&source=docs" height="500"></iframe>

[Abrir este exemplo no mgt.dev](https://mgt.dev/?path=/story/components-mgt-todo--tasks&source=docs)

## <a name="properties"></a>Propriedades

Você pode usar os seguintes atributos e propriedades para personalizar o componente.

| Atributo | Propriedade | Descrição |
| -- | -- | -- |
| somente leitura | readOnly | Um Boolean para definir a interface da tarefa a ser lida somente (sem adicionar ou remover tarefas). O padrão é `false`. |
| hide-header | hideHeader | Um Boolean para mostrar ou ocultar o header do componente. O padrão é `false`. |
| hide-options | hideOptions | Um Boolean para mostrar ou ocultar as opções em tarefas. O padrão é `false`.
| initial-id="folder_id" | initialId | Uma ID de cadeia de caracteres para definir a pasta inicialmente exibida como a ID fornecida. |
| target-id="folder_id"| targetId | Uma ID de cadeia de caracteres para bloquear a interface de tarefas na ID da pasta fornecida. |
| N/D | isNewTaskVisible  | Determina se o novo exibição de tarefa está visível na renderização. |
| N/D | taskFilter  | Uma função opcional para filtrar quais tarefas são mostradas ao usuário. |

O exemplo a seguir mostra apenas tarefas da pasta com a ID *12345* e não permite que o usuário crie novas tarefas.

```html
<mgt-todo read-only initial-id="12345"></mgt-todo>
```

## <a name="custom-css-variables"></a>Variáveis CSS personalizadas

O `mgt-todo` componente define as seguintes propriedades personalizadas CSS.

````css
mgt-todo {
  --tasks-background-color
  --tasks-header-padding
  --tasks-title-padding
  --tasks-plan-title-font-size
  --tasks-plan-title-padding

  --tasks-new-button-width
  --tasks-new-button-height
  --tasks-new-button-color
  --tasks-new-button-background
  --tasks-new-button-border
  --tasks-new-button-hover-background
  --tasks-new-button-active-background

  --task-margin
  --task-background
  --task-border
  --task-header-color
  --task-header-margin

  --task-new-margin
  --task-new-border
  --task-new-input-margin
  --task-new-input-padding
  --task-new-input-font-size
  --task-new-select-border

  --task-new-add-button-background
  --task-new-add-button-disabled-background
  --task-new-cancel-button-color

  --task-complete-background
  --task-complete-border

  --task-icon-alignment: flex-start (default) | center | flex-end
  --task-icon-background
  --task-icon-background-completed
  --task-icon-border
  --task-icon-border-completed
  --task-icon-border-radius
  --task-icon-color
  --task-icon-color-completed
}
````

Para saber mais, confira [componentes de estilo](/graph/toolkit/style.md).

## <a name="events"></a>Eventos

Os eventos a seguir são disparados do componente.

Evento | Quando é emitido | Dados personalizados | Cancelável | Bolhas | Funciona com modelo personalizado
------|-------------------|--------------|:-----------:|:---------:|:---------------------------:|
`taskClick` | Dispara quando o usuário clica ou toca em uma tarefa | Tarefa [selecionada](https://github.com/microsoftgraph/microsoft-graph-toolkit/blob/66a5bbb6591e6260e95dbc00c0d06bcbe8dcef38/packages/mgt-components/src/components/mgt-todo/graph.todo.ts#L41) | Não | Não | Não

Para obter mais informações sobre como lidar com eventos, consulte [eventos](../customize-components/events.md).

## <a name="templates"></a>Modelos

O `tasks` componente dá suporte a [vários modelos](../customize-components/templates.md) que permitem substituir determinadas partes do componente. Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e de `data-type` definir o valor como um dos seguintes.

| Tipo de dados     | Contexto de dados              | Descrição                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| tarefa     | tarefa: um objeto de tarefa a ser usado | Substitui toda a tarefa padrão. |
| detalhes da tarefa | tarefa: um objeto de tarefa a ser usado | O modelo substitui a seção de detalhes da tarefa. |

O exemplo a seguir define um modelo para o componente de tarefas.

```html
<mgt-todo>
    <template data-type="task-details">
        <div>
            Importance Level: {{task.importance}}
        </div>
    </template>
</mgt-todo>
```

## <a name="microsoft-graph-permissions"></a>Permissões do Microsoft Graph

Esse controle usa as seguintes APIs Graph Microsoft e permissões.

| Configuração | Permissão | API |
| ------------- | ---------- | --- |
| `targetId` set | Tasks.Read | [/me/todo/lists/${listId}](/graph/api/todotasklist-get?tabs=http), [/me/todo/lists/{todoTaskListId}/tasks](/graph/api/todotasklist-list-tasks) |
| `targetId` não definido | Tasks.Read | [/me/todo/lists](/graph/api/todo-list-lists?tabs=http), [/me/todo/lists/{todoTaskListId}/tasks](/graph/api/todotasklist-list-tasks) |
| criar, atualizar ou excluir tarefa | Tasks.ReadWrite | [/me/todo/lists/{todoTaskListId}/tasks/{taskId}](/graph/api/todotask-get) |

## <a name="authentication"></a>Autenticação

O componente tarefas usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md).

## <a name="cache"></a>Cache

O `mgt-todo` componente não armazena dados em cache.