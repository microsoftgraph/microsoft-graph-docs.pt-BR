---
title: Obter unifiedRoleAssignmentMultiple
description: Recupere as propriedades e as relações de um objeto unifiedRoleAssignmentMultiple.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6b1aeecdae5b36e4c10768ee37b1505aba25687b
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334497"
---
# <a name="get-unifiedroleassignmentmultiple"></a><span data-ttu-id="2ef03-103">Obter unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="2ef03-103">Get unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="2ef03-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ef03-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ef03-105">Obter as propriedades e as relações de [um objeto unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) de um provedor RBAC.</span><span class="sxs-lookup"><span data-stu-id="2ef03-105">Get the properties and relationships of a [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object of an RBAC provider.</span></span> 

<span data-ttu-id="2ef03-106">No momento, há suporte para os seguintes provedores RBAC:</span><span class="sxs-lookup"><span data-stu-id="2ef03-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="2ef03-107">cloud PC</span><span class="sxs-lookup"><span data-stu-id="2ef03-107">cloud PC</span></span> 
- <span data-ttu-id="2ef03-108">gerenciamento de dispositivos (Intune)</span><span class="sxs-lookup"><span data-stu-id="2ef03-108">device management (Intune)</span></span>

<span data-ttu-id="2ef03-109">Para outros Microsoft 365 (como o Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2ef03-109">For other Microsoft 365 applications (like Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="2ef03-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="2ef03-110">Permissions</span></span>

<span data-ttu-id="2ef03-111">Dependendo do provedor RBAC e do tipo de permissão (delegado ou aplicativo) necessário, escolha na tabela a seguinte permissão com menos privilégios necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="2ef03-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="2ef03-112">Para saber mais, incluindo [ter cuidado antes](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) de escolher permissões mais privilegiadas, consulte [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ef03-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, see [Permissions](/graph/permissions-reference).</span></span> 

### <a name="for-cloud-pc-provider"></a><span data-ttu-id="2ef03-113">Para provedor de computadores na nuvem</span><span class="sxs-lookup"><span data-stu-id="2ef03-113">For Cloud PC provider</span></span>

|<span data-ttu-id="2ef03-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ef03-114">Permission type</span></span>      | <span data-ttu-id="2ef03-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2ef03-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ef03-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ef03-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="2ef03-117">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ef03-117">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>   |
|<span data-ttu-id="2ef03-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ef03-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ef03-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ef03-119">Not supported.</span></span>    |
|<span data-ttu-id="2ef03-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ef03-120">Application</span></span> | <span data-ttu-id="2ef03-121">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ef03-121">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>  |

### <a name="for-device-management-intune-provider"></a><span data-ttu-id="2ef03-122">Para o provedor de gerenciamento de dispositivos (Intune)</span><span class="sxs-lookup"><span data-stu-id="2ef03-122">For Device management (Intune) provider</span></span>

|<span data-ttu-id="2ef03-123">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2ef03-123">Permission type</span></span>      | <span data-ttu-id="2ef03-124">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2ef03-124">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ef03-125">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2ef03-125">Delegated (work or school account)</span></span> |  <span data-ttu-id="2ef03-126">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ef03-126">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span>   |
|<span data-ttu-id="2ef03-127">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2ef03-127">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ef03-128">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2ef03-128">Not supported.</span></span>    |
|<span data-ttu-id="2ef03-129">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ef03-129">Application</span></span> | <span data-ttu-id="2ef03-130">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ef03-130">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> |



## <a name="http-request"></a><span data-ttu-id="2ef03-131">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2ef03-131">HTTP request</span></span>

<span data-ttu-id="2ef03-132">Para obter as propriedades e as relações de um unifiedRoleAssignmentMultiple para um provedor de computadores na nuvem:</span><span class="sxs-lookup"><span data-stu-id="2ef03-132">To get the properties and relationships of a unifiedRoleAssignmentMultiple for a cloud PC provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/cloudPC/roleAssignments/{id}
```

<span data-ttu-id="2ef03-133">Para obter as propriedades e as relações de um unifiedRoleAssignmentMultiple para um provedor do Intune:</span><span class="sxs-lookup"><span data-stu-id="2ef03-133">To get the properties and relationships of a unifiedRoleAssignmentMultiple for an Intune provider:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /roleManagement/deviceManagement/roleAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2ef03-134">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2ef03-134">Optional query parameters</span></span>

<span data-ttu-id="2ef03-135">Este método dá suporte a Parâmetros de consulta do OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2ef03-135">This method supports OData query parameters to help customize the response.</span></span> <span data-ttu-id="2ef03-136">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="2ef03-136">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2ef03-137">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2ef03-137">Request headers</span></span>

| <span data-ttu-id="2ef03-138">Nome</span><span class="sxs-lookup"><span data-stu-id="2ef03-138">Name</span></span>  | <span data-ttu-id="2ef03-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ef03-139">Description</span></span> |
|:----- |:----------- |
| <span data-ttu-id="2ef03-140">Autorização</span><span class="sxs-lookup"><span data-stu-id="2ef03-140">Authorization</span></span> | <span data-ttu-id="2ef03-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2ef03-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ef03-143">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2ef03-143">Request body</span></span>

<span data-ttu-id="2ef03-144">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2ef03-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ef03-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ef03-145">Response</span></span>

<span data-ttu-id="2ef03-146">Se tiver êxito, este método retornará um código de resposta e `200 OK` o objeto [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2ef03-146">If successful, this method returns a `200 OK` response code and the requested [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2ef03-147">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2ef03-147">Examples</span></span>

### <a name="example-1-get-a-directory-scoped-roleassignmentmultiple-in-an-intune-provider"></a><span data-ttu-id="2ef03-148">Exemplo 1: Obter uma função com escopo de diretórioAssignmentMultiple em um provedor do Intune</span><span class="sxs-lookup"><span data-stu-id="2ef03-148">Example 1: Get a directory-scoped roleAssignmentMultiple in an Intune provider</span></span>

#### <a name="request"></a><span data-ttu-id="2ef03-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ef03-149">Request</span></span>

<span data-ttu-id="2ef03-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ef03-150">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2ef03-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ef03-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentmultiple_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1
```
# <a name="c"></a>[<span data-ttu-id="2ef03-152">C#</span><span class="sxs-lookup"><span data-stu-id="2ef03-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignmentmultiple-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ef03-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ef03-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignmentmultiple-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ef03-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ef03-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignmentmultiple-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2ef03-155">Java</span><span class="sxs-lookup"><span data-stu-id="2ef03-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignmentmultiple-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2ef03-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ef03-156">Response</span></span>

<span data-ttu-id="2ef03-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2ef03-157">The following is an example of the response.</span></span>
> <span data-ttu-id="2ef03-158">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2ef03-158">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-a-roleassignmentmultiple-assigned-to-a-group-in-an-intune-provider"></a><span data-ttu-id="2ef03-159">Exemplo 2: Obter uma funçãoAssignmentMultiple atribuída a um grupo em um provedor do Intune</span><span class="sxs-lookup"><span data-stu-id="2ef03-159">Example 2: Get a roleAssignmentMultiple assigned to a group in an Intune provider</span></span>

#### <a name="request"></a><span data-ttu-id="2ef03-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ef03-160">Request</span></span>

<span data-ttu-id="2ef03-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ef03-161">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="2ef03-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ef03-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentmultiple_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments?$filter = principalIds/any(x:x eq '564ae70c-73d9-476b-820b-fb61eb7384b9')
```
# <a name="c"></a>[<span data-ttu-id="2ef03-163">C#</span><span class="sxs-lookup"><span data-stu-id="2ef03-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignmentmultiple-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ef03-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ef03-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignmentmultiple-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ef03-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ef03-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignmentmultiple-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2ef03-166">Java</span><span class="sxs-lookup"><span data-stu-id="2ef03-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignmentmultiple-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2ef03-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ef03-167">Response</span></span>

<span data-ttu-id="2ef03-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2ef03-168">The following is an example of the response.</span></span>
> <span data-ttu-id="2ef03-169">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2ef03-169">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-3-get-a-directory-scoped-roleassignmentmultiple-in-an-intune-provider-with-expand"></a><span data-ttu-id="2ef03-170">Exemplo 3: Obter uma função com escopo de diretórioAssignmentMultiple em um provedor do Intune com `$expand`</span><span class="sxs-lookup"><span data-stu-id="2ef03-170">Example 3: Get a directory-scoped roleAssignmentMultiple in an Intune provider with `$expand`</span></span>

#### <a name="request"></a><span data-ttu-id="2ef03-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ef03-171">Request</span></span>

<span data-ttu-id="2ef03-172">A seguir, um exemplo da solicitação com o `$expand` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="2ef03-172">The following is an example of the request with the `$expand` query parameter.</span></span>


# <a name="http"></a>[<span data-ttu-id="2ef03-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ef03-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment_3"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1?$expand=roleDefinition,principals,directoryScopes
```
# <a name="c"></a>[<span data-ttu-id="2ef03-174">C#</span><span class="sxs-lookup"><span data-stu-id="2ef03-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ef03-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ef03-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ef03-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ef03-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2ef03-177">Java</span><span class="sxs-lookup"><span data-stu-id="2ef03-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2ef03-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ef03-178">Response</span></span>

<span data-ttu-id="2ef03-179">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2ef03-179">The following is an example of the response.</span></span>
> <span data-ttu-id="2ef03-180">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2ef03-180">**Note:** The response object shown here might be shortened for readability.</span></span>

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
### <a name="example-4-get-a-roleassignmentmultiple-in-a-cloud-pc-provider"></a><span data-ttu-id="2ef03-181">Exemplo 4: Obter uma roleAssignmentMultiple em um provedor de computadores na nuvem</span><span class="sxs-lookup"><span data-stu-id="2ef03-181">Example 4: Get a roleAssignmentMultiple in a cloud PC provider</span></span>

#### <a name="request"></a><span data-ttu-id="2ef03-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ef03-182">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2ef03-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ef03-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentmultiple_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/cloudPC/roleAssignments/dbe9d288-fd87-41f4-b33d-b498ed207096
```
# <a name="c"></a>[<span data-ttu-id="2ef03-184">C#</span><span class="sxs-lookup"><span data-stu-id="2ef03-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignmentmultiple-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ef03-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ef03-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignmentmultiple-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ef03-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ef03-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignmentmultiple-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2ef03-187">Java</span><span class="sxs-lookup"><span data-stu-id="2ef03-187">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignmentmultiple-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2ef03-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ef03-188">Response</span></span>
> <span data-ttu-id="2ef03-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2ef03-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/cloudPC/roleAssignments/$entity",
    "id": "dbe9d288-fd87-41f4-b33d-b498ed207096",
    "description": null,
    "displayName": "My test role assignment 1",
    "roleDefinitionId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
    "principalIds": [
        "8e811502-ebda-4782-8f81-071d17f0f892",
        "30e3492f-964c-4d73-88c6-986a53c6e2a0"
    ],
    "directoryScopeIds": [
        "/"
    ],
    "appScopeIds": []
}
```

### <a name="example-5-get-a-roleassignmentmultiple-in-a-cloud-pc-provider-with-expand"></a><span data-ttu-id="2ef03-191">Exemplo 5: Obter uma roleAssignmentMultiple em um provedor de computadores na nuvem com `$expand`</span><span class="sxs-lookup"><span data-stu-id="2ef03-191">Example 5: Get a roleAssignmentMultiple in a cloud PC provider with `$expand`</span></span>

#### <a name="request"></a><span data-ttu-id="2ef03-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2ef03-192">Request</span></span>

<span data-ttu-id="2ef03-193">A seguir, um exemplo da solicitação com o `$expand` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="2ef03-193">The following is an example of the request with the `$expand` query parameter.</span></span>


# <a name="http"></a>[<span data-ttu-id="2ef03-194">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ef03-194">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignment_3"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/cloudPC/roleAssignments/dbe9d288-fd87-41f4-b33d-b498ed207096?$expand=roleDefinition
```
# <a name="c"></a>[<span data-ttu-id="2ef03-195">C#</span><span class="sxs-lookup"><span data-stu-id="2ef03-195">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedroleassignment-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ef03-196">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ef03-196">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedroleassignment-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ef03-197">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ef03-197">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedroleassignment-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2ef03-198">Java</span><span class="sxs-lookup"><span data-stu-id="2ef03-198">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedroleassignment-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2ef03-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="2ef03-199">Response</span></span>
> <span data-ttu-id="2ef03-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2ef03-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignment"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/cloudPC/roleAssignments/$entity",
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
    "id": "dbe9d288-fd87-41f4-b33d-b498ed207096",
    "roleDefinitionId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
    "principalIds": ["8e811502-ebda-4782-8f81-071d17f0f892", "30e3492f-964c-4d73-88c6-986a53c6e2a0"],
    "directoryScopeIds": [
        "/"
    ],
    "appScopeIds": [],
    "roleDefinitions": {
        "id": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
        "description": "Have read and write access to all Cloud PC features.",
        "displayName": "Cloud PC Administrator",
        "isBuiltIn": true,
        "isEnabled": true,
        "resourceScopes": [
            "/"
        ],
        "templateId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
        "version": null,
        "rolePermissions": [
            {
                "allowedResourceActions": [
                    "Microsoft.CloudPC/CloudPCs/Read",
                    "Microsoft.CloudPC/CloudPCs/Reprovision",
                    "Microsoft.CloudPC/DeviceImages/Create",
                    "Microsoft.CloudPC/DeviceImages/Delete",
                    "Microsoft.CloudPC/DeviceImages/Read",
                    "Microsoft.CloudPC/OnPremisesConnections/Create",
                    "Microsoft.CloudPC/OnPremisesConnections/Delete",
                    "Microsoft.CloudPC/OnPremisesConnections/Read",
                    "Microsoft.CloudPC/OnPremisesConnections/Update",
                    "Microsoft.CloudPC/OnPremisesConnections/RunHealthChecks",
                    "Microsoft.CloudPC/OnPremisesConnections/UpdateAdDomainPassword",
                    "Microsoft.CloudPC/ProvisioningPolicies/Assign",
                    "Microsoft.CloudPC/ProvisioningPolicies/Create",
                    "Microsoft.CloudPC/ProvisioningPolicies/Delete",
                    "Microsoft.CloudPC/ProvisioningPolicies/Read",
                    "Microsoft.CloudPC/ProvisioningPolicies/Update",
                    "Microsoft.CloudPC/RoleAssignments/Create",
                    "Microsoft.CloudPC/RoleAssignments/Update",
                    "Microsoft.CloudPC/RoleAssignments/Delete",
                    "Microsoft.CloudPC/Roles/Read",
                    "Microsoft.CloudPC/SelfServiceSettings/Read",
                    "Microsoft.CloudPC/SelfServiceSettings/Update"
                ],
                "condition": null
            }
        ]
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


