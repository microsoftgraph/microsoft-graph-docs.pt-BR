---
title: Permissões
description: 'Atualize um aplicativo publicado anteriormente para o catálogo de aplicativos do Microsoft Teams. '
author: nkramer
ms.openlocfilehash: 60fb80ff6400e7c1d78898b28e3b9f591c01290e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359497"
---
# <a name="update-apps-published-to-your-organizations-app-catalog"></a><span data-ttu-id="a29d2-103">Atualizar aplicativos publicados no catálogo de aplicativos da sua organização</span><span class="sxs-lookup"><span data-stu-id="a29d2-103">Update apps published to your organization's app catalog</span></span>

> <span data-ttu-id="a29d2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a29d2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a29d2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a29d2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a29d2-106">Atualização de um [aplicativo](../resources/teamsapp.md) publicado anteriormente para o catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="a29d2-106">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span> <span data-ttu-id="a29d2-107">Essa API especificamente atualiza um aplicativo publicado no catálogo de aplicativos da sua organização (o catálogo de aplicativos do inquilino).</span><span class="sxs-lookup"><span data-stu-id="a29d2-107">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="a29d2-108">Para publicar o catálogo de aplicativos da sua organização, especifique `organization` como o **distributionMethod** no recurso [teamsCatalogApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="a29d2-108">To publish to your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="a29d2-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="a29d2-109">Permissions</span></span>

<span data-ttu-id="a29d2-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="a29d2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="a29d2-112">**Observação:** Somente os administradores globais podem chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="a29d2-112">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="a29d2-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a29d2-113">Permission Type</span></span>                        | <span data-ttu-id="a29d2-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a29d2-114">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="a29d2-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a29d2-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="a29d2-116">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a29d2-116">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="a29d2-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a29d2-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a29d2-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a29d2-118">Not supported</span></span>|
| <span data-ttu-id="a29d2-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a29d2-119">Application</span></span>                            | <span data-ttu-id="a29d2-120">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a29d2-120">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="a29d2-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a29d2-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a29d2-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a29d2-122">Request headers</span></span>

| <span data-ttu-id="a29d2-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a29d2-123">Header</span></span>        | <span data-ttu-id="a29d2-124">Valor</span><span class="sxs-lookup"><span data-stu-id="a29d2-124">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="a29d2-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a29d2-125">Authorization</span></span> | <span data-ttu-id="a29d2-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a29d2-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a29d2-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a29d2-128">Content-Type</span></span>  | <span data-ttu-id="a29d2-129">aplicativo/zip</span><span class="sxs-lookup"><span data-stu-id="a29d2-129">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="a29d2-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a29d2-130">Request body</span></span>

<span data-ttu-id="a29d2-131">Carga de manifesto de Zip equipes: Para o aplicativo de equipes zip arquivo, [consulte Criar um pacote de aplicativos](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="a29d2-131">Teams Zip Manifest Payload: For Teams application zip file [see Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

><span data-ttu-id="a29d2-132">**Observação:** Use a identificação retornada da chamada [lista publicada apps](./teamsapp-list.md) para referenciar o aplicativo que você gostaria de atualizar.</span><span class="sxs-lookup"><span data-stu-id="a29d2-132">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="a29d2-133">Não use a ID do manifesto do pacote zip app.</span><span class="sxs-lookup"><span data-stu-id="a29d2-133">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="a29d2-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a29d2-134">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="a29d2-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a29d2-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="a29d2-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a29d2-136">Request</span></span>

```
PUT https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="a29d2-137">Para o aplicativo de equipes zip arquivo, [consulte Criar pacote de aplicativos](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="a29d2-137">For Teams application zip file [see Create app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

### <a name="response"></a><span data-ttu-id="a29d2-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a29d2-138">Response</span></span>

```
HTTP/1.1 204 No Content
```
