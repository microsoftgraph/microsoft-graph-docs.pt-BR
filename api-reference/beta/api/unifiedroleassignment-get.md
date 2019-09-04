---
title: Obter unifiedRoleAssignment
description: Recupere as propriedades e os relacionamentos de um objeto unifiedRoleAssignment.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8861b1973c270d025786b44ca7a7696aa63fd881
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36722108"
---
# <a name="get-unifiedroleassignment"></a><span data-ttu-id="ad931-103">Obter unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="ad931-103">Get unifiedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad931-104">Recupere as propriedades e os relacionamentos de um objeto [unifiedRoleAssignment](../resources/unifiedroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="ad931-104">Retrieve the properties and relationships of a [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad931-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ad931-105">Permissions</span></span>

<span data-ttu-id="ad931-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad931-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad931-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ad931-108">Permission type</span></span>      | <span data-ttu-id="ad931-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ad931-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad931-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ad931-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ad931-111">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="ad931-111">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ad931-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ad931-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad931-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ad931-113">Not supported.</span></span>    |
|<span data-ttu-id="ad931-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ad931-114">Application</span></span> | <span data-ttu-id="ad931-115">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ad931-115">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad931-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ad931-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ad931-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ad931-117">Optional query parameters</span></span>

<span data-ttu-id="ad931-118">Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ad931-118">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="ad931-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ad931-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ad931-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ad931-120">Request headers</span></span>

| <span data-ttu-id="ad931-121">Nome</span><span class="sxs-lookup"><span data-stu-id="ad931-121">Name</span></span>      |<span data-ttu-id="ad931-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad931-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ad931-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ad931-123">Authorization</span></span> | <span data-ttu-id="ad931-124">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="ad931-124">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ad931-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ad931-125">Request body</span></span>

<span data-ttu-id="ad931-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ad931-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ad931-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad931-127">Response</span></span>

<span data-ttu-id="ad931-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [unifiedRoleAssignment](../resources/unifiedroleassignment.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ad931-128">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad931-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ad931-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="ad931-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ad931-130">Request</span></span>

<span data-ttu-id="ad931-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ad931-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ad931-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad931-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ad931-133">C#</span><span class="sxs-lookup"><span data-stu-id="ad931-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ad931-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad931-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ad931-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ad931-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ad931-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ad931-136">Response</span></span>

<span data-ttu-id="ad931-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ad931-137">The following is an example of the response.</span></span>

> <span data-ttu-id="ad931-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ad931-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments/$entity",
    "id": "lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1",
    "principalId": "4ab0b690-479b-47ff-af8f-2576cf521872",
    "resourceScope": "/",
    "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get unifiedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
