---
title: Excluir educationRubric
description: Exclua um objeto educationRubric.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 15d455e665026c3e0c86f7ef162a5602772d84aa
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991180"
---
# <a name="delete-educationrubric"></a><span data-ttu-id="e6190-103">Excluir educationRubric</span><span class="sxs-lookup"><span data-stu-id="e6190-103">Delete educationRubric</span></span>

<span data-ttu-id="e6190-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6190-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e6190-105">[Exclua um objeto educationRubric.](../resources/educationrubric.md)</span><span class="sxs-lookup"><span data-stu-id="e6190-105">Delete an [educationRubric](../resources/educationrubric.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6190-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e6190-106">Permissions</span></span>

<span data-ttu-id="e6190-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6190-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e6190-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e6190-109">Permission type</span></span>                        | <span data-ttu-id="e6190-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e6190-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e6190-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e6190-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e6190-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e6190-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span> |
| <span data-ttu-id="e6190-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e6190-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6190-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6190-114">Not supported.</span></span> |
| <span data-ttu-id="e6190-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e6190-115">Application</span></span>                            | <span data-ttu-id="e6190-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6190-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6190-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6190-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/me/rubrics/ceb3863e-6912-4ea9-ac41-3c2bb7b6672d
```

## <a name="request-headers"></a><span data-ttu-id="e6190-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6190-118">Request headers</span></span>

| <span data-ttu-id="e6190-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e6190-119">Name</span></span>          | <span data-ttu-id="e6190-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6190-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e6190-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6190-121">Authorization</span></span> | <span data-ttu-id="e6190-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="e6190-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="e6190-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e6190-123">Request body</span></span>

<span data-ttu-id="e6190-124">Não fornece um corpo de solicitação para este método.</span><span class="sxs-lookup"><span data-stu-id="e6190-124">Don't supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6190-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6190-125">Response</span></span>

<span data-ttu-id="e6190-p102">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6190-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e6190-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e6190-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e6190-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6190-129">Request</span></span>

<span data-ttu-id="e6190-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6190-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e6190-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="e6190-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_educationrubric"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/education/me/rubrics/ceb3863e-6912-4ea9-ac41-3c2bb7b6672d
```
# <a name="c"></a>[<span data-ttu-id="e6190-132">C#</span><span class="sxs-lookup"><span data-stu-id="e6190-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-educationrubric-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e6190-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6190-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-educationrubric-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e6190-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6190-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-educationrubric-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e6190-135">Java</span><span class="sxs-lookup"><span data-stu-id="e6190-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-educationrubric-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e6190-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6190-136">Response</span></span>

<span data-ttu-id="e6190-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e6190-137">The following is an example of the response.</span></span>

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
  "description": "Delete educationRubric",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


