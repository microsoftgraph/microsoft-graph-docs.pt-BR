---
title: Listar appRoleAssignments concedido a um usuário
description: Recuperar a lista de atribuições de funções do aplicativo concedidas a um usuário.
localization_priority: Priority
doc_type: apiPageType
ms.prod: users
author: psignoret
ms.openlocfilehash: 9988f98ac197eceb6b3f54910f5338803954f084
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036321"
---
# <a name="list-approleassignments-granted-to-a-user"></a><span data-ttu-id="2a4c3-103">Listar appRoleAssignments concedido a um usuário</span><span class="sxs-lookup"><span data-stu-id="2a4c3-103">List appRoleAssignments granted to a user</span></span>

<span data-ttu-id="2a4c3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a4c3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a4c3-105">Recuperar a lista[appRoleAssignment](../resources/approleassignment.md) concedida a um usuário.</span><span class="sxs-lookup"><span data-stu-id="2a4c3-105">Retrieve the list of [appRoleAssignment](../resources/approleassignment.md) that a user has been granted.</span></span> <span data-ttu-id="2a4c3-106">Essa operação também retorna funções de aplicativo atribuídas a grupos dos quais o usuário é membro direto.</span><span class="sxs-lookup"><span data-stu-id="2a4c3-106">This operation also returns app roles assigned to groups that the user is a direct member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a4c3-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="2a4c3-107">Permissions</span></span>

<span data-ttu-id="2a4c3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a4c3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a4c3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2a4c3-110">Permission type</span></span>      | <span data-ttu-id="2a4c3-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2a4c3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2a4c3-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2a4c3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2a4c3-113">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2a4c3-113">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="2a4c3-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2a4c3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a4c3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a4c3-115">Not supported.</span></span>    |
|<span data-ttu-id="2a4c3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2a4c3-116">Application</span></span> | <span data-ttu-id="2a4c3-117">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a4c3-117">Directory.Read.All, AppRoleAssignment.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a4c3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2a4c3-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/appRoleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2a4c3-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2a4c3-119">Optional query parameters</span></span>

<span data-ttu-id="2a4c3-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2a4c3-120">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2a4c3-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2a4c3-121">Request headers</span></span>

| <span data-ttu-id="2a4c3-122">Nome</span><span class="sxs-lookup"><span data-stu-id="2a4c3-122">Name</span></span>           | <span data-ttu-id="2a4c3-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a4c3-123">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="2a4c3-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2a4c3-124">Authorization</span></span>  | <span data-ttu-id="2a4c3-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2a4c3-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2a4c3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2a4c3-127">Request body</span></span>

<span data-ttu-id="2a4c3-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2a4c3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a4c3-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a4c3-129">Response</span></span>

<span data-ttu-id="2a4c3-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [appRoleAssignment](../resources/approleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2a4c3-130">If successful, this method returns a `200 OK` response code and a collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2a4c3-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2a4c3-131">Examples</span></span>

### <a name="example-1-list-approleassignments-granted-to-a-user"></a><span data-ttu-id="2a4c3-132">Exemplo 1: listar atribuições de função de aplicativo concedidas a um usuário</span><span class="sxs-lookup"><span data-stu-id="2a4c3-132">Example 1: List appRoleAssignments granted to a user</span></span>

#### <a name="request"></a><span data-ttu-id="2a4c3-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a4c3-133">Request</span></span>

<span data-ttu-id="2a4c3-134">Veja a seguir um exemplo de uma solicitação para recuperar as funções de aplicativo que foram atribuídas a um usuário.</span><span class="sxs-lookup"><span data-stu-id="2a4c3-134">Here is an example of the request to retrieve the app roles that have been assigned to a user.</span></span>


# <a name="http"></a>[<span data-ttu-id="2a4c3-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="2a4c3-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_approleassignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/cdb555e3-b33e-4fd5-a427-17fadacbdfa7/appRoleAssignments
```
# <a name="c"></a>[<span data-ttu-id="2a4c3-136">C#</span><span class="sxs-lookup"><span data-stu-id="2a4c3-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-approleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2a4c3-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2a4c3-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-approleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2a4c3-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2a4c3-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-approleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2a4c3-139">Java</span><span class="sxs-lookup"><span data-stu-id="2a4c3-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-approleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2a4c3-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a4c3-140">Response</span></span>

<span data-ttu-id="2a4c3-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2a4c3-141">The following is an example of the response.</span></span> 

><span data-ttu-id="2a4c3-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2a4c3-142">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "creationTimestamp": "2021-02-02T04:22:45.9480566Z",
      "principalDisplayName": "Alex Wilber",
      "principalId": "cdb555e3-b33e-4fd5-a427-17fadacbdfa7",
      "principalType": "User",
      "resourceDisplayName": "dxprovisioning-graphapi-client",
      "resourceId": "8e881353-1735-45af-af21-ee1344582a4d"
    }
  ]
}
```

### <a name="example-2-list-approleassignments-granted-to-a-user-filtered-by-resourceid"></a><span data-ttu-id="2a4c3-143">Exemplo 2: Listar atribuições de função de aplicativo concedidas a um usuário, filtradas por ID de recurso</span><span class="sxs-lookup"><span data-stu-id="2a4c3-143">Example 2: List appRoleAssignments granted to a user, filtered by resourceId</span></span>

#### <a name="request"></a><span data-ttu-id="2a4c3-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a4c3-144">Request</span></span>

<span data-ttu-id="2a4c3-145">Aqui está um exemplo da solicitação para recuperar as funções do aplicativo que foram atribuídas a um usuário, filtrando por um `resourceId`, que é um tipo de GUID.</span><span class="sxs-lookup"><span data-stu-id="2a4c3-145">Here is an example of the request to retrieve the app roles that have been assigned to a user, filtering by a `resourceId`, which is a GUID type.</span></span>


# <a name="http"></a>[<span data-ttu-id="2a4c3-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="2a4c3-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_approleassignments_filterby_resourceId"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/users/cdb555e3-b33e-4fd5-a427-17fadacbdfa7/appRoleAssignments?$filter=resourceId eq 8e881353-1735-45af-af21-ee1344582a4d
```
# <a name="c"></a>[<span data-ttu-id="2a4c3-147">C#</span><span class="sxs-lookup"><span data-stu-id="2a4c3-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-approleassignments-filterby-resourceid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2a4c3-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2a4c3-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-approleassignments-filterby-resourceid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2a4c3-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2a4c3-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-approleassignments-filterby-resourceid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2a4c3-150">Java</span><span class="sxs-lookup"><span data-stu-id="2a4c3-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-approleassignments-filterby-resourceid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2a4c3-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a4c3-151">Response</span></span>

<span data-ttu-id="2a4c3-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2a4c3-152">The following is an example of the response.</span></span> 

><span data-ttu-id="2a4c3-153">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2a4c3-153">**Note:** The response object shown here might be shortened for readability.</span></span> 

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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#appRoleAssignments",
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

