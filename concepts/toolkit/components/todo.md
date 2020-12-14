---
title: Componente tarefas pendentes no Microsoft Graph Toolkit
description: O componente tarefas pendentes permite ao usuário exibir, adicionar, remover, concluir ou editar tarefas pendentes. Ele funciona com qualquer tarefa no Microsoft to-do.
localization_priority: Normal
author: shweaver-MSFT
ms.openlocfilehash: 1a00d045da55dc14da47770b0e56522590f4b5bc
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659159"
---
# <a name="to-do-component-in-the-microsoft-graph-toolkit"></a>Componente tarefas pendentes no Microsoft Graph Toolkit

O componente tarefas pendentes é usado para permitir que o usuário conectado exiba, adicione, remova, conclua e/ou edite tarefas da Microsoft para usar a API tarefas pendentes no Microsoft Graph.

## <a name="example"></a>Exemplo

O exemplo a seguir exibe as tarefas do usuário conectado da Microsoft usando o `mgt-todo` componente. Você pode usar o editor de código para ver como [as propriedades](#properties) alteram o comportamento do componente.

<iframe src="https://mgt.dev/iframe.html?id=components-mgt-todo--tasks&source=docs" height="500"></iframe>

[Abra este exemplo em gerenciamento de. dev](https://mgt.dev/?path=/story/components-mgt-todo--tasks&source=docs)

## <a name="properties"></a>Propriedades

Você pode usar os seguintes atributos e propriedades para personalizar o componente.

| Atributo | Propriedade | Descrição |
| -- | -- | -- |
| somente leitura | readOnly | Um booliano para definir a interface de tarefa como somente leitura (sem adicionar ou remover tarefas). O padrão é `false`. |
| Ocultar-cabeçalho | hideHeader | Um booliano para mostrar ou ocultar o cabeçalho do componente. O padrão é `false`. |
| Hide-opções | hideoptions | Um booliano para mostrar ou ocultar as opções nas tarefas. O padrão é `false`.
| Initial-ID = "folder_id" | initialid | Uma ID de cadeia de caracteres para definir a pasta exibida inicialmente com a ID fornecida. |
| Target-ID = "folder_id"| targetId | Uma ID de cadeia de caracteres para bloquear a interface de tarefas para a ID de pasta fornecida. |
| N/D | isNewTaskVisible  | Determina se a exibição de nova tarefa é visível no processamento. |
| N/D | taskFilter  | Uma função opcional para filtrar quais tarefas são exibidas para o usuário. |

O exemplo a seguir mostra apenas as tarefas da pasta com a ID *12345* e não permite que o usuário crie novas tarefas.

```html
<mgt-todo read-only initial-id="12345"></mgt-todo>
```

## <a name="custom-css-variables"></a>Variáveis CSS personalizadas

O `mgt-todo` componente define as seguintes propriedades personalizadas de CSS.

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

Para saber mais, confira [estilos de componentes](https://docs.microsoft.com/graph/toolkit/style.md).

## <a name="events"></a>Eventos

Os eventos a seguir são acionados do componente.

| Evento | Detalhe | Descrição |
| --- | --- | --- |
| taskAdded | O detalhe contém o respectivo `task` objeto | Dispara quando uma nova tarefa é criada. |
| taskchanged | O detalhe contém o respectivo `task` objeto | Dispara quando os metadados da tarefa são alterados, como marcação concluída. |
| taskClick | O detalhe contém o respectivo `task` objeto | Dispara quando o usuário clica ou toca em uma tarefa. |
| taskRemoved | O detalhe contém o respectivo `task` objeto | Dispara quando uma tarefa existente foi excluída. |

## <a name="templates"></a>Modelos

O `tasks` componente oferece suporte a vários [modelos](../customize-components/templates.md) que permitem substituir determinadas partes do componente. Para especificar um modelo, inclua um `<template>` elemento dentro de um componente e defina o `data-type` valor como um dos seguintes.

| Tipo de dados     | Contexto de dados              | Descrição                                                       |
| ---------     | ------------------------- | ----------------------------------------------------------------- |
| tarefa     | tarefa: um objeto de tarefa tarefas pendentes | Substitui toda a tarefa padrão. |
| tarefa-detalhes | tarefa: um objeto de tarefa tarefas pendentes | O modelo substitui a seção de detalhes da tarefa. |

O exemplo a seguir define um modelo para o componente tarefas.

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

Este controle usa as seguintes APIs e permissões do Microsoft Graph.

| Recurso | Permissão |
| - | - |
| [/me/todo/lists/](/graph/api/todo-list-lists) | Tasks.ReadWrite |
| [/me/todo/lists/{todoTaskListId}/tasks](/graph/api/todotasklist-list-tasks) | Tasks.ReadWrite |
| [/me/todo/lists/{todoTaskListId}/tasks/{taskId}](/graph/api/todotask-get) | Tasks.ReadWrite |

## <a name="authentication"></a>Autenticação

O componente tarefas usa o provedor de autenticação global descrito na [documentação de autenticação](../providers/providers.md).
