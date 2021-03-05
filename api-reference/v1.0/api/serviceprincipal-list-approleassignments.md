---
title: Listar appRoleAssignments concedidos a uma entidade de serviço
description: Recuperar a lista de atribuições de funções do aplicativo concedidas a uma entidade de serviço.
localization_priority: Priority
doc_type: apiPageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 02e95099b760c506b7da328cdc99ea3efc07f5f9
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443913"
---
# <a name="list-approleassignments-granted-to-a-service-principal"></a><span data-ttu-id="70070-103">Listar appRoleAssignments concedidos a uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="70070-103">List appRoleAssignments granted to a service principal</span></span>

<span data-ttu-id="70070-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70070-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="70070-105">Recuperar a lista[appRoleAssignment](../resources/approleassignment.md) concedida a uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="70070-105">Retrieve the list of [appRoleAssignment](../resources/approleassignment.md) that have been granted to a service principal.</span></span>

<span data-ttu-id="70070-106">As funções do aplicativo atribuídas às entidades de serviço também são conhecidas como [permissões de aplicativo](/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span><span class="sxs-lookup"><span data-stu-id="70070-106">App roles that are assigned to service principals are also known as [application permissions](/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span> <span data-ttu-id="70070-107">As permissões de aplicativo podem ser concedidas diretamente, criando atribuições de função de aplicativo ou por meio de uma [experiência de consentimento](/azure/active-directory/develop/application-consent-experience).</span><span class="sxs-lookup"><span data-stu-id="70070-107">Application permissions can be granted directly by creating app role assignments, or through a [consent experience](/azure/active-directory/develop/application-consent-experience).</span></span>

## <a name="permissions"></a><span data-ttu-id="70070-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="70070-108">Permissions</span></span>

<span data-ttu-id="70070-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70070-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70070-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="70070-111">Permission type</span></span>      | <span data-ttu-id="70070-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="70070-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70070-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="70070-113">Delegated (work or school account)</span></span> | <span data-ttu-id="70070-114">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="70070-114">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="70070-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="70070-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70070-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="70070-116">Not supported.</span></span>    |
|<span data-ttu-id="70070-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="70070-117">Application</span></span> | <span data-ttu-id="70070-118">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70070-118">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="70070-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="70070-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/appRoleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="70070-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="70070-120">Optional query parameters</span></span>

<span data-ttu-id="70070-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="70070-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="70070-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="70070-122">Request headers</span></span>

| <span data-ttu-id="70070-123">Nome</span><span class="sxs-lookup"><span data-stu-id="70070-123">Name</span></span>           | <span data-ttu-id="70070-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="70070-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="70070-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="70070-125">Authorization</span></span>  | <span data-ttu-id="70070-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70070-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="70070-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="70070-128">Request body</span></span>

<span data-ttu-id="70070-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="70070-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="70070-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="70070-130">Response</span></span>

<span data-ttu-id="70070-131">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [appRoleAssignment](../resources/approleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="70070-131">If successful, this method returns a `200 OK` response code and a collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70070-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="70070-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="70070-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="70070-133">Request</span></span>

<span data-ttu-id="70070-134">Veja a seguir um exemplo de uma solicitação para recuperar as funções de aplicativo que foram atribuídas a uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="70070-134">The following is an example of a request to retrieve the app roles that have been assigned to a service principal.</span></span>


# <a name="http"></a>[<span data-ttu-id="70070-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="70070-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_get_approleassignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/8e881353-1735-45af-af21-ee1344582a4d/appRoleAssignments
```
# <a name="c"></a>[<span data-ttu-id="70070-136">C#</span><span class="sxs-lookup"><span data-stu-id="70070-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-get-approleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="70070-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70070-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-get-approleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="70070-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="70070-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-get-approleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="70070-139">Java</span><span class="sxs-lookup"><span data-stu-id="70070-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-get-approleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="70070-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="70070-140">Response</span></span>

<span data-ttu-id="70070-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="70070-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="70070-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="70070-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "id": "UxOIjjUXr0WvIe4TRFgqTY4z9Wu5KxpBtlEpoTGjw-A",
      "creationTimestamp": "2021-02-02T04:22:45.4980259Z",
      "appRoleId": "e2a3a72e-5f79-4c64-b1b1-878b674786c9",
      "principalDisplayName": "dxprovisioning-graphapi-client",
      "principalId": "8e881353-1735-45af-af21-ee1344582a4d",
      "principalType": "ServicePrincipal",
      "resourceDisplayName": "Microsoft Graph",
      "resourceId": "fea94d6d-b5bf-44d2-a887-4f72a8d74f44"
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
