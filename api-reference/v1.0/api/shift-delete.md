---
title: Excluir turno
description: Exclua um turno da agenda.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6c1db199016bcd8d81d7c4209240f854a218d53d
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787748"
---
# <a name="delete-shift"></a><span data-ttu-id="b9b06-103">Excluir turno</span><span class="sxs-lookup"><span data-stu-id="b9b06-103">Delete shift</span></span>

<span data-ttu-id="b9b06-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9b06-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b9b06-105">[Exclua um turno](../resources/shift.md) da agenda.</span><span class="sxs-lookup"><span data-stu-id="b9b06-105">Delete a [shift](../resources/shift.md) from the schedule.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9b06-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b9b06-106">Permissions</span></span>

<span data-ttu-id="b9b06-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9b06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9b06-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9b06-109">Permission type</span></span>      | <span data-ttu-id="b9b06-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b9b06-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9b06-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9b06-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b9b06-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9b06-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b9b06-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9b06-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9b06-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9b06-114">Not supported.</span></span>    |
|<span data-ttu-id="b9b06-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9b06-115">Application</span></span> | <span data-ttu-id="b9b06-116">Schedule.Read.All, Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9b06-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9b06-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9b06-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="b9b06-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9b06-118">Request headers</span></span>

| <span data-ttu-id="b9b06-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b9b06-119">Header</span></span>       | <span data-ttu-id="b9b06-120">Valor</span><span class="sxs-lookup"><span data-stu-id="b9b06-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b9b06-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9b06-121">Authorization</span></span>  | <span data-ttu-id="b9b06-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9b06-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b9b06-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9b06-124">Request body</span></span>
<span data-ttu-id="b9b06-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b9b06-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9b06-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9b06-126">Response</span></span>

<span data-ttu-id="b9b06-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9b06-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9b06-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9b06-129">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b9b06-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9b06-130">Request</span></span>

<span data-ttu-id="b9b06-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9b06-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b9b06-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9b06-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-delete"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/shifts/{shiftId}
```
# <a name="c"></a>[<span data-ttu-id="b9b06-133">C#</span><span class="sxs-lookup"><span data-stu-id="b9b06-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b9b06-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9b06-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b9b06-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b9b06-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b9b06-136">Java</span><span class="sxs-lookup"><span data-stu-id="b9b06-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/shift-delete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


#### <a name="response"></a><span data-ttu-id="b9b06-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9b06-137">Response</span></span>

<span data-ttu-id="b9b06-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b9b06-138">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Deletes a shift from the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

