---
title: Configurando os tipos de guia interna no Microsoft Teams
description: 'Para criar ou configurar um Microsoft às equipes guia usando APIs do Microsoft Graph, '
ms.openlocfilehash: 2485e65ebac0c7201fe8b8210f8e4af9b9c8f164
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091593"
---
# <a name="configuring-the-built-in-tab-types-in-microsoft-teams"></a>Configurando os tipos de guia interna no Microsoft Teams

Para [criar](/graph/api/teamstab-add?view=graph-rest-beta) ou [Configurar](/graph/api/teamstab-update?view=graph-rest-beta) uma guia de Teams da Microsoft usando o Microsoft Graph APIs, você precisa saber o `teamsAppId` do aplicativo e o `entityId`, `contentUrl`, `removeUrl`, e `websiteUrl` fornecer para esse tipo de aplicativo.
Este artigo explica como obter esses valores para os tipos de guia interna.

## <a name="custom-tabs"></a>Guias personalizadas

Para usar o Microsoft Graph para configurar uma guia associada a um [provedor de guia](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/tabs/tabs-overview) que você escreveu, identificar o `entityId`, `contentUrl`, `removeUrl`, e `websiteUrl` que do aplicativo [configuração de interface do usuário fornece às equipes da Microsoft](https://docs.microsoft.com/en-us/javascript/api/@microsoft/teams-js/microsoftteams.settings.settings?view=msteams-client-js-latest)e passe a mesma `entityId`, `contentUrl`, `removeUrl`, e `websiteUrl` valores para o Microsoft Graph.

O `teamsAppId` é igual a `id` no [esquema para equipes da Microsoft de manifesto do aplicativo](https://docs.microsoft.com/en-us/microsoftteams/platform/resources/schema/manifest-schema).

## <a name="website-tabs"></a>Guias de site

Para guias de site, o `teamsAppId` é `com.microsoft.teamspace.tab.web`. O seguinte é a configuração.

| Propriedade   | Tipo        | Descrição                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | Nulo                                                     |
| contentUrl | string      | URL do site                                       |
| removeUrl  | string      | Nulo                                                     |
| websiteUrl | string      | URL do site                                       |

## <a name="planner-tabs"></a>Guias de Planejador

Para guias de planejador, o teamsAppId é `com.microsoft.teamspace.tab.planner`. O seguinte é a configuração.

| Propriedade   | Tipo        | Descrição                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | A identificação do plano (o ID a ser usada com GET /planner/planos / {id}).                                              |
| contentUrl | string      | `https://tasks.office.com/{tenantName}/Home/PlannerFrame?page=7&planId={planId}`, onde {tenantName} é o nome do inquilino (por exemplo, example.onmicrosoft.com) e {planId} é o mesmo que a ID de entidade.  |
| removeUrl  | string      | Mesmo valor que o contentUrl.    |
| websiteUrl | string      | Mesmo valor que o contentUrl.   |

Para criar um novo plano para exibir na guia seu planejador, consulte [criar plannerPlan](/graph/api/planner-post-plans?view=graph-rest-beta).

## <a name="microsoft-stream-tabs"></a>Guias de Stream Microsoft

Para guias de Microsoft Stream, o `teamsAppId` é `com.microsoftstream.embed.skypeteamstab`. O seguinte é a configuração.

| Propriedade   | Tipo        | Descrição                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | Nulo                                                     |
| contentUrl | string      | `https://web.microsoftstream.com/embed/video/{id}?autoplay=false&showinfo=true&app=microsoftteams&l={locale}`, onde {id} é a ID do fluxo de vídeo. Para localizar a identificação {} de um stream, abra o fluxo no seu navegador e examinar é a URL – será do formulário `https://{domain}.microsoftstream.com/video/{id}`.  |
| removeUrl  | string      | Nulo                                                     |
| websiteUrl | string      | `https://web.microsoftstream.com/video/{id}`, onde {id} é a ID do fluxo de vídeo.    |

## <a name="microsoft-forms-tabs"></a>Guias do Microsoft Forms

Para guias do Microsoft Forms, o `teamsAppId` é `81fef3a6-72aa-4648-a763-de824aeafb7d`.
Configuração:

| Propriedade   | Tipo        | Descrição                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | A identificação do formulário.  Definir esse valor, navegue até o formulário no site do Forms e encontre a URL do formulário `https://forms.office.com/Pages/DesignPage.aspx#FormId={formId}`.      |
| contentUrl | string      | `https://forms.office.com/Pages/TeamsDesignPage.aspx?Host=Teams&lang={locale}&groupId={groupId}&tid={tid}&teamsTheme={theme}&upn={upn}&fragment=FormId%3D{formId}`, onde {formId} é o mesmo como o ID da entidade e {local}, {groupId}, {tid}, {upn} são literais.   |
| removeUrl  | string      | Nulo                                                     |
| websiteUrl | string      |  `https://forms.office.com`    |

## <a name="word-excel-powerpoint-and-pdf-tabs"></a>Guias PDF, Excel, PowerPoint e Word

A seguinte tabela lista os `teamsAppId` para cada aplicativo.

| App   | teamsAppId | tipo (extensão)                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| Word | `com.microsoft.teamspace.tab.file.staticviewer.word` | `docx` |
| Excel | `com.microsoft.teamspace.tab.file.staticviewer.excel` | `xlsx` |
| PowerPoint  | `com.microsoft.teamspace.tab.file.staticviewer.powerpoint` | `pptx` |
| PDF | `com.microsoft.teamspace.tab.file.staticviewer.pdf` | `pdf` |

Não há suporte para a configuração.

## <a name="wiki-tabs"></a>Guias de wiki

Para guias de wiki, o `teamsAppId` é `com.microsoft.teamspace.tab.wiki`.
Guias de wiki não dão suporte a configuração por meio do gráfico.
No entanto, observe que há muito configurar – na guia wiki não configurados, o primeiro usuário apenas precisa clique em **Configurar a guia** para configurá-la.

## <a name="document-library-tabs"></a>Guias de biblioteca de documentos

Para guias de biblioteca de documentos, o `teamsAppId` é `com.microsoft.teamspace.tab.files.sharepoint`. Não há suporte para a configuração.

## <a name="onenote-tabs"></a>Guias do OneNote

Para guias do OneNote, o `teamsAppId` é `0d820ecd-def2-4297-adad-78056cde7c78`. O seguinte é a configuração.

| Propriedade   | Tipo        | Descrição                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | `{randomGuid}_{notebookId}`, onde {randomGuid} é um GUID que você gerar.                                      |
| contentUrl | string      | Uma URL do formulário `https://www.onenote.com/teams/TabContent?entityid=%7BentityId%7D&subentityid=%7BsubEntityId%7D&auth_upn=%7Bupn%7D&notebookSource=New&notebookSelfUrl=https%3A%2F%2Fwww.onenote.com%2Fapi%2Fv1.0%2FmyOrganization%2Fgroups%2F{sectionsUrl}%2Fnotes%2Fnotebooks%2F{notebookId}&oneNoteWebUrl={oneNoteWebUrl}&notebookName=note&ui={locale}&tenantId={tid}`, onde `{sectionsUrl}`, `{notebookId}`, e `{oneNoteWebUrl}` podem ser encontradas no [obter /groups//onenote/blocos de anotações {id}](/graph/api/onenote-list-notebooks?view=graph-rest-beta). Deve ser precedidas invertida. {local} e {tid} são literais. |
| removeUrl  | string      | Uma URL do formulário `https://www.onenote.com/teams/TabRemove?entityid=%7BentityId%7D&subentityid=%7BsubEntityId%7D&auth_upn=%7Bupn%7D&notebookSource=New&notebookSelfUrl=https%3A%2F%2Fwww.onenote.com%2Fapi%2Fv1.0%2FmyOrganization%2Fgroups%2F{sectionsUrl}%2Fnotes%2Fnotebooks%2F{notebookId}&oneNoteWebUrl={oneNoteWebUrl}&notebookName=note&ui={locale}&tenantId={tid}`, onde `{sectionsUrl}`, `{notebookId}`, e `{oneNoteWebUrl}` podem ser encontradas no [obter /groups//onenote/blocos de anotações {id}](/graph/api/onenote-list-notebooks?view=graph-rest-beta). Deve ser precedidas invertida. {local} e {tid} são literais. |
| websiteUrl | string      | Uma URL do formulário `https://www.onenote.com/teams/TabRedirect?redirectUrl={oneNoteWebUrl}`, onde `oneNoteWebUrl` podem ser encontradas no [obter /groups//onenote/blocos de anotações {id}](/graph/api/onenote-list-notebooks?view=graph-rest-beta) |

## <a name="power-bi-tabs"></a>Guias do Power BI

Para guias de Power BI, o `teamsAppId` é `com.microsoft.teamspace.tab.powerbi`.
Não há suporte para a configuração.

## <a name="sharepoint-page-and-list-tabs"></a>Guias de página e a lista do SharePoint

Para guias de página e lista do SharePoint, o `teamsAppId` é `2a527703-1f6f-4559-a332-d8a7d288cd88`.
Não há suporte para a configuração.
Se a configuração for desejada, considere o uso de uma guia de site.
