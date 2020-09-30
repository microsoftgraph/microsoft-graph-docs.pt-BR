---
title: Excluir teamsApp
description: 'Remover um aplicativo do teams do catálogo de aplicativos de uma organização (o catálogo de aplicativos do locatário). '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5077d7f2a55f9ad6d3382ab3fc65af5f12260c4f
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48315553"
---
# <a name="delete-teamsapp"></a><span data-ttu-id="3801e-103">Excluir teamsApp</span><span class="sxs-lookup"><span data-stu-id="3801e-103">Delete teamsApp</span></span>

<span data-ttu-id="3801e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3801e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<!-- markdownlint-disable MD001 -->

<span data-ttu-id="3801e-105">Excluir um [aplicativo](../resources/teamsapp.md) do catálogo de aplicativos de uma organização (o catálogo de aplicativos do locatário).</span><span class="sxs-lookup"><span data-stu-id="3801e-105">Delete an [app](../resources/teamsapp.md) from an organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="3801e-106">Para excluir um aplicativo, a propriedade **distributionMethod** para o aplicativo deve ser definida como `organization` .</span><span class="sxs-lookup"><span data-stu-id="3801e-106">To delete an app, the **distributionMethod** property for the app must be set to `organization`.</span></span>

<span data-ttu-id="3801e-107">Você também pode usar essa API para remover um aplicativo enviado do processo de revisão.</span><span class="sxs-lookup"><span data-stu-id="3801e-107">You can also use this API to remove a submitted app from the review process.</span></span>

## <a name="permissions"></a><span data-ttu-id="3801e-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="3801e-108">Permissions</span></span>

<span data-ttu-id="3801e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3801e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="3801e-111">**Observação:** Somente os administradores globais podem chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="3801e-111">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="3801e-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3801e-112">Permission Type</span></span>                        | <span data-ttu-id="3801e-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3801e-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="3801e-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3801e-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="3801e-115">AppCatalog. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3801e-115">AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="3801e-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3801e-116">Delegated (work or school account)</span></span> | <span data-ttu-id="3801e-117">AppCatalog.Submit</span><span class="sxs-lookup"><span data-stu-id="3801e-117">AppCatalog.Submit</span></span> |
| <span data-ttu-id="3801e-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3801e-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3801e-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3801e-119">Not supported.</span></span>|
| <span data-ttu-id="3801e-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3801e-120">Application</span></span>                            | <span data-ttu-id="3801e-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3801e-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3801e-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3801e-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="3801e-123">Para excluir um aplicativo do catálogo de aplicativos:</span><span class="sxs-lookup"><span data-stu-id="3801e-123">To delete an app from the app catalog:</span></span>

```http
DELETE /appCatalogs/teamsApps/{id}
```

<span data-ttu-id="3801e-124">Para excluir um aplicativo que foi enviado, mas que não foi aprovado:</span><span class="sxs-lookup"><span data-stu-id="3801e-124">To delete an app that has been submitted but has not been approved:</span></span>

```http
DELETE appCatalogs/teamsApps/{appId}/appDefinitions/{appDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="3801e-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3801e-125">Request headers</span></span>

| <span data-ttu-id="3801e-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3801e-126">Header</span></span>        | <span data-ttu-id="3801e-127">Valor</span><span class="sxs-lookup"><span data-stu-id="3801e-127">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="3801e-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="3801e-128">Authorization</span></span> | <span data-ttu-id="3801e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3801e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3801e-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3801e-131">Request body</span></span>

<span data-ttu-id="3801e-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3801e-132">Do not supply a request body for this method.</span></span>

><span data-ttu-id="3801e-133">**Observação:** Use a ID retornada da chamada [lista de aplicativos publicados](./teamsapp-list.md) para fazer referência ao aplicativo que você deseja excluir.</span><span class="sxs-lookup"><span data-stu-id="3801e-133">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call to reference the app you'd like to delete.</span></span> <span data-ttu-id="3801e-134">Não use a ID do manifesto do pacote de aplicativos zip.</span><span class="sxs-lookup"><span data-stu-id="3801e-134">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="3801e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="3801e-135">Response</span></span>

<span data-ttu-id="3801e-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3801e-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3801e-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3801e-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="3801e-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3801e-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3801e-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="3801e-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_teamsapp"
}-->

```http
DELETE https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```
# <a name="c"></a>[<span data-ttu-id="3801e-141">C#</span><span class="sxs-lookup"><span data-stu-id="3801e-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3801e-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3801e-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3801e-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3801e-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="3801e-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="3801e-144">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```