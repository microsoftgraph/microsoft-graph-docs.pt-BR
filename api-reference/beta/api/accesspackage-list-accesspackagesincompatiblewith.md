---
title: Listar accessPackagesIncompatibleWith
description: Recupere uma lista de pacotes de acesso que indicaram que seus direitos de acesso são incompatíveis com um pacote de acesso específico.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: def48d58dbbc757c6a248fe8dac40adff9372320
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439200"
---
# <a name="list-accesspackagesincompatiblewith"></a><span data-ttu-id="6d8e1-103">Listar accessPackagesIncompatibleWith</span><span class="sxs-lookup"><span data-stu-id="6d8e1-103">List accessPackagesIncompatibleWith</span></span>

<span data-ttu-id="6d8e1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d8e1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d8e1-105">Recupere uma lista dos [objetos accessPackage](../resources/accesspackage.md) que marcaram um [accessPackage especificado](../resources/accesspackage.md) como incompatível.</span><span class="sxs-lookup"><span data-stu-id="6d8e1-105">Retrieve a list of the [accessPackage](../resources/accesspackage.md) objects that have marked a specified [accessPackage](../resources/accesspackage.md) as incompatible.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d8e1-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="6d8e1-106">Permissions</span></span>

<span data-ttu-id="6d8e1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d8e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6d8e1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6d8e1-109">Permission type</span></span>                        | <span data-ttu-id="6d8e1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6d8e1-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6d8e1-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6d8e1-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6d8e1-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d8e1-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="6d8e1-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6d8e1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d8e1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6d8e1-114">Not supported.</span></span> |
| <span data-ttu-id="6d8e1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6d8e1-115">Application</span></span>                            | <span data-ttu-id="6d8e1-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d8e1-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d8e1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6d8e1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackage/{id}/accessPackagesIncompatibleWith
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6d8e1-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6d8e1-118">Optional query parameters</span></span>

<span data-ttu-id="6d8e1-119">Este método dá suporte aos parâmetros de consulta OData para pajamento no lado do servidor por meio de uma resposta grande.</span><span class="sxs-lookup"><span data-stu-id="6d8e1-119">This method supports the OData query parameters for server-side paging through a large response.</span></span> <span data-ttu-id="6d8e1-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="6d8e1-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6d8e1-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6d8e1-121">Request headers</span></span>

| <span data-ttu-id="6d8e1-122">Nome</span><span class="sxs-lookup"><span data-stu-id="6d8e1-122">Name</span></span>      |<span data-ttu-id="6d8e1-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d8e1-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6d8e1-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="6d8e1-124">Authorization</span></span> | <span data-ttu-id="6d8e1-p103">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6d8e1-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d8e1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6d8e1-127">Request body</span></span>

<span data-ttu-id="6d8e1-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6d8e1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d8e1-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d8e1-129">Response</span></span>

<span data-ttu-id="6d8e1-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos accessPackage](../resources/accesspackage.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6d8e1-130">If successful, this method returns a `200 OK` response code and a collection of [accessPackage](../resources/accesspackage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6d8e1-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6d8e1-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6d8e1-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6d8e1-132">Request</span></span>

<span data-ttu-id="6d8e1-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6d8e1-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6d8e1-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6d8e1-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackagesincompatiblewith"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}/accessPackagesIncompatibleWith
```
# <a name="c"></a>[<span data-ttu-id="6d8e1-135">C#</span><span class="sxs-lookup"><span data-stu-id="6d8e1-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackagesincompatiblewith-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6d8e1-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6d8e1-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackagesincompatiblewith-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6d8e1-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6d8e1-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackagesincompatiblewith-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6d8e1-138">Java</span><span class="sxs-lookup"><span data-stu-id="6d8e1-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackagesincompatiblewith-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="6d8e1-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="6d8e1-139">Response</span></span>

<span data-ttu-id="6d8e1-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6d8e1-140">The following is an example of the response.</span></span>

> <span data-ttu-id="6d8e1-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6d8e1-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "id": "c0a74b4d-2694-4d5d-a964-1bee4ff0aaf2",
      "catalogId": "c955f54f-e248-4155-b314-0bdd63f5aae9",
      "displayName": "accesspackage"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackagesIncompatibleWith",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


