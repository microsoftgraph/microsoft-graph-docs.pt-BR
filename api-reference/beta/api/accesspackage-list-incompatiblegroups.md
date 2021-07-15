---
title: Listar incompatibleGroups
description: Recupere uma lista de grupos cujos direitos de acesso são incompatíveis com um pacote de acesso específico.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c5af81b8995b0fc0662a35157ab4579631b5f189
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439907"
---
# <a name="list-incompatiblegroups"></a><span data-ttu-id="54c5d-103">Listar incompatibleGroups</span><span class="sxs-lookup"><span data-stu-id="54c5d-103">List incompatibleGroups</span></span>

<span data-ttu-id="54c5d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54c5d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54c5d-105">Recupere uma lista dos objetos [de](../resources/group.md) grupo que foram marcados como incompatíveis em [um accessPackage](../resources/accesspackage.md).</span><span class="sxs-lookup"><span data-stu-id="54c5d-105">Retrieve a list of the [group](../resources/group.md) objects that have been marked as incompatible on an [accessPackage](../resources/accesspackage.md).</span></span>  

## <a name="permissions"></a><span data-ttu-id="54c5d-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="54c5d-106">Permissions</span></span>

<span data-ttu-id="54c5d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54c5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="54c5d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="54c5d-109">Permission type</span></span>                        | <span data-ttu-id="54c5d-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="54c5d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="54c5d-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="54c5d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="54c5d-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54c5d-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="54c5d-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="54c5d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54c5d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="54c5d-114">Not supported.</span></span> |
| <span data-ttu-id="54c5d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="54c5d-115">Application</span></span>                            | <span data-ttu-id="54c5d-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54c5d-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="54c5d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54c5d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackage/{id}/incompatibleGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="54c5d-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="54c5d-118">Optional query parameters</span></span>

<span data-ttu-id="54c5d-119">Este método dá suporte aos parâmetros de consulta OData para pajamento no lado do servidor por meio de uma resposta grande.</span><span class="sxs-lookup"><span data-stu-id="54c5d-119">This method supports the OData query parameters for server-side paging through a large response.</span></span> <span data-ttu-id="54c5d-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="54c5d-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="54c5d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54c5d-121">Request headers</span></span>

| <span data-ttu-id="54c5d-122">Nome</span><span class="sxs-lookup"><span data-stu-id="54c5d-122">Name</span></span>      |<span data-ttu-id="54c5d-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="54c5d-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="54c5d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="54c5d-124">Authorization</span></span> | <span data-ttu-id="54c5d-p103">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54c5d-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="54c5d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54c5d-127">Request body</span></span>

<span data-ttu-id="54c5d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="54c5d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54c5d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="54c5d-129">Response</span></span>

<span data-ttu-id="54c5d-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [de](../resources/group.md) grupo no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54c5d-130">If successful, this method returns a `200 OK` response code and a collection of [group](../resources/group.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="54c5d-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="54c5d-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="54c5d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54c5d-132">Request</span></span>

<span data-ttu-id="54c5d-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="54c5d-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="54c5d-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="54c5d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_incompatiblegroups"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleGroups
```
# <a name="c"></a>[<span data-ttu-id="54c5d-135">C#</span><span class="sxs-lookup"><span data-stu-id="54c5d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-incompatiblegroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="54c5d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54c5d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-incompatiblegroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="54c5d-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="54c5d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-incompatiblegroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="54c5d-138">Java</span><span class="sxs-lookup"><span data-stu-id="54c5d-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-incompatiblegroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="54c5d-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="54c5d-139">Response</span></span>

<span data-ttu-id="54c5d-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="54c5d-140">The following is an example of the response.</span></span>

> <span data-ttu-id="54c5d-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="54c5d-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "a743348f-5667-41a4-89a3-5ad8a94da5d2",
      "displayName": "group"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List incompatibleGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

