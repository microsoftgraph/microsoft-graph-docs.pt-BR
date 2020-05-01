---
title: Obter unifiedRoleAssignmentMultiple
description: Recupere as propriedades e os relacionamentos de um objeto unifiedRoleAssignmentMultiple.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4252147e23f0c71d4e7acd04976ca73b457a78ba
ms.sourcegitcommit: feebe30e62aa19ce5cb8e8338e043326e464ed9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991772"
---
# <a name="get-unifiedroleassignmentmultiple"></a><span data-ttu-id="d87e2-103">Obter unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="d87e2-103">Get unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="d87e2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d87e2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d87e2-105">Recupere as propriedades e os relacionamentos de um objeto [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) .</span><span class="sxs-lookup"><span data-stu-id="d87e2-105">Retrieve the properties and relationships of a [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.</span></span> <span data-ttu-id="d87e2-106">Use este objeto para obter atribuições de função no Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="d87e2-106">Use this object for get role assignments in Microsoft Intune.</span></span> <span data-ttu-id="d87e2-107">Para outros aplicativos do Micrsoft 365 (como o Azure AD), use o [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d87e2-107">For other Micrsoft 365 applications (like Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d87e2-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="d87e2-108">Permissions</span></span>

<span data-ttu-id="d87e2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d87e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d87e2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d87e2-111">Permission type</span></span> | <span data-ttu-id="d87e2-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d87e2-112">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="d87e2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d87e2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d87e2-114">DeviceManagementRBAC. Read. All, DeviceManagementRBAC. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d87e2-114">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="d87e2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d87e2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d87e2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d87e2-116">Not supported.</span></span> |
| <span data-ttu-id="d87e2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d87e2-117">Application</span></span> | <span data-ttu-id="d87e2-118">DeviceManagementRBAC. Read. All, DeviceManagementRBAC. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="d87e2-118">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d87e2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d87e2-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/deviceManagement/roleAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d87e2-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d87e2-120">Optional query parameters</span></span>

<span data-ttu-id="d87e2-121">Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d87e2-121">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="d87e2-122">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d87e2-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d87e2-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d87e2-123">Request headers</span></span>

| <span data-ttu-id="d87e2-124">Nome</span><span class="sxs-lookup"><span data-stu-id="d87e2-124">Name</span></span>  | <span data-ttu-id="d87e2-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="d87e2-125">Description</span></span> |
|:----- |:----------- |
| <span data-ttu-id="d87e2-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="d87e2-126">Authorization</span></span> | <span data-ttu-id="d87e2-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d87e2-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d87e2-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d87e2-129">Request body</span></span>

<span data-ttu-id="d87e2-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d87e2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d87e2-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d87e2-131">Response</span></span>

<span data-ttu-id="d87e2-132">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d87e2-132">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d87e2-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d87e2-133">Examples</span></span>

### <a name="example-1-get-a-directory-scoped-roleassignmentmultiple-in-intune"></a><span data-ttu-id="d87e2-134">Exemplo 1: obter um roleAssignmentMultiple com escopo de diretório no Intune</span><span class="sxs-lookup"><span data-stu-id="d87e2-134">Example 1: Get a directory-scoped roleAssignmentMultiple in Intune</span></span>

#### <a name="request"></a><span data-ttu-id="d87e2-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d87e2-135">Request</span></span>

<span data-ttu-id="d87e2-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d87e2-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d87e2-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="d87e2-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentmultiple"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="d87e2-138">C#</span><span class="sxs-lookup"><span data-stu-id="d87e2-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignmentmultiple-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d87e2-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d87e2-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignmentmultiple-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d87e2-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d87e2-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignmentmultiple-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d87e2-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d87e2-141">Response</span></span>

<span data-ttu-id="d87e2-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d87e2-142">The following is an example of the response.</span></span>
> <span data-ttu-id="d87e2-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d87e2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-directory-scoped-roleassignmentmultiple-with-expand"></a><span data-ttu-id="d87e2-145">Exemplo 2: obter um roleAssignmentMultiple com escopo de diretório com`$expand`</span><span class="sxs-lookup"><span data-stu-id="d87e2-145">Example 2: Get a directory-scoped roleAssignmentMultiple with `$expand`</span></span>

#### <a name="request"></a><span data-ttu-id="d87e2-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d87e2-146">Request</span></span>

<span data-ttu-id="d87e2-147">Veja a seguir um exemplo da solicitação com o parâmetro `$expand` de consulta.</span><span class="sxs-lookup"><span data-stu-id="d87e2-147">The following is an example of the request with the `$expand` query parameter.</span></span>


# <a name="http"></a>[<span data-ttu-id="d87e2-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="d87e2-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1?$expand=roleDefinition,principals,directoryScopes
```
# <a name="c"></a>[<span data-ttu-id="d87e2-149">C#</span><span class="sxs-lookup"><span data-stu-id="d87e2-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d87e2-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d87e2-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d87e2-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d87e2-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d87e2-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="d87e2-152">Response</span></span>

<span data-ttu-id="d87e2-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d87e2-153">The following is an example of the response.</span></span>
> <span data-ttu-id="d87e2-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d87e2-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
