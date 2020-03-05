---
title: Obter unifiedRoleAssignment
description: Recupere as propriedades e os relacionamentos de um objeto unifiedRoleAssignment.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 43cf52fde2719f44ac03c6c31444d135e925e460
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452061"
---
# <a name="get-unifiedroleassignment"></a><span data-ttu-id="ce8d7-103">Obter unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="ce8d7-103">Get unifiedRoleAssignment</span></span>

<span data-ttu-id="ce8d7-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ce8d7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce8d7-105">Recupere as propriedades e os relacionamentos de um objeto [unifiedRoleAssignment](../resources/unifiedroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="ce8d7-105">Retrieve the properties and relationships of a [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce8d7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ce8d7-106">Permissions</span></span>

<span data-ttu-id="ce8d7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce8d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce8d7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ce8d7-109">Permission type</span></span>      | <span data-ttu-id="ce8d7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ce8d7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ce8d7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ce8d7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ce8d7-112">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="ce8d7-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ce8d7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ce8d7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce8d7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce8d7-114">Not supported.</span></span>    |
|<span data-ttu-id="ce8d7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ce8d7-115">Application</span></span> | <span data-ttu-id="ce8d7-116">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="ce8d7-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce8d7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ce8d7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ce8d7-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ce8d7-118">Optional query parameters</span></span>

<span data-ttu-id="ce8d7-119">Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ce8d7-119">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="ce8d7-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ce8d7-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ce8d7-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ce8d7-121">Request headers</span></span>

| <span data-ttu-id="ce8d7-122">Nome</span><span class="sxs-lookup"><span data-stu-id="ce8d7-122">Name</span></span>      |<span data-ttu-id="ce8d7-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce8d7-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ce8d7-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ce8d7-124">Authorization</span></span> | <span data-ttu-id="ce8d7-125">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="ce8d7-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce8d7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ce8d7-126">Request body</span></span>

<span data-ttu-id="ce8d7-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ce8d7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce8d7-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce8d7-128">Response</span></span>

<span data-ttu-id="ce8d7-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [unifiedRoleAssignment](../resources/unifiedroleassignment.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ce8d7-129">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce8d7-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ce8d7-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce8d7-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ce8d7-131">Request</span></span>

<span data-ttu-id="ce8d7-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ce8d7-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ce8d7-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ce8d7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="ce8d7-134">C#</span><span class="sxs-lookup"><span data-stu-id="ce8d7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ce8d7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ce8d7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ce8d7-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce8d7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ce8d7-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce8d7-137">Response</span></span>

<span data-ttu-id="ce8d7-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ce8d7-138">The following is an example of the response.</span></span>

> <span data-ttu-id="ce8d7-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ce8d7-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
