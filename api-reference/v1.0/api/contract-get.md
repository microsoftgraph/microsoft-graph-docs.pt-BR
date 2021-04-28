---
title: Obter Contrato
description: Recupere as propriedades e as relações do objeto contract.
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: b543431318db3a53b96e0c122ca7ad489063c2df
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52035698"
---
# <a name="get-contract"></a><span data-ttu-id="a72e2-103">Obter Contrato</span><span class="sxs-lookup"><span data-stu-id="a72e2-103">Get Contract</span></span>

<span data-ttu-id="a72e2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a72e2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a72e2-105">Recupere as propriedades e as relações do [objeto contract.](../resources/contract.md)</span><span class="sxs-lookup"><span data-stu-id="a72e2-105">Retrieve the properties and relationships of [contract](../resources/contract.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a72e2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a72e2-106">Permissions</span></span>

<span data-ttu-id="a72e2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a72e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a72e2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a72e2-109">Permission type</span></span>      | <span data-ttu-id="a72e2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a72e2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a72e2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a72e2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a72e2-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a72e2-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a72e2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a72e2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a72e2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a72e2-114">Not supported.</span></span>    |
|<span data-ttu-id="a72e2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a72e2-115">Application</span></span> | <span data-ttu-id="a72e2-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a72e2-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a72e2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a72e2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contracts/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a72e2-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a72e2-118">Optional query parameters</span></span>

<span data-ttu-id="a72e2-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a72e2-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a72e2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a72e2-120">Request headers</span></span>

| <span data-ttu-id="a72e2-121">Nome</span><span class="sxs-lookup"><span data-stu-id="a72e2-121">Name</span></span>      |<span data-ttu-id="a72e2-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a72e2-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a72e2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a72e2-123">Authorization</span></span>  | <span data-ttu-id="a72e2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a72e2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a72e2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a72e2-126">Request body</span></span>

<span data-ttu-id="a72e2-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a72e2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a72e2-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="a72e2-128">Response</span></span>

<span data-ttu-id="a72e2-129">Se tiver êxito, este método retornará um código de resposta e `200 OK` [um objeto Contract](../resources/contract.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a72e2-129">If successful, this method returns a `200 OK` response code and [Contract](../resources/contract.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a72e2-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a72e2-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a72e2-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a72e2-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="a72e2-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a72e2-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contract_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contracts/{id}
```
# <a name="c"></a>[<span data-ttu-id="a72e2-133">C#</span><span class="sxs-lookup"><span data-stu-id="a72e2-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contract-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a72e2-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a72e2-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contract-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a72e2-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a72e2-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contract-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a72e2-136">Java</span><span class="sxs-lookup"><span data-stu-id="a72e2-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contract-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a72e2-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="a72e2-137">Response</span></span>
<span data-ttu-id="a72e2-138">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a72e2-138">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contract"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 186

{
  "contractType": "contractType-value",
  "customerId": "customerId-value",
  "defaultDomainName": "defaultDomainName-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Contract",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
