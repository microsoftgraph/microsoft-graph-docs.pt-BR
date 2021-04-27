---
title: Excluir calendarGroup
description: Exclui um grupo de calendários diferente do grupo de calendários padrão.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4de731bf72ebd91ec39132c6bd371f2efb5468a2
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047718"
---
# <a name="delete-calendargroup"></a><span data-ttu-id="d6ac7-103">Excluir calendarGroup</span><span class="sxs-lookup"><span data-stu-id="d6ac7-103">Delete calendarGroup</span></span>

<span data-ttu-id="d6ac7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6ac7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6ac7-105">Exclui um grupo de calendários diferente do grupo de calendários padrão.</span><span class="sxs-lookup"><span data-stu-id="d6ac7-105">Delete a calendar group other than the default calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6ac7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d6ac7-106">Permissions</span></span>

<span data-ttu-id="d6ac7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6ac7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d6ac7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6ac7-109">Permission type</span></span>                        | <span data-ttu-id="d6ac7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d6ac7-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="d6ac7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6ac7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d6ac7-112">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6ac7-112">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="d6ac7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6ac7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6ac7-114">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6ac7-114">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="d6ac7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6ac7-115">Application</span></span>                            | <span data-ttu-id="d6ac7-116">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d6ac7-116">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d6ac7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6ac7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/calendarGroups/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d6ac7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6ac7-118">Request headers</span></span>

| <span data-ttu-id="d6ac7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d6ac7-119">Name</span></span>          | <span data-ttu-id="d6ac7-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6ac7-120">Type</span></span>   | <span data-ttu-id="d6ac7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6ac7-121">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="d6ac7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6ac7-122">Authorization</span></span> | <span data-ttu-id="d6ac7-123">string</span><span class="sxs-lookup"><span data-stu-id="d6ac7-123">string</span></span> | <span data-ttu-id="d6ac7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6ac7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d6ac7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d6ac7-126">Request body</span></span>

<span data-ttu-id="d6ac7-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d6ac7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6ac7-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6ac7-128">Response</span></span>

<span data-ttu-id="d6ac7-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6ac7-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6ac7-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d6ac7-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d6ac7-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6ac7-132">Request</span></span>

<span data-ttu-id="d6ac7-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6ac7-133">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d6ac7-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6ac7-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_calendargroup"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/calendarGroups/{id}
```
# <a name="c"></a>[<span data-ttu-id="d6ac7-135">C#</span><span class="sxs-lookup"><span data-stu-id="d6ac7-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-calendargroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d6ac7-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d6ac7-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-calendargroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d6ac7-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d6ac7-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-calendargroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d6ac7-138">Java</span><span class="sxs-lookup"><span data-stu-id="d6ac7-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-calendargroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d6ac7-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6ac7-139">Response</span></span>

<span data-ttu-id="d6ac7-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6ac7-140">Here is an example of the response.</span></span> <span data-ttu-id="d6ac7-141">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d6ac7-141">Note: The response object shown here might be shortened for readability.</span></span>

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
  "description": "Delete calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


