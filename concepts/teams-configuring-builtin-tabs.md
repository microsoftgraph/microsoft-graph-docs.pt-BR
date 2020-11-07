---
title: Configurar tipos de guia internos no Microsoft Teams
description: Para criar ou configurar uma guia do Microsoft Teams usando as APIs do Microsoft Graph
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3f1aa2a88a6852e39dbcf791997e19cc214086e1
ms.sourcegitcommit: 5b0b254cc6d8224b3126331eeff6bd0d903e9060
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/07/2020
ms.locfileid: "48945105"
---
# <a name="configuring-the-built-in-tab-types-in-microsoft-teams"></a><span data-ttu-id="d8d14-103">Configurar tipos de guia internos no Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="d8d14-103">Configuring the built-in tab types in Microsoft Teams</span></span>

<span data-ttu-id="d8d14-104">Para [criar](/graph/api/teamstab-add?view=graph-rest-beta) ou [configurar](/graph/api/teamstab-update?view=graph-rest-beta) uma guia do Microsoft Teams usando as APIs REST do Microsoft Graph, você precisa saber a `teamsAppId` do aplicativo e `entityId`, `contentUrl`, `removeUrl` e `websiteUrl` a fornecer para esse tipo de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d8d14-104">To [create](/graph/api/teamstab-add?view=graph-rest-beta) or [configure](/graph/api/teamstab-update?view=graph-rest-beta) a Microsoft Teams tab using Microsoft Graph APIs, you need to know the `teamsAppId` of the app, and the `entityId`, `contentUrl`, `removeUrl`, and `websiteUrl` to provide for that kind of app.</span></span>
<span data-ttu-id="d8d14-105">Este artigo explica como obter esses valores para os tipos internos de guia.</span><span class="sxs-lookup"><span data-stu-id="d8d14-105">This article explains how to get those values for the built-in tab types.</span></span>

## <a name="custom-tabs"></a><span data-ttu-id="d8d14-106">Guias personalizadas</span><span class="sxs-lookup"><span data-stu-id="d8d14-106">Custom tabs</span></span>

<span data-ttu-id="d8d14-107">Para usar o Microsoft Graph para configurar uma guia associada a um [provedor de guia](/microsoftteams/platform/concepts/tabs/tabs-overview) que você escreveu, identifique o `entityId`, o `contentUrl`, o `removeUrl` e o `websiteUrl` que a [interface do usuário de configuração do aplicativo fornece ao Microsoft Teams](/javascript/api/@microsoft/teams-js/microsoftteams.settings.settings?view=msteams-client-js-latest) e passe os mesmos valores de `entityId`, `contentUrl`, `removeUrl`, e `websiteUrl` valores para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d8d14-107">To use Microsoft Graph to configure a tab associated with a [tab provider](/microsoftteams/platform/concepts/tabs/tabs-overview) that you wrote, identify the `entityId`, `contentUrl`, `removeUrl`, and `websiteUrl` that the app's [configuration UI provides to Microsoft Teams](/javascript/api/@microsoft/teams-js/microsoftteams.settings.settings?view=msteams-client-js-latest), and pass the same `entityId`, `contentUrl`, `removeUrl`, and `websiteUrl` values to Microsoft Graph.</span></span>

<span data-ttu-id="d8d14-108">O `teamsAppId` é igual a `id` no [esquema manifesto de aplicativo do Microsoft Teams](/microsoftteams/platform/resources/schema/manifest-schema).</span><span class="sxs-lookup"><span data-stu-id="d8d14-108">The `teamsAppId` is the same as the `id` in the [app manifest schema for Microsoft Teams](/microsoftteams/platform/resources/schema/manifest-schema).</span></span>

## <a name="website-tabs"></a><span data-ttu-id="d8d14-109">Guias de site</span><span class="sxs-lookup"><span data-stu-id="d8d14-109">Website tabs</span></span>

<span data-ttu-id="d8d14-110">Para as guias de site, o `teamsAppId` é `com.microsoft.teamspace.tab.web`.</span><span class="sxs-lookup"><span data-stu-id="d8d14-110">For website tabs, the `teamsAppId` is `com.microsoft.teamspace.tab.web`.</span></span> <span data-ttu-id="d8d14-111">A configuração é a mostrada a seguir.</span><span class="sxs-lookup"><span data-stu-id="d8d14-111">The following is the configuration.</span></span>

| <span data-ttu-id="d8d14-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8d14-112">Property</span></span>   | <span data-ttu-id="d8d14-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8d14-113">Type</span></span>        | <span data-ttu-id="d8d14-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8d14-114">Description</span></span>                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| <span data-ttu-id="d8d14-115">entityId</span><span class="sxs-lookup"><span data-stu-id="d8d14-115">entityId</span></span>   | <span data-ttu-id="d8d14-116">string</span><span class="sxs-lookup"><span data-stu-id="d8d14-116">string</span></span>      | <span data-ttu-id="d8d14-117">Nulo</span><span class="sxs-lookup"><span data-stu-id="d8d14-117">Null</span></span>                                                     |
| <span data-ttu-id="d8d14-118">contentUrl</span><span class="sxs-lookup"><span data-stu-id="d8d14-118">contentUrl</span></span> | <span data-ttu-id="d8d14-119">string</span><span class="sxs-lookup"><span data-stu-id="d8d14-119">string</span></span>      | <span data-ttu-id="d8d14-120">URL do site</span><span class="sxs-lookup"><span data-stu-id="d8d14-120">URL of the website</span></span>                                       |
| <span data-ttu-id="d8d14-121">removeUrl</span><span class="sxs-lookup"><span data-stu-id="d8d14-121">removeUrl</span></span>  | <span data-ttu-id="d8d14-122">string</span><span class="sxs-lookup"><span data-stu-id="d8d14-122">string</span></span>      | <span data-ttu-id="d8d14-123">Nulo</span><span class="sxs-lookup"><span data-stu-id="d8d14-123">Null</span></span>                                                     |
| <span data-ttu-id="d8d14-124">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="d8d14-124">websiteUrl</span></span> | <span data-ttu-id="d8d14-125">string</span><span class="sxs-lookup"><span data-stu-id="d8d14-125">string</span></span>      | <span data-ttu-id="d8d14-126">URL do site</span><span class="sxs-lookup"><span data-stu-id="d8d14-126">URL of the website</span></span>                                       |

## <a name="word-excel-powerpoint-and-pdf-tabs"></a><span data-ttu-id="d8d14-127">Guias do Word, Excel, PowerPoint e PDF</span><span class="sxs-lookup"><span data-stu-id="d8d14-127">Word, Excel, PowerPoint, and PDF tabs</span></span>

<span data-ttu-id="d8d14-128">A tabela a seguir lista o `teamsAppId` para cada aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d8d14-128">The following table lists the `teamsAppId` for each app.</span></span>

| <span data-ttu-id="d8d14-129">App</span><span class="sxs-lookup"><span data-stu-id="d8d14-129">App</span></span>   | <span data-ttu-id="d8d14-130">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="d8d14-130">teamsAppId</span></span> | <span data-ttu-id="d8d14-131">tipo (extensão)</span><span class="sxs-lookup"><span data-stu-id="d8d14-131">type (extension)</span></span>                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| <span data-ttu-id="d8d14-132">Word</span><span class="sxs-lookup"><span data-stu-id="d8d14-132">Word</span></span> | `com.microsoft.teamspace.tab.file.staticviewer.word` | `docx` |
| <span data-ttu-id="d8d14-133">Excel</span><span class="sxs-lookup"><span data-stu-id="d8d14-133">Excel</span></span> | `com.microsoft.teamspace.tab.file.staticviewer.excel` | `xlsx` |
| <span data-ttu-id="d8d14-134">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="d8d14-134">PowerPoint</span></span>  | `com.microsoft.teamspace.tab.file.staticviewer.powerpoint` | `pptx` |
| <span data-ttu-id="d8d14-135">PDF</span><span class="sxs-lookup"><span data-stu-id="d8d14-135">PDF</span></span> | `com.microsoft.teamspace.tab.file.staticviewer.pdf` | `pdf` |

<span data-ttu-id="d8d14-136">A configuração é a mostrada a seguir.</span><span class="sxs-lookup"><span data-stu-id="d8d14-136">The following is the configuration.</span></span>

| <span data-ttu-id="d8d14-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8d14-137">Property</span></span>   | <span data-ttu-id="d8d14-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8d14-138">Type</span></span>        | <span data-ttu-id="d8d14-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8d14-139">Description</span></span>                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| <span data-ttu-id="d8d14-140">entityId</span><span class="sxs-lookup"><span data-stu-id="d8d14-140">entityId</span></span>   | <span data-ttu-id="d8d14-141">string</span><span class="sxs-lookup"><span data-stu-id="d8d14-141">string</span></span>      | <span data-ttu-id="d8d14-142">A ID de sourceDoc do arquivo.</span><span class="sxs-lookup"><span data-stu-id="d8d14-142">The sourceDoc ID of the file.</span></span> <span data-ttu-id="d8d14-143">Para encontrá-la, abra o arquivo no SharePoint e procure a barra de endereços - a URL terá uma cláusula `sourcedoc=%7B{sourceDocId}%7D`.</span><span class="sxs-lookup"><span data-stu-id="d8d14-143">You can find this by opening the file in SharePoint and looking at the address bar – the URL will have a `sourcedoc=%7B{sourceDocId}%7D` clause.</span></span> <span data-ttu-id="d8d14-144">Você também pode derivar isso na webUrl do item de unidade do SharePoint para o documento.</span><span class="sxs-lookup"><span data-stu-id="d8d14-144">You can also derive this from the webUrl of the SharePoint drive item for the document.</span></span> <span data-ttu-id="d8d14-145">Para saber mais, confira [GET /groups/{group-id}/drive/items/{item-id}](/graph/api/driveitem-get?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="d8d14-145">For details, see [GET /groups/{group-id}/drive/items/{item-id}](/graph/api/driveitem-get?view=graph-rest-beta).</span></span> |
| <span data-ttu-id="d8d14-146">contentUrl</span><span class="sxs-lookup"><span data-stu-id="d8d14-146">contentUrl</span></span> | <span data-ttu-id="d8d14-147">string</span><span class="sxs-lookup"><span data-stu-id="d8d14-147">string</span></span>      | <span data-ttu-id="d8d14-148">A URL do arquivo no formato `{folder-webUrl}/{item-name}`.</span><span class="sxs-lookup"><span data-stu-id="d8d14-148">The URL of file in the format `{folder-webUrl}/{item-name}`.</span></span> <span data-ttu-id="d8d14-149">{folder-webUrl} é a webUrl da pasta do SharePoint que contém o arquivo. Para localizá-la, abra o arquivo no SharePoint e procure na barra de endereços, ou use a propriedade webUrl em [GET /groups/{group-id}/drive/items/{folder-item-id}](/graph/api/driveitem-get?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="d8d14-149">{folder-webUrl} is the webUrl of the SharePoint folder containing the file, which can be found by opening the file in SharePoint and looking at the address bar, or by using the webUrl property from [GET /groups/{group-id}/drive/items/{folder-item-id}](/graph/api/driveitem-get?view=graph-rest-beta).</span></span> <span data-ttu-id="d8d14-150">{item-name} é o nome do arquivo (por exemplo, file.docx), que é a propriedade `name` em [GET /groups/{group-id}/drive/items/{item-id}](/graph/api/driveitem-get?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="d8d14-150">{item-name} is the file name (for example, file.docx), which is the `name` property in [GET /groups/{group-id}/drive/items/{item-id}](/graph/api/driveitem-get?view=graph-rest-beta).</span></span> |
| <span data-ttu-id="d8d14-151">removeUrl</span><span class="sxs-lookup"><span data-stu-id="d8d14-151">removeUrl</span></span>  | <span data-ttu-id="d8d14-152">string</span><span class="sxs-lookup"><span data-stu-id="d8d14-152">string</span></span>      | <span data-ttu-id="d8d14-153">Nulo</span><span class="sxs-lookup"><span data-stu-id="d8d14-153">Null</span></span>                                                     |
| <span data-ttu-id="d8d14-154">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="d8d14-154">websiteUrl</span></span> | <span data-ttu-id="d8d14-155">string</span><span class="sxs-lookup"><span data-stu-id="d8d14-155">string</span></span>      | <span data-ttu-id="d8d14-156">Nulo</span><span class="sxs-lookup"><span data-stu-id="d8d14-156">Null</span></span>                                       |

### <a name="example-create-a-configured-word-tab"></a><span data-ttu-id="d8d14-157">Exemplo: criar uma guia configurada do Word</span><span class="sxs-lookup"><span data-stu-id="d8d14-157">Example: Create a configured Word tab</span></span>

<span data-ttu-id="d8d14-158">O exemplo a seguir criar uma guia configurada do Word.</span><span class="sxs-lookup"><span data-stu-id="d8d14-158">The following example creates a configured Word tab.</span></span>

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

## <a name="document-library-tabs"></a><span data-ttu-id="d8d14-159">Guias de biblioteca de documentos</span><span class="sxs-lookup"><span data-stu-id="d8d14-159">Document library tabs</span></span>

<span data-ttu-id="d8d14-160">Para as guias de biblioteca de documentos, o `teamsAppId` é `com.microsoft.teamspace.tab.files.sharepoint`.</span><span class="sxs-lookup"><span data-stu-id="d8d14-160">For document library tabs, the `teamsAppId` is `com.microsoft.teamspace.tab.files.sharepoint`.</span></span> <span data-ttu-id="d8d14-161">A configuração é a mostrada a seguir.</span><span class="sxs-lookup"><span data-stu-id="d8d14-161">The following is the configuration.</span></span>

| <span data-ttu-id="d8d14-162">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8d14-162">Property</span></span>   | <span data-ttu-id="d8d14-163">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8d14-163">Type</span></span>        | <span data-ttu-id="d8d14-164">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8d14-164">Description</span></span>                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| <span data-ttu-id="d8d14-165">entityId</span><span class="sxs-lookup"><span data-stu-id="d8d14-165">entityId</span></span>   | <span data-ttu-id="d8d14-166">string</span><span class="sxs-lookup"><span data-stu-id="d8d14-166">string</span></span>      | <span data-ttu-id="d8d14-167">Cadeia de caracteres vazia ("")</span><span class="sxs-lookup"><span data-stu-id="d8d14-167">Empty string ("")</span></span>                                        |
| <span data-ttu-id="d8d14-168">contentUrl</span><span class="sxs-lookup"><span data-stu-id="d8d14-168">contentUrl</span></span> | <span data-ttu-id="d8d14-169">string</span><span class="sxs-lookup"><span data-stu-id="d8d14-169">string</span></span>      | <span data-ttu-id="d8d14-170">A URL da pasta raiz da biblioteca de documentos.</span><span class="sxs-lookup"><span data-stu-id="d8d14-170">The URL of the root folder of the document library.</span></span> <span data-ttu-id="d8d14-171">Você pode encontrar essa URL abrindo a pasta do SharePoint em seu navegador, copiando a URL e excluindo o "/Forms/AllItems.aspx" e tudo o que quiser.</span><span class="sxs-lookup"><span data-stu-id="d8d14-171">You can find this URL by opening the SharePoint folder in your browser, copying the URL, and deleting "/Forms/AllItems.aspx" and everything after that.</span></span> |
| <span data-ttu-id="d8d14-172">removeUrl</span><span class="sxs-lookup"><span data-stu-id="d8d14-172">removeUrl</span></span>  | <span data-ttu-id="d8d14-173">string</span><span class="sxs-lookup"><span data-stu-id="d8d14-173">string</span></span>      | <span data-ttu-id="d8d14-174">Nulo</span><span class="sxs-lookup"><span data-stu-id="d8d14-174">Null</span></span>                                                     |
| <span data-ttu-id="d8d14-175">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="d8d14-175">websiteUrl</span></span> | <span data-ttu-id="d8d14-176">string</span><span class="sxs-lookup"><span data-stu-id="d8d14-176">string</span></span>      | <span data-ttu-id="d8d14-177">Nulo</span><span class="sxs-lookup"><span data-stu-id="d8d14-177">Null</span></span>                                                     |

### <a name="example-create-a-configured-document-library-tab"></a><span data-ttu-id="d8d14-178">Exemplo: criar uma guia de biblioteca de documentos configurada</span><span class="sxs-lookup"><span data-stu-id="d8d14-178">Example: Create a configured document library tab</span></span>

<span data-ttu-id="d8d14-179">O exemplo a seguir cria uma guia de biblioteca de documentos configurada.</span><span class="sxs-lookup"><span data-stu-id="d8d14-179">The following example creates a configured document library tab.</span></span>

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

## <a name="wiki-tabs"></a><span data-ttu-id="d8d14-180">Guias da wiki</span><span class="sxs-lookup"><span data-stu-id="d8d14-180">Wiki tabs</span></span>

<span data-ttu-id="d8d14-181">Para as guias da wiki, o `teamsAppId` é `com.microsoft.teamspace.tab.wiki`.</span><span class="sxs-lookup"><span data-stu-id="d8d14-181">For wiki tabs, the `teamsAppId` is `com.microsoft.teamspace.tab.wiki`.</span></span>
<span data-ttu-id="d8d14-182">As guias da wiki não dão suporte à configuração por meio do Graph.</span><span class="sxs-lookup"><span data-stu-id="d8d14-182">Wiki tabs do not support configuration through Graph.</span></span>
<span data-ttu-id="d8d14-183">Observe, contudo, que não há muito o que configurar. Em uma guia da wiki não configurada, o primeiro usuário precisa apenas escolher **Configurar guia** para configurá-la.</span><span class="sxs-lookup"><span data-stu-id="d8d14-183">Note, however, that there isn't much to configure -- in an un-configured wiki tab, the first user just needs to select **Set up tab** to configure it.</span></span>

## <a name="planner-tabs"></a><span data-ttu-id="d8d14-184">Guias do Planner</span><span class="sxs-lookup"><span data-stu-id="d8d14-184">Planner tabs</span></span>

<span data-ttu-id="d8d14-185">Para as guias do Planner, o teamsAppId é `com.microsoft.teamspace.tab.planner`.</span><span class="sxs-lookup"><span data-stu-id="d8d14-185">For Planner tabs, the teamsAppId is `com.microsoft.teamspace.tab.planner`.</span></span> <span data-ttu-id="d8d14-186">Essa configuração não é compatível.</span><span class="sxs-lookup"><span data-stu-id="d8d14-186">Configuration is not supported.</span></span>

## <a name="microsoft-stream-tabs"></a><span data-ttu-id="d8d14-187">Guias do Microsoft Stream</span><span class="sxs-lookup"><span data-stu-id="d8d14-187">Microsoft Stream tabs</span></span>

<span data-ttu-id="d8d14-188">Para as guias do Microsoft Stream, o `teamsAppId` é `com.microsoftstream.embed.skypeteamstab`.</span><span class="sxs-lookup"><span data-stu-id="d8d14-188">For Microsoft Stream tabs, the `teamsAppId` is `com.microsoftstream.embed.skypeteamstab`.</span></span> <span data-ttu-id="d8d14-189">Essa configuração não é compatível.</span><span class="sxs-lookup"><span data-stu-id="d8d14-189">Configuration is not supported.</span></span>

## <a name="microsoft-forms-tabs"></a><span data-ttu-id="d8d14-190">Guias do Microsoft Forms</span><span class="sxs-lookup"><span data-stu-id="d8d14-190">Microsoft Forms tabs</span></span>

<span data-ttu-id="d8d14-191">Para as guias do Microsoft Forms, o `teamsAppId` é `81fef3a6-72aa-4648-a763-de824aeafb7d`.</span><span class="sxs-lookup"><span data-stu-id="d8d14-191">For Microsoft Forms tabs, the `teamsAppId` is `81fef3a6-72aa-4648-a763-de824aeafb7d`.</span></span>
<span data-ttu-id="d8d14-192">Essa configuração não é compatível.</span><span class="sxs-lookup"><span data-stu-id="d8d14-192">Configuration is not supported.</span></span>

## <a name="onenote-tabs"></a><span data-ttu-id="d8d14-193">Guias do OneNote</span><span class="sxs-lookup"><span data-stu-id="d8d14-193">OneNote tabs</span></span>

<span data-ttu-id="d8d14-194">Para as guias do OneNote, o `teamsAppId` é `0d820ecd-def2-4297-adad-78056cde7c78`.</span><span class="sxs-lookup"><span data-stu-id="d8d14-194">For OneNote tabs, the `teamsAppId` is `0d820ecd-def2-4297-adad-78056cde7c78`.</span></span> <span data-ttu-id="d8d14-195">Essa configuração não é compatível.</span><span class="sxs-lookup"><span data-stu-id="d8d14-195">Configuration is not supported.</span></span>

## <a name="power-bi-tabs"></a><span data-ttu-id="d8d14-196">Guias do Power BI</span><span class="sxs-lookup"><span data-stu-id="d8d14-196">Power BI tabs</span></span>

<span data-ttu-id="d8d14-197">Para as guias do Power BI, o `teamsAppId` é `com.microsoft.teamspace.tab.powerbi`.</span><span class="sxs-lookup"><span data-stu-id="d8d14-197">For Power BI tabs, the `teamsAppId` is `com.microsoft.teamspace.tab.powerbi`.</span></span>
<span data-ttu-id="d8d14-198">Essa configuração não é compatível.</span><span class="sxs-lookup"><span data-stu-id="d8d14-198">Configuration is not supported.</span></span>

## <a name="sharepoint-page-and-list-tabs"></a><span data-ttu-id="d8d14-199">Guias de lista e de página do SharePoint</span><span class="sxs-lookup"><span data-stu-id="d8d14-199">SharePoint page and list tabs</span></span>

<span data-ttu-id="d8d14-200">Para as guias de lista e de página do SharePoint, o `teamsAppId` é `2a527703-1f6f-4559-a332-d8a7d288cd88`.</span><span class="sxs-lookup"><span data-stu-id="d8d14-200">For SharePoint page and list tabs, the `teamsAppId` is `2a527703-1f6f-4559-a332-d8a7d288cd88`.</span></span>
<span data-ttu-id="d8d14-201">Essa configuração não é compatível.</span><span class="sxs-lookup"><span data-stu-id="d8d14-201">Configuration is not supported.</span></span>
<span data-ttu-id="d8d14-202">Se você quiser configurar a guia, considere usar uma guia do site.</span><span class="sxs-lookup"><span data-stu-id="d8d14-202">If you want to configure the tab, consider using a Website tab.</span></span>
