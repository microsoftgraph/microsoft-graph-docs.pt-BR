---
title: Listar accessPackageAssignmentResourceRoles
description: Recupere uma lista de objetos accessPackageAssignmentResourceRole.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 63ece8b5abcf6014e6ccbc293a773ea3dab8f462
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868006"
---
# <a name="list-accesspackageassignmentresourceroles"></a><span data-ttu-id="de075-103">Listar accessPackageAssignmentResourceRoles</span><span class="sxs-lookup"><span data-stu-id="de075-103">List accessPackageAssignmentResourceRoles</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de075-104">Recupere uma lista de objetos [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) .</span><span class="sxs-lookup"><span data-stu-id="de075-104">Retrieve a list of [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) objects.</span></span>  <span data-ttu-id="de075-105">A lista resultante inclui todas as funções de recurso de todas as atribuições que o chamador tem acesso para ler, entre todos os catálogos e pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="de075-105">The resulting list includes all the resource roles of all assignments that the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="de075-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="de075-106">Permissions</span></span>

<span data-ttu-id="de075-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de075-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="de075-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de075-109">Permission type</span></span>                        | <span data-ttu-id="de075-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="de075-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="de075-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de075-111">Delegated (work or school account)</span></span>     |  <span data-ttu-id="de075-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de075-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="de075-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de075-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de075-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de075-114">Not supported.</span></span> |
| <span data-ttu-id="de075-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="de075-115">Application</span></span>                            | <span data-ttu-id="de075-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de075-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="de075-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de075-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles
```

## <a name="optional-query-parameters"></a><span data-ttu-id="de075-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="de075-118">Optional query parameters</span></span>

<span data-ttu-id="de075-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="de075-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="de075-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="de075-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="de075-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de075-121">Request headers</span></span>

| <span data-ttu-id="de075-122">Nome</span><span class="sxs-lookup"><span data-stu-id="de075-122">Name</span></span>      |<span data-ttu-id="de075-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="de075-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="de075-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="de075-124">Authorization</span></span> | <span data-ttu-id="de075-125">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="de075-125">Bearer \{token\}.</span></span> <span data-ttu-id="de075-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de075-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="de075-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de075-127">Request body</span></span>

<span data-ttu-id="de075-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="de075-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de075-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="de075-129">Response</span></span>

<span data-ttu-id="de075-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de075-130">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="de075-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="de075-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="de075-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de075-132">Request</span></span>

<span data-ttu-id="de075-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="de075-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="de075-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="de075-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentresourceroles"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="de075-135">C#</span><span class="sxs-lookup"><span data-stu-id="de075-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentresourceroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de075-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de075-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentresourceroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="de075-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="de075-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentresourceroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="de075-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="de075-138">Response</span></span>

<span data-ttu-id="de075-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="de075-139">The following is an example of the response.</span></span>

> <span data-ttu-id="de075-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="de075-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentResourceRole",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "1bf101d2-4d9c-437f-bbf5-3d13d98f5479",
      "originId": "originId-value",
      "originSystem": "SharePointOnline",
      "status": "Fulfilled"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageAssignmentResourceRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
