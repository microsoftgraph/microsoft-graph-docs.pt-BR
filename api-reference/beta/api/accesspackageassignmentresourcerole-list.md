---
title: Listar accessPackageAssignmentResourceRoles
description: Recupere uma lista de objetos accessPackageAssignmentResourceRrole.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 07fc724591b99bb18d1a1540e7e3ec3da4f767ac
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994293"
---
# <a name="list-accesspackageassignmentresourceroles"></a><span data-ttu-id="1b0ca-103">Listar accessPackageAssignmentResourceRoles</span><span class="sxs-lookup"><span data-stu-id="1b0ca-103">List accessPackageAssignmentResourceRoles</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b0ca-104">Recupere uma lista de objetos [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) .</span><span class="sxs-lookup"><span data-stu-id="1b0ca-104">Retrieve a list of [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) objects.</span></span>  <span data-ttu-id="1b0ca-105">A lista resultante inclui todas as funções de recurso de todas as atribuições que o chamador tem acesso para ler, entre todos os catálogos e pacotes de acesso.</span><span class="sxs-lookup"><span data-stu-id="1b0ca-105">The resulting list includes all the resource roles of all assignments that the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b0ca-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1b0ca-106">Permissions</span></span>

<span data-ttu-id="1b0ca-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b0ca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1b0ca-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1b0ca-109">Permission type</span></span>                        | <span data-ttu-id="1b0ca-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1b0ca-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1b0ca-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1b0ca-111">Delegated (work or school account)</span></span>     |  <span data-ttu-id="1b0ca-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b0ca-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="1b0ca-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1b0ca-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b0ca-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b0ca-114">Not supported.</span></span> |
| <span data-ttu-id="1b0ca-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1b0ca-115">Application</span></span>                            | <span data-ttu-id="1b0ca-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1b0ca-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b0ca-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1b0ca-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1b0ca-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1b0ca-118">Optional query parameters</span></span>

<span data-ttu-id="1b0ca-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1b0ca-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1b0ca-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1b0ca-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1b0ca-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1b0ca-121">Request headers</span></span>

| <span data-ttu-id="1b0ca-122">Nome</span><span class="sxs-lookup"><span data-stu-id="1b0ca-122">Name</span></span>      |<span data-ttu-id="1b0ca-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b0ca-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1b0ca-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1b0ca-124">Authorization</span></span> | <span data-ttu-id="1b0ca-125">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="1b0ca-125">Bearer \{token\}.</span></span> <span data-ttu-id="1b0ca-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1b0ca-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1b0ca-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1b0ca-127">Request body</span></span>

<span data-ttu-id="1b0ca-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1b0ca-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b0ca-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b0ca-129">Response</span></span>

<span data-ttu-id="1b0ca-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1b0ca-130">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1b0ca-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1b0ca-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1b0ca-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1b0ca-132">Request</span></span>

<span data-ttu-id="1b0ca-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1b0ca-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="1b0ca-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b0ca-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentresourceroles"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1b0ca-135">C#</span><span class="sxs-lookup"><span data-stu-id="1b0ca-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentresourceroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1b0ca-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b0ca-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentresourceroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1b0ca-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b0ca-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentresourceroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1b0ca-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="1b0ca-138">Response</span></span>

<span data-ttu-id="1b0ca-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1b0ca-139">The following is an example of the response.</span></span>

> <span data-ttu-id="1b0ca-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1b0ca-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
