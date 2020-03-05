---
title: Remover professor
description: Remova um professor de uma aula.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a900c16e96d4cc91846de86b757987032ba2fd18
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42426994"
---
# <a name="remove-teacher"></a><span data-ttu-id="c7724-103">Remover professor</span><span class="sxs-lookup"><span data-stu-id="c7724-103">Remove teacher</span></span>

<span data-ttu-id="c7724-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c7724-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7724-105">Remova um professor de uma aula.</span><span class="sxs-lookup"><span data-stu-id="c7724-105">Remove a teacher from a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7724-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c7724-106">Permissions</span></span>

<span data-ttu-id="c7724-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7724-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c7724-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7724-109">Permission type</span></span>                        | <span data-ttu-id="c7724-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c7724-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="c7724-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7724-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c7724-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7724-112">Not supported.</span></span>                              |
| <span data-ttu-id="c7724-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7724-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7724-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c7724-114">Not supported.</span></span>                              |
| <span data-ttu-id="c7724-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7724-115">Application</span></span>                            | <span data-ttu-id="c7724-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7724-116">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="c7724-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7724-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{id}/teachers/{userId}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="c7724-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7724-118">Request headers</span></span>

| <span data-ttu-id="c7724-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c7724-119">Header</span></span>        | <span data-ttu-id="c7724-120">Valor</span><span class="sxs-lookup"><span data-stu-id="c7724-120">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="c7724-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7724-121">Authorization</span></span> | <span data-ttu-id="c7724-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7724-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7724-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7724-124">Request body</span></span>

<span data-ttu-id="c7724-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c7724-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7724-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7724-126">Response</span></span>

<span data-ttu-id="c7724-127">Se bem-sucedido, esse método retornará um código de resposta `204 No Content` e um corpo de resposta vazio.</span><span class="sxs-lookup"><span data-stu-id="c7724-127">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7724-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7724-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c7724-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c7724-129">Request</span></span>

<span data-ttu-id="c7724-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7724-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c7724-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7724-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->

```http
DELETE https://graph.microsoft.com/beta/education/classes/{id}/teachers/14012
```
# <a name="c"></a>[<span data-ttu-id="c7724-132">C#</span><span class="sxs-lookup"><span data-stu-id="c7724-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7724-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7724-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7724-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7724-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c7724-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7724-135">Response</span></span>

<span data-ttu-id="c7724-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c7724-136">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
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
