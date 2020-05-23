---
title: Configurar tipos de guia internos no Microsoft Teams
description: Para criar ou configurar uma guia do Microsoft Teams usando as APIs do Microsoft Graph
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ffe2799f557b12dd72fa72e6bf8b20f72f507647
ms.sourcegitcommit: c1935e442ee973c6c3fcb01a15d76bcfa625362e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2020
ms.locfileid: "44345986"
---
# <a name="configuring-the-built-in-tab-types-in-microsoft-teams"></a>Configurar tipos de guia internos no Microsoft Teams

Para [criar](/graph/api/teamstab-add?view=graph-rest-beta) ou [configurar](/graph/api/teamstab-update?view=graph-rest-beta) uma guia do Microsoft Teams usando as APIs REST do Microsoft Graph, você precisa saber a `teamsAppId` do aplicativo e `entityId`, `contentUrl`, `removeUrl` e `websiteUrl` a fornecer para esse tipo de aplicativo.
Este artigo explica como obter esses valores para os tipos internos de guia.

## <a name="website-tabs"></a>Guias de site

Para as guias de site, o `teamsAppId` é `com.microsoft.teamspace.tab.web`. A configuração é a mostrada a seguir.

| Propriedade   | Tipo        | Descrição                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | Nulo                                                     |
| contentUrl | string      | URL do site                                       |
| removeUrl  | string      | Nulo                                                     |
| websiteUrl | string      | URL do site                                       |

## <a name="word-excel-powerpoint-and-pdf-tabs"></a>Guias do Word, Excel, PowerPoint e PDF

A tabela a seguir lista o `teamsAppId` para cada aplicativo.

| App   | teamsAppId | tipo (extensão)                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| Word | `com.microsoft.teamspace.tab.file.staticviewer.word` | `docx` |
| Excel | `com.microsoft.teamspace.tab.file.staticviewer.excel` | `xlsx` |
| PowerPoint  | `com.microsoft.teamspace.tab.file.staticviewer.powerpoint` | `pptx` |
| PDF | `com.microsoft.teamspace.tab.file.staticviewer.pdf` | `pdf` |

A configuração é a mostrada a seguir.

| Propriedade   | Tipo        | Descrição                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | A ID de sourceDoc do arquivo. Para encontrá-la, abra o arquivo no SharePoint e procure a barra de endereços - a URL terá uma cláusula `sourcedoc=%7B{sourceDocId}%7D`. Você também pode derivar isso na webUrl do item de unidade do SharePoint para o documento. Para saber mais, confira [GET /groups/{group-id}/drive/items/{item-id}](/graph/api/driveitem-get?view=graph-rest-beta). |
| contentUrl | string      | A URL do arquivo no formato `{folder-webUrl}/{item-name}`. {folder-webUrl} é a webUrl da pasta do SharePoint que contém o arquivo. Para localizá-la, abra o arquivo no SharePoint e procure na barra de endereços, ou use a propriedade webUrl em [GET /groups/{group-id}/drive/items/{folder-item-id}](/graph/api/driveitem-get?view=graph-rest-beta). {item-name} é o nome do arquivo (por exemplo, file.docx), que é a propriedade `name` em [GET /groups/{group-id}/drive/items/{item-id}](/graph/api/driveitem-get?view=graph-rest-beta). |
| removeUrl  | string      | Nulo                                                     |
| websiteUrl | string      | Nulo                                       |

### <a name="example-create-a-configured-word-tab"></a>Exemplo: criar uma guia configurada do Word

O exemplo a seguir criar uma guia configurada do Word.

```http
POST https://graph.microsoft.com/v1.0/teams/{team-id}/channels/{channel-id}/tabs
{
  "displayName": "word",
  "teamsApp@odata.bind" : "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/com.microsoft.teamspace.tab.file.staticviewer.word",
  "configuration": {
     "entityId": "115A90F4-AC9C-4F79-9837-36D1EFB3BE08",
     "contentUrl": "https://m365x165177.sharepoint.com/sites/4NewCloneWithClonableParts/Shared%20Documents/General/Employee Handbook.docx",
     "removeUrl": null,
     "websiteUrl": null
  }
}
```
