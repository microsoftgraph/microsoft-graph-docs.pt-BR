---
title: Configurar tipos de guia internos no Microsoft Teams
description: Para criar ou configurar uma guia do Microsoft Teams usando as APIs do Microsoft Graph
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2940edf1cef2adc6c240fe8dd737d91f434c27e8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574593"
---
# <a name="configuring-the-built-in-tab-types-in-microsoft-teams"></a>Configurar tipos de guia internos no Microsoft Teams

Para [criar](/graph/api/teamstab-add?view=graph-rest-beta) ou [configurar](/graph/api/teamstab-update?view=graph-rest-beta) uma guia do Microsoft Teams usando as APIs REST do Microsoft Graph, você precisa saber a `teamsAppId` do aplicativo e `entityId`, `contentUrl`, `removeUrl` e `websiteUrl` a fornecer para esse tipo de aplicativo.
Este artigo explica como obter esses valores para os tipos internos de guia.

## <a name="custom-tabs"></a>Guias personalizadas

Para usar o Microsoft Graph para configurar uma guia associada a um [provedor de guia](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/tabs/tabs-overview) que você escreveu, identifique o `entityId`, o `contentUrl`, o `removeUrl` e o `websiteUrl` que a [interface do usuário de configuração do aplicativo fornece ao Microsoft Teams](https://docs.microsoft.com/en-us/javascript/api/@microsoft/teams-js/microsoftteams.settings.settings?view=msteams-client-js-latest) e passe os mesmos valores de `entityId`, `contentUrl`, `removeUrl`, e `websiteUrl` valores para o Microsoft Graph.

O `teamsAppId` é igual a `id` no [esquema manifesto de aplicativo do Microsoft Teams](https://docs.microsoft.com/en-us/microsoftteams/platform/resources/schema/manifest-schema).

## <a name="website-tabs"></a>Guias de site

Para as guias de site, o `teamsAppId` é `com.microsoft.teamspace.tab.web`. A configuração é a mostrada a seguir.

| Propriedade   | Tipo        | Descrição                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | Nulo                                                     |
| contentUrl | string      | URL do site                                       |
| removeUrl  | string      | Nulo                                                     |
| websiteUrl | string      | URL do site                                       |

## <a name="planner-tabs"></a>Guias do Planner

Para as guias do Planner, o teamsAppId é `com.microsoft.teamspace.tab.planner`. A configuração é a mostrada a seguir.

| Propriedade   | Tipo        | Descrição                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | A ID do plano (a ID a usar com GET /planner/plans/{id}).                                              |
| contentUrl | string      | `https://tasks.office.com/{tenantName}/Home/PlannerFrame?page=7&planId={planId}`, em que {tenantName} é o nome do locatário (por exemplo, exemplo.onmicrosoft.com) e {planId} é igual a ID da entidade.  |
| removeUrl  | string      | O mesmo valor que a contentUrl.    |
| websiteUrl | string      | O mesmo valor que a contentUrl.   |

Para criar um novo plano para exibir na guia do Planner, veja [criar plannerPlan](/graph/api/planner-post-plans?view=graph-rest-beta).

## <a name="microsoft-stream-tabs"></a>Guias do Microsoft Stream

Para as guias do Microsoft Stream, o `teamsAppId` é `com.microsoftstream.embed.skypeteamstab`. A configuração é a mostrada a seguir.

| Propriedade   | Tipo        | Descrição                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | Nulo                                                     |
| contentUrl | string      | `https://web.microsoftstream.com/embed/video/{id}?autoplay=false&showinfo=true&app=microsoftteams&l={locale}`, em que {id} é a ID do fluxo de vídeo. Para encontrar a {id} de um fluxo, abra o fluxo em seu navegador e veja a URL, que será no formato `https://{domain}.microsoftstream.com/video/{id}`.  |
| removeUrl  | string      | Nulo                                                     |
| websiteUrl | string      | `https://web.microsoftstream.com/video/{id}`, em que {id} é a ID do fluxo de vídeo.    |

## <a name="microsoft-forms-tabs"></a>Guias do Microsoft Forms

Para as guias do Microsoft Forms, o `teamsAppId` é `81fef3a6-72aa-4648-a763-de824aeafb7d`.
A configuração é a mostrada a seguir.

| Propriedade   | Tipo        | Descrição                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | A ID do formulário.  Defina esse valor, navegue até o formulário no site do Forms e encontre a URL no formato `https://forms.office.com/Pages/DesignPage.aspx#FormId={formId}`.      |
| contentUrl | string      | `https://forms.office.com/Pages/TeamsDesignPage.aspx?Host=Teams&lang={locale}&groupId={groupId}&tid={tid}&teamsTheme={theme}&upn={upn}&fragment=FormId%3D{formId}`, em que é {formId} o mesmo que a ID da entidade e {locale}, {groupId}, {tid} e {upn} são literais.   |
| removeUrl  | string      | Nulo                                                     |
| websiteUrl | string      |  `https://forms.office.com`    |

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
  "teamsApp@odata.bind" : "https://graph.microsoft.com/beta/appCatalogs/teamsApps/com.microsoft.teamspace.tab.file.staticviewer.word",
  "configuration": {
     "entityId": "115A90F4-AC9C-4F79-9837-36D1EFB3BE08",
     "contentUrl": "https://m365x165177.sharepoint.com/sites/4NewCloneWithClonableParts/Shared%20Documents/General/Employee Handbook.docx",
     "removeUrl": null,
     "websiteUrl": null
  }
}
```

## <a name="wiki-tabs"></a>Guias da wiki

Para as guias da wiki, o `teamsAppId` é `com.microsoft.teamspace.tab.wiki`.
As guias da wiki não dão suporte à configuração por meio do Graph.
Observe, contudo, que não há muito o que configurar. Em uma guia da wiki não configurada, o primeiro usuário precisa apenas escolher **Configurar guia** para configurá-la.

## <a name="document-library-tabs"></a>Guias de biblioteca de documentos

Para as guias de biblioteca de documentos, o `teamsAppId` é `com.microsoft.teamspace.tab.files.sharepoint`. A configuração é a mostrada a seguir.

| Propriedade   | Tipo        | Descrição                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | Cadeia de caracteres vazia ("")                                        |
| contentUrl | string      | A URL da pasta raiz da biblioteca de documentos. Você pode encontrar essa URL abrindo a pasta do SharePoint em seu navegador, copiando a URL e excluindo o "/Forms/AllItems.aspx" e tudo o que quiser. |
| removeUrl  | string      | Nulo                                                     |
| websiteUrl | string      | Nulo                                                     |

### <a name="example-create-a-configured-document-library-tab"></a>Exemplo: criar uma guia de biblioteca de documentos configurada

O exemplo a seguir criar uma guia configurada do Word.

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

## <a name="onenote-tabs"></a>Guias do OneNote

Para as guias do OneNote, o `teamsAppId` é `0d820ecd-def2-4297-adad-78056cde7c78`. A configuração é a mostrada a seguir.

| Propriedade   | Tipo        | Descrição                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | `{randomGuid}_{notebookId}`, em que {randomGuid} é um GUID que você gera.                                      |
| contentUrl | string      | Uma URL no formato `https://www.onenote.com/teams/TabContent?entityid=%7BentityId%7D&subentityid=%7BsubEntityId%7D&auth_upn=%7Bupn%7D&notebookSource=New&notebookSelfUrl=https%3A%2F%2Fwww.onenote.com%2Fapi%2Fv1.0%2FmyOrganization%2Fgroups%2F{sectionsUrl}%2Fnotes%2Fnotebooks%2F{notebookId}&oneNoteWebUrl={oneNoteWebUrl}&notebookName=note&ui={locale}&tenantId={tid}`, em que `{sectionsUrl}`, `{notebookId}` e `{oneNoteWebUrl}` podem ser encontradas em [GET /groups/{id}/onenote/notebooks](/graph/api/onenote-list-notebooks?view=graph-rest-beta). Barras invertidas devem conter sequências de escape. {locale} e {tid} são literais. |
| removeUrl  | string      | Uma URL no formato `https://www.onenote.com/teams/TabRemove?entityid=%7BentityId%7D&subentityid=%7BsubEntityId%7D&auth_upn=%7Bupn%7D&notebookSource=New&notebookSelfUrl=https%3A%2F%2Fwww.onenote.com%2Fapi%2Fv1.0%2FmyOrganization%2Fgroups%2F{sectionsUrl}%2Fnotes%2Fnotebooks%2F{notebookId}&oneNoteWebUrl={oneNoteWebUrl}&notebookName=note&ui={locale}&tenantId={tid}`, em que `{sectionsUrl}`, `{notebookId}` e `{oneNoteWebUrl}` podem ser encontradas em [GET /groups/{id}/onenote/notebooks](/graph/api/onenote-list-notebooks?view=graph-rest-beta). Barras invertidas devem conter sequências de escape. {locale} e {tid} são literais. |
| websiteUrl | string      | Uma URL no formato `https://www.onenote.com/teams/TabRedirect?redirectUrl={oneNoteWebUrl}`, em que `oneNoteWebUrl` pode ser encontrado em [GET /groups/{id}/onenote/notebooks](/graph/api/onenote-list-notebooks?view=graph-rest-beta) |

## <a name="power-bi-tabs"></a>Guias do Power BI

Para as guias do Power BI, o `teamsAppId` é `com.microsoft.teamspace.tab.powerbi`.
Essa configuração não é compatível.

## <a name="sharepoint-page-and-list-tabs"></a>Guias de lista e de página do SharePoint

Para as guias de lista e de página do SharePoint, o `teamsAppId` é `2a527703-1f6f-4559-a332-d8a7d288cd88`.
Essa configuração não é compatível.
Se você quiser configurar a guia, considere usar uma guia do site.
