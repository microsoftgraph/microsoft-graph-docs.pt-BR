---
title: Permissões
description: 'Atualize um aplicativo publicado anteriormente para o catálogo de aplicativos do Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b89380a423bf01f6a2bd7e56086cc9290be094cb
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016622"
---
# <a name="update-apps-published-to-your-organizations-app-catalog"></a><span data-ttu-id="cd620-103">Atualizar aplicativos publicados no catálogo de aplicativos da sua organização</span><span class="sxs-lookup"><span data-stu-id="cd620-103">Update apps published to your organization's app catalog</span></span>



<span data-ttu-id="cd620-104">Atualização de um [aplicativo](../resources/teamsapp.md) publicado anteriormente para o catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="cd620-104">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span> <span data-ttu-id="cd620-105">Essa API especificamente atualiza um aplicativo publicado no catálogo de aplicativos da sua organização (o catálogo de aplicativos do inquilino).</span><span class="sxs-lookup"><span data-stu-id="cd620-105">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="cd620-106">Para publicar o catálogo de aplicativos da sua organização, especifique `organization` como o **distributionMethod** no recurso [teamsCatalogApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="cd620-106">To publish to your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="cd620-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="cd620-107">Permissions</span></span>

<span data-ttu-id="cd620-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="cd620-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="cd620-110">**Observação:** Somente os administradores globais podem chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="cd620-110">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="cd620-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cd620-111">Permission Type</span></span>                        | <span data-ttu-id="cd620-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cd620-112">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="cd620-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cd620-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="cd620-114">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd620-114">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="cd620-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cd620-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd620-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="cd620-116">Not supported</span></span>|
| <span data-ttu-id="cd620-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cd620-117">Application</span></span>                            | <span data-ttu-id="cd620-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="cd620-118">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd620-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cd620-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cd620-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cd620-120">Request headers</span></span>

| <span data-ttu-id="cd620-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cd620-121">Header</span></span>        | <span data-ttu-id="cd620-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cd620-122">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="cd620-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cd620-123">Authorization</span></span> | <span data-ttu-id="cd620-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cd620-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cd620-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cd620-126">Content-Type</span></span>  | <span data-ttu-id="cd620-127">aplicativo/zip</span><span class="sxs-lookup"><span data-stu-id="cd620-127">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="cd620-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cd620-128">Request body</span></span>

<span data-ttu-id="cd620-129">Carga de manifesto de Zip equipes: Para o aplicativo de equipes zip arquivo, [consulte Criar um pacote de aplicativos](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="cd620-129">Teams Zip Manifest Payload: For Teams application zip file [see Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

><span data-ttu-id="cd620-130">**Observação:** Use a identificação retornada da chamada [lista publicada apps](./teamsapp-list.md) para referenciar o aplicativo que você gostaria de atualizar.</span><span class="sxs-lookup"><span data-stu-id="cd620-130">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="cd620-131">Não use a ID do manifesto do pacote zip app.</span><span class="sxs-lookup"><span data-stu-id="cd620-131">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="cd620-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd620-132">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="cd620-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cd620-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd620-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cd620-134">Request</span></span>

```
PUT https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="cd620-135">Para o aplicativo de equipes zip arquivo, [consulte Criar pacote de aplicativos](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="cd620-135">For Teams application zip file [see Create app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

### <a name="response"></a><span data-ttu-id="cd620-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd620-136">Response</span></span>

```
HTTP/1.1 204 No Content
```
