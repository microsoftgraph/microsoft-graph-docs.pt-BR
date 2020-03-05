---
title: Listar unifiedRoleAssignments
description: Obtenha uma lista de objetos unifiedRoleAssignment.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bca0895ca14d5d41dab43a22d26fba6129afe1c6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42454529"
---
# <a name="list-unifiedroleassignments"></a><span data-ttu-id="acd7f-103">Listar unifiedRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="acd7f-103">List unifiedRoleAssignments</span></span>

<span data-ttu-id="acd7f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="acd7f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="acd7f-105">Obtenha uma lista de objetos [unifiedRoleAssignment](../resources/unifiedroleassignment.md) para o provedor.</span><span class="sxs-lookup"><span data-stu-id="acd7f-105">Get a list of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) objects for the provider.</span></span>

## <a name="permissions"></a><span data-ttu-id="acd7f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="acd7f-106">Permissions</span></span>

<span data-ttu-id="acd7f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="acd7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="acd7f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="acd7f-109">Permission type</span></span>      | <span data-ttu-id="acd7f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="acd7f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="acd7f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="acd7f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="acd7f-112">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="acd7f-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="acd7f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="acd7f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="acd7f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="acd7f-114">Not supported.</span></span>    |
|<span data-ttu-id="acd7f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="acd7f-115">Application</span></span> | <span data-ttu-id="acd7f-116">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="acd7f-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="acd7f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="acd7f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="acd7f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="acd7f-118">Optional query parameters</span></span>

<span data-ttu-id="acd7f-119">Essa operação requer o `$filter` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="acd7f-119">This operation requires the `$filter` query parameter.</span></span> <span data-ttu-id="acd7f-120">Você pode filtrar as `roleDefinitionId` Propriedades ou `principalId` .</span><span class="sxs-lookup"><span data-stu-id="acd7f-120">You can filter on the `roleDefinitionId` or `principalId` properties.</span></span> <span data-ttu-id="acd7f-121">A `roleDefinitionId` propriedade pode ser uma ID de objeto role ou uma ID de objeto de modelo de função.</span><span class="sxs-lookup"><span data-stu-id="acd7f-121">The `roleDefinitionId` property can be either a role object ID or a role template object ID.</span></span> <span data-ttu-id="acd7f-122">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="acd7f-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="acd7f-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="acd7f-123">Request headers</span></span>

| <span data-ttu-id="acd7f-124">Nome</span><span class="sxs-lookup"><span data-stu-id="acd7f-124">Name</span></span>      |<span data-ttu-id="acd7f-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="acd7f-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="acd7f-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="acd7f-126">Authorization</span></span> | <span data-ttu-id="acd7f-127">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="acd7f-127">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="acd7f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="acd7f-128">Request body</span></span>

<span data-ttu-id="acd7f-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="acd7f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="acd7f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="acd7f-130">Response</span></span>

<span data-ttu-id="acd7f-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [unifiedRoleAssignment](../resources/unifiedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="acd7f-131">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="acd7f-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="acd7f-132">Examples</span></span>

### <a name="example-1-request-using-a-filter-on-role-definition-id"></a><span data-ttu-id="acd7f-133">Exemplo 1: solicitação usando um filtro em ID de definição de função</span><span class="sxs-lookup"><span data-stu-id="acd7f-133">Example 1: Request using a filter on role definition ID</span></span>

#### <a name="request"></a><span data-ttu-id="acd7f-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="acd7f-134">Request</span></span>

<span data-ttu-id="acd7f-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="acd7f-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="acd7f-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="acd7f-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roleAssignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments?$filter=roleDefinitionId eq '62e90394-69f5-4237-9190-012177145e10'
```
# <a name="c"></a>[<span data-ttu-id="acd7f-137">C#</span><span class="sxs-lookup"><span data-stu-id="acd7f-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="acd7f-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="acd7f-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="acd7f-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="acd7f-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="acd7f-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="acd7f-140">Response</span></span>

<span data-ttu-id="acd7f-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="acd7f-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments",
    "value": [
        {
            "id": "lAPpYvVpN0KRkAEhdxReEGm3jqnUe4lEhvatluHVi2I-1",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "resourceScope": "/",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10"
        },
        {
            "id": "lAPpYvVpN0KRkAEhdxReEGnbHktRMANMpnGtLZ3MXeY-1",
            "principalId": "4b1edb69-3051-4c03-a671-ad2d9dcc5de6",
            "resourceScope": "/",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10"
        },
        {
            "id": "lAPpYvVpN0KRkAEhdxReEKLh1vKaL9NIi6cTuyyN_6Q-1",
            "principalId": "f2d6e1a2-2f9a-48d3-8ba7-13bb2c8dffa4",
            "resourceScope": "/",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10"
        },
        {
            "id": "lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1",
            "principalId": "4ab0b690-479b-47ff-af8f-2576cf521872",
            "resourceScope": "/",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10"
        },
        {
            "id": "lAPpYvVpN0KRkAEhdxReEGXxIcn3O7hBqaGB0NGuCwE-1",
            "principalId": "c921f165-3bf7-41b8-a9a1-81d0d1ae0b01",
            "resourceScope": "/",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10"
        },
        {
            "id": "lAPpYvVpN0KRkAEhdxReEAWO6-FSXqhEg1mkkLETmA8-1",
            "principalId": "e1eb8e05-5e52-44a8-8359-a490b113980f",
            "resourceScope": "/",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10"
        }
    ]
}
```

### <a name="example-2-request-using-a-filter-on-principal-id"></a><span data-ttu-id="acd7f-142">Exemplo 2: solicitação usando um filtro na ID da entidade de segurança</span><span class="sxs-lookup"><span data-stu-id="acd7f-142">Example 2: Request using a filter on principal ID</span></span>

#### <a name="request"></a><span data-ttu-id="acd7f-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="acd7f-143">Request</span></span>

<span data-ttu-id="acd7f-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="acd7f-144">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="acd7f-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="acd7f-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roleAssignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments?$filter=principalId eq 'a98eb769-7bd4-4489-86f6-ad96e1d58b62'
```
# <a name="c"></a>[<span data-ttu-id="acd7f-146">C#</span><span class="sxs-lookup"><span data-stu-id="acd7f-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="acd7f-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="acd7f-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="acd7f-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="acd7f-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="acd7f-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="acd7f-149">Response</span></span>

<span data-ttu-id="acd7f-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="acd7f-150">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments",
    "value": [
        {
            "id": "lAPpYvVpN0KRkAEhdxReEGm3jqnUe4lEhvatluHVi2I-1",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "resourceScope": "/",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10"
        },
        {
            "id": "uBph6InB6EaU4WAhOrH4FGm3jqnUe4lEhvatluHVi2I-1",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "resourceScope": "/",
            "roleDefinitionId": "e8611ab8-c189-46e8-94e1-60213ab1f814"
        },
        {
            "id": "5wuT_mJe20eRr5jDpJo4sWm3jqnUe4lEhvatluHVi2I-1",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "resourceScope": "/",
            "roleDefinitionId": "fe930be7-5e62-47db-91af-98c3a49a38b1"
        },
        {
            "id": "5TgczyE2BECny4eWJNztfGm3jqnUe4lEhvatluHVi2I-1",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "resourceScope": "/",
            "roleDefinitionId": "cf1c38e5-3621-4004-a7cb-879624dced7c"
        },
        {
            "id": "CRCUdVqRaUir52kb_xgnnmm3jqnUe4lEhvatluHVi2I-1",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "resourceScope": "/",
            "roleDefinitionId": "75941009-915a-4869-abe7-691bff18279e"
        },
        {
            "id": "4yeYchSc90m7G5YI8Va7uGm3jqnUe4lEhvatluHVi2I-1",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "resourceScope": "/",
            "roleDefinitionId": "729827e3-9c14-49f7-bb1b-9608f156bbb8"
        },
        {
            "id": "y-RKGSaxskC9W2CRs4CXfWm3jqnUe4lEhvatluHVi2I-1",
            "principalId": "a98eb769-7bd4-4489-86f6-ad96e1d58b62",
            "resourceScope": "/",
            "roleDefinitionId": "194ae4cb-b126-40b2-bd5b-6091b380977d"
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List roleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
