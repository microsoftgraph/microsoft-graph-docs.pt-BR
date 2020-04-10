---
title: 'servicePrincipalName: listar appRoleAssignments'
description: Recupere uma lista de objetos approleassignment.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: e9e4780b6a0a0743a0d89c0eb5d076a65864f1b8
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219274"
---
# <a name="serviceprincipal-list-approleassignments"></a><span data-ttu-id="20c48-103">servicePrincipalName: listar appRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="20c48-103">servicePrincipal: List appRoleAssignments</span></span>

<span data-ttu-id="20c48-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20c48-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20c48-105">Recupere uma lista de objetos approleassignment.</span><span class="sxs-lookup"><span data-stu-id="20c48-105">Retrieve a list of approleassignment objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="20c48-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="20c48-106">Permissions</span></span>
<span data-ttu-id="20c48-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20c48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20c48-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20c48-109">Permission type</span></span>      | <span data-ttu-id="20c48-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="20c48-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20c48-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20c48-111">Delegated (work or school account)</span></span> | <span data-ttu-id="20c48-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="20c48-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="20c48-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20c48-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20c48-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20c48-114">Not supported.</span></span>    |
|<span data-ttu-id="20c48-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20c48-115">Application</span></span> | <span data-ttu-id="20c48-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20c48-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="20c48-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20c48-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/appRoleAssignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="20c48-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="20c48-118">Optional query parameters</span></span>
<span data-ttu-id="20c48-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="20c48-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="20c48-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20c48-120">Request headers</span></span>
| <span data-ttu-id="20c48-121">Nome</span><span class="sxs-lookup"><span data-stu-id="20c48-121">Name</span></span>       | <span data-ttu-id="20c48-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="20c48-122">Type</span></span> | <span data-ttu-id="20c48-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="20c48-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="20c48-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="20c48-124">Authorization</span></span>  | <span data-ttu-id="20c48-125">string</span><span class="sxs-lookup"><span data-stu-id="20c48-125">string</span></span>  | <span data-ttu-id="20c48-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20c48-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="20c48-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20c48-128">Request body</span></span>
<span data-ttu-id="20c48-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="20c48-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20c48-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="20c48-130">Response</span></span>

<span data-ttu-id="20c48-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [appRoleAssignment](../resources/approleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20c48-131">If successful, this method returns a `200 OK` response code and collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="20c48-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20c48-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="20c48-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20c48-133">Request</span></span>
<span data-ttu-id="20c48-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="20c48-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="20c48-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="20c48-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_approleassignments"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignments
```
# <a name="c"></a>[<span data-ttu-id="20c48-136">C#</span><span class="sxs-lookup"><span data-stu-id="20c48-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-approleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="20c48-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20c48-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-approleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="20c48-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20c48-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-approleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="20c48-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="20c48-139">Response</span></span>
<span data-ttu-id="20c48-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="20c48-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 306

{
  "value": [
    {
      "creationTimestamp": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "principalDisplayName": "principalDisplayName-value",
      "principalId": "principalId-value",
      "principalType": "principalType-value",
      "resourceDisplayName": "resourceDisplayName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List appRoleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
