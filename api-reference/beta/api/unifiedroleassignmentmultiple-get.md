---
title: Obter unifiedRoleAssignmentMultiple
description: Recupere as propriedades e as relações de um objeto unifiedRoleAssignmentMultiple.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 9e9867d2c314534115f7c620d52329805d8b890e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960562"
---
# <a name="get-unifiedroleassignmentmultiple"></a><span data-ttu-id="9ef5d-103">Obter unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="9ef5d-103">Get unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="9ef5d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ef5d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ef5d-105">Recupere as propriedades e as relações de [um objeto unifiedRoleAssignmentMultiple.](../resources/unifiedroleassignmentmultiple.md)</span><span class="sxs-lookup"><span data-stu-id="9ef5d-105">Retrieve the properties and relationships of a [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="9ef5d-106">Use este objeto para obter atribuições de função no Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="9ef5d-106">Use this object for get role assignments in Microsoft Intune.</span></span> <span data-ttu-id="9ef5d-107">Para outros aplicativos do Microsoft 365 (como o Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="9ef5d-107">For other Microsoft 365 applications (like Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9ef5d-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="9ef5d-108">Permissions</span></span>

<span data-ttu-id="9ef5d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ef5d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9ef5d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ef5d-111">Permission type</span></span> | <span data-ttu-id="9ef5d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9ef5d-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="9ef5d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ef5d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9ef5d-114">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef5d-114">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="9ef5d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9ef5d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ef5d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ef5d-116">Not supported.</span></span> |
| <span data-ttu-id="9ef5d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ef5d-117">Application</span></span> | <span data-ttu-id="9ef5d-118">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ef5d-118">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ef5d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ef5d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/deviceManagement/roleAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9ef5d-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9ef5d-120">Optional query parameters</span></span>

<span data-ttu-id="9ef5d-121">Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9ef5d-121">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="9ef5d-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="9ef5d-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9ef5d-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ef5d-123">Request headers</span></span>

| <span data-ttu-id="9ef5d-124">Nome</span><span class="sxs-lookup"><span data-stu-id="9ef5d-124">Name</span></span>  | <span data-ttu-id="9ef5d-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ef5d-125">Description</span></span> |
|:----- |:----------- |
| <span data-ttu-id="9ef5d-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="9ef5d-126">Authorization</span></span> | <span data-ttu-id="9ef5d-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9ef5d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ef5d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ef5d-129">Request body</span></span>

<span data-ttu-id="9ef5d-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9ef5d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ef5d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ef5d-131">Response</span></span>

<span data-ttu-id="9ef5d-132">Se tiver êxito, este método retornará um código de resposta e `200 OK` o objeto [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ef5d-132">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9ef5d-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9ef5d-133">Examples</span></span>

### <a name="example-1-get-a-directory-scoped-roleassignmentmultiple-in-intune"></a><span data-ttu-id="9ef5d-134">Exemplo 1: Obter uma função com escopo de diretórioAssignmentMultiple no Intune</span><span class="sxs-lookup"><span data-stu-id="9ef5d-134">Example 1: Get a directory-scoped roleAssignmentMultiple in Intune</span></span>

#### <a name="request"></a><span data-ttu-id="9ef5d-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ef5d-135">Request</span></span>

<span data-ttu-id="9ef5d-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9ef5d-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9ef5d-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ef5d-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentmultiple_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="9ef5d-138">C#</span><span class="sxs-lookup"><span data-stu-id="9ef5d-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignmentmultiple-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ef5d-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ef5d-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignmentmultiple-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ef5d-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ef5d-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignmentmultiple-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9ef5d-141">Java</span><span class="sxs-lookup"><span data-stu-id="9ef5d-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignmentmultiple-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9ef5d-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ef5d-142">Response</span></span>

<span data-ttu-id="9ef5d-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9ef5d-143">The following is an example of the response.</span></span>
> <span data-ttu-id="9ef5d-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9ef5d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/deviceManagement/roleAssignments/$entity",
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "id": "lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1",
    "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
    "principalIds[]": ["4ab0b690-479b-47ff-af8f-2576cf521872", "f8ca5a85-489a-49a0-b555-0a6d81e56f0d"],
    "directoryScopeIds[]": ["28ca5a85-489a-49a0-b555-0a6d81e56f0", "8152656a-cf9a-4928-a457-1512d4cae295"]
}
```

### <a name="example-2-get-a-roleassignmentmultiple-in-intune-assigned-to-a-group"></a><span data-ttu-id="9ef5d-146">Exemplo 2: Obter uma roleAssignmentMultiple no Intune atribuída a um grupo</span><span class="sxs-lookup"><span data-stu-id="9ef5d-146">Example 2: Get a roleAssignmentMultiple in Intune assigned to a group</span></span>

#### <a name="request"></a><span data-ttu-id="9ef5d-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ef5d-147">Request</span></span>

<span data-ttu-id="9ef5d-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9ef5d-148">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9ef5d-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ef5d-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentmultiple_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments?$filter = principalIds/any(x:x eq '564ae70c-73d9-476b-820b-fb61eb7384b9')
```
# <a name="c"></a>[<span data-ttu-id="9ef5d-150">C#</span><span class="sxs-lookup"><span data-stu-id="9ef5d-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignmentmultiple-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ef5d-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ef5d-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignmentmultiple-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ef5d-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ef5d-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignmentmultiple-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9ef5d-153">Java</span><span class="sxs-lookup"><span data-stu-id="9ef5d-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignmentmultiple-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9ef5d-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ef5d-154">Response</span></span>

<span data-ttu-id="9ef5d-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9ef5d-155">The following is an example of the response.</span></span>
> <span data-ttu-id="9ef5d-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9ef5d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/deviceManagement/roleAssignments",
    "@odata.count": 7,
    "value": [
        {
            "id": "893fc648-73fc-482b-b964-ddd1cabf0db4",
            "condition": null,
            "displayName": "Assign Contoso_App_Admin to School Admin",
            "description": "test",
            "roleDefinitionId": "2f9f4f7e-2d13-427b-adf2-361a1eef7ae8",
            "principalIds": [
                "564ae70c-73d9-476b-820b-fb61eb7384b9"
            ],
            "directoryScopeIds": [],
            "appScopeIds": [
                "0",
                "AllLicensedUsers"
            ]
        }
    ]
}
```

### <a name="example-3-get-a-directory-scoped-roleassignmentmultiple-with-expand"></a><span data-ttu-id="9ef5d-158">Exemplo 3: Obter uma função com escopo de diretórioAssignmentMultiple com `$expand`</span><span class="sxs-lookup"><span data-stu-id="9ef5d-158">Example 3: Get a directory-scoped roleAssignmentMultiple with `$expand`</span></span>

#### <a name="request"></a><span data-ttu-id="9ef5d-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ef5d-159">Request</span></span>

<span data-ttu-id="9ef5d-160">A seguir, um exemplo da solicitação com o `$expand` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="9ef5d-160">The following is an example of the request with the `$expand` query parameter.</span></span>


# <a name="http"></a>[<span data-ttu-id="9ef5d-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ef5d-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment_3"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1?$expand=roleDefinition,principals,directoryScopes
```
# <a name="c"></a>[<span data-ttu-id="9ef5d-162">C#</span><span class="sxs-lookup"><span data-stu-id="9ef5d-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ef5d-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ef5d-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ef5d-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ef5d-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9ef5d-165">Java</span><span class="sxs-lookup"><span data-stu-id="9ef5d-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9ef5d-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ef5d-166">Response</span></span>

<span data-ttu-id="9ef5d-167">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9ef5d-167">The following is an example of the response.</span></span>
> <span data-ttu-id="9ef5d-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9ef5d-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#roleManagement/deviceManagement/roleAssignments/$entity",
  "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
  "id": "lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1",
  "roleDefinitionId": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
  "roleDefinition": {
    "id": "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    "displayName": "Application Manager",
    "description": "Manages mobile and managed applications",
    "rolePermissions": [
      {
        "allowedResourceActions": [],
        "excludedResourceActions": [],
    }],
    "isEnabled": true,
    "isBuiltIn": true,
  },
  "principalIds": ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"],
  "principals": [
    {
      "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
      "id": "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
      "displayName": "Global IT"
    },
    {
      "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
      "id": "c1518aa9-4da5-4c84-a902-a31404023890",
      "displayName": "Americas IT"
    }
],
  "directoryScopeIds": ["28ca5a85-489a-49a0-b555-0a6d81e56f0d", "8152656a-cf9a-4928-a457-1512d4cae295"],
  "directoryScopes": [
    {
      "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
      "id": "28ca5a85-489a-49a0-b555-0a6d81e56f0d",
      "displayName": "Washington Sales Region"
    },
    {
      "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
      "id": "8152656a-cf9a-4928-a457-1512d4cae295",
      "displayName": "Oregon Sales Region"
    }
  ]
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


