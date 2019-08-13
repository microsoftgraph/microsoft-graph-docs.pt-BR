---
title: Create appRoleAssignment
description: Use esta API para criar um novo appRoleAssignment.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 5e78229f1e23afc185def38e4dc2b615e2714dbc
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36363911"
---
# <a name="create-approleassignment"></a><span data-ttu-id="667e2-103">Create appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="667e2-103">Create appRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="667e2-104">Use esta API para criar um novo appRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="667e2-104">Use this API to create a new appRoleAssignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="667e2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="667e2-105">Permissions</span></span>
<span data-ttu-id="667e2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="667e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="667e2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="667e2-108">Permission type</span></span>      | <span data-ttu-id="667e2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="667e2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="667e2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="667e2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="667e2-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="667e2-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="667e2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="667e2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="667e2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="667e2-113">Not supported.</span></span>    |
|<span data-ttu-id="667e2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="667e2-114">Application</span></span> | <span data-ttu-id="667e2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="667e2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="667e2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="667e2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignments

```
## <a name="request-headers"></a><span data-ttu-id="667e2-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="667e2-117">Request headers</span></span>
| <span data-ttu-id="667e2-118">Nome</span><span class="sxs-lookup"><span data-stu-id="667e2-118">Name</span></span>       | <span data-ttu-id="667e2-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="667e2-119">Type</span></span> | <span data-ttu-id="667e2-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="667e2-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="667e2-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="667e2-121">Authorization</span></span>  | <span data-ttu-id="667e2-122">string</span><span class="sxs-lookup"><span data-stu-id="667e2-122">string</span></span>  | <span data-ttu-id="667e2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="667e2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="667e2-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="667e2-125">Request body</span></span>
<span data-ttu-id="667e2-126">No corpo da solicitação, forneça uma representação JSON do objeto [appRoleAssignment](../resources/approleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="667e2-126">In the request body, supply a JSON representation of [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="667e2-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="667e2-127">Response</span></span>

<span data-ttu-id="667e2-128">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [appRoleAssignment](../resources/approleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="667e2-128">If successful, this method returns `201 Created` response code and [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="667e2-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="667e2-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="667e2-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="667e2-130">Request</span></span>
<span data-ttu-id="667e2-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="667e2-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="667e2-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="667e2-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_approleassignment_from_serviceprincipal"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignments
Content-type: application/json
Content-length: 233

{
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "principalDisplayName": "principalDisplayName-value",
  "principalId": "principalId-value",
  "principalType": "principalType-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="667e2-133">C#</span><span class="sxs-lookup"><span data-stu-id="667e2-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-approleassignment-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="667e2-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="667e2-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-approleassignment-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="667e2-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="667e2-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-approleassignment-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="667e2-136">Java</span><span class="sxs-lookup"><span data-stu-id="667e2-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-approleassignment-from-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="667e2-137">No corpo da solicitação, forneça uma representação JSON do objeto [appRoleAssignment](../resources/approleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="667e2-137">In the request body, supply a JSON representation of [appRoleAssignment](../resources/approleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="667e2-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="667e2-138">Response</span></span>
<span data-ttu-id="667e2-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="667e2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 253

{
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "id": "id-value",
  "principalDisplayName": "principalDisplayName-value",
  "principalId": "principalId-value",
  "principalType": "principalType-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
