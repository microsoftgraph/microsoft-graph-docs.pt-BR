---
title: Remover membro da função de diretório
description: Remove um membro de um directoryRole.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5d02031382482a1835bf12cc68c894cb3f3249fb
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891395"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="3cb1c-103">Remover membro da função de diretório</span><span class="sxs-lookup"><span data-stu-id="3cb1c-103">Remove directory role member</span></span>

<span data-ttu-id="3cb1c-104">Remove um membro de um directoryRole.</span><span class="sxs-lookup"><span data-stu-id="3cb1c-104">Remove a member from a directoryRole.</span></span>

## <a name="permissions"></a><span data-ttu-id="3cb1c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3cb1c-105">Permissions</span></span>

<span data-ttu-id="3cb1c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cb1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3cb1c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3cb1c-108">Permission type</span></span>      | <span data-ttu-id="3cb1c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3cb1c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3cb1c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3cb1c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3cb1c-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3cb1c-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3cb1c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3cb1c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3cb1c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3cb1c-113">Not supported.</span></span>    |
|<span data-ttu-id="3cb1c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3cb1c-114">Application</span></span> | <span data-ttu-id="3cb1c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3cb1c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3cb1c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3cb1c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryRoles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="3cb1c-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3cb1c-117">Request headers</span></span>

| <span data-ttu-id="3cb1c-118">Nome</span><span class="sxs-lookup"><span data-stu-id="3cb1c-118">Name</span></span>       | <span data-ttu-id="3cb1c-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="3cb1c-119">Type</span></span> | <span data-ttu-id="3cb1c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cb1c-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3cb1c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3cb1c-121">Authorization</span></span>  | <span data-ttu-id="3cb1c-122">string</span><span class="sxs-lookup"><span data-stu-id="3cb1c-122">string</span></span>  | <span data-ttu-id="3cb1c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3cb1c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3cb1c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3cb1c-125">Request body</span></span>

<span data-ttu-id="3cb1c-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3cb1c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3cb1c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cb1c-127">Response</span></span>

<span data-ttu-id="3cb1c-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3cb1c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cb1c-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3cb1c-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3cb1c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3cb1c-131">Request</span></span>

<span data-ttu-id="3cb1c-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3cb1c-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3cb1c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3cb1c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directoryRoles/{id}/members/{id}/$ref
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3cb1c-134">C#</span><span class="sxs-lookup"><span data-stu-id="3cb1c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3cb1c-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="3cb1c-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3cb1c-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3cb1c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3cb1c-137">Java</span><span class="sxs-lookup"><span data-stu-id="3cb1c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-from-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3cb1c-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="3cb1c-138">Response</span></span>

<span data-ttu-id="3cb1c-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3cb1c-139">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete a member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
