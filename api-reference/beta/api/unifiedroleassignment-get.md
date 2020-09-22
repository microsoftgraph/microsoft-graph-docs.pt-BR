---
title: Obter unifiedRoleAssignment
description: Recupere as propriedades e os relacionamentos de um objeto unifiedRoleAssignment.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 00b9a325ec79b555476b0ff153266c267141efc5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48004316"
---
# <a name="get-unifiedroleassignment"></a><span data-ttu-id="57f59-103">Obter unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="57f59-103">Get unifiedRoleAssignment</span></span>

<span data-ttu-id="57f59-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57f59-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57f59-105">Recupere as propriedades e os relacionamentos de um objeto [unifiedRoleAssignment](../resources/unifiedroleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="57f59-105">Retrieve the properties and relationships of a [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="57f59-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="57f59-106">Permissions</span></span>

<span data-ttu-id="57f59-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57f59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57f59-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="57f59-109">Permission type</span></span>      | <span data-ttu-id="57f59-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="57f59-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57f59-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57f59-111">Delegated (work or school account)</span></span> | <span data-ttu-id="57f59-112">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All, Directory. AccessAsUser. All</span><span class="sxs-lookup"><span data-stu-id="57f59-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="57f59-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="57f59-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57f59-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57f59-114">Not supported.</span></span>    |
|<span data-ttu-id="57f59-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="57f59-115">Application</span></span> | <span data-ttu-id="57f59-116">RoleManagement. Read. Directory, Directory. Read. All, RoleManagement. ReadWrite. Directory, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="57f59-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="57f59-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57f59-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="57f59-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="57f59-118">Optional query parameters</span></span>

<span data-ttu-id="57f59-119">Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="57f59-119">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="57f59-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="57f59-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="57f59-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="57f59-121">Request headers</span></span>

| <span data-ttu-id="57f59-122">Nome</span><span class="sxs-lookup"><span data-stu-id="57f59-122">Name</span></span>      |<span data-ttu-id="57f59-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="57f59-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="57f59-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="57f59-124">Authorization</span></span> | <span data-ttu-id="57f59-125">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="57f59-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="57f59-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="57f59-126">Request body</span></span>

<span data-ttu-id="57f59-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="57f59-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57f59-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="57f59-128">Response</span></span>

<span data-ttu-id="57f59-129">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [unifiedRoleAssignment](../resources/unifiedroleassignment.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="57f59-129">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="57f59-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="57f59-130">Examples</span></span>

### <a name="example-1--get-details-of-a-role-assignment"></a><span data-ttu-id="57f59-131">Exemplo 1: obter detalhes de uma atribuição de função</span><span class="sxs-lookup"><span data-stu-id="57f59-131">Example 1 : Get details of a role assignment</span></span>

#### <a name="request"></a><span data-ttu-id="57f59-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57f59-132">Request</span></span>

<span data-ttu-id="57f59-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="57f59-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="57f59-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="57f59-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="57f59-135">C#</span><span class="sxs-lookup"><span data-stu-id="57f59-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="57f59-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57f59-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="57f59-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="57f59-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="57f59-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="57f59-138">Response</span></span>

<span data-ttu-id="57f59-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="57f59-139">The following is an example of the response.</span></span>

> <span data-ttu-id="57f59-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="57f59-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-details-of-a-role-assignment-with-expand"></a><span data-ttu-id="57f59-142">Exemplo 2: obter detalhes de uma atribuição de função com `$expand`</span><span class="sxs-lookup"><span data-stu-id="57f59-142">Example 2: Get details of a role assignment with `$expand`</span></span>

#### <a name="request"></a><span data-ttu-id="57f59-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57f59-143">Request</span></span>

<span data-ttu-id="57f59-144">Veja a seguir um exemplo da solicitação com o `$expand` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="57f59-144">The following is an example of the request with the `$expand` query parameter.</span></span>


# <a name="http"></a>[<span data-ttu-id="57f59-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="57f59-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1?$expand=roleDefinition,principal,directoryScope
```
# <a name="c"></a>[<span data-ttu-id="57f59-146">C#</span><span class="sxs-lookup"><span data-stu-id="57f59-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="57f59-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57f59-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="57f59-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="57f59-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="57f59-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="57f59-149">Response</span></span>

<span data-ttu-id="57f59-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="57f59-150">The following is an example of the response.</span></span>
> <span data-ttu-id="57f59-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="57f59-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


