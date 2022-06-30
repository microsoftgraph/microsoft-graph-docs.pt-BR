---
title: Configurar os tipos de guia internos no Microsoft Teams
description: Você pode usar o Microsoft API do Graph para criar uma guia do Microsoft Teams. Saiba como obter a ID do aplicativo e os valores apropriados para os vários tipos de guia internos.
author: nkramer
ms.localizationpriority: medium
ms.prod: microsoft-teams
ms.openlocfilehash: d8d54f864ff9a51cf775bcecdb1569b18cd72af2
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2022
ms.locfileid: "66556154"
---
# <a name="configure-the-built-in-tab-types-in-microsoft-teams"></a>Configurar os tipos de guia internos no Microsoft Teams

Para [criar](/graph/api/channel-post-tabs) ou [configurar](/graph/api/channel-patch-tabs) uma guia do Microsoft Teams usando o Microsoft API do Graph, `teamsAppId` você precisa saber o aplicativo e `entityId``contentUrl`o , , `removeUrl``websiteUrl` e fornecer para esse tipo de aplicativo. Este artigo explica como obter esses valores para os tipos internos de guia.

## <a name="custom-tabs"></a>Guias personalizadas

Para usar o Microsoft Graph para configurar uma guia associada a um [provedor de guia](/microsoftteams/platform/concepts/tabs/tabs-overview) que você escreveu, identifique o `entityId`, o `contentUrl`, o `removeUrl` e o `websiteUrl` que a [interface do usuário de configuração do aplicativo fornece ao Microsoft Teams](/javascript/api/@microsoft/teams-js/microsoftteams.settings.settings?view=msteams-client-js-latest&preserve-view=true) e passe os mesmos valores de `entityId`, `contentUrl`, `removeUrl`, e `websiteUrl` valores para o Microsoft Graph.

O `teamsAppId` é igual a `id` no [esquema manifesto de aplicativo do Microsoft Teams](/microsoftteams/platform/resources/schema/manifest-schema).

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
| entityId   | string      | A ID de sourceDoc do arquivo. Para encontrá-la, abra o arquivo no SharePoint e procure a barra de endereços - a URL terá uma cláusula `sourcedoc=%7B{sourceDocId}%7D`. Você também pode derivar isso na webUrl do item de unidade do SharePoint para o documento. Para saber mais, confira [GET /groups/{group-id}/drive/items/{item-id}](/graph/api/driveitem-get). |
| contentUrl | string      | A URL do arquivo no formato `{folder-webUrl}/{item-name}`. {folder-webUrl} é a webUrl da pasta do SharePoint que contém o arquivo. Para localizá-la, abra o arquivo no SharePoint e procure na barra de endereços, ou use a propriedade webUrl em [GET /groups/{group-id}/drive/items/{folder-item-id}](/graph/api/driveitem-get). {item-name} é o nome do arquivo (por exemplo, file.docx), que é a propriedade `name` em [GET /groups/{group-id}/drive/items/{item-id}](/graph/api/driveitem-get). |
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

## <a name="document-library-tabs"></a>Guias de biblioteca de documentos

Para as guias de biblioteca de documentos, o `teamsAppId` é `com.microsoft.teamspace.tab.files.sharepoint`. A configuração é a mostrada a seguir.

| Propriedade   | Tipo        | Descrição                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | Cadeia de caracteres vazia ("")                                        |
| contentUrl | string      | A URL da pasta raiz da biblioteca de documentos. Você pode encontrar essa URL abrindo a pasta do SharePoint em seu navegador, copiando a URL e excluindo "/Forms/AllItems.aspx" e tudo depois disso. |
| removeUrl  | string      | Nulo                                                     |
| websiteUrl | string      | Nulo                                                     |

### <a name="example-create-a-configured-document-library-tab"></a>Exemplo: criar uma guia de biblioteca de documentos configurada

O exemplo a seguir cria uma guia de biblioteca de documentos configurada.

```http
POST https://graph.microsoft.com/v1.0/teams/{team-id}/channels/{channel-id}/tabs
{
    "displayName": "Document%20Library1",
    "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/com.microsoft.teamspace.tab.files.sharepoint",
    "configuration": {
        "entityId": "",
        "contentUrl": "https://microsoft.sharepoint.com/teams/WWWtest/Shared%20Documents",
        "removeUrl": null,
        "websiteUrl": null
    }
}
```

## <a name="wiki-tabs"></a>Guias da wiki

Para as guias da wiki, o `teamsAppId` é `com.microsoft.teamspace.tab.wiki`.
As guias wiki não dão suporte à configuração por meio do Microsoft Graph.
Observe, no entanto, que não há muito para configurar – em uma guia wiki não configurada, o primeiro usuário só precisa selecionar a guia Configurar para  configurá-la.

## <a name="planner-tabs"></a>Guias do Planner

Para guias do Planner, o `teamsAppId` valor é `com.microsoft.teamspace.tab.planner`. Essa configuração não é compatível.

## <a name="microsoft-stream-tabs"></a>Guias do Microsoft Stream

Para as guias do Microsoft Stream, o `teamsAppId` é `com.microsoftstream.embed.skypeteamstab`. Essa configuração não é compatível.

## <a name="microsoft-forms-tabs"></a>Guias do Microsoft Forms

Para as guias do Microsoft Forms, o `teamsAppId` é `81fef3a6-72aa-4648-a763-de824aeafb7d`.
Essa configuração não é compatível.

## <a name="onenote-tabs"></a>Guias do OneNote

Para as guias do OneNote, o `teamsAppId` é `0d820ecd-def2-4297-adad-78056cde7c78`. Essa configuração não é compatível.

## <a name="power-bi-tabs"></a>Guias do Power BI

Para as guias do Power BI, o `teamsAppId` é `com.microsoft.teamspace.tab.powerbi`.
Essa configuração não é compatível.

## <a name="sharepoint-page-and-list-tabs"></a>Guias de lista e de página do SharePoint

Para as guias de lista e de página do SharePoint, o `teamsAppId` é `2a527703-1f6f-4559-a332-d8a7d288cd88`.
Essa configuração não é compatível.
Se você quiser configurar a guia, considere usar uma guia do site.

## <a name="sharepoint-framework-based-tabs"></a>Estrutura do SharePoint baseadas em Estrutura do SharePoint

Guias personalizadas criadas usando Estrutura do SharePoint podem ser criadas usando o Microsoft Graph, mas não há suporte para configuração.

## <a name="see-also"></a>Confira também

- [Visão geral da API do Microsoft Teams](teams-concept-overview.md)