---
title: Tipo de recurso outlookUser
description: Representa os serviços do Outlook disponíveis para um usuário.
author: angelgolfer-ms
ms.openlocfilehash: 51926b84b2e8ed19225369eda774408ae6031b58
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319968"
---
# <a name="outlookuser-resource-type"></a>Tipo de recurso outlookUser

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa os serviços do Outlook disponíveis para um usuário.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar categoria](../api/outlookuser-post-mastercategories.md) | [outlookCategory](outlookcategory.md) |Cria um objeto **outlookCategory** na lista mestra de categorias do usuário.|
|[Listar categorias](../api/outlookuser-list-mastercategories.md) | Coleção [outlookCategory](outlookcategory.md) |Obtém todas as categorias que foram definidas para o usuário.|
|[Criar outlookTaskFolder](../api/outlookuser-post-taskfolders.md) |[outlookTaskFolder](outlooktaskfolder.md)| Crie uma pasta de tarefa no grupo de tarefa padrão (`My Tasks`) da caixa de correio do usuário.|
|[Lista taskFolders](../api/outlookuser-list-taskfolders.md) |coleção [outlookTaskFolder](outlooktaskfolder.md)| Obtenha todas as pastas de tarefas do Outlook na caixa de correio do usuário.|
|[Criar outlookTaskGroup](../api/outlookuser-post-taskgroups.md) |[outlookTaskGroup](outlooktaskgroup.md)| Crie um grupo de tarefas do Outlook na caixa de correio do usuário.|
|[Lista taskGroups](../api/outlookuser-list-taskgroups.md) |coleção [outlookTaskGroup](outlooktaskgroup.md)| Obtenha todos os grupos de tarefas do Outlook na caixa de correio do usuário.|
|[Criar outlookTask](../api/outlookuser-post-tasks.md) |[outlookTask](outlooktask.md)| Criar uma tarefa do Outlook no grupo de tarefa padrão (`My Tasks`) e a pasta de tarefas padrão (`Tasks`) na caixa de correio do usuário.|
|[Listar tarefas](../api/outlookuser-list-tasks.md) |coleção [outlookTask](outlooktask.md)| Obtenha todas as tarefas do Outlook na caixa de correio do usuário.|
|[supportedLanguages](../api/outlookuser-supportedlanguages.md) | Coleção [localeInfo](localeinfo.md) | Obtém a lista de localidades e idiomas com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário. |
|[supportedTimeZones](../api/outlookuser-supportedtimezones.md) | Coleção [timeZoneInformation](timezoneinformation.md) | Obtém a lista de fusos horários com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário. |


## <a name="properties"></a>Propriedades
Nenhum

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|masterCategories|Coleção [outlookCategory](../resources/outlookcategory.md)| Uma lista de categorias definidas para o usuário. | 
|taskFolders|coleção [outlookTaskFolder](outlooktaskfolder.md)| Pastas de tarefas do Outlook do usuário. Somente leitura. Anulável.|
|taskGroups|coleção [outlookTaskGroup](outlooktaskgroup.md)| Grupos de tarefas do Outlook do usuário. Somente leitura. Anulável.|
|tarefas|coleção [outlookTask](outlooktask.md)| Tarefas do Outlook do usuário. Somente leitura. Anulável.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->