---
title: Excluir proprietários registrados
description: Remova um usuário como proprietário registrado do dispositivo.
localization_priority: Normal
author: michaelrm97
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 094c7aa46102d10cd61267b0056654d3e463a335
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437229"
---
# <a name="delete-registeredowner"></a><span data-ttu-id="deeda-103">Excluir registeredOwner</span><span class="sxs-lookup"><span data-stu-id="deeda-103">Delete registeredOwner</span></span>

<span data-ttu-id="deeda-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="deeda-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="deeda-105">Remova um usuário como proprietário registrado do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="deeda-105">Remove a user as a registered owner of the device.</span></span>

## <a name="permissions"></a><span data-ttu-id="deeda-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="deeda-106">Permissions</span></span>

<span data-ttu-id="deeda-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="deeda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="deeda-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="deeda-109">Permission type</span></span>      | <span data-ttu-id="deeda-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="deeda-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="deeda-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="deeda-111">Delegated (work or school account)</span></span> |<span data-ttu-id="deeda-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="deeda-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="deeda-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="deeda-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="deeda-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="deeda-114">Not supported.</span></span>    |
|<span data-ttu-id="deeda-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="deeda-115">Application</span></span> | <span data-ttu-id="deeda-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="deeda-116">Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="deeda-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="deeda-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}/registeredOwners/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="deeda-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="deeda-118">Request headers</span></span>
| <span data-ttu-id="deeda-119">Nome</span><span class="sxs-lookup"><span data-stu-id="deeda-119">Name</span></span>       | <span data-ttu-id="deeda-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="deeda-120">Type</span></span> | <span data-ttu-id="deeda-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="deeda-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="deeda-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="deeda-122">Authorization</span></span>  | <span data-ttu-id="deeda-123">string</span><span class="sxs-lookup"><span data-stu-id="deeda-123">string</span></span>  | <span data-ttu-id="deeda-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="deeda-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="deeda-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="deeda-126">Request body</span></span>
<span data-ttu-id="deeda-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="deeda-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="deeda-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="deeda-128">Response</span></span>

<span data-ttu-id="deeda-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="deeda-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="deeda-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="deeda-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="deeda-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="deeda-131">Request</span></span>
<span data-ttu-id="deeda-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="deeda-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="deeda-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="deeda-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_registeredowners"
}-->
```msgraph-interactive
DELETE https://graph.microsoft.com/beta/devices/{id}/registeredOwners/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="deeda-134">C#</span><span class="sxs-lookup"><span data-stu-id="deeda-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-registeredowners-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="deeda-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="deeda-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-registeredowners-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="deeda-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="deeda-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-registeredowners-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="deeda-137">Java</span><span class="sxs-lookup"><span data-stu-id="deeda-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-registeredowners-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

##### <a name="response"></a><span data-ttu-id="deeda-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="deeda-138">Response</span></span>
<span data-ttu-id="deeda-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="deeda-139">Here is an example of the response.</span></span>
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
  "description": "Delete registeredOwners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


