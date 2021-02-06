---
title: Listar appRoleAssignments concedidos para uma entidade de serviço
description: Recuperar uma lista de atribuições de funções do aplicativo concedidas para uma entidade de serviço.
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 17a12a1f401a63042dd41f1e0e0f7f89c3d94bb2
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134402"
---
# <a name="list-approleassignments-granted-for-a-service-principal"></a><span data-ttu-id="f3b9d-103">Listar appRoleAssignments concedidos para uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="f3b9d-103">List appRoleAssignments granted for a service principal</span></span>

<span data-ttu-id="f3b9d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3b9d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3b9d-105">Recuperar uma lista de [appRoleAssignment](../resources/approleassignment.md) que os usuários, grupos ou entidades de serviço de cliente receberam para a determinada entidade de serviço do recurso.</span><span class="sxs-lookup"><span data-stu-id="f3b9d-105">Retrieve a list of [appRoleAssignment](../resources/approleassignment.md) that users, groups, or client service principals have been granted for the given resource service principal.</span></span>

<span data-ttu-id="f3b9d-106">Por exemplo, se a entidade de serviço do recurso for a entidade de serviço para a API do Microsoft Graph, isso retornará todas as entidades de serviço que receberam todas as permissões de aplicativo para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f3b9d-106">For example, if the resource service principal is the service principal for the Microsoft Graph API, this will return all service principals that have been granted any app-only permissions to Microsoft Graph.</span></span>

<span data-ttu-id="f3b9d-107">Se a entidade de serviço do recurso for um aplicativo com funções de aplicativo concedidas a usuários e grupos, isso retornará todos as funções de aplicativo dos usuários e grupos atribuídas para esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f3b9d-107">If the resource service principal is an application that has app roles granted to users and groups, this will return all the users and groups assigned app roles for this application.</span></span>

## <a name="permissions"></a><span data-ttu-id="f3b9d-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="f3b9d-108">Permissions</span></span>

<span data-ttu-id="f3b9d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3b9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3b9d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f3b9d-111">Permission type</span></span>      | <span data-ttu-id="f3b9d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f3b9d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f3b9d-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f3b9d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f3b9d-114">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f3b9d-114">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="f3b9d-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f3b9d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f3b9d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3b9d-116">Not supported.</span></span>    |
|<span data-ttu-id="f3b9d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f3b9d-117">Application</span></span> | <span data-ttu-id="f3b9d-118">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3b9d-118">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f3b9d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f3b9d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/appRoleAssignedTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f3b9d-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f3b9d-120">Optional query parameters</span></span>

<span data-ttu-id="f3b9d-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f3b9d-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f3b9d-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f3b9d-122">Request headers</span></span>

| <span data-ttu-id="f3b9d-123">Nome</span><span class="sxs-lookup"><span data-stu-id="f3b9d-123">Name</span></span>           | <span data-ttu-id="f3b9d-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3b9d-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="f3b9d-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f3b9d-125">Authorization</span></span>  | <span data-ttu-id="f3b9d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f3b9d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f3b9d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f3b9d-128">Request body</span></span>

<span data-ttu-id="f3b9d-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f3b9d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3b9d-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3b9d-130">Response</span></span>

<span data-ttu-id="f3b9d-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [appRoleAssignment](../resources/approleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f3b9d-131">If successful, this method returns a `200 OK` response code and a collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3b9d-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f3b9d-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3b9d-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3b9d-133">Request</span></span>

<span data-ttu-id="f3b9d-134">Veja a seguir um exemplo da solicitação para recuperar as atribuições das funções de aplicativo que foram concedidas a uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="f3b9d-134">The following is an example of the request to retrieve the app roles assignments that have been granted for a given resource service principal.</span></span>


# <a name="http"></a>[<span data-ttu-id="f3b9d-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f3b9d-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_get_approleassignedto"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignedTo
```
# <a name="c"></a>[<span data-ttu-id="f3b9d-136">C#</span><span class="sxs-lookup"><span data-stu-id="f3b9d-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-get-approleassignedto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f3b9d-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f3b9d-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-get-approleassignedto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f3b9d-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f3b9d-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-get-approleassignedto-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f3b9d-139">Java</span><span class="sxs-lookup"><span data-stu-id="f3b9d-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-get-approleassignedto-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f3b9d-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3b9d-140">Response</span></span>

<span data-ttu-id="f3b9d-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f3b9d-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="f3b9d-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f3b9d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 306

{
  "value": [
    {
      "creationTimestamp": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "principalDisplayName": "principalDisplayName-value",
      "principalId": "principalId-value",
      "principalType": "principalType-value",
      "resourceDisplayName": "resourceDisplayName-value"
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



