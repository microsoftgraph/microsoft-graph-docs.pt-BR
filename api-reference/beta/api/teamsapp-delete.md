---
title: Permissões
description: 'Remova o aplicativo do catálogo de aplicativos da sua organização (o catálogo de aplicativos do locatário). '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 98fd90538619dc3c41c8f48413346266742b404d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452525"
---
# <a name="remove-an-app-from-your-organizations-app-catalog"></a><span data-ttu-id="7fe26-103">Remover um aplicativo do catálogo de aplicativos da sua organização</span><span class="sxs-lookup"><span data-stu-id="7fe26-103">Remove an app from your organization's app catalog</span></span>

<span data-ttu-id="7fe26-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7fe26-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7fe26-105">Remova o [aplicativo](../resources/teamsapp.md) do catálogo de aplicativos da sua organização (o catálogo de aplicativos do locatário).</span><span class="sxs-lookup"><span data-stu-id="7fe26-105">Remove the [app](../resources/teamsapp.md) from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="7fe26-106">Para remover o aplicativo do catálogo de aplicativos da sua organização, `organization` especifique como **DistributionMethod** no recurso [teamsCatalogApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="7fe26-106">To remove your app from your organization's app catalog, specify `organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="7fe26-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="7fe26-107">Permissions</span></span>

<span data-ttu-id="7fe26-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="7fe26-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="7fe26-110">**Observação:** Somente os administradores globais podem chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="7fe26-110">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="7fe26-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7fe26-111">Permission Type</span></span>                        | <span data-ttu-id="7fe26-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7fe26-112">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="7fe26-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7fe26-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="7fe26-114">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7fe26-114">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="7fe26-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7fe26-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7fe26-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7fe26-116">Not supported</span></span>|
| <span data-ttu-id="7fe26-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7fe26-117">Application</span></span>                            | <span data-ttu-id="7fe26-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="7fe26-118">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="7fe26-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7fe26-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /appCatalogs/teamsApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7fe26-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7fe26-120">Request headers</span></span>

| <span data-ttu-id="7fe26-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7fe26-121">Header</span></span>        | <span data-ttu-id="7fe26-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7fe26-122">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="7fe26-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7fe26-123">Authorization</span></span> | <span data-ttu-id="7fe26-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7fe26-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7fe26-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7fe26-126">Request body</span></span>

<span data-ttu-id="7fe26-127">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7fe26-127">None.</span></span>

><span data-ttu-id="7fe26-128">**Observação:** Use o ID retornado da [lista de aplicativos publicados](./teamsapp-list.md) chamada para fazer referência ao aplicativo que você deseja atualizar.</span><span class="sxs-lookup"><span data-stu-id="7fe26-128">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="7fe26-129">Não use a ID do manifesto do pacote de aplicativos zip.</span><span class="sxs-lookup"><span data-stu-id="7fe26-129">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="7fe26-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fe26-130">Response</span></span>

```
HTTP/1.1 204 No Content
```

## <a name="example"></a><span data-ttu-id="7fe26-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7fe26-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7fe26-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7fe26-132">Request</span></span>

```http
DELETE https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```

### <a name="response"></a><span data-ttu-id="7fe26-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="7fe26-133">Response</span></span>

```http
HTTP/1.1 204 No Content
```
