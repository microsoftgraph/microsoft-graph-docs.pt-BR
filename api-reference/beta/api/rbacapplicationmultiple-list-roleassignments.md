---
title: Listar UnifiedRoleAssignmentMultiple
description: Recupere as propriedades e as relações do objeto unifiedRoleAssignmentMultiple.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 0a70bfab57b398e0ac904cee02411a7b7c665bf9
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869000"
---
# <a name="list-unifiedroleassignmentmultiple"></a><span data-ttu-id="ee089-103">Listar UnifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="ee089-103">List unifiedRoleAssignmentMultiple</span></span>

<span data-ttu-id="ee089-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee089-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee089-105">Obter uma lista de [objetos unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) para um provedor RBAC.</span><span class="sxs-lookup"><span data-stu-id="ee089-105">Get a list of [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) objects for an RBAC provider.</span></span>

<span data-ttu-id="ee089-106">No momento, há suporte para os seguintes provedores RBAC:</span><span class="sxs-lookup"><span data-stu-id="ee089-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="ee089-107">cloud PC</span><span class="sxs-lookup"><span data-stu-id="ee089-107">cloud PC</span></span> 
- <span data-ttu-id="ee089-108">gerenciamento de dispositivos (Intune)</span><span class="sxs-lookup"><span data-stu-id="ee089-108">device management (Intune)</span></span>

<span data-ttu-id="ee089-109">Para outros Microsoft 365 (como o Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span><span class="sxs-lookup"><span data-stu-id="ee089-109">For other Microsoft 365 applications (like Azure AD), use [unifiedRoleAssignment](../resources/unifiedroleassignment.md).</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="ee089-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="ee089-110">Permissions</span></span>

<span data-ttu-id="ee089-111">Dependendo do provedor RBAC e do tipo de permissão (delegado ou aplicativo) necessário, escolha na tabela a seguinte permissão com menos privilégios necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="ee089-111">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="ee089-112">Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher as permissões mais privilegiadas, pesquise as seguintes permissões em [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ee089-112">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span> 

|<span data-ttu-id="ee089-113">Provedor com suporte</span><span class="sxs-lookup"><span data-stu-id="ee089-113">Supported provider</span></span>      | <span data-ttu-id="ee089-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ee089-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="ee089-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ee089-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee089-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ee089-116">Application</span></span> |
|:-----------------------|:------------------------------------|:---------------------------------------|:------------|
| <span data-ttu-id="ee089-117">Cloud PC</span><span class="sxs-lookup"><span data-stu-id="ee089-117">Cloud PC</span></span> | <span data-ttu-id="ee089-118">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee089-118">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span> | <span data-ttu-id="ee089-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee089-119">Not supported.</span></span> | <span data-ttu-id="ee089-120">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee089-120">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span> |
| <span data-ttu-id="ee089-121">Intune</span><span class="sxs-lookup"><span data-stu-id="ee089-121">Intune</span></span> | <span data-ttu-id="ee089-122">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee089-122">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> | <span data-ttu-id="ee089-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ee089-123">Not supported.</span></span>| <span data-ttu-id="ee089-124">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee089-124">DeviceManagementRBAC.Read.All, DeviceManagementRBAC.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee089-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ee089-125">HTTP request</span></span>

<span data-ttu-id="ee089-126">Para listar atribuições de função para um provedor de computadores na nuvem:</span><span class="sxs-lookup"><span data-stu-id="ee089-126">To list role assignments for a cloud PC provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/cloudPc/roleAssignments
```

<span data-ttu-id="ee089-127">Para listar atribuições de função para um provedor do Intune:</span><span class="sxs-lookup"><span data-stu-id="ee089-127">To list role assignments for an Intune provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/deviceManagement/roleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ee089-128">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ee089-128">Optional query parameters</span></span>
<span data-ttu-id="ee089-129">Você pode filtrar as `roleDefinitionId` propriedades `principalId` ou.</span><span class="sxs-lookup"><span data-stu-id="ee089-129">You can filter on the `roleDefinitionId` or `principalId` properties.</span></span> <span data-ttu-id="ee089-130">A propriedade pode ser uma ID de objeto de função ou uma ID de objeto `roleDefinitionId` de modelo de função.</span><span class="sxs-lookup"><span data-stu-id="ee089-130">The `roleDefinitionId` property can be either a role object ID or a role template object ID.</span></span> <span data-ttu-id="ee089-131">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ee089-131">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ee089-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ee089-132">Request headers</span></span>

| <span data-ttu-id="ee089-133">Nome</span><span class="sxs-lookup"><span data-stu-id="ee089-133">Name</span></span> | <span data-ttu-id="ee089-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee089-134">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="ee089-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="ee089-135">Authorization</span></span> | <span data-ttu-id="ee089-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ee089-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ee089-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ee089-138">Request body</span></span>

<span data-ttu-id="ee089-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ee089-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee089-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee089-140">Response</span></span>

<span data-ttu-id="ee089-141">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ee089-141">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee089-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ee089-142">Example</span></span>

### <a name="example-1-list-the-role-assignments-for-a-specific-principal-for-an-intune-provider"></a><span data-ttu-id="ee089-143">Exemplo 1: listar as atribuições de função para uma entidade específica para um provedor do Intune</span><span class="sxs-lookup"><span data-stu-id="ee089-143">Example 1: List the role assignments for a specific principal for an Intune provider</span></span>

### <a name="request"></a><span data-ttu-id="ee089-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee089-144">Request</span></span>

<span data-ttu-id="ee089-145">Veja a seguir um exemplo da solicitação:</span><span class="sxs-lookup"><span data-stu-id="ee089-145">The following is an example of the request:</span></span>

<!-- {
  "blockType": "request",
  "name": "list_unifiedroleassignmentmultiple"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments/$filter=principalId eq '9e47fc6f-2d7a-464c-944e-d3dd0de522e4'
```

### <a name="response"></a><span data-ttu-id="ee089-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee089-146">Response</span></span>

<span data-ttu-id="ee089-147">Veja a seguir um exemplo da resposta:</span><span class="sxs-lookup"><span data-stu-id="ee089-147">The following is an example of the response:</span></span>
> <span data-ttu-id="ee089-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ee089-148">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/deviceManagement/roleAssignments/$entity",
    "value": [ 
       {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
            "id": "lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principalIds[]": ["9e47fc6f-2d7a-464c-944e-d3dd0de522e4", "f8ca5a85-489a-49a0-b555-0a6d81e56f0d"],
            "directoryScopeIds[]": ["28ca5a85-489a-49a0-b555-0a6d81e56f0", "8152656a-cf9a-4928-a457-1512d4cae295"]
       },
       {
            "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
            "id": "2BNpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SWRD-2",
            "roleDefinitionId": "9e47fc6f-2d7a-464c-944e-d3dd0de522e4",
            "principalIds[]": ["9e47fc6f-2d7a-464c-944e-d3dd0de522e4", "53a6c08d-0227-41bd-8bc6-2728df6be749", "a4991fe1-6d7c-427c-969b-bda6df78c458"],
            "appScopeIds[]": ["28ca5a85-489a-49a0-b555-0a6d81e56f0"]
       }
    ]
}
```
### <a name="example-2-list-role-assignments-for-a-cloud-pc-provider"></a><span data-ttu-id="ee089-149">Exemplo 2: Listar atribuições de função para um provedor de computadores na nuvem</span><span class="sxs-lookup"><span data-stu-id="ee089-149">Example 2: List role assignments for a cloud PC provider</span></span>

### <a name="request"></a><span data-ttu-id="ee089-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee089-150">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ee089-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee089-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpcunifiedroleassignmentmultiple_1"
}-->

```msgraph-interactive
GET  https://graph.microsoft.com/beta/roleManagement/cloudPC/roleAssignments
```
# <a name="c"></a>[<span data-ttu-id="ee089-152">C#</span><span class="sxs-lookup"><span data-stu-id="ee089-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-cloudpcunifiedroleassignmentmultiple-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ee089-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee089-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-cloudpcunifiedroleassignmentmultiple-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ee089-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee089-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-cloudpcunifiedroleassignmentmultiple-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ee089-155">Java</span><span class="sxs-lookup"><span data-stu-id="ee089-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-cloudpcunifiedroleassignmentmultiple-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ee089-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee089-156">Response</span></span>

> <span data-ttu-id="ee089-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ee089-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/cloudPC/roleAssignments/$entity",
    "value": [
        {
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
        },
        {
            "id": "fad74173-3fe3-4e64-9a80-297bdad2b36e",
            "description": null,
            "displayName": "My test role assignment 2",
            "roleDefinitionId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
            "principalIds": [
                "8e811502-ebda-4782-8f81-071d17f0f892",
            ],
            "directoryScopeIds": [
                "/"
            ],
            "appScopeIds": []
        }
    ]
}
```

### <a name="example-3-list-role-assignments-for-specific-role-of-a-cloud-pc-provider"></a><span data-ttu-id="ee089-159">Exemplo 3: Listar atribuições de função para função específica de um provedor de computadores na nuvem</span><span class="sxs-lookup"><span data-stu-id="ee089-159">Example 3: List role assignments for specific role of a cloud PC provider</span></span>

### <a name="request"></a><span data-ttu-id="ee089-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ee089-160">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ee089-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="ee089-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_cloudpcunifiedroleassignmentmultiple_2"
}-->

```msgraph-interactive
GET  https://graph.microsoft.com/beta/roleManagement/cloudPC/roleAssignments?$filter=roleDefinitionId eq 'b5c08161-a7af-481c-ace2-a20a69a48fb1'
```
# <a name="c"></a>[<span data-ttu-id="ee089-162">C#</span><span class="sxs-lookup"><span data-stu-id="ee089-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-cloudpcunifiedroleassignmentmultiple-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ee089-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ee089-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-cloudpcunifiedroleassignmentmultiple-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ee089-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ee089-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-cloudpcunifiedroleassignmentmultiple-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ee089-165">Java</span><span class="sxs-lookup"><span data-stu-id="ee089-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-cloudpcunifiedroleassignmentmultiple-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ee089-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="ee089-166">Response</span></span>

> <span data-ttu-id="ee089-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ee089-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/cloudPC/roleAssignments",
    "value": [{
        "id": "ed9e247f-f23b-4d72-9e8c-97fa6f385246",
        "description": "",
        "displayName": "test",
        "roleDefinitionId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
        "principalIds": ["689c9051-77ff-4f14-9b39-3d22de07321a"],
        "directoryScopeIds": ["/"],
        "appScopeIds": []
    }, {
        "id": "3d8e564b-761a-4b32-8f50-63d555f7bc00",
        "description": "test1",
        "displayName": "AssignmentTest",
        "roleDefinitionId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
        "principalIds": ["0ec7855b-4057-4b7c-9217-09ee9bf4dfd7"],
        "directoryScopeIds": ["/"],
        "appScopeIds": []
    }, {
        "id": "f36a3269-d03d-4d33-81e7-190bded40ad2",
        "description": "",
        "displayName": "test3",
        "roleDefinitionId": "b5c08161-a7af-481c-ace2-a20a69a48fb1",
        "principalIds": ["e4ea53cf-cdd6-46b5-bf38-570033a0fba3"],
        "directoryScopeIds": ["/"],
        "appScopeIds": []
    }]
}
```
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List roleAssignmentsMultiple",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


