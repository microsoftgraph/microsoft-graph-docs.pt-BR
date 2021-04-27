---
title: Obter unifiedRoleAssignment
description: Recupere as propriedades e as relações de um objeto unifiedRoleAssignment.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: f40465ac0e6c7bb4f9a2419063e3b91a647128e0
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050742"
---
# <a name="get-unifiedroleassignment"></a><span data-ttu-id="02cac-103">Obter unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="02cac-103">Get unifiedRoleAssignment</span></span>

<span data-ttu-id="02cac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02cac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02cac-105">Recupere as propriedades e as relações de um [objeto unifiedRoleAssignment.](../resources/unifiedroleassignment.md)</span><span class="sxs-lookup"><span data-stu-id="02cac-105">Retrieve the properties and relationships of a [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="02cac-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="02cac-106">Permissions</span></span>

<span data-ttu-id="02cac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02cac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02cac-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02cac-109">Permission type</span></span>      | <span data-ttu-id="02cac-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="02cac-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02cac-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02cac-111">Delegated (work or school account)</span></span> | <span data-ttu-id="02cac-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="02cac-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="02cac-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02cac-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02cac-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02cac-114">Not supported.</span></span>    |
|<span data-ttu-id="02cac-115">Application</span><span class="sxs-lookup"><span data-stu-id="02cac-115">Application</span></span> | <span data-ttu-id="02cac-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02cac-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="02cac-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02cac-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="02cac-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="02cac-118">Optional query parameters</span></span>

<span data-ttu-id="02cac-119">Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="02cac-119">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="02cac-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="02cac-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="02cac-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02cac-121">Request headers</span></span>

| <span data-ttu-id="02cac-122">Nome</span><span class="sxs-lookup"><span data-stu-id="02cac-122">Name</span></span>      |<span data-ttu-id="02cac-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="02cac-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="02cac-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="02cac-124">Authorization</span></span> | <span data-ttu-id="02cac-125">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="02cac-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="02cac-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02cac-126">Request body</span></span>

<span data-ttu-id="02cac-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="02cac-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02cac-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="02cac-128">Response</span></span>

<span data-ttu-id="02cac-129">Se tiver êxito, este método retornará um código de resposta e `200 OK` o objeto [unifiedRoleAssignment](../resources/unifiedroleassignment.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02cac-129">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="02cac-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="02cac-130">Examples</span></span>

### <a name="example-1--get-details-of-a-role-assignment"></a><span data-ttu-id="02cac-131">Exemplo 1 : Obter detalhes de uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="02cac-131">Example 1 : Get details of a role assignment</span></span>

#### <a name="request"></a><span data-ttu-id="02cac-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02cac-132">Request</span></span>

<span data-ttu-id="02cac-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="02cac-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="02cac-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="02cac-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="02cac-135">C#</span><span class="sxs-lookup"><span data-stu-id="02cac-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="02cac-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02cac-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="02cac-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02cac-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="02cac-138">Java</span><span class="sxs-lookup"><span data-stu-id="02cac-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="02cac-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="02cac-139">Response</span></span>

<span data-ttu-id="02cac-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="02cac-140">The following is an example of the response.</span></span>

> <span data-ttu-id="02cac-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="02cac-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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
    "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
    "principalId": "4ab0b690-479b-47ff-af8f-2576cf521872",
    "directoryScopeId": "28ca5a85-489a-49a0-b555-0a6d81e56f0"
}
```

### <a name="example-2-get-details-of-a-role-assignment-with-expand"></a><span data-ttu-id="02cac-142">Exemplo 2: Obter detalhes de uma atribuição de função com `$expand`</span><span class="sxs-lookup"><span data-stu-id="02cac-142">Example 2: Get details of a role assignment with `$expand`</span></span>

#### <a name="request"></a><span data-ttu-id="02cac-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02cac-143">Request</span></span>

<span data-ttu-id="02cac-144">A seguir, um exemplo da solicitação com o `$expand` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="02cac-144">The following is an example of the request with the `$expand` query parameter.</span></span>


# <a name="http"></a>[<span data-ttu-id="02cac-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="02cac-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1?$expand=roleDefinition,principal,directoryScope
```
# <a name="c"></a>[<span data-ttu-id="02cac-146">C#</span><span class="sxs-lookup"><span data-stu-id="02cac-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="02cac-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02cac-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="02cac-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02cac-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="02cac-149">Java</span><span class="sxs-lookup"><span data-stu-id="02cac-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="02cac-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="02cac-150">Response</span></span>

<span data-ttu-id="02cac-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="02cac-151">The following is an example of the response.</span></span>
> <span data-ttu-id="02cac-152">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="02cac-152">**Note:** The response object shown here might be shortened for readability.</span></span>

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
    "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
    "id": "lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1",
    "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "roleDefinition": {
      "id": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
      "displayName": "Billing Administrator",
      "description": "Can perform common billing related tasks like updating payment information.",
      "rolePermissions": [
        {
          "allowedResourceActions": [
            "microsoft.commerce.billing/allEntities/allTasks",
            "microsoft.directory/organization/basic/update",
          ],
          "excludedResourceActions": []
        }],
      "isEnabled": true,
      },
    "principalId": "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "principal": {
      "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
      "id": "f8ca5a85-489a-49a0-b555-0a6d81e56f0d ",
      "userPrincipalName": "alice@contoso.com",
      "displayName": "Alice Smith"
    },
    "directoryScopeId": "28ca5a85-489a-49a0-b555-0a6d81e56f0d",
    "directoryScope": {
      "@odata.context": "https://graph.microsoft.com/beta/$metadata#organization/$entity",
      "id": "28ca5a85-489a-49a0-b555-0a6d81e56f0d",
      "displayName": "Contoso_Seattle_Admins"
    }
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


