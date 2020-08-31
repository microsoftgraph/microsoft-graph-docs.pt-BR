---
title: Tipo de recurso outlookUser
description: Representa os serviços do Outlook disponíveis para um usuário.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 25aae9eeea7c2bf216ec94ffa2f1ac9654e04d79
ms.sourcegitcommit: ae2e4b8963edcdcc8ce572c06a531db4769d7779
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/29/2020
ms.locfileid: "47312107"
---
# <a name="outlookuser-resource-type"></a>Tipo de recurso outlookUser

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [outlooktask-deprecate-sharedfeature](../../includes/outlooktask-deprecate-sharedfeature.md)]

Representa os serviços do Outlook disponíveis para um usuário.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar categoria](../api/outlookuser-post-mastercategories.md) | [outlookCategory](outlookcategory.md) |Cria um objeto **outlookCategory** na lista mestra de categorias do usuário.|
|[Listar categorias](../api/outlookuser-list-mastercategories.md) | Coleção [outlookCategory](outlookcategory.md) |Obtém todas as categorias que foram definidas para o usuário.|
|[supportedLanguages](../api/outlookuser-supportedlanguages.md) | Coleção [localeInfo](localeinfo.md) | Obtém a lista de localidades e idiomas com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário. |
|[supportedTimeZones](../api/outlookuser-supportedtimezones.md) | Coleção [timeZoneInformation](timezoneinformation.md) | Obtém a lista de fusos horários com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário. |
|[Criar outlookTaskFolder](../api/outlookuser-post-taskfolders.md) (preterido) |[outlookTaskFolder](outlooktaskfolder.md)| Crie uma pasta de tarefas no grupo de tarefas padrão ( `My Tasks` ) da caixa de correio do usuário.|
|[Listar taskFolders](../api/outlookuser-list-taskfolders.md) (preterido) |coleção [outlookTaskFolder](outlooktaskfolder.md)| Obter todas as pastas de tarefas do Outlook na caixa de correio do usuário.|
|[Criar outlookTaskGroup](../api/outlookuser-post-taskgroups.md) (preterido) |[outlookTaskGroup](outlooktaskgroup.md)| Criar um grupo de tarefas do Outlook na caixa de correio do usuário.|
|[Listar taskGroups](../api/outlookuser-list-taskgroups.md) (preterido) |coleção [outlookTaskGroup](outlooktaskgroup.md)| Obter todos os grupos de tarefas do Outlook na caixa de correio do usuário.|
|[Criar outlookTask](../api/outlookuser-post-tasks.md) (preterido) |[outlookTask](outlooktask.md)| Crie uma tarefa do Outlook no grupo de tarefas padrão ( `My Tasks` ) e na pasta de tarefas padrão ( `Tasks` ) na caixa de correio do usuário.|
|[Listar tarefas](../api/outlookuser-list-tasks.md) (preterido) |coleção [outlookTask](outlooktask.md)| Obtenha todas as tarefas do Outlook na caixa de correio do usuário.|



## <a name="properties"></a>Propriedades
Nenhuma

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|masterCategories|Coleção [outlookCategory](../resources/outlookcategory.md)| Uma lista de categorias definidas para o usuário. | 
|taskFolders (preterido)|coleção [outlookTaskFolder](outlooktaskfolder.md)| As pastas de tarefas do Outlook do usuário. Somente leitura. Anulável.|
|taskGroups (preterido)|coleção [outlookTaskGroup](outlooktaskgroup.md)| Grupos de tarefas do Outlook do usuário. Somente leitura. Anulável.|
|tarefas (preterido)|coleção [outlookTask](outlooktask.md)| As tarefas do Outlook do usuário. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.outlookUser"
}-->
```json
{  
    "id": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "outlookUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
