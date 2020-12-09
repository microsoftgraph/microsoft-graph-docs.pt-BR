---
title: Excluir teamsApp
description: 'Excluir um aplicativo do teams do catálogo de aplicativos de uma organização (o catálogo de aplicativos do locatário). '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 53f18e0bfcdde3280629bf5ca6b6217119739d3c
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2020
ms.locfileid: "49606794"
---
# <a name="delete-teamsapp"></a><span data-ttu-id="39bd7-103">Excluir teamsApp</span><span class="sxs-lookup"><span data-stu-id="39bd7-103">Delete teamsApp</span></span>

<span data-ttu-id="39bd7-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="39bd7-104">Namespace: microsoft.graph</span></span>

<!-- markdownlint-disable MD001 -->
### <a name="delete-an-app-from-your-organizations-app-catalog"></a><span data-ttu-id="39bd7-105">Excluir um aplicativo do catálogo de aplicativos da sua organização</span><span class="sxs-lookup"><span data-stu-id="39bd7-105">Delete an app from your organization's app catalog</span></span>

<span data-ttu-id="39bd7-106">Excluir um [aplicativo](../resources/teamsapp.md) do catálogo de aplicativos de uma organização (o catálogo de aplicativos do locatário).</span><span class="sxs-lookup"><span data-stu-id="39bd7-106">Delete an [app](../resources/teamsapp.md) from an organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="39bd7-107">Para excluir um aplicativo, a propriedade **distributionMethod** para o aplicativo deve ser definida como `organization` .</span><span class="sxs-lookup"><span data-stu-id="39bd7-107">To delete an app, the **distributionMethod** property for the app must be set to `organization`.</span></span>

<span data-ttu-id="39bd7-108">Você também pode usar essa API para remover um aplicativo enviado do processo de revisão.</span><span class="sxs-lookup"><span data-stu-id="39bd7-108">You can also use this API to remove a submitted app from the review process.</span></span>

## <a name="permissions"></a><span data-ttu-id="39bd7-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="39bd7-109">Permissions</span></span>

<span data-ttu-id="39bd7-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39bd7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="39bd7-112">**Observação:** Somente os administradores globais podem chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="39bd7-112">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="39bd7-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="39bd7-113">Permission Type</span></span>                        | <span data-ttu-id="39bd7-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="39bd7-114">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="39bd7-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="39bd7-115">Delegated (work or school account)</span></span> | <span data-ttu-id="39bd7-116">AppCatalog. Submit, AppCatalog. ReadWrite. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="39bd7-116">AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="39bd7-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="39bd7-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39bd7-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="39bd7-118">Not supported</span></span>|
| <span data-ttu-id="39bd7-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="39bd7-119">Application</span></span>                            | <span data-ttu-id="39bd7-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39bd7-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="39bd7-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="39bd7-121">HTTP request</span></span>

<span data-ttu-id="39bd7-122">Para excluir um aplicativo do catálogo de aplicativos:</span><span class="sxs-lookup"><span data-stu-id="39bd7-122">To delete an app from the app catalog:</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /appCatalogs/teamsApps/{id}
```

<span data-ttu-id="39bd7-123">Para excluir um aplicativo que foi enviado, mas que não foi aprovado:</span><span class="sxs-lookup"><span data-stu-id="39bd7-123">To delete an app that has been submitted but has not been approved:</span></span>

```http
DELETE appCatalogs/teamsApps/{appId}/appDefinitions/{appDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="39bd7-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="39bd7-124">Request headers</span></span>

| <span data-ttu-id="39bd7-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="39bd7-125">Header</span></span>        | <span data-ttu-id="39bd7-126">Valor</span><span class="sxs-lookup"><span data-stu-id="39bd7-126">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="39bd7-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="39bd7-127">Authorization</span></span> | <span data-ttu-id="39bd7-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="39bd7-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="39bd7-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="39bd7-130">Request body</span></span>

<span data-ttu-id="39bd7-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="39bd7-131">Do not supply a request body for this method.</span></span>

><span data-ttu-id="39bd7-132">**Observação:** Use a ID retornada da chamada [lista de aplicativos publicados](./appcatalogs-list-teamsapps.md) para fazer referência ao aplicativo que você deseja atualizar.</span><span class="sxs-lookup"><span data-stu-id="39bd7-132">**Note:** Use the ID returned from the [List published apps](./appcatalogs-list-teamsapps.md) call to reference the app you'd like to update.</span></span> <span data-ttu-id="39bd7-133">Não use a ID do manifesto do pacote de aplicativos zip.</span><span class="sxs-lookup"><span data-stu-id="39bd7-133">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="39bd7-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="39bd7-134">Response</span></span>

<span data-ttu-id="39bd7-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="39bd7-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39bd7-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="39bd7-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="39bd7-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="39bd7-138">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="39bd7-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="39bd7-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_teamsapp"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```
# <a name="c"></a>[<span data-ttu-id="39bd7-140">C#</span><span class="sxs-lookup"><span data-stu-id="39bd7-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39bd7-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39bd7-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39bd7-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39bd7-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="39bd7-143">Java</span><span class="sxs-lookup"><span data-stu-id="39bd7-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="39bd7-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="39bd7-144">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

