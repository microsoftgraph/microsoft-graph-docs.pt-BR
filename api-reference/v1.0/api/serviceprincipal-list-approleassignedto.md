---
title: Listar appRoleAssignments concedidos para uma entidade de serviço
description: Recuperar uma lista de atribuições de funções do aplicativo concedidas para uma entidade de serviço.
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 9a9cfd5330d21fe8e8199c9a7fec58c8bb470e7d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049426"
---
# <a name="list-approleassignments-granted-for-a-service-principal"></a><span data-ttu-id="c935e-103">Listar appRoleAssignments concedidos para uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="c935e-103">List appRoleAssignments granted for a service principal</span></span>

<span data-ttu-id="c935e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c935e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c935e-105">Recuperar uma lista de [appRoleAssignment](../resources/approleassignment.md) que os usuários, grupos ou entidades de serviço de cliente receberam para a determinada entidade de serviço do recurso.</span><span class="sxs-lookup"><span data-stu-id="c935e-105">Retrieve a list of [appRoleAssignment](../resources/approleassignment.md) that users, groups, or client service principals have been granted for the given resource service principal.</span></span>

<span data-ttu-id="c935e-106">Por exemplo, se a entidade de serviço do recurso for a entidade de serviço para a API do Microsoft Graph, isso retornará todas as entidades de serviço que receberam todas as permissões de aplicativo para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c935e-106">For example, if the resource service principal is the service principal for the Microsoft Graph API, this will return all service principals that have been granted any app-only permissions to Microsoft Graph.</span></span>

<span data-ttu-id="c935e-107">Se a entidade de serviço do recurso for um aplicativo com funções de aplicativo concedidas a usuários e grupos, isso retornará todos as funções de aplicativo dos usuários e grupos atribuídas para esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c935e-107">If the resource service principal is an application that has app roles granted to users and groups, this will return all the users and groups assigned app roles for this application.</span></span>

## <a name="permissions"></a><span data-ttu-id="c935e-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="c935e-108">Permissions</span></span>

<span data-ttu-id="c935e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c935e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c935e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c935e-111">Permission type</span></span>      | <span data-ttu-id="c935e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c935e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c935e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c935e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c935e-114">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c935e-114">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="c935e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c935e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c935e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c935e-116">Not supported.</span></span>    |
|<span data-ttu-id="c935e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c935e-117">Application</span></span> | <span data-ttu-id="c935e-118">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c935e-118">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c935e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c935e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/appRoleAssignedTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c935e-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c935e-120">Optional query parameters</span></span>

<span data-ttu-id="c935e-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c935e-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c935e-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c935e-122">Request headers</span></span>

| <span data-ttu-id="c935e-123">Nome</span><span class="sxs-lookup"><span data-stu-id="c935e-123">Name</span></span>           | <span data-ttu-id="c935e-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="c935e-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="c935e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c935e-125">Authorization</span></span>  | <span data-ttu-id="c935e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c935e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c935e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c935e-128">Request body</span></span>

<span data-ttu-id="c935e-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c935e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c935e-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c935e-130">Response</span></span>

<span data-ttu-id="c935e-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [appRoleAssignment](../resources/approleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c935e-131">If successful, this method returns a `200 OK` response code and a collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c935e-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c935e-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c935e-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c935e-133">Request</span></span>

<span data-ttu-id="c935e-134">Veja a seguir um exemplo da solicitação para recuperar as atribuições das funções de aplicativo que foram concedidas a uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="c935e-134">The following is an example of the request to retrieve the app roles assignments that have been granted for a given resource service principal.</span></span>


# <a name="http"></a>[<span data-ttu-id="c935e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c935e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_get_approleassignedto"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/8e881353-1735-45af-af21-ee1344582a4d/appRoleAssignedTo
```
# <a name="c"></a>[<span data-ttu-id="c935e-136">C#</span><span class="sxs-lookup"><span data-stu-id="c935e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-get-approleassignedto-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c935e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c935e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-get-approleassignedto-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c935e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c935e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-get-approleassignedto-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c935e-139">Java</span><span class="sxs-lookup"><span data-stu-id="c935e-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-get-approleassignedto-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c935e-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="c935e-140">Response</span></span>

<span data-ttu-id="c935e-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c935e-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="c935e-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c935e-142">**Note:** The response object shown here might be shortened for readability.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#servicePrincipals('8e881353-1735-45af-af21-ee1344582a4d')/appRoleAssignedTo",
  "value": [
    {
      "id": "41W1zT6z1U-kJxf62svfp1HFE8pMZhxDun-ThPczmJE",
      "deletedDateTime": null,
      "appRoleId": "00000000-0000-0000-0000-000000000000",
      "createdDateTime": "2021-02-02T04:22:45.9480566Z",
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

