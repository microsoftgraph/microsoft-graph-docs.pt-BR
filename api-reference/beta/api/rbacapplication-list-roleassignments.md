---
title: Listar unifiedRoleAssignments
description: Obter uma lista de objetos unifiedRoleAssignment.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 2877f9bca06eed962257e2c8c43c5f776d06ff76
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241139"
---
# <a name="list-unifiedroleassignments"></a><span data-ttu-id="f23a3-103">Listar unifiedRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="f23a3-103">List unifiedRoleAssignments</span></span>

<span data-ttu-id="f23a3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f23a3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f23a3-105">Obter uma lista de [objetos unifiedRoleAssignment](../resources/unifiedroleassignment.md) para o provedor.</span><span class="sxs-lookup"><span data-stu-id="f23a3-105">Get a list of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) objects for the provider.</span></span>

## <a name="permissions"></a><span data-ttu-id="f23a3-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f23a3-106">Permissions</span></span>

<span data-ttu-id="f23a3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f23a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f23a3-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f23a3-109">Permission type</span></span>      | <span data-ttu-id="f23a3-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f23a3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f23a3-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f23a3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f23a3-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f23a3-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f23a3-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f23a3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f23a3-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f23a3-114">Not supported.</span></span>    |
|<span data-ttu-id="f23a3-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f23a3-115">Application</span></span> | <span data-ttu-id="f23a3-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f23a3-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f23a3-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f23a3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleAssignments?$filter=principalId eq '{principal id}'

GET /roleManagement/directory/roleAssignments?$filter=roleDefinitionId eq '{roleDefinition id}'
```

## <a name="query-parameters"></a><span data-ttu-id="f23a3-118">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="f23a3-118">Query parameters</span></span>

<span data-ttu-id="f23a3-119">Essa operação requer `$filter` o parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="f23a3-119">This operation requires the `$filter` query parameter.</span></span> <span data-ttu-id="f23a3-120">Você pode filtrar as `roleDefinitionId` propriedades `principalId` ou.</span><span class="sxs-lookup"><span data-stu-id="f23a3-120">You can filter on the `roleDefinitionId` or `principalId` properties.</span></span> <span data-ttu-id="f23a3-121">A propriedade pode ser uma ID de objeto de função ou uma ID de objeto `roleDefinitionId` de modelo de função.</span><span class="sxs-lookup"><span data-stu-id="f23a3-121">The `roleDefinitionId` property can be either a role object ID or a role template object ID.</span></span> <span data-ttu-id="f23a3-122">O `$expand` parâmetro de consulta também é suportado na entidade **principal**.</span><span class="sxs-lookup"><span data-stu-id="f23a3-122">The `$expand` query parameter is also supported on **principal**.</span></span> <span data-ttu-id="f23a3-123">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f23a3-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f23a3-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f23a3-124">Request headers</span></span>

| <span data-ttu-id="f23a3-125">Nome</span><span class="sxs-lookup"><span data-stu-id="f23a3-125">Name</span></span>      |<span data-ttu-id="f23a3-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="f23a3-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f23a3-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="f23a3-127">Authorization</span></span> | <span data-ttu-id="f23a3-128">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="f23a3-128">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f23a3-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f23a3-129">Request body</span></span>

<span data-ttu-id="f23a3-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f23a3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f23a3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="f23a3-131">Response</span></span>

<span data-ttu-id="f23a3-132">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos unifiedRoleAssignment](../resources/unifiedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f23a3-132">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f23a3-133">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f23a3-133">Examples</span></span>

### <a name="example-1-request-using-filter-on-role-definition-id-and-expand-principal"></a><span data-ttu-id="f23a3-134">Exemplo 1: Solicitar usando $filter ID de definição de função e expandir principal</span><span class="sxs-lookup"><span data-stu-id="f23a3-134">Example 1: Request using $filter on role definition ID and expand principal</span></span>

#### <a name="request"></a><span data-ttu-id="f23a3-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f23a3-135">Request</span></span>

<span data-ttu-id="f23a3-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f23a3-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f23a3-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="f23a3-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roleAssignments_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments?$filter=roleDefinitionId eq '62e90394-69f5-4237-9190-012177145e10'&$expand=principal
```
# <a name="c"></a>[<span data-ttu-id="f23a3-138">C#</span><span class="sxs-lookup"><span data-stu-id="f23a3-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roleassignments-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f23a3-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f23a3-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roleassignments-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f23a3-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f23a3-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roleassignments-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f23a3-141">Java</span><span class="sxs-lookup"><span data-stu-id="f23a3-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-roleassignments-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f23a3-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="f23a3-142">Response</span></span>

<span data-ttu-id="f23a3-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f23a3-143">The following is an example of the response.</span></span>

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

### <a name="example-2-request-using-a-filter-on-principal-id"></a><span data-ttu-id="f23a3-144">Exemplo 2: Solicitar usando um filtro na ID principal</span><span class="sxs-lookup"><span data-stu-id="f23a3-144">Example 2: Request using a filter on principal ID</span></span>

#### <a name="request"></a><span data-ttu-id="f23a3-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f23a3-145">Request</span></span>

<span data-ttu-id="f23a3-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f23a3-146">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f23a3-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="f23a3-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roleAssignments_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments?$filter = principalId eq 'f1847572-48aa-47aa-96a3-2ec61904f41f'
```
# <a name="c"></a>[<span data-ttu-id="f23a3-148">C#</span><span class="sxs-lookup"><span data-stu-id="f23a3-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roleassignments-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f23a3-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f23a3-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roleassignments-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f23a3-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f23a3-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roleassignments-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f23a3-151">Java</span><span class="sxs-lookup"><span data-stu-id="f23a3-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-roleassignments-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f23a3-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="f23a3-152">Response</span></span>

<span data-ttu-id="f23a3-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f23a3-153">The following is an example of the response.</span></span>

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


