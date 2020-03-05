---
title: Create appRoleAssignment
description: Use esta API para criar um novo appRoleAssignment.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 196bed2ed7b860c344e83e3c0ffde38d51d967d4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453370"
---
# <a name="create-approleassignment"></a><span data-ttu-id="c6665-103">Create appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="c6665-103">Create appRoleAssignment</span></span>

<span data-ttu-id="c6665-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c6665-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6665-105">Use esta API para criar um novo appRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="c6665-105">Use this API to create a new appRoleAssignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6665-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c6665-106">Permissions</span></span>
<span data-ttu-id="c6665-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6665-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6665-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c6665-109">Permission type</span></span>      | <span data-ttu-id="c6665-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c6665-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6665-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c6665-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c6665-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c6665-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c6665-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c6665-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6665-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6665-114">Not supported.</span></span>    |
|<span data-ttu-id="c6665-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c6665-115">Application</span></span> | <span data-ttu-id="c6665-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6665-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6665-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c6665-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignments

```
## <a name="request-headers"></a><span data-ttu-id="c6665-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c6665-118">Request headers</span></span>
| <span data-ttu-id="c6665-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c6665-119">Name</span></span>       | <span data-ttu-id="c6665-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6665-120">Type</span></span> | <span data-ttu-id="c6665-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6665-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c6665-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c6665-122">Authorization</span></span>  | <span data-ttu-id="c6665-123">string</span><span class="sxs-lookup"><span data-stu-id="c6665-123">string</span></span>  | <span data-ttu-id="c6665-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6665-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c6665-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c6665-126">Request body</span></span>
<span data-ttu-id="c6665-127">No corpo da solicitação, forneça uma representação JSON do objeto [appRoleAssignment](../resources/approleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="c6665-127">In the request body, supply a JSON representation of [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c6665-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6665-128">Response</span></span>

<span data-ttu-id="c6665-129">Se bem-sucedido, este método retorna `201 Created` o código de resposta e o objeto [appRoleAssignment](../resources/approleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c6665-129">If successful, this method returns `201 Created` response code and [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6665-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6665-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c6665-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c6665-131">Request</span></span>
<span data-ttu-id="c6665-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c6665-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c6665-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c6665-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="c6665-134">C#</span><span class="sxs-lookup"><span data-stu-id="c6665-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-approleassignment-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c6665-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c6665-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-approleassignment-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c6665-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c6665-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-approleassignment-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="c6665-137">No corpo da solicitação, forneça uma representação JSON do objeto [appRoleAssignment](../resources/approleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="c6665-137">In the request body, supply a JSON representation of [appRoleAssignment](../resources/approleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c6665-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6665-138">Response</span></span>
<span data-ttu-id="c6665-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c6665-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
