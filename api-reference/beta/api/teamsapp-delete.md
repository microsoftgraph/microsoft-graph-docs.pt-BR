---
title: Excluir teamsApp
description: 'Remova um Teams do catálogo de aplicativos de uma organização (o catálogo de aplicativos de locatário). '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 34e9e7a1f8e98eda66bf34950c9d7f0b9cac7d6e
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786696"
---
# <a name="delete-teamsapp"></a><span data-ttu-id="58c0f-103">Excluir teamsApp</span><span class="sxs-lookup"><span data-stu-id="58c0f-103">Delete teamsApp</span></span>

<span data-ttu-id="58c0f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58c0f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<!-- markdownlint-disable MD001 -->

<span data-ttu-id="58c0f-105">[Exclua um aplicativo](../resources/teamsapp.md) do catálogo de aplicativos de uma organização (o catálogo de aplicativos do locatário).</span><span class="sxs-lookup"><span data-stu-id="58c0f-105">Delete an [app](../resources/teamsapp.md) from an organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="58c0f-106">Para excluir um aplicativo, a **propriedade distributionMethod** para o aplicativo deve ser definida como `organization` .</span><span class="sxs-lookup"><span data-stu-id="58c0f-106">To delete an app, the **distributionMethod** property for the app must be set to `organization`.</span></span>

<span data-ttu-id="58c0f-107">Você também pode usar essa API para remover um aplicativo enviado do processo de revisão.</span><span class="sxs-lookup"><span data-stu-id="58c0f-107">You can also use this API to remove a submitted app from the review process.</span></span>

## <a name="permissions"></a><span data-ttu-id="58c0f-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="58c0f-108">Permissions</span></span>

<span data-ttu-id="58c0f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58c0f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="58c0f-111">**Observação:** Somente administradores globais podem chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="58c0f-111">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="58c0f-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58c0f-112">Permission Type</span></span>                        | <span data-ttu-id="58c0f-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="58c0f-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="58c0f-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58c0f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="58c0f-115">AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58c0f-115">AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="58c0f-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58c0f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58c0f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58c0f-117">Not supported.</span></span>|
| <span data-ttu-id="58c0f-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58c0f-118">Application</span></span>                            | <span data-ttu-id="58c0f-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58c0f-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="58c0f-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58c0f-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="58c0f-121">Para excluir um aplicativo do catálogo de aplicativos:</span><span class="sxs-lookup"><span data-stu-id="58c0f-121">To delete an app from the app catalog:</span></span>

```http
DELETE /appCatalogs/teamsApps/{id}
```

<span data-ttu-id="58c0f-122">Para excluir um aplicativo que foi enviado, mas não foi aprovado:</span><span class="sxs-lookup"><span data-stu-id="58c0f-122">To delete an app that has been submitted but has not been approved:</span></span>

```http
DELETE appCatalogs/teamsApps/{appId}/appDefinitions/{appDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="58c0f-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58c0f-123">Request headers</span></span>

| <span data-ttu-id="58c0f-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="58c0f-124">Header</span></span>        | <span data-ttu-id="58c0f-125">Valor</span><span class="sxs-lookup"><span data-stu-id="58c0f-125">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="58c0f-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="58c0f-126">Authorization</span></span> | <span data-ttu-id="58c0f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58c0f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="58c0f-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58c0f-129">Request body</span></span>

<span data-ttu-id="58c0f-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="58c0f-130">Do not supply a request body for this method.</span></span>

><span data-ttu-id="58c0f-131">**Observação:** Use a ID retornada da chamada Lista [de](./appcatalogs-list-teamsapps.md) aplicativos publicados para fazer referência ao aplicativo que você gostaria de excluir.</span><span class="sxs-lookup"><span data-stu-id="58c0f-131">**Note:** Use the ID returned from the [List published apps](./appcatalogs-list-teamsapps.md) call to reference the app you'd like to delete.</span></span> <span data-ttu-id="58c0f-132">Não use a ID do manifesto do pacote do aplicativo zip.</span><span class="sxs-lookup"><span data-stu-id="58c0f-132">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="58c0f-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="58c0f-133">Response</span></span>

<span data-ttu-id="58c0f-p105">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58c0f-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58c0f-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58c0f-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="58c0f-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58c0f-137">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="58c0f-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="58c0f-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_teamsapp"
}-->

```http
DELETE https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```
# <a name="c"></a>[<span data-ttu-id="58c0f-139">C#</span><span class="sxs-lookup"><span data-stu-id="58c0f-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="58c0f-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="58c0f-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="58c0f-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="58c0f-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="58c0f-142">Java</span><span class="sxs-lookup"><span data-stu-id="58c0f-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="58c0f-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="58c0f-143">Response</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```
