---
title: Obter appRoleAssignment
description: Recupere as propriedades e os relacionamentos do objeto approleassignment.
localization_priority: Priority
ms.openlocfilehash: b80b6975deb1a9af5ec280c4398d77c341b61c96
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636356"
---
# <a name="get-approleassignment"></a><span data-ttu-id="36bde-103">Obter appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="36bde-103">Get appRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36bde-104">Recupere as propriedades e os relacionamentos do objeto approleassignment.</span><span class="sxs-lookup"><span data-stu-id="36bde-104">Retrieve the properties and relationships of approleassignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="36bde-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="36bde-105">Permissions</span></span>
<span data-ttu-id="36bde-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36bde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36bde-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36bde-108">Permission type</span></span>      | <span data-ttu-id="36bde-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="36bde-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36bde-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36bde-110">Delegated (work or school account)</span></span> | <span data-ttu-id="36bde-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="36bde-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="36bde-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36bde-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36bde-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36bde-113">Not supported.</span></span>    |
|<span data-ttu-id="36bde-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36bde-114">Application</span></span> | <span data-ttu-id="36bde-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36bde-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="36bde-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36bde-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/appRoleAssignments/{id}
GET /servicePrincipals/{id}/appRoleAssignedTo
GET /groups/{id}/appRoleAssignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="36bde-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="36bde-117">Optional query parameters</span></span>
<span data-ttu-id="36bde-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="36bde-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="36bde-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="36bde-119">Request headers</span></span>
| <span data-ttu-id="36bde-120">Nome</span><span class="sxs-lookup"><span data-stu-id="36bde-120">Name</span></span>       | <span data-ttu-id="36bde-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="36bde-121">Type</span></span> | <span data-ttu-id="36bde-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="36bde-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="36bde-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="36bde-123">Authorization</span></span>  | <span data-ttu-id="36bde-124">string</span><span class="sxs-lookup"><span data-stu-id="36bde-124">string</span></span>  | <span data-ttu-id="36bde-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36bde-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="36bde-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36bde-127">Request body</span></span>
<span data-ttu-id="36bde-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="36bde-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36bde-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="36bde-129">Response</span></span>

<span data-ttu-id="36bde-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [appRoleAssignment](../resources/approleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36bde-130">If successful, this method returns a `200 OK` response code and [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="36bde-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="36bde-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="36bde-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36bde-132">Request</span></span>
<span data-ttu-id="36bde-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="36bde-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_approleassignment"
}-->
```http
GET https://graph.microsoft.com/beta/appRoleAssignments/{id}
```
##### <a name="response"></a><span data-ttu-id="36bde-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="36bde-134">Response</span></span>
<span data-ttu-id="36bde-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="36bde-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="36bde-138">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="36bde-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="36bde-139">C#</span><span class="sxs-lookup"><span data-stu-id="36bde-139">C</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_approleassignment-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="36bde-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="36bde-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_approleassignment-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/approleassignment-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/approleassignment-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
