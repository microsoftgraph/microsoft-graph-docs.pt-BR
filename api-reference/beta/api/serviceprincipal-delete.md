---
title: Excluir o servicePrincipalName
description: Exclua o servicePrincipalName.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: cad7df48a955dbe06a239b120d6b32f079a7043b
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219302"
---
# <a name="delete-serviceprincipal"></a><span data-ttu-id="9a411-103">Excluir o servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="9a411-103">Delete servicePrincipal</span></span>

<span data-ttu-id="9a411-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a411-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a411-105">Exclua o servicePrincipalName.</span><span class="sxs-lookup"><span data-stu-id="9a411-105">Delete servicePrincipal.</span></span>
## <a name="permissions"></a><span data-ttu-id="9a411-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9a411-106">Permissions</span></span>
<span data-ttu-id="9a411-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a411-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a411-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a411-109">Permission type</span></span>      | <span data-ttu-id="9a411-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9a411-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a411-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a411-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9a411-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9a411-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9a411-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a411-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a411-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a411-114">Not supported.</span></span>    |
|<span data-ttu-id="9a411-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a411-115">Application</span></span> | <span data-ttu-id="9a411-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a411-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a411-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a411-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /servicePrincipals/{id}

```
## <a name="request-headers"></a><span data-ttu-id="9a411-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a411-118">Request headers</span></span>
| <span data-ttu-id="9a411-119">Nome</span><span class="sxs-lookup"><span data-stu-id="9a411-119">Name</span></span>       | <span data-ttu-id="9a411-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a411-120">Type</span></span> | <span data-ttu-id="9a411-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a411-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9a411-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a411-122">Authorization</span></span>  | <span data-ttu-id="9a411-123">string</span><span class="sxs-lookup"><span data-stu-id="9a411-123">string</span></span>  | <span data-ttu-id="9a411-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a411-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a411-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a411-126">Request body</span></span>
<span data-ttu-id="9a411-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9a411-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a411-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a411-128">Response</span></span>

<span data-ttu-id="9a411-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a411-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a411-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9a411-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a411-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a411-132">Request</span></span>
<span data-ttu-id="9a411-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a411-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9a411-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a411-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_serviceprincipal"
}-->
```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}
```
# <a name="c"></a>[<span data-ttu-id="9a411-135">C#</span><span class="sxs-lookup"><span data-stu-id="9a411-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9a411-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a411-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9a411-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a411-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9a411-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a411-138">Response</span></span>
<span data-ttu-id="9a411-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a411-139">Here is an example of the response.</span></span> 
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
