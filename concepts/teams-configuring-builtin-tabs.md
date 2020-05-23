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
# <a name="configuring-the-built-in-tab-types-in-microsoft-teams"></a><span data-ttu-id="5dcf5-103">Configurar tipos de guia internos no Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="5dcf5-103">Configuring the built-in tab types in Microsoft Teams</span></span>

<span data-ttu-id="5dcf5-104">Para [criar](/graph/api/teamstab-add?view=graph-rest-beta) ou [configurar](/graph/api/teamstab-update?view=graph-rest-beta) uma guia do Microsoft Teams usando as APIs REST do Microsoft Graph, você precisa saber a `teamsAppId` do aplicativo e `entityId`, `contentUrl`, `removeUrl` e `websiteUrl` a fornecer para esse tipo de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5dcf5-104">To [create](/graph/api/teamstab-add?view=graph-rest-beta) or [configure](/graph/api/teamstab-update?view=graph-rest-beta) a Microsoft Teams tab using Microsoft Graph APIs, you need to know the `teamsAppId` of the app, and the `entityId`, `contentUrl`, `removeUrl`, and `websiteUrl` to provide for that kind of app.</span></span>
<span data-ttu-id="5dcf5-105">Este artigo explica como obter esses valores para os tipos internos de guia.</span><span class="sxs-lookup"><span data-stu-id="5dcf5-105">This article explains how to get those values for the built-in tab types.</span></span>

## <a name="website-tabs"></a><span data-ttu-id="5dcf5-106">Guias de site</span><span class="sxs-lookup"><span data-stu-id="5dcf5-106">Website tabs</span></span>

<span data-ttu-id="5dcf5-107">Para as guias de site, o `teamsAppId` é `com.microsoft.teamspace.tab.web`.</span><span class="sxs-lookup"><span data-stu-id="5dcf5-107">For website tabs, the `teamsAppId` is `com.microsoft.teamspace.tab.web`.</span></span> <span data-ttu-id="5dcf5-108">A configuração é a mostrada a seguir.</span><span class="sxs-lookup"><span data-stu-id="5dcf5-108">The following is the configuration.</span></span>

| <span data-ttu-id="5dcf5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5dcf5-109">Property</span></span>   | <span data-ttu-id="5dcf5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5dcf5-110">Type</span></span>        | <span data-ttu-id="5dcf5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5dcf5-111">Description</span></span>                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| <span data-ttu-id="5dcf5-112">entityId</span><span class="sxs-lookup"><span data-stu-id="5dcf5-112">entityId</span></span>   | <span data-ttu-id="5dcf5-113">string</span><span class="sxs-lookup"><span data-stu-id="5dcf5-113">string</span></span>      | <span data-ttu-id="5dcf5-114">Nulo</span><span class="sxs-lookup"><span data-stu-id="5dcf5-114">Null</span></span>                                                     |
| <span data-ttu-id="5dcf5-115">contentUrl</span><span class="sxs-lookup"><span data-stu-id="5dcf5-115">contentUrl</span></span> | <span data-ttu-id="5dcf5-116">string</span><span class="sxs-lookup"><span data-stu-id="5dcf5-116">string</span></span>      | <span data-ttu-id="5dcf5-117">URL do site</span><span class="sxs-lookup"><span data-stu-id="5dcf5-117">URL of the website</span></span>                                       |
| <span data-ttu-id="5dcf5-118">removeUrl</span><span class="sxs-lookup"><span data-stu-id="5dcf5-118">removeUrl</span></span>  | <span data-ttu-id="5dcf5-119">string</span><span class="sxs-lookup"><span data-stu-id="5dcf5-119">string</span></span>      | <span data-ttu-id="5dcf5-120">Nulo</span><span class="sxs-lookup"><span data-stu-id="5dcf5-120">Null</span></span>                                                     |
| <span data-ttu-id="5dcf5-121">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="5dcf5-121">websiteUrl</span></span> | <span data-ttu-id="5dcf5-122">string</span><span class="sxs-lookup"><span data-stu-id="5dcf5-122">string</span></span>      | <span data-ttu-id="5dcf5-123">URL do site</span><span class="sxs-lookup"><span data-stu-id="5dcf5-123">URL of the website</span></span>                                       |

## <a name="word-excel-powerpoint-and-pdf-tabs"></a><span data-ttu-id="5dcf5-124">Guias do Word, Excel, PowerPoint e PDF</span><span class="sxs-lookup"><span data-stu-id="5dcf5-124">Word, Excel, PowerPoint, and PDF tabs</span></span>

<span data-ttu-id="5dcf5-125">A tabela a seguir lista o `teamsAppId` para cada aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5dcf5-125">The following table lists the `teamsAppId` for each app.</span></span>

| <span data-ttu-id="5dcf5-126">App</span><span class="sxs-lookup"><span data-stu-id="5dcf5-126">App</span></span>   | <span data-ttu-id="5dcf5-127">teamsAppId</span><span class="sxs-lookup"><span data-stu-id="5dcf5-127">teamsAppId</span></span> | <span data-ttu-id="5dcf5-128">tipo (extensão)</span><span class="sxs-lookup"><span data-stu-id="5dcf5-128">type (extension)</span></span>                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| <span data-ttu-id="5dcf5-129">Word</span><span class="sxs-lookup"><span data-stu-id="5dcf5-129">Word</span></span> | `com.microsoft.teamspace.tab.file.staticviewer.word` | `docx` |
| <span data-ttu-id="5dcf5-130">Excel</span><span class="sxs-lookup"><span data-stu-id="5dcf5-130">Excel</span></span> | `com.microsoft.teamspace.tab.file.staticviewer.excel` | `xlsx` |
| <span data-ttu-id="5dcf5-131">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="5dcf5-131">PowerPoint</span></span>  | `com.microsoft.teamspace.tab.file.staticviewer.powerpoint` | `pptx` |
| <span data-ttu-id="5dcf5-132">PDF</span><span class="sxs-lookup"><span data-stu-id="5dcf5-132">PDF</span></span> | `com.microsoft.teamspace.tab.file.staticviewer.pdf` | `pdf` |

<span data-ttu-id="5dcf5-133">A configuração é a mostrada a seguir.</span><span class="sxs-lookup"><span data-stu-id="5dcf5-133">The following is the configuration.</span></span>

| <span data-ttu-id="5dcf5-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5dcf5-134">Property</span></span>   | <span data-ttu-id="5dcf5-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="5dcf5-135">Type</span></span>        | <span data-ttu-id="5dcf5-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="5dcf5-136">Description</span></span>                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| <span data-ttu-id="5dcf5-137">entityId</span><span class="sxs-lookup"><span data-stu-id="5dcf5-137">entityId</span></span>   | <span data-ttu-id="5dcf5-138">string</span><span class="sxs-lookup"><span data-stu-id="5dcf5-138">string</span></span>      | <span data-ttu-id="5dcf5-139">A ID de sourceDoc do arquivo.</span><span class="sxs-lookup"><span data-stu-id="5dcf5-139">The sourceDoc ID of the file.</span></span> <span data-ttu-id="5dcf5-140">Para encontrá-la, abra o arquivo no SharePoint e procure a barra de endereços - a URL terá uma cláusula `sourcedoc=%7B{sourceDocId}%7D`.</span><span class="sxs-lookup"><span data-stu-id="5dcf5-140">You can find this by opening the file in SharePoint and looking at the address bar – the URL will have a `sourcedoc=%7B{sourceDocId}%7D` clause.</span></span> <span data-ttu-id="5dcf5-141">Você também pode derivar isso na webUrl do item de unidade do SharePoint para o documento.</span><span class="sxs-lookup"><span data-stu-id="5dcf5-141">You can also derive this from the webUrl of the SharePoint drive item for the document.</span></span> <span data-ttu-id="5dcf5-142">Para saber mais, confira [GET /groups/{group-id}/drive/items/{item-id}](/graph/api/driveitem-get?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="5dcf5-142">For details, see [GET /groups/{group-id}/drive/items/{item-id}](/graph/api/driveitem-get?view=graph-rest-beta).</span></span> |
| <span data-ttu-id="5dcf5-143">contentUrl</span><span class="sxs-lookup"><span data-stu-id="5dcf5-143">contentUrl</span></span> | <span data-ttu-id="5dcf5-144">string</span><span class="sxs-lookup"><span data-stu-id="5dcf5-144">string</span></span>      | <span data-ttu-id="5dcf5-145">A URL do arquivo no formato `{folder-webUrl}/{item-name}`.</span><span class="sxs-lookup"><span data-stu-id="5dcf5-145">The URL of file in the format `{folder-webUrl}/{item-name}`.</span></span> <span data-ttu-id="5dcf5-146">{folder-webUrl} é a webUrl da pasta do SharePoint que contém o arquivo. Para localizá-la, abra o arquivo no SharePoint e procure na barra de endereços, ou use a propriedade webUrl em [GET /groups/{group-id}/drive/items/{folder-item-id}](/graph/api/driveitem-get?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="5dcf5-146">{folder-webUrl} is the webUrl of the SharePoint folder containing the file, which can be found by opening the file in SharePoint and looking at the address bar, or by using the webUrl property from [GET /groups/{group-id}/drive/items/{folder-item-id}](/graph/api/driveitem-get?view=graph-rest-beta).</span></span> <span data-ttu-id="5dcf5-147">{item-name} é o nome do arquivo (por exemplo, file.docx), que é a propriedade `name` em [GET /groups/{group-id}/drive/items/{item-id}](/graph/api/driveitem-get?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="5dcf5-147">{item-name} is the file name (for example, file.docx), which is the `name` property in [GET /groups/{group-id}/drive/items/{item-id}](/graph/api/driveitem-get?view=graph-rest-beta).</span></span> |
| <span data-ttu-id="5dcf5-148">removeUrl</span><span class="sxs-lookup"><span data-stu-id="5dcf5-148">removeUrl</span></span>  | <span data-ttu-id="5dcf5-149">string</span><span class="sxs-lookup"><span data-stu-id="5dcf5-149">string</span></span>      | <span data-ttu-id="5dcf5-150">Nulo</span><span class="sxs-lookup"><span data-stu-id="5dcf5-150">Null</span></span>                                                     |
| <span data-ttu-id="5dcf5-151">websiteUrl</span><span class="sxs-lookup"><span data-stu-id="5dcf5-151">websiteUrl</span></span> | <span data-ttu-id="5dcf5-152">string</span><span class="sxs-lookup"><span data-stu-id="5dcf5-152">string</span></span>      | <span data-ttu-id="5dcf5-153">Nulo</span><span class="sxs-lookup"><span data-stu-id="5dcf5-153">Null</span></span>                                       |

### <a name="example-create-a-configured-word-tab"></a><span data-ttu-id="5dcf5-154">Exemplo: criar uma guia configurada do Word</span><span class="sxs-lookup"><span data-stu-id="5dcf5-154">Example: Create a configured Word tab</span></span>

<span data-ttu-id="5dcf5-155">O exemplo a seguir criar uma guia configurada do Word.</span><span class="sxs-lookup"><span data-stu-id="5dcf5-155">The following example creates a configured Word tab.</span></span>

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
