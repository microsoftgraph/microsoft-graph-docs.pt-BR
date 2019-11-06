---
title: Listar accessPackages
description: Recupere uma lista de objetos accessPackage.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c431216078d72a7515820e0c7ace5234cd08254f
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994138"
---
# <a name="list-accesspackages"></a><span data-ttu-id="623e1-103">Listar accessPackages</span><span class="sxs-lookup"><span data-stu-id="623e1-103">List accessPackages</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="623e1-104">Recupere uma lista de objetos [accessPackage](../resources/accesspackage.md) .</span><span class="sxs-lookup"><span data-stu-id="623e1-104">Retrieve a list of [accessPackage](../resources/accesspackage.md) objects.</span></span>  <span data-ttu-id="623e1-105">A lista resultante inclui todos os pacotes de acesso que o chamador tem acesso para ler, em todos os catálogos.</span><span class="sxs-lookup"><span data-stu-id="623e1-105">The resulting list includes all the access packages that the caller has access to read, across all catalogs.</span></span>

## <a name="permissions"></a><span data-ttu-id="623e1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="623e1-106">Permissions</span></span>

<span data-ttu-id="623e1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="623e1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="623e1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="623e1-109">Permission type</span></span>                        | <span data-ttu-id="623e1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="623e1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="623e1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="623e1-111">Delegated (work or school account)</span></span>     |  <span data-ttu-id="623e1-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="623e1-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="623e1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="623e1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="623e1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="623e1-114">Not supported.</span></span> |
| <span data-ttu-id="623e1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="623e1-115">Application</span></span>                            | <span data-ttu-id="623e1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="623e1-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="623e1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="623e1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="623e1-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="623e1-118">Optional query parameters</span></span>

<span data-ttu-id="623e1-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="623e1-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="623e1-120">Por exemplo, para recuperar as políticas de pacote de acesso para cada pacote de `$expand=accessPackageAssignmentPolicies`acesso, adicione.</span><span class="sxs-lookup"><span data-stu-id="623e1-120">For example, to retrieve the access package policies for each access package, add `$expand=accessPackageAssignmentPolicies`.</span></span> <span data-ttu-id="623e1-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="623e1-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="623e1-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="623e1-122">Request headers</span></span>

| <span data-ttu-id="623e1-123">Nome</span><span class="sxs-lookup"><span data-stu-id="623e1-123">Name</span></span>      |<span data-ttu-id="623e1-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="623e1-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="623e1-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="623e1-125">Authorization</span></span> | <span data-ttu-id="623e1-126">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="623e1-126">Bearer \{token\}.</span></span> <span data-ttu-id="623e1-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="623e1-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="623e1-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="623e1-128">Request body</span></span>

<span data-ttu-id="623e1-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="623e1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="623e1-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="623e1-130">Response</span></span>

<span data-ttu-id="623e1-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [accessPackage](../resources/accesspackage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="623e1-131">If successful, this method returns a `200 OK` response code and a collection of [accessPackage](../resources/accesspackage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="623e1-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="623e1-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="623e1-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="623e1-133">Request</span></span>

<span data-ttu-id="623e1-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="623e1-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="623e1-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="623e1-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackages"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="623e1-136">C#</span><span class="sxs-lookup"><span data-stu-id="623e1-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="623e1-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="623e1-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="623e1-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="623e1-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="623e1-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="623e1-139">Response</span></span>

<span data-ttu-id="623e1-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="623e1-140">The following is an example of the response.</span></span>

> <span data-ttu-id="623e1-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="623e1-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackage",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id":"360fa7de-90be-48dc-a2ce-fc40094a93dd",
      "description":"Sample access package",
      "displayName":"Access package for testing",
      "isHidden":false,
      "catalogId":"662d99e7-6ceb-4c21-9cb4-9b0bbfdefccc",
      "isRoleScopesVisible":false,
      "createdDateTime":"2019-01-27T18:19:50.74Z",
      "modifiedDateTime":"2019-01-27T18:19:50.74Z",
      "createdBy":"TestGA@example.com",
      "modifiedBy":"TestGA@example.com"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
