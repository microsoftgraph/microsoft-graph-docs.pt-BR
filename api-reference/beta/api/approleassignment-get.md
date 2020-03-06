---
title: Obter appRoleAssignment
description: Recupere as propriedades e os relacionamentos do objeto approleassignment.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 7e6909518820bb4f6702de05121f79310a428fe8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441368"
---
# <a name="get-approleassignment"></a><span data-ttu-id="8abc7-103">Obter appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="8abc7-103">Get appRoleAssignment</span></span>

<span data-ttu-id="8abc7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8abc7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8abc7-105">Recupere as propriedades e os relacionamentos do objeto approleassignment.</span><span class="sxs-lookup"><span data-stu-id="8abc7-105">Retrieve the properties and relationships of approleassignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8abc7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8abc7-106">Permissions</span></span>
<span data-ttu-id="8abc7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8abc7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8abc7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8abc7-109">Permission type</span></span>      | <span data-ttu-id="8abc7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8abc7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8abc7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8abc7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8abc7-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8abc7-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8abc7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8abc7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8abc7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8abc7-114">Not supported.</span></span>    |
|<span data-ttu-id="8abc7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8abc7-115">Application</span></span> | <span data-ttu-id="8abc7-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8abc7-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8abc7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8abc7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/appRoleAssignments/{id}
GET /groups/{id}/appRoleAssignments/{id}
GET /servicePrincipals/{id}/appRoleAssignments/{id}
GET /servicePrincipals/{id}/appRoleAssignedTo/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8abc7-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8abc7-118">Optional query parameters</span></span>
<span data-ttu-id="8abc7-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8abc7-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8abc7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8abc7-120">Request headers</span></span>
| <span data-ttu-id="8abc7-121">Nome</span><span class="sxs-lookup"><span data-stu-id="8abc7-121">Name</span></span>       | <span data-ttu-id="8abc7-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="8abc7-122">Type</span></span> | <span data-ttu-id="8abc7-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="8abc7-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8abc7-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8abc7-124">Authorization</span></span>  | <span data-ttu-id="8abc7-125">string</span><span class="sxs-lookup"><span data-stu-id="8abc7-125">string</span></span>  | <span data-ttu-id="8abc7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8abc7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8abc7-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8abc7-128">Request body</span></span>
<span data-ttu-id="8abc7-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8abc7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8abc7-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="8abc7-130">Response</span></span>

<span data-ttu-id="8abc7-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [appRoleAssignment](../resources/approleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8abc7-131">If successful, this method returns a `200 OK` response code and [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8abc7-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8abc7-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8abc7-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8abc7-133">Request</span></span>
<span data-ttu-id="8abc7-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8abc7-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8abc7-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="8abc7-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_approleassignment"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignedTo/{id}
```
# <a name="c"></a>[<span data-ttu-id="8abc7-136">C#</span><span class="sxs-lookup"><span data-stu-id="8abc7-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8abc7-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8abc7-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8abc7-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8abc7-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8abc7-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="8abc7-139">Response</span></span>
<span data-ttu-id="8abc7-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8abc7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Get appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
