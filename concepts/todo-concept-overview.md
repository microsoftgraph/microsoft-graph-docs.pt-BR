---
title: Visão geral da API do To Do
description: Use a API de Tarefas Pendentes da Microsoft no Microsoft Graph para gerenciar tarefas e planejar seu dia. As tarefas são organizadas em listas de tarefas acessadas através de clientes do Tarefas Pendentes, Outlook e Teams.
author: avijityadav
ms.localizationpriority: high
ms.prod: outlook
ms.openlocfilehash: 30e4655ddcf4ff96b6cd3c82df80402c2f83d330
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2022
ms.locfileid: "66556287"
---
# <a name="to-do-api-overview"></a>Visão geral da API do Tarefa Pendente

A API de Tarefas Pendentes da Microsoft fornece uma maneira simples para as pessoas gerenciarem suas tarefas e planejarem seu dia. As tarefas são organizadas em listas de tarefas, que podem ser acessadas através de clientes do Tarefas Pendentes, Outlook e Teams a partir de qualquer dispositivo.

**Aplicativo To Do para Windows**

![Captura de tela de um aplicativo Microsoft To Do para Windows](./images/todo-windows-app.png "Imagem de um aplicativo Microsoft To Do para Windows")

## <a name="why-integrate-with-to-do"></a>Vantagens da integração no To Do

### <a name="ease-of-organizing-and-tracking-tasks"></a>Facilidade para organizar e acompanhar tarefas
O Microsoft To Do ajuda você a criar uma lista para qualquer coisa, desde tarefas de trabalho até projetos caseiros até compras em supermercado. Você pode acompanhar os prazos adicionando lembretes, datas de vencimento e anotações. Você pode acessar suas listas de qualquer lugar com os aplicativos da Microsoft To-Do para iOS, Android, Mac, Windows e para a Web. 

### <a name="integrate-across-microsoft-365"></a>Integração através da Microsoft 365
To Do é o único destino para tarefas pessoais no Microsoft 365. Portanto, está profundamente integrado aos hubs, da Microsoft 365, Outlook e Teams. As tarefas criadas nesses produtos são sincronizadas com o To Do, para que você possa acessá-las e gerenciá-las através de dispositivos. A integração do To Do pode ajudá-lo a alcançar milhões de usuários que usam o To Do para reunir tarefas do Outlook e do Teams em uma exibição integrada.  

### <a name="support-task-completion-using-linked-resources"></a>Dar suporte a conclusão de tarefas usando recursos vinculados
O Microsoft To Do fornece uma nova entidade chamada _linkedResource_, que você pode usar para criar tarefas que podem ser vinculadas de volta às suas fontes originais. Você pode usar isto para integrar perfeitamente ao To Do em seu fluxo de trabalho, criando tarefas que são vinculadas ao seu produto ou serviço. 

## <a name="common-to-do-api-operations"></a>Operações comuns da API To Do.

|Operação|Solicitação|
|:--------|:--|
| Listar todas as listas de tarefas | GET https://graph.microsoft.com/v1.0/me/todo/lists |
| Lista de todas as tarefas em uma lista de tarefas | GET https://graph.microsoft.com/v1.0/me/todo/lists/{todoTaskListId}/tasks |
| Criar uma nova tarefa | POST https://graph.microsoft.com/v1.0/me/todo/lists/{todoTaskListId}/tasks |
| Atualizar uma tarefa | PATCH https://graph.microsoft.com/v1.0/me/todo/lists/{todoTaskListId}/tasks/{todoTaskId} |
| Excluir uma tarefa | DELETE https://graph.microsoft.com/v1.0/me/todo/lists/{todoTaskListId}/tasks/{todoTaskId} |

## <a name="api-reference"></a>Referência da API

Está procurando a referência de API para esse serviço?

- [API de Tarefas Pendentes no Microsoft Graph v1.0](/graph/api/resources/todo-overview?view=graph-rest-1.0&preserve-view=true)
- [API de Tarefas Pendentes no Microsoft Graph beta](/graph/api/resources/todo-overview?view=graph-rest-beta&preserve-view=true)
