---
title: Permissions
description: 'Remova o aplicativo de catálogo de aplicativos da sua organização (o catálogo de aplicativos do inquilino). '
ms.openlocfilehash: c3ee6433f38cfd52548af5ac27f3e3c9891af8d1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040821"
---
# <a name="remove-an-app-from-your-organizations-app-catalog"></a><span data-ttu-id="a1183-103">Remova um aplicativo de catálogo de aplicativos da sua organização</span><span class="sxs-lookup"><span data-stu-id="a1183-103">Remove an app from your organization's app catalog</span></span>

> <span data-ttu-id="a1183-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a1183-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a1183-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a1183-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a1183-106">Remova o [aplicativo](../resources/teamsapp.md) de catálogo de aplicativos da sua organização (o catálogo de aplicativos do inquilino).</span><span class="sxs-lookup"><span data-stu-id="a1183-106">Remove the [app](../resources/teamsapp.md) from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="a1183-107">Para remover o seu aplicativo de catálogo de aplicativos da sua organização, especifique `organization` como o **distributionMethod** no recurso [teamsCatalogApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="a1183-107">To remove your app from your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1183-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="a1183-108">Permissions</span></span>

<span data-ttu-id="a1183-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="a1183-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="a1183-111">**Observação:** Somente os administradores globais podem chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="a1183-111">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="a1183-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1183-112">Permission Type</span></span>                        | <span data-ttu-id="a1183-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a1183-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="a1183-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1183-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="a1183-115">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1183-115">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="a1183-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1183-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1183-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a1183-117">Not supported</span></span>|
| <span data-ttu-id="a1183-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1183-118">Application</span></span>                            | <span data-ttu-id="a1183-119">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a1183-119">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1183-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1183-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a1183-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1183-121">Request headers</span></span>

| <span data-ttu-id="a1183-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a1183-122">Header</span></span>        | <span data-ttu-id="a1183-123">Valor</span><span class="sxs-lookup"><span data-stu-id="a1183-123">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="a1183-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1183-124">Authorization</span></span> | <span data-ttu-id="a1183-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1183-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a1183-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1183-127">Request body</span></span>

<span data-ttu-id="a1183-128">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a1183-128">None.</span></span>

><span data-ttu-id="a1183-129">**Observação:** Use a identificação retornada da chamada [lista publicada apps](./teamsapp-list.md) para referenciar o aplicativo que você gostaria de atualizar.</span><span class="sxs-lookup"><span data-stu-id="a1183-129">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="a1183-130">Não use a ID do manifesto do pacote zip app.</span><span class="sxs-lookup"><span data-stu-id="a1183-130">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="a1183-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1183-131">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="a1183-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1183-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1183-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1183-133">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```

### <a name="response"></a><span data-ttu-id="a1183-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1183-134">Response</span></span>

```http
HTTP/1.1 204 No Content
```
