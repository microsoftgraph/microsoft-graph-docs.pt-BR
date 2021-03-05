---
title: Listar appRoleAssignments concedido a um usuário
description: Recuperar a lista de atribuições de funções do aplicativo concedidas a um usuário.
localization_priority: Priority
doc_type: apiPageType
ms.prod: users
author: psignoret
ms.openlocfilehash: ce56a5cbaae9f72d5cce6a890aec67c5f40b7930
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444445"
---
# <a name="list-approleassignments-granted-to-a-user"></a><span data-ttu-id="f7d83-103">Listar appRoleAssignments concedido a um usuário</span><span class="sxs-lookup"><span data-stu-id="f7d83-103">List appRoleAssignments granted to a user</span></span>

<span data-ttu-id="f7d83-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7d83-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="f7d83-105">Recuperar a lista[appRoleAssignment](../resources/approleassignment.md) concedida a um usuário.</span><span class="sxs-lookup"><span data-stu-id="f7d83-105">Retrieve the list of [appRoleAssignment](../resources/approleassignment.md) that a user has been granted.</span></span> <span data-ttu-id="f7d83-106">Essa operação também retorna funções de aplicativo atribuídas a grupos dos quais o usuário é membro direto.</span><span class="sxs-lookup"><span data-stu-id="f7d83-106">This operation also returns app roles assigned to groups that the user is a direct member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7d83-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f7d83-107">Permissions</span></span>

<span data-ttu-id="f7d83-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7d83-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7d83-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7d83-110">Permission type</span></span>      | <span data-ttu-id="f7d83-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f7d83-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7d83-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7d83-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f7d83-113">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f7d83-113">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="f7d83-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7d83-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7d83-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7d83-115">Not supported.</span></span>    |
|<span data-ttu-id="f7d83-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7d83-116">Application</span></span> | <span data-ttu-id="f7d83-117">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7d83-117">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7d83-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7d83-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/appRoleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f7d83-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f7d83-119">Optional query parameters</span></span>

<span data-ttu-id="f7d83-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f7d83-120">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f7d83-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7d83-121">Request headers</span></span>

| <span data-ttu-id="f7d83-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f7d83-122">Name</span></span>           | <span data-ttu-id="f7d83-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7d83-123">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="f7d83-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7d83-124">Authorization</span></span>  | <span data-ttu-id="f7d83-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7d83-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f7d83-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7d83-127">Request body</span></span>

<span data-ttu-id="f7d83-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f7d83-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7d83-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7d83-129">Response</span></span>

<span data-ttu-id="f7d83-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [appRoleAssignment](../resources/approleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7d83-130">If successful, this method returns a `200 OK` response code and a collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f7d83-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f7d83-131">Examples</span></span>

### <a name="example-1-list-approleassignments-granted-to-a-user"></a><span data-ttu-id="f7d83-132">Exemplo 1: listar atribuições de função de aplicativo concedidas a um usuário</span><span class="sxs-lookup"><span data-stu-id="f7d83-132">Example 1: List appRoleAssignments granted to a user</span></span>

#### <a name="request"></a><span data-ttu-id="f7d83-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7d83-133">Request</span></span>

<span data-ttu-id="f7d83-134">Veja a seguir um exemplo de uma solicitação para recuperar as funções de aplicativo que foram atribuídas a um usuário.</span><span class="sxs-lookup"><span data-stu-id="f7d83-134">Here is an example of the request to retrieve the app roles that have been assigned to a user.</span></span>


# <a name="http"></a>[<span data-ttu-id="f7d83-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7d83-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_approleassignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/cdb555e3-b33e-4fd5-a427-17fadacbdfa7/appRoleAssignments
```
# <a name="c"></a>[<span data-ttu-id="f7d83-136">C#</span><span class="sxs-lookup"><span data-stu-id="f7d83-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-approleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7d83-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7d83-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-approleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7d83-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7d83-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-approleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f7d83-139">Java</span><span class="sxs-lookup"><span data-stu-id="f7d83-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-approleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f7d83-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7d83-140">Response</span></span>

<span data-ttu-id="f7d83-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f7d83-141">The following is an example of the response.</span></span> 

><span data-ttu-id="f7d83-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f7d83-142">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "41W1zT6z1U-kJxf62svfp1HFE8pMZhxDun-ThPczmJE",
      "deletedDateTime": null,
      "appRoleId": "00000000-0000-0000-0000-000000000000",
      "createdDateTime": "2021-02-02T04:22:45.9480566Z",
      "principalDisplayName": "Alex Wilber",
      "principalId": "cdb555e3-b33e-4fd5-a427-17fadacbdfa7",
      "principalType": "User",
      "resourceDisplayName": "dxprovisioning-graphapi-client",
      "resourceId": "8e881353-1735-45af-af21-ee1344582a4d"
    }
  ]
}
```
### <a name="example-2-list-approleassignments-granted-to-a-user-filtered-by-resourceid"></a><span data-ttu-id="f7d83-143">Exemplo 2: Listar atribuições de função de aplicativo concedidas a um usuário, filtradas por ID de recurso</span><span class="sxs-lookup"><span data-stu-id="f7d83-143">Example 2: List appRoleAssignments granted to a user, filtered by resourceId</span></span>

#### <a name="request"></a><span data-ttu-id="f7d83-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7d83-144">Request</span></span>

<span data-ttu-id="f7d83-145">Aqui está um exemplo da solicitação para recuperar as funções do aplicativo que foram atribuídas a um usuário, filtrando por um `resourceId`, que é um tipo de GUID.</span><span class="sxs-lookup"><span data-stu-id="f7d83-145">Here is an example of the request to retrieve the app roles that have been assigned to a user, filtering by a `resourceId`, which is a GUID type.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_approleassignments_filterby_resourceId"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/cdb555e3-b33e-4fd5-a427-17fadacbdfa7/appRoleAssignments?$filter=resourceId eq 8e881353-1735-45af-af21-ee1344582a4d
```

#### <a name="response"></a><span data-ttu-id="f7d83-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7d83-146">Response</span></span>

<span data-ttu-id="f7d83-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f7d83-147">The following is an example of the response.</span></span> 

><span data-ttu-id="f7d83-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f7d83-148">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#appRoleAssignments",
  "value": [
    {
      "id": "41W1zT6z1U-kJxf62svfp1HFE8pMZhxDun-ThPczmJE",
      "creationTimestamp": "2021-02-02T04:22:45.9480566Z",
      "appRoleId": "00000000-0000-0000-0000-000000000000",
      "principalDisplayName": "MOD Administrator",
      "principalId": "cdb555e3-b33e-4fd5-a427-17fadacbdfa7",
      "principalType": "User",
      "resourceDisplayName": "dxprovisioning-graphapi-client",
      "resourceId": "8e881353-1735-45af-af21-ee1344582a4d"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List appRoleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

