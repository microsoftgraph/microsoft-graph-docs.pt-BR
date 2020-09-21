---
title: Excluir workforceIntegration
description: Excluir uma instância de um workforceIntegration.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 216ebcdf7bd22cac6724c7e7b86132bb9784f159
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989774"
---
# <a name="delete-workforceintegration"></a><span data-ttu-id="4e621-103">Excluir workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="4e621-103">Delete workforceIntegration</span></span>

<span data-ttu-id="4e621-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e621-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e621-105">Excluir uma instância de um [workforceIntegration](../resources/workforceintegration.md).</span><span class="sxs-lookup"><span data-stu-id="4e621-105">Delete an instance of a [workforceIntegration](../resources/workforceintegration.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4e621-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4e621-106">Permissions</span></span>

<span data-ttu-id="4e621-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e621-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4e621-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4e621-109">Permission type</span></span>                        | <span data-ttu-id="4e621-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4e621-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4e621-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4e621-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4e621-112">WorkforceIntegration. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="4e621-112">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="4e621-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4e621-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e621-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e621-114">Not supported.</span></span> |
| <span data-ttu-id="4e621-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4e621-115">Application</span></span>                            | <span data-ttu-id="4e621-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e621-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4e621-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4e621-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teamwork/workforceIntegrations/{workforceIntegrationId}
```

## <a name="request-headers"></a><span data-ttu-id="4e621-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4e621-118">Request headers</span></span>

| <span data-ttu-id="4e621-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4e621-119">Name</span></span>          | <span data-ttu-id="4e621-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e621-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4e621-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4e621-121">Authorization</span></span> | <span data-ttu-id="4e621-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="4e621-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4e621-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4e621-123">Request body</span></span>

<span data-ttu-id="4e621-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4e621-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e621-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e621-125">Response</span></span>

<span data-ttu-id="4e621-p102">Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4e621-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4e621-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4e621-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4e621-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4e621-129">Request</span></span>

<span data-ttu-id="4e621-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4e621-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4e621-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="4e621-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_workforceintegration"
}-->

```http
DELETE https://graph.microsoft.com/beta/teamwork/workforceIntegrations/{workforceIntegrationId}
```
# <a name="c"></a>[<span data-ttu-id="4e621-132">C#</span><span class="sxs-lookup"><span data-stu-id="4e621-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4e621-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4e621-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4e621-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4e621-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4e621-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e621-135">Response</span></span>

<span data-ttu-id="4e621-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4e621-136">The following is an example of the response.</span></span>

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


