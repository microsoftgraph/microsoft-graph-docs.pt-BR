---
title: Listar unifiedRoleAssignments
description: Obter uma lista de objetos unifiedRoleAssignment.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 5b4066c59eedb5ddc98912f263e586a095dde4eb
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440938"
---
# <a name="list-unifiedroleassignments"></a><span data-ttu-id="12ea7-103">Listar unifiedRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="12ea7-103">List unifiedRoleAssignments</span></span>

<span data-ttu-id="12ea7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12ea7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12ea7-105">Obter uma lista de [objetos unifiedRoleAssignment](../resources/unifiedroleassignment.md) para o provedor.</span><span class="sxs-lookup"><span data-stu-id="12ea7-105">Get a list of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) objects for the provider.</span></span>

## <a name="permissions"></a><span data-ttu-id="12ea7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="12ea7-106">Permissions</span></span>

<span data-ttu-id="12ea7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12ea7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12ea7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12ea7-109">Permission type</span></span>      | <span data-ttu-id="12ea7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="12ea7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="12ea7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12ea7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="12ea7-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="12ea7-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="12ea7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12ea7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12ea7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12ea7-114">Not supported.</span></span>    |
|<span data-ttu-id="12ea7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12ea7-115">Application</span></span> | <span data-ttu-id="12ea7-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12ea7-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="12ea7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12ea7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="12ea7-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="12ea7-118">Optional query parameters</span></span>

<span data-ttu-id="12ea7-119">Essa operação requer `$filter` o parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="12ea7-119">This operation requires the `$filter` query parameter.</span></span> <span data-ttu-id="12ea7-120">Você pode filtrar as `roleDefinitionId` propriedades `principalId` ou.</span><span class="sxs-lookup"><span data-stu-id="12ea7-120">You can filter on the `roleDefinitionId` or `principalId` properties.</span></span> <span data-ttu-id="12ea7-121">A propriedade pode ser uma ID de objeto de função ou uma ID de objeto `roleDefinitionId` de modelo de função.</span><span class="sxs-lookup"><span data-stu-id="12ea7-121">The `roleDefinitionId` property can be either a role object ID or a role template object ID.</span></span> <span data-ttu-id="12ea7-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="12ea7-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="12ea7-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12ea7-123">Request headers</span></span>

| <span data-ttu-id="12ea7-124">Nome</span><span class="sxs-lookup"><span data-stu-id="12ea7-124">Name</span></span>      |<span data-ttu-id="12ea7-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="12ea7-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="12ea7-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="12ea7-126">Authorization</span></span> | <span data-ttu-id="12ea7-127">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="12ea7-127">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="12ea7-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12ea7-128">Request body</span></span>

<span data-ttu-id="12ea7-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="12ea7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12ea7-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="12ea7-130">Response</span></span>

<span data-ttu-id="12ea7-131">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos unifiedRoleAssignment](../resources/unifiedroleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12ea7-131">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleAssignment](../resources/unifiedroleassignment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="12ea7-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="12ea7-132">Examples</span></span>

### <a name="example-1-request-using-a-filter-on-role-definition-id"></a><span data-ttu-id="12ea7-133">Exemplo 1: Solicitar usando um filtro na ID de definição de função</span><span class="sxs-lookup"><span data-stu-id="12ea7-133">Example 1: Request using a filter on role definition ID</span></span>

#### <a name="request"></a><span data-ttu-id="12ea7-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12ea7-134">Request</span></span>

<span data-ttu-id="12ea7-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="12ea7-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="12ea7-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="12ea7-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roleAssignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments?$filter=roleDefinitionId eq '62e90394-69f5-4237-9190-012177145e10'&$expand=principal
```
# <a name="c"></a>[<span data-ttu-id="12ea7-137">C#</span><span class="sxs-lookup"><span data-stu-id="12ea7-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="12ea7-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="12ea7-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="12ea7-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="12ea7-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="12ea7-140">Java</span><span class="sxs-lookup"><span data-stu-id="12ea7-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-roleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="12ea7-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="12ea7-141">Response</span></span>

<span data-ttu-id="12ea7-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="12ea7-142">The following is an example of the response.</span></span>

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

### <a name="example-2-request-using-a-filter-on-principal-id"></a><span data-ttu-id="12ea7-143">Exemplo 2: Solicitar usando um filtro na ID principal</span><span class="sxs-lookup"><span data-stu-id="12ea7-143">Example 2: Request using a filter on principal ID</span></span>

#### <a name="request"></a><span data-ttu-id="12ea7-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12ea7-144">Request</span></span>

<span data-ttu-id="12ea7-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="12ea7-145">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="12ea7-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="12ea7-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roleAssignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments?$filter = principalId eq 'f1847572-48aa-47aa-96a3-2ec61904f41f'
```
# <a name="c"></a>[<span data-ttu-id="12ea7-147">C#</span><span class="sxs-lookup"><span data-stu-id="12ea7-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="12ea7-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="12ea7-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="12ea7-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="12ea7-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="12ea7-150">Java</span><span class="sxs-lookup"><span data-stu-id="12ea7-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-roleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="12ea7-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="12ea7-151">Response</span></span>

<span data-ttu-id="12ea7-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="12ea7-152">The following is an example of the response.</span></span>

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


