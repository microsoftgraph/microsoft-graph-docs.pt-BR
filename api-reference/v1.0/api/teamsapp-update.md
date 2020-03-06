---
title: Permissões
description: 'Atualize um aplicativo publicado anteriormente no catálogo de aplicativos do Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: cf0111d656ea4d16b20ed28ef5d033396a878307
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509311"
---
# <a name="update-apps-published-to-your-organizations-app-catalog"></a><span data-ttu-id="e75c6-103">Atualizar aplicativos publicados no catálogo de aplicativos da sua organização</span><span class="sxs-lookup"><span data-stu-id="e75c6-103">Update apps published to your organization's app catalog</span></span>

<span data-ttu-id="e75c6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e75c6-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="e75c6-105">Atualize um [aplicativo](../resources/teamsapp.md) publicado anteriormente no catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e75c6-105">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span>
<span data-ttu-id="e75c6-106">Essa API atualiza especificamente um aplicativo publicado no catálogo de aplicativos da sua organização (o catálogo de aplicativos do locatário).</span><span class="sxs-lookup"><span data-stu-id="e75c6-106">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span>
<span data-ttu-id="e75c6-107">Para publicar no catálogo de aplicativos da sua organização, `organization` especifique como **DistributionMethod** no recurso [teamsCatalogApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="e75c6-107">To publish to your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="e75c6-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="e75c6-108">Permissions</span></span>

<span data-ttu-id="e75c6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="e75c6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="e75c6-111">**Observação:** Somente os administradores globais podem chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="e75c6-111">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="e75c6-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e75c6-112">Permission Type</span></span>                        | <span data-ttu-id="e75c6-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e75c6-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="e75c6-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e75c6-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="e75c6-115">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e75c6-115">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="e75c6-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e75c6-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e75c6-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e75c6-117">Not supported</span></span>|
| <span data-ttu-id="e75c6-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e75c6-118">Application</span></span>                            | <span data-ttu-id="e75c6-119">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e75c6-119">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="e75c6-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e75c6-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e75c6-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e75c6-121">Request headers</span></span>

| <span data-ttu-id="e75c6-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e75c6-122">Header</span></span>        | <span data-ttu-id="e75c6-123">Valor</span><span class="sxs-lookup"><span data-stu-id="e75c6-123">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="e75c6-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="e75c6-124">Authorization</span></span> | <span data-ttu-id="e75c6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e75c6-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e75c6-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e75c6-127">Content-Type</span></span>  | <span data-ttu-id="e75c6-128">aplicativo/zip</span><span class="sxs-lookup"><span data-stu-id="e75c6-128">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="e75c6-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e75c6-129">Request body</span></span>

<span data-ttu-id="e75c6-130">Carga do manifesto zip do teams: para o aplicativo do teams arquivo zip [consulte criar um pacote de aplicativos](/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="e75c6-130">Teams Zip Manifest Payload: For Teams application zip file [see Create an app package](/microsoftteams/platform/concepts/apps/apps-package)</span></span>

><span data-ttu-id="e75c6-131">**Observação:** Use o ID retornado da [lista de aplicativos publicados](./teamsapp-list.md) chamada para fazer referência ao aplicativo que você deseja atualizar.</span><span class="sxs-lookup"><span data-stu-id="e75c6-131">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span>
<span data-ttu-id="e75c6-132">Não use a ID do manifesto do pacote de aplicativos zip.</span><span class="sxs-lookup"><span data-stu-id="e75c6-132">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="e75c6-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e75c6-133">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="e75c6-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e75c6-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="e75c6-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e75c6-135">Request</span></span>

```
PUT https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="e75c6-136">Para o aplicativo do teams arquivo zip [consulte CREATE app Package](/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="e75c6-136">For Teams application zip file [see Create app package](/microsoftteams/platform/concepts/apps/apps-package)</span></span>

### <a name="response"></a><span data-ttu-id="e75c6-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e75c6-137">Response</span></span>

```
HTTP/1.1 204 No Content
```
