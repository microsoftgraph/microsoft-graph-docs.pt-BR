---
title: Permissions
description: 'Atualize um aplicativo publicado anteriormente para o catálogo de aplicativos do Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 125d078b5882e08ff5053acee372d8f352f6a2b3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861666"
---
# <a name="update-apps-published-to-your-organizations-app-catalog"></a><span data-ttu-id="408be-103">Atualizar aplicativos publicados no catálogo de aplicativos da sua organização</span><span class="sxs-lookup"><span data-stu-id="408be-103">Update apps published to your organization's app catalog</span></span>

> <span data-ttu-id="408be-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="408be-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="408be-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="408be-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="408be-106">Atualização de um [aplicativo](../resources/teamsapp.md) publicado anteriormente para o catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="408be-106">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span> <span data-ttu-id="408be-107">Essa API especificamente atualiza um aplicativo publicado no catálogo de aplicativos da sua organização (o catálogo de aplicativos do inquilino).</span><span class="sxs-lookup"><span data-stu-id="408be-107">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="408be-108">Para publicar o catálogo de aplicativos da sua organização, especifique `organization` como o **distributionMethod** no recurso [teamsCatalogApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="408be-108">To publish to your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="408be-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="408be-109">Permissions</span></span>

<span data-ttu-id="408be-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="408be-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="408be-112">**Observação:** Somente os administradores globais podem chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="408be-112">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="408be-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="408be-113">Permission Type</span></span>                        | <span data-ttu-id="408be-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="408be-114">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="408be-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="408be-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="408be-116">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="408be-116">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="408be-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="408be-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="408be-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="408be-118">Not supported</span></span>|
| <span data-ttu-id="408be-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="408be-119">Application</span></span>                            | <span data-ttu-id="408be-120">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="408be-120">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="408be-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="408be-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="408be-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="408be-122">Request headers</span></span>

| <span data-ttu-id="408be-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="408be-123">Header</span></span>        | <span data-ttu-id="408be-124">Valor</span><span class="sxs-lookup"><span data-stu-id="408be-124">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="408be-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="408be-125">Authorization</span></span> | <span data-ttu-id="408be-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="408be-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="408be-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="408be-128">Content-Type</span></span>  | <span data-ttu-id="408be-129">aplicativo/zip</span><span class="sxs-lookup"><span data-stu-id="408be-129">application/zip</span></span> |

## <a name="request-body"></a><span data-ttu-id="408be-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="408be-130">Request body</span></span>

<span data-ttu-id="408be-131">Carga de manifesto de Zip equipes: Para o aplicativo de equipes zip arquivo, [consulte Criar um pacote de aplicativos](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="408be-131">Teams Zip Manifest Payload: For Teams application zip file [see Create an app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

><span data-ttu-id="408be-132">**Observação:** Use a identificação retornada da chamada [lista publicada apps](./teamsapp-list.md) para referenciar o aplicativo que você gostaria de atualizar.</span><span class="sxs-lookup"><span data-stu-id="408be-132">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="408be-133">Não use a ID do manifesto do pacote zip app.</span><span class="sxs-lookup"><span data-stu-id="408be-133">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="408be-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="408be-134">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="408be-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="408be-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="408be-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="408be-136">Request</span></span>

```
PUT https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="408be-137">Para o aplicativo de equipes zip arquivo, [consulte Criar pacote de aplicativos](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="408be-137">For Teams application zip file [see Create app package](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/apps/apps-package)</span></span>

### <a name="response"></a><span data-ttu-id="408be-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="408be-138">Response</span></span>

```
HTTP/1.1 204 No Content
```
