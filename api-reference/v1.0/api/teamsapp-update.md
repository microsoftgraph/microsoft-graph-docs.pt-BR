---
title: Permissões
description: 'Atualize um aplicativo publicado anteriormente no catálogo de aplicativos do Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a963b2f91c149cef6fd5c291888aa2f6a8bb1ad2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027304"
---
# <a name="update-apps-published-to-your-organizations-app-catalog"></a><span data-ttu-id="56513-103">Atualizar aplicativos publicados no catálogo de aplicativos da sua organização</span><span class="sxs-lookup"><span data-stu-id="56513-103">Update apps published to your organization's app catalog</span></span>



<span data-ttu-id="56513-104">Atualize um [aplicativo](../resources/teamsapp.md) publicado anteriormente no catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="56513-104">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span> <span data-ttu-id="56513-105">Essa API atualiza especificamente um aplicativo publicado no catálogo de aplicativos da sua organização (o catálogo de aplicativos do locatário).</span><span class="sxs-lookup"><span data-stu-id="56513-105">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="56513-106">Para publicar no catálogo de aplicativos da sua organização, `organization` especifique como **DistributionMethod** no recurso [teamsCatalogApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="56513-106">To publish to your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="56513-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="56513-107">Permissions</span></span>

<span data-ttu-id="56513-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="56513-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="56513-110">**Observação:** Somente os administradores globais podem chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="56513-110">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="56513-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56513-111">Permission Type</span></span>                        | <span data-ttu-id="56513-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="56513-112">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="56513-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56513-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="56513-114">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56513-114">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="56513-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56513-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56513-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="56513-116">Not supported</span></span>|
| <span data-ttu-id="56513-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56513-117">Application</span></span>                            | <span data-ttu-id="56513-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="56513-118">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="56513-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56513-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="56513-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56513-120">Request headers</span></span>

| <span data-ttu-id="56513-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="56513-121">Header</span></span>        | <span data-ttu-id="56513-122">Valor</span><span class="sxs-lookup"><span data-stu-id="56513-122">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="56513-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="56513-123">Authorization</span></span> | <span data-ttu-id="56513-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56513-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="56513-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="56513-126">Content-Type</span></span>  | <span data-ttu-id="56513-127">aplicativo/zip</span><span class="sxs-lookup"><span data-stu-id="56513-127">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="56513-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56513-128">Request body</span></span>

<span data-ttu-id="56513-129">Carga do manifesto zip do teams: para o aplicativo do teams arquivo zip [consulte criar um pacote de aplicativos](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="56513-129">Teams Zip Manifest Payload: For Teams application zip file [see Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

><span data-ttu-id="56513-130">**Observação:** Use o ID retornado da [lista de aplicativos publicados](./teamsapp-list.md) chamada para fazer referência ao aplicativo que você deseja atualizar.</span><span class="sxs-lookup"><span data-stu-id="56513-130">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="56513-131">Não use a ID do manifesto do pacote de aplicativos zip.</span><span class="sxs-lookup"><span data-stu-id="56513-131">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="56513-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="56513-132">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="56513-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56513-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="56513-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56513-134">Request</span></span>

```
PUT https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="56513-135">Para o aplicativo do teams arquivo zip [consulte CREATE app Package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="56513-135">For Teams application zip file [see Create app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

### <a name="response"></a><span data-ttu-id="56513-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="56513-136">Response</span></span>

```
HTTP/1.1 204 No Content
```
