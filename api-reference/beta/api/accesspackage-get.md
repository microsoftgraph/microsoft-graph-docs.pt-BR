---
title: Obter accessPackage
description: Recupere as propriedades e os relacionamentos de um objeto accessPackage.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1278c352cb69b5a25c64437a554911866f23294b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448554"
---
# <a name="get-accesspackage"></a><span data-ttu-id="1a0a2-103">Obter accessPackage</span><span class="sxs-lookup"><span data-stu-id="1a0a2-103">Get accessPackage</span></span>

<span data-ttu-id="1a0a2-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1a0a2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a0a2-105">Recupere as propriedades e os relacionamentos de um objeto [accessPackage](../resources/accesspackage.md) .</span><span class="sxs-lookup"><span data-stu-id="1a0a2-105">Retrieve the properties and relationships of an [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a0a2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1a0a2-106">Permissions</span></span>

<span data-ttu-id="1a0a2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a0a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1a0a2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1a0a2-109">Permission type</span></span>                        | <span data-ttu-id="1a0a2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1a0a2-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1a0a2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1a0a2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1a0a2-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a0a2-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="1a0a2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1a0a2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a0a2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a0a2-114">Not supported.</span></span> |
| <span data-ttu-id="1a0a2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1a0a2-115">Application</span></span>                            | <span data-ttu-id="1a0a2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a0a2-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a0a2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1a0a2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1a0a2-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1a0a2-118">Optional query parameters</span></span>

<span data-ttu-id="1a0a2-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1a0a2-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1a0a2-120">Por exemplo, para recuperar as políticas de pacote de acesso `$expand=accessPackageAssignmentPolicies`, adicione.</span><span class="sxs-lookup"><span data-stu-id="1a0a2-120">For example, to retrieve the access package policies, add `$expand=accessPackageAssignmentPolicies`.</span></span> <span data-ttu-id="1a0a2-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1a0a2-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1a0a2-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1a0a2-122">Request headers</span></span>

| <span data-ttu-id="1a0a2-123">Nome</span><span class="sxs-lookup"><span data-stu-id="1a0a2-123">Name</span></span>      |<span data-ttu-id="1a0a2-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a0a2-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1a0a2-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="1a0a2-125">Authorization</span></span> | <span data-ttu-id="1a0a2-126">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="1a0a2-126">Bearer \{token\}.</span></span> <span data-ttu-id="1a0a2-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a0a2-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a0a2-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1a0a2-128">Request body</span></span>

<span data-ttu-id="1a0a2-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1a0a2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a0a2-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a0a2-130">Response</span></span>

<span data-ttu-id="1a0a2-131">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [accessPackage](../resources/accesspackage.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1a0a2-131">If successful, this method returns a `200 OK` response code and the requested [accessPackage](../resources/accesspackage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1a0a2-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1a0a2-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1a0a2-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1a0a2-133">Request</span></span>

<span data-ttu-id="1a0a2-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1a0a2-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1a0a2-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a0a2-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackage"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}
```
# <a name="c"></a>[<span data-ttu-id="1a0a2-136">C#</span><span class="sxs-lookup"><span data-stu-id="1a0a2-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1a0a2-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a0a2-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1a0a2-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a0a2-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1a0a2-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a0a2-139">Response</span></span>

<span data-ttu-id="1a0a2-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1a0a2-140">The following is an example of the response.</span></span>

> <span data-ttu-id="1a0a2-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1a0a2-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackage"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get accessPackage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
