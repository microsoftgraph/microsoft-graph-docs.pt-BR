---
title: Excluir workforceIntegration
description: Excluir uma instância de um workforceIntegration.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b3c3b0c33c617ba03b56a53e1ebb4be9c51bcaa2
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/04/2020
ms.locfileid: "44217278"
---
# <a name="delete-workforceintegration"></a><span data-ttu-id="886bc-103">Excluir workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="886bc-103">Delete workforceIntegration</span></span>

<span data-ttu-id="886bc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="886bc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="886bc-105">Excluir uma instância de um [workforceIntegration](../resources/workforceintegration.md).</span><span class="sxs-lookup"><span data-stu-id="886bc-105">Delete an instance of a [workforceIntegration](../resources/workforceintegration.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="886bc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="886bc-106">Permissions</span></span>

<span data-ttu-id="886bc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="886bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="886bc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="886bc-109">Permission type</span></span>                        | <span data-ttu-id="886bc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="886bc-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="886bc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="886bc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="886bc-112">WorkforceIntegration. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="886bc-112">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="886bc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="886bc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="886bc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="886bc-114">Not supported.</span></span> |
| <span data-ttu-id="886bc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="886bc-115">Application</span></span>                            | <span data-ttu-id="886bc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="886bc-116">Not supported.</span></span> |

> <span data-ttu-id="886bc-117">**Observação**: esta API oferece transporte a permissões de administrador.</span><span class="sxs-lookup"><span data-stu-id="886bc-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="886bc-118">Os administradores globais podem acessar grupos dos quais eles não são membros.</span><span class="sxs-lookup"><span data-stu-id="886bc-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="886bc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="886bc-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teamwork/workforceIntegrations/{workforceIntegrationId}
```

## <a name="request-headers"></a><span data-ttu-id="886bc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="886bc-120">Request headers</span></span>

| <span data-ttu-id="886bc-121">Nome</span><span class="sxs-lookup"><span data-stu-id="886bc-121">Name</span></span>          | <span data-ttu-id="886bc-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="886bc-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="886bc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="886bc-123">Authorization</span></span> | <span data-ttu-id="886bc-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="886bc-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="886bc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="886bc-126">Request body</span></span>

<span data-ttu-id="886bc-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="886bc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="886bc-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="886bc-128">Response</span></span>

<span data-ttu-id="886bc-p104">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="886bc-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="886bc-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="886bc-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="886bc-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="886bc-132">Request</span></span>

<span data-ttu-id="886bc-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="886bc-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="886bc-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="886bc-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_workforceintegration"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/teamwork/workforceIntegrations/{workforceIntegrationId}
```
# <a name="c"></a>[<span data-ttu-id="886bc-135">C#</span><span class="sxs-lookup"><span data-stu-id="886bc-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="886bc-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="886bc-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="886bc-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="886bc-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="886bc-138">Java</span><span class="sxs-lookup"><span data-stu-id="886bc-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-workforceintegration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="886bc-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="886bc-139">Response</span></span>

<span data-ttu-id="886bc-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="886bc-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete workforceIntegration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
