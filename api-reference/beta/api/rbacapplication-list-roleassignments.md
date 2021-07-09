---
title: Listar unifiedRoleAssignments
description: Obter uma lista de objetos unifiedRoleAssignment.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 5c58ce5123bf7ea3bb29af5b5e67fb5e259d6c75
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351059"
---
# <a name="list-unifiedroleassignments"></a><span data-ttu-id="520cd-103">Listar unifiedRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="520cd-103">List unifiedRoleAssignments</span></span>

<span data-ttu-id="520cd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="520cd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="520cd-105">Obter uma lista de [objetos unifiedRoleAssignment](../resources/unifiedroleassignment.md) para o provedor.</span><span class="sxs-lookup"><span data-stu-id="520cd-105">Get a list of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) objects for the provider.</span></span>

<span data-ttu-id="520cd-106">No momento, há suporte para os seguintes provedores RBAC:</span><span class="sxs-lookup"><span data-stu-id="520cd-106">The following RBAC providers are currently supported:</span></span>
- <span data-ttu-id="520cd-107">directory (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="520cd-107">directory (Azure AD)</span></span>
- <span data-ttu-id="520cd-108">gerenciamento de direitos (Azure AD)</span><span class="sxs-lookup"><span data-stu-id="520cd-108">entitlement management (Azure AD)</span></span>

## <a name="permissions"></a><span data-ttu-id="520cd-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="520cd-109">Permissions</span></span>


<span data-ttu-id="520cd-110">Dependendo do provedor RBAC e do tipo de permissão (delegado ou aplicativo) necessário, escolha na tabela a seguinte permissão com menos privilégios necessária para chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="520cd-110">Depending on the RBAC provider and the permission type (delegated or application) that is needed, choose from the following table the least privileged permission required to call this API.</span></span> <span data-ttu-id="520cd-111">Para saber mais, incluindo [tomar cuidado](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) antes de escolher as permissões mais privilegiadas, pesquise as seguintes permissões em [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="520cd-111">To learn more, including [taking caution](/graph/auth/auth-concepts#best-practices-for-requesting-permissions) before choosing more privileged permissions, search for the following permissions in [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-directory-azure-ad-provider"></a><span data-ttu-id="520cd-112">Provedor do Azure AD (Diretório)</span><span class="sxs-lookup"><span data-stu-id="520cd-112">For Directory (Azure AD) provider</span></span>

|<span data-ttu-id="520cd-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="520cd-113">Permission type</span></span>      | <span data-ttu-id="520cd-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="520cd-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="520cd-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="520cd-115">Delegated (work or school account)</span></span> |  <span data-ttu-id="520cd-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="520cd-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="520cd-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="520cd-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="520cd-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="520cd-118">Not supported.</span></span>    |
|<span data-ttu-id="520cd-119">Application</span><span class="sxs-lookup"><span data-stu-id="520cd-119">Application</span></span> | <span data-ttu-id="520cd-120">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="520cd-120">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

### <a name="for-entitlement-management-provider"></a><span data-ttu-id="520cd-121">Para provedor de gerenciamento de direitos</span><span class="sxs-lookup"><span data-stu-id="520cd-121">For Entitlement management provider</span></span>

|<span data-ttu-id="520cd-122">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="520cd-122">Permission type</span></span>      | <span data-ttu-id="520cd-123">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="520cd-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="520cd-124">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="520cd-124">Delegated (work or school account)</span></span> |  <span data-ttu-id="520cd-125">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="520cd-125">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>   |
|<span data-ttu-id="520cd-126">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="520cd-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="520cd-127">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="520cd-127">Not supported.</span></span>    |
|<span data-ttu-id="520cd-128">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="520cd-128">Application</span></span> | <span data-ttu-id="520cd-129">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="520cd-129">Not supported.</span></span> |


## <a name="http-request"></a><span data-ttu-id="520cd-130">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="520cd-130">HTTP request</span></span>

<span data-ttu-id="520cd-131">Para listar atribuições de função para um provedor de diretórios:</span><span class="sxs-lookup"><span data-stu-id="520cd-131">To list role assignments for a directory provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleAssignments?$filter=principalId eq '{principal id}'

GET /roleManagement/directory/roleAssignments?$filter=roleDefinitionId eq '{roleDefinition id}'
```

<span data-ttu-id="520cd-132">Para listar atribuições de função para o provedor de gerenciamento de direitos:</span><span class="sxs-lookup"><span data-stu-id="520cd-132">To list role assignments for the entitlement management provider:</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/entitlementManagement/roleAssignments?$filter=principalId eq '{principal id}'

GET /roleManagement/entitlementManagement/roleAssignments?$filter=roleDefinitionId eq '{roleDefinition id}'
```

## <a name="query-parameters"></a><span data-ttu-id="520cd-133">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="520cd-133">Query parameters</span></span>

<span data-ttu-id="520cd-134">Essa operação requer `$filter` o parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="520cd-134">This operation requires the `$filter` query parameter.</span></span> <span data-ttu-id="520cd-135">Você pode filtrar as `roleDefinitionId` propriedades `principalId` ou.</span><span class="sxs-lookup"><span data-stu-id="520cd-135">You can filter on the `roleDefinitionId` or `principalId` properties.</span></span> <span data-ttu-id="520cd-136">A propriedade pode ser uma ID de objeto de função ou uma ID de objeto `roleDefinitionId` de modelo de função.</span><span class="sxs-lookup"><span data-stu-id="520cd-136">The `roleDefinitionId` property can be either a role object ID or a role template object ID.</span></span> <span data-ttu-id="520cd-137">O `$expand` parâmetro de consulta também é suportado na entidade **principal**.</span><span class="sxs-lookup"><span data-stu-id="520cd-137">The `$expand` query parameter is also supported on **principal**.</span></span> <span data-ttu-id="520cd-138">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="520cd-138">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="520cd-139">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="520cd-139">Request headers</span></span>

| <span data-ttu-id="520cd-140">Nome</span><span class="sxs-lookup"><span data-stu-id="520cd-140">Name</span></span>      |<span data-ttu-id="520cd-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="520cd-141">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="520cd-142">Autorização</span><span class="sxs-lookup"><span data-stu-id="520cd-142">Authorization</span></span> | <span data-ttu-id="520cd-143">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="520cd-143">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="520cd-144">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="520cd-144">Request body</span></span>

<span data-ttu-id="520cd-145">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="520cd-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="520cd-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="520cd-146">Response</span></span>

<span data-ttu-id="520cd-147">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos unifiedRoleAssignment](../resources/unifiedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="520cd-147">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="520cd-148">Exemplos</span><span class="sxs-lookup"><span data-stu-id="520cd-148">Examples</span></span>

### <a name="example-1-request-using-filter-on-role-definition-id-and-expand-principal"></a><span data-ttu-id="520cd-149">Exemplo 1: Solicitar usando $filter ID de definição de função e expandir principal</span><span class="sxs-lookup"><span data-stu-id="520cd-149">Example 1: Request using $filter on role definition ID and expand principal</span></span>

#### <a name="request"></a><span data-ttu-id="520cd-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="520cd-150">Request</span></span>

<span data-ttu-id="520cd-151">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="520cd-151">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="520cd-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="520cd-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roleAssignments_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments?$filter=roleDefinitionId eq '62e90394-69f5-4237-9190-012177145e10'&$expand=principal
```
# <a name="c"></a>[<span data-ttu-id="520cd-153">C#</span><span class="sxs-lookup"><span data-stu-id="520cd-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roleassignments-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="520cd-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="520cd-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roleassignments-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="520cd-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="520cd-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roleassignments-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="520cd-156">Java</span><span class="sxs-lookup"><span data-stu-id="520cd-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-roleassignments-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="520cd-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="520cd-157">Response</span></span>

<span data-ttu-id="520cd-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="520cd-158">The following is an example of the response.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleAssignments(principal())",
    "value": [
        {
            "id": "lAPpYvVpN0KRkAEhdxReEMmO4KwRqtpKkUWt3wOYIz4-1",
            "principalId": "ace08ec9-aa11-4ada-9145-addf0398233e",
            "resourceScope": "/",
            "directoryScopeId": "/",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principal": {
                "@odata.type": "#microsoft.graph.user",
                "id": "ace08ec9-aa11-4ada-9145-addf0398233e",
                "deletedDateTime": null,
                "accountEnabled": true,
                "ageGroup": null,
                "businessPhones": [],
                "city": "Redmond",
                "createdDateTime": "2019-02-22T20:29:07Z",
                "creationType": null,
                "companyName": null,
                "consentProvidedForMinor": null,
                "country": "US",
                "department": "Office of the CEO",
                "displayName": "Joey Cruz",
                "employeeId": null,
                "faxNumber": null,
                "givenName": "Joey",
                "imAddresses": [
                    "joeyc@woodgrove.ms"
                ],
                "infoCatalogs": [],
                "isResourceAccount": null,
                "jobTitle": "Chief Security Officer",
                "legalAgeGroupClassification": null,
                "mail": "joeyc@woodgrove.ms",
                "mailNickname": "joeyc",
                "mobilePhone": null,
                "onPremisesDistinguishedName": null,
                "officeLocation": null,
                "userType": "Member",   

            }
        },
        {
            "id": "lAPpYvVpN0KRkAEhdxReEC6Xh29-LklLmYDrOIi9z-E-1",
            "principalId": "6f87972e-2e7e-4b49-9980-eb3888bdcfe1",
            "resourceScope": "/",
            "directoryScopeId": "/",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principal": {
                "@odata.type": "#microsoft.graph.user",
                "id": "6f87972e-2e7e-4b49-9980-eb3888bdcfe1",
                "deletedDateTime": null,
                "accountEnabled": true,
                "ageGroup": null,
                "businessPhones": [],
                "city": null,
                "createdDateTime": "2019-07-18T01:38:36Z",
                "creationType": "Invitation",
                "companyName": null,
                "consentProvidedForMinor": null,
                "country": null,
                "department": null,
                "displayName": "Kalyan Krishna",
                "employeeId": null,
                "faxNumber": null,
                "givenName": null,
                "imAddresses": [],
                "userType": "Guest",
    
            }
        },
        {
            "id": "lAPpYvVpN0KRkAEhdxReEMgc_BA2rIZBuZsM-BSqLdU-1",
            "principalId": "10fc1cc8-ac36-4186-b99b-0cf814aa2dd5",
            "resourceScope": "/",
            "directoryScopeId": "/",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10",
            "principal": {
                "@odata.type": "#microsoft.graph.user",
                "id": "10fc1cc8-ac36-4186-b99b-0cf814aa2dd5",
                "deletedDateTime": null,
                "accountEnabled": true,
                "ageGroup": null,
                "businessPhones": [],
                "city": null,
                "createdDateTime": "2019-11-13T21:54:27Z",
                "creationType": "Invitation",
                "companyName": null,
                "consentProvidedForMinor": null,
                "country": null,
                "department": null,
                "displayName": "Markie Downing",
                "employeeId": null,
                "faxNumber": null,
                "givenName": null,
                "imAddresses": [],
                "userType": "Guest",
        
            }
        }
    ]
}
```

### <a name="example-2-request-using-a-filter-on-principal-id"></a><span data-ttu-id="520cd-159">Exemplo 2: Solicitar usando um filtro na ID principal</span><span class="sxs-lookup"><span data-stu-id="520cd-159">Example 2: Request using a filter on principal ID</span></span>

#### <a name="request"></a><span data-ttu-id="520cd-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="520cd-160">Request</span></span>

<span data-ttu-id="520cd-161">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="520cd-161">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="520cd-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="520cd-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roleAssignments_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments?$filter = principalId eq 'f1847572-48aa-47aa-96a3-2ec61904f41f'
```
# <a name="c"></a>[<span data-ttu-id="520cd-163">C#</span><span class="sxs-lookup"><span data-stu-id="520cd-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roleassignments-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="520cd-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="520cd-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roleassignments-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="520cd-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="520cd-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roleassignments-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="520cd-166">Java</span><span class="sxs-lookup"><span data-stu-id="520cd-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-roleassignments-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="520cd-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="520cd-167">Response</span></span>

<span data-ttu-id="520cd-168">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="520cd-168">The following is an example of the response.</span></span>

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
            "id": "lAPpYvVpN0KRkAEhdxReEHJ1hPGqSKpHlqMuxhkE9B8-1",
            "principalId": "f1847572-48aa-47aa-96a3-2ec61904f41f",
            "resourceScope": "/",
            "directoryScopeId": "/",
            "roleDefinitionId": "62e90394-69f5-4237-9190-012177145e10"
        },
        {
            "id": "LJnv8vs6uUa3z6Em7nTEUXJ1hPGqSKpHlqMuxhkE9B8-1",
            "principalId": "f1847572-48aa-47aa-96a3-2ec61904f41f",
            "resourceScope": "/",
            "directoryScopeId": "/",
            "roleDefinitionId": "f2ef992c-3afb-46b9-b7cf-a126ee74c451"
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


