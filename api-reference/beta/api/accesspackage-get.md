---
title: Obter accessPackage
description: Recupere as propriedades e as relações de um objeto accessPackage.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 192ddb37ef7b6ab1372d7504d1785299cbcf0e86
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52038660"
---
# <a name="get-accesspackage"></a><span data-ttu-id="416af-103">Obter accessPackage</span><span class="sxs-lookup"><span data-stu-id="416af-103">Get accessPackage</span></span>

<span data-ttu-id="416af-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="416af-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="416af-105">Recupere as propriedades e as relações de um [objeto accessPackage.](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="416af-105">Retrieve the properties and relationships of an [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="416af-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="416af-106">Permissions</span></span>

<span data-ttu-id="416af-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="416af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="416af-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="416af-109">Permission type</span></span>                        | <span data-ttu-id="416af-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="416af-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="416af-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="416af-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="416af-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="416af-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="416af-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="416af-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="416af-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="416af-114">Not supported.</span></span> |
| <span data-ttu-id="416af-115">Application</span><span class="sxs-lookup"><span data-stu-id="416af-115">Application</span></span>                            | <span data-ttu-id="416af-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="416af-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="416af-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="416af-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="416af-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="416af-118">Optional query parameters</span></span>

<span data-ttu-id="416af-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="416af-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="416af-120">Por exemplo, para recuperar as políticas de pacote de acesso, adicione `$expand=accessPackageAssignmentPolicies` .</span><span class="sxs-lookup"><span data-stu-id="416af-120">For example, to retrieve the access package policies, add `$expand=accessPackageAssignmentPolicies`.</span></span> <span data-ttu-id="416af-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="416af-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="416af-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="416af-122">Request headers</span></span>

| <span data-ttu-id="416af-123">Nome</span><span class="sxs-lookup"><span data-stu-id="416af-123">Name</span></span>      |<span data-ttu-id="416af-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="416af-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="416af-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="416af-125">Authorization</span></span> | <span data-ttu-id="416af-p103">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="416af-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="416af-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="416af-128">Request body</span></span>

<span data-ttu-id="416af-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="416af-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="416af-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="416af-130">Response</span></span>

<span data-ttu-id="416af-131">Se tiver êxito, este método retornará um código `200 OK` de resposta e o objeto [accessPackage](../resources/accesspackage.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="416af-131">If successful, this method returns a `200 OK` response code and the requested [accessPackage](../resources/accesspackage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="416af-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="416af-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="416af-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="416af-133">Request</span></span>

<span data-ttu-id="416af-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="416af-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="416af-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="416af-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackage"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}
```
# <a name="c"></a>[<span data-ttu-id="416af-136">C#</span><span class="sxs-lookup"><span data-stu-id="416af-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="416af-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="416af-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="416af-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="416af-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="416af-139">Java</span><span class="sxs-lookup"><span data-stu-id="416af-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="416af-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="416af-140">Response</span></span>

<span data-ttu-id="416af-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="416af-141">The following is an example of the response.</span></span>

> <span data-ttu-id="416af-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="416af-142">**Note:** The response object shown here might be shortened for readability.</span></span>

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


