---
title: Listar appRoleAssignments concedidos a uma entidade de serviço
description: Recuperar a lista de atribuições de funções do aplicativo concedidas a uma entidade de serviço.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 345a454f8638c6a5de5ba5d35c061941bd8f9865
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48313566"
---
# <a name="list-approleassignments-granted-to-a-service-principal"></a><span data-ttu-id="613e0-103">Listar appRoleAssignments concedidos a uma entidade de serviço</span><span class="sxs-lookup"><span data-stu-id="613e0-103">List appRoleAssignments granted to a service principal</span></span>

<span data-ttu-id="613e0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="613e0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="613e0-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="613e0-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="613e0-106">Recuperar a lista[appRoleAssignment](../resources/approleassignment.md) concedida a uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="613e0-106">Retrieve the list of [appRoleAssignment](../resources/approleassignment.md) that have been granted to a service principal.</span></span>

<span data-ttu-id="613e0-107">As funções do aplicativo atribuídas às entidades de serviço também são conhecidas como [permissões de aplicativo](/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span><span class="sxs-lookup"><span data-stu-id="613e0-107">App roles that are assigned to service principals are also known as [application permissions](/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span> <span data-ttu-id="613e0-108">As permissões de aplicativo podem ser concedidas diretamente, criando atribuições de função de aplicativo ou por meio de uma [experiência de consentimento](/azure/active-directory/develop/application-consent-experience).</span><span class="sxs-lookup"><span data-stu-id="613e0-108">Application permissions can be granted directly by creating app role assignments, or through a [consent experience](/azure/active-directory/develop/application-consent-experience).</span></span>

## <a name="permissions"></a><span data-ttu-id="613e0-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="613e0-109">Permissions</span></span>

<span data-ttu-id="613e0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="613e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="613e0-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="613e0-112">Permission type</span></span>      | <span data-ttu-id="613e0-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="613e0-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="613e0-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="613e0-114">Delegated (work or school account)</span></span> | <span data-ttu-id="613e0-115">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="613e0-115">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>  |
|<span data-ttu-id="613e0-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="613e0-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="613e0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="613e0-117">Not supported.</span></span>    |
|<span data-ttu-id="613e0-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="613e0-118">Application</span></span> | <span data-ttu-id="613e0-119">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="613e0-119">Application.Read.All, Directory.Read.All, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="613e0-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="613e0-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/appRoleAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="613e0-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="613e0-121">Optional query parameters</span></span>

<span data-ttu-id="613e0-122">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="613e0-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="613e0-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="613e0-123">Request headers</span></span>

| <span data-ttu-id="613e0-124">Nome</span><span class="sxs-lookup"><span data-stu-id="613e0-124">Name</span></span>           | <span data-ttu-id="613e0-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="613e0-125">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="613e0-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="613e0-126">Authorization</span></span>  | <span data-ttu-id="613e0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="613e0-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="613e0-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="613e0-129">Request body</span></span>

<span data-ttu-id="613e0-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="613e0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="613e0-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="613e0-131">Response</span></span>

<span data-ttu-id="613e0-132">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [appRoleAssignment](../resources/approleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="613e0-132">If successful, this method returns a `200 OK` response code and a collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="613e0-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="613e0-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="613e0-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="613e0-134">Request</span></span>

<span data-ttu-id="613e0-135">Veja a seguir um exemplo de uma solicitação para recuperar as funções de aplicativo que foram atribuídas a uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="613e0-135">The following is an example of a request to retrieve the app roles that have been assigned to a service principal.</span></span>


# <a name="http"></a>[<span data-ttu-id="613e0-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="613e0-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_get_approleassignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignments
```
# <a name="c"></a>[<span data-ttu-id="613e0-137">C#</span><span class="sxs-lookup"><span data-stu-id="613e0-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-get-approleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="613e0-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="613e0-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-get-approleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="613e0-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="613e0-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-get-approleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="613e0-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="613e0-140">Response</span></span>

<span data-ttu-id="613e0-141">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="613e0-141">Here is an example of the response.</span></span> 

> <span data-ttu-id="613e0-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="613e0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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