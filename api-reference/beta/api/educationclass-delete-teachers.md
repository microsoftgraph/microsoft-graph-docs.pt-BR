---
title: Remover professor
description: Remova um professor de uma aula.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 905edc2dee2aa1400b72a0da88faca33a7fcf829
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52785988"
---
# <a name="remove-teacher"></a><span data-ttu-id="3be36-103">Remover professor</span><span class="sxs-lookup"><span data-stu-id="3be36-103">Remove teacher</span></span>

<span data-ttu-id="3be36-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3be36-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3be36-105">Remova um professor de uma aula.</span><span class="sxs-lookup"><span data-stu-id="3be36-105">Remove a teacher from a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="3be36-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="3be36-106">Permissions</span></span>

<span data-ttu-id="3be36-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3be36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3be36-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3be36-109">Permission type</span></span>                        | <span data-ttu-id="3be36-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3be36-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="3be36-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3be36-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3be36-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3be36-112">Not supported.</span></span>                              |
| <span data-ttu-id="3be36-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3be36-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3be36-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3be36-114">Not supported.</span></span>                              |
| <span data-ttu-id="3be36-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3be36-115">Application</span></span>                            | <span data-ttu-id="3be36-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3be36-116">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="3be36-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3be36-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/teachers/{userId}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="3be36-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3be36-118">Request headers</span></span>

| <span data-ttu-id="3be36-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3be36-119">Header</span></span>        | <span data-ttu-id="3be36-120">Valor</span><span class="sxs-lookup"><span data-stu-id="3be36-120">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="3be36-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3be36-121">Authorization</span></span> | <span data-ttu-id="3be36-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3be36-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3be36-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3be36-124">Request body</span></span>

<span data-ttu-id="3be36-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3be36-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3be36-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="3be36-126">Response</span></span>

<span data-ttu-id="3be36-127">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um corpo de resposta vazio.</span><span class="sxs-lookup"><span data-stu-id="3be36-127">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="3be36-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3be36-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3be36-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3be36-129">Request</span></span>

<span data-ttu-id="3be36-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3be36-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3be36-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="3be36-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool_2"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/{id}/teachers/14012
```
# <a name="c"></a>[<span data-ttu-id="3be36-132">C#</span><span class="sxs-lookup"><span data-stu-id="3be36-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationschool-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3be36-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3be36-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationschool-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3be36-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3be36-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationschool-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3be36-135">Java</span><span class="sxs-lookup"><span data-stu-id="3be36-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationclass-from-educationschool-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3be36-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3be36-136">Response</span></span>

<span data-ttu-id="3be36-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3be36-137">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


