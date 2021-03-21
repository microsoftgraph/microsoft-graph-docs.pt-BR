---
title: Listar contratos
description: Recupere uma lista de objetos de contrato associados a um locatário parceiro.
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 5c0ee3ae9ac6017978620914425a676c0dde4c91
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963873"
---
# <a name="list-contracts"></a><span data-ttu-id="1dc62-103">Listar contratos</span><span class="sxs-lookup"><span data-stu-id="1dc62-103">List contracts</span></span>

<span data-ttu-id="1dc62-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1dc62-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1dc62-105">Recupere uma lista de [objetos de](../resources/contract.md) contrato associados a um locatário parceiro.</span><span class="sxs-lookup"><span data-stu-id="1dc62-105">Retrieve a list of [contract](../resources/contract.md) objects associated to a partner tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="1dc62-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1dc62-106">Permissions</span></span>

<span data-ttu-id="1dc62-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1dc62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1dc62-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1dc62-109">Permission type</span></span>      | <span data-ttu-id="1dc62-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1dc62-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1dc62-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1dc62-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1dc62-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1dc62-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1dc62-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1dc62-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1dc62-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1dc62-114">Not supported.</span></span>    |
|<span data-ttu-id="1dc62-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1dc62-115">Application</span></span> | <span data-ttu-id="1dc62-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dc62-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1dc62-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1dc62-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /contracts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1dc62-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1dc62-118">Optional query parameters</span></span>

<span data-ttu-id="1dc62-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1dc62-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span> 

> <span data-ttu-id="1dc62-120">A filtragem é suportada para customerId, defaultDomainName e displayName.</span><span class="sxs-lookup"><span data-stu-id="1dc62-120">Filtering is supported for customerId, defaultDomainName, and displayName.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1dc62-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1dc62-121">Request headers</span></span>

| <span data-ttu-id="1dc62-122">Nome</span><span class="sxs-lookup"><span data-stu-id="1dc62-122">Name</span></span>      |<span data-ttu-id="1dc62-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="1dc62-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1dc62-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1dc62-124">Authorization</span></span>  | <span data-ttu-id="1dc62-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1dc62-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1dc62-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1dc62-127">Request body</span></span>

<span data-ttu-id="1dc62-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1dc62-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1dc62-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dc62-129">Response</span></span>

<span data-ttu-id="1dc62-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [Contract](../resources/contract.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1dc62-130">If successful, this method returns a `200 OK` response code and a collection of [Contract](../resources/contract.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1dc62-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1dc62-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1dc62-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1dc62-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1dc62-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1dc62-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contract_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contracts
```
# <a name="c"></a>[<span data-ttu-id="1dc62-134">C#</span><span class="sxs-lookup"><span data-stu-id="1dc62-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contract-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1dc62-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1dc62-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contract-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1dc62-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1dc62-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contract-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1dc62-137">Java</span><span class="sxs-lookup"><span data-stu-id="1dc62-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contract-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1dc62-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="1dc62-138">Response</span></span>

<span data-ttu-id="1dc62-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1dc62-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contract",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
    {
      "contractType": "contractType-value",
      "customerId": "customerId-value",
      "defaultDomainName": "defaultDomainName-value",
      "displayName": "displayName-value",
      "id": "id-value"
    }
  ]
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
