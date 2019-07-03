---
title: Remover membro da função de diretório
description: Remove um membro de um directoryRole.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e141a8d24319aa501c782006b337bdd6486efbc5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436967"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="04568-103">Remover membro da função de diretório</span><span class="sxs-lookup"><span data-stu-id="04568-103">Remove directory role member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04568-104">Remove um membro de um directoryRole.</span><span class="sxs-lookup"><span data-stu-id="04568-104">Remove a member from a directoryRole.</span></span>

## <a name="permissions"></a><span data-ttu-id="04568-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="04568-105">Permissions</span></span>

<span data-ttu-id="04568-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04568-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="04568-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="04568-108">Permission type</span></span>      | <span data-ttu-id="04568-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="04568-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04568-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="04568-110">Delegated (work or school account)</span></span> | <span data-ttu-id="04568-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="04568-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="04568-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="04568-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04568-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04568-113">Not supported.</span></span>    |
|<span data-ttu-id="04568-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="04568-114">Application</span></span> | <span data-ttu-id="04568-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="04568-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="04568-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="04568-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryroles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="04568-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="04568-117">Request headers</span></span>

| <span data-ttu-id="04568-118">Nome</span><span class="sxs-lookup"><span data-stu-id="04568-118">Name</span></span>       | <span data-ttu-id="04568-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="04568-119">Type</span></span> | <span data-ttu-id="04568-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="04568-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="04568-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="04568-121">Authorization</span></span>  | <span data-ttu-id="04568-122">string</span><span class="sxs-lookup"><span data-stu-id="04568-122">string</span></span>  | <span data-ttu-id="04568-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="04568-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="04568-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="04568-125">Request body</span></span>

<span data-ttu-id="04568-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="04568-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04568-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="04568-127">Response</span></span>

<span data-ttu-id="04568-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="04568-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04568-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="04568-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="04568-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="04568-131">Request</span></span>

<span data-ttu-id="04568-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="04568-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="04568-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="04568-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole"
}-->

```http
DELETE https://graph.microsoft.com/beta/directoryroles/{id}/members/{id}/$ref
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="04568-134">C#</span><span class="sxs-lookup"><span data-stu-id="04568-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="04568-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="04568-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="04568-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="04568-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="04568-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="04568-137">Response</span></span>

<span data-ttu-id="04568-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="04568-138">Here is an example of the response.</span></span> 
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
  "description": "Delete a member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
