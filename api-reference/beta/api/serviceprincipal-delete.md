---
title: Excluir o servicePrincipalName
description: Exclua o servicePrincipalName.
localization_priority: Normal
ms.openlocfilehash: c604886416eba49ae7bbd8c614ce2200a3bc9948
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870208"
---
# <a name="delete-serviceprincipal"></a><span data-ttu-id="3317e-103">Excluir o servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="3317e-103">Delete servicePrincipal</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3317e-104">Exclua o servicePrincipalName.</span><span class="sxs-lookup"><span data-stu-id="3317e-104">Delete servicePrincipal.</span></span>
## <a name="permissions"></a><span data-ttu-id="3317e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3317e-105">Permissions</span></span>
<span data-ttu-id="3317e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3317e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3317e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3317e-108">Permission type</span></span>      | <span data-ttu-id="3317e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3317e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3317e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3317e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3317e-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3317e-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3317e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3317e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3317e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3317e-113">Not supported.</span></span>    |
|<span data-ttu-id="3317e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3317e-114">Application</span></span> | <span data-ttu-id="3317e-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3317e-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3317e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3317e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}

```
## <a name="request-headers"></a><span data-ttu-id="3317e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3317e-117">Request headers</span></span>
| <span data-ttu-id="3317e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="3317e-118">Name</span></span>       | <span data-ttu-id="3317e-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="3317e-119">Type</span></span> | <span data-ttu-id="3317e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3317e-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3317e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3317e-121">Authorization</span></span>  | <span data-ttu-id="3317e-122">string</span><span class="sxs-lookup"><span data-stu-id="3317e-122">string</span></span>  | <span data-ttu-id="3317e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3317e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3317e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3317e-125">Request body</span></span>
<span data-ttu-id="3317e-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3317e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3317e-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="3317e-127">Response</span></span>

<span data-ttu-id="3317e-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3317e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3317e-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3317e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3317e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3317e-131">Request</span></span>
<span data-ttu-id="3317e-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3317e-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3317e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3317e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_serviceprincipal"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3317e-134">C#</span><span class="sxs-lookup"><span data-stu-id="3317e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3317e-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="3317e-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3317e-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="3317e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3317e-137">Java</span><span class="sxs-lookup"><span data-stu-id="3317e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3317e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="3317e-138">Response</span></span>
<span data-ttu-id="3317e-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3317e-139">Here is an example of the response.</span></span> 
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
  "description": "Delete servicePrincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
