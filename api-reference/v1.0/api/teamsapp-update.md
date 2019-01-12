---
title: Permissões
description: 'Atualize um aplicativo publicado anteriormente para o catálogo de aplicativos do Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 44ca5870fd585ef7cd5aa0c0282eac42d41c1a18
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948519"
---
# <a name="update-apps-published-to-your-organizations-app-catalog"></a><span data-ttu-id="e1923-103">Atualizar aplicativos publicados no catálogo de aplicativos da sua organização</span><span class="sxs-lookup"><span data-stu-id="e1923-103">Update apps published to your organization's app catalog</span></span>



<span data-ttu-id="e1923-104">Atualização de um [aplicativo](../resources/teamsapp.md) publicado anteriormente para o catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e1923-104">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span> <span data-ttu-id="e1923-105">Essa API especificamente atualiza um aplicativo publicado no catálogo de aplicativos da sua organização (o catálogo de aplicativos do inquilino).</span><span class="sxs-lookup"><span data-stu-id="e1923-105">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="e1923-106">Para publicar o catálogo de aplicativos da sua organização, especifique `organization` como o **distributionMethod** no recurso [teamsCatalogApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="e1923-106">To publish to your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1923-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="e1923-107">Permissions</span></span>

<span data-ttu-id="e1923-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="e1923-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="e1923-110">**Observação:** Somente os administradores globais podem chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="e1923-110">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="e1923-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1923-111">Permission Type</span></span>                        | <span data-ttu-id="e1923-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e1923-112">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="e1923-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1923-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="e1923-114">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1923-114">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="e1923-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1923-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1923-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e1923-116">Not supported</span></span>|
| <span data-ttu-id="e1923-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1923-117">Application</span></span>                            | <span data-ttu-id="e1923-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e1923-118">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1923-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1923-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e1923-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1923-120">Request headers</span></span>

| <span data-ttu-id="e1923-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e1923-121">Header</span></span>        | <span data-ttu-id="e1923-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e1923-122">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="e1923-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1923-123">Authorization</span></span> | <span data-ttu-id="e1923-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1923-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e1923-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e1923-126">Content-Type</span></span>  | <span data-ttu-id="e1923-127">aplicativo/zip</span><span class="sxs-lookup"><span data-stu-id="e1923-127">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1923-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1923-128">Request body</span></span>

<span data-ttu-id="e1923-129">Carga de manifesto de Zip equipes: Para o aplicativo de equipes zip arquivo, [consulte Criar um pacote de aplicativos](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="e1923-129">Teams Zip Manifest Payload: For Teams application zip file [see Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

><span data-ttu-id="e1923-130">**Observação:** Use a identificação retornada da chamada [lista publicada apps](./teamsapp-list.md) para referenciar o aplicativo que você gostaria de atualizar.</span><span class="sxs-lookup"><span data-stu-id="e1923-130">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="e1923-131">Não use a ID do manifesto do pacote zip app.</span><span class="sxs-lookup"><span data-stu-id="e1923-131">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="e1923-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1923-132">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="e1923-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1923-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1923-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1923-134">Request</span></span>

```
PUT https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="e1923-135">Para o aplicativo de equipes zip arquivo, [consulte Criar pacote de aplicativos](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="e1923-135">For Teams application zip file [see Create app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

### <a name="response"></a><span data-ttu-id="e1923-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1923-136">Response</span></span>

```
HTTP/1.1 204 No Content
```
