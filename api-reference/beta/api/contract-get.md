---
title: Obter contrato
description: Recupere as propriedades e os relacionamentos do objeto Contract.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 211ab44f694ae7df56023526159d21896b0b1304
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48002830"
---
# <a name="get-contract"></a><span data-ttu-id="577fb-103">Obter contrato</span><span class="sxs-lookup"><span data-stu-id="577fb-103">Get Contract</span></span>

<span data-ttu-id="577fb-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="577fb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="577fb-105">Recupere as propriedades e os relacionamentos do objeto [Contract](../resources/contract.md) .</span><span class="sxs-lookup"><span data-stu-id="577fb-105">Retrieve the properties and relationships of [contract](../resources/contract.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="577fb-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="577fb-106">Permissions</span></span>

<span data-ttu-id="577fb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="577fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="577fb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="577fb-109">Permission type</span></span>      | <span data-ttu-id="577fb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="577fb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="577fb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="577fb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="577fb-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="577fb-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="577fb-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="577fb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="577fb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="577fb-114">Not supported.</span></span>    |
|<span data-ttu-id="577fb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="577fb-115">Application</span></span> | <span data-ttu-id="577fb-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="577fb-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="577fb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="577fb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contracts/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="577fb-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="577fb-118">Optional query parameters</span></span>

<span data-ttu-id="577fb-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="577fb-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="577fb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="577fb-120">Request headers</span></span>

| <span data-ttu-id="577fb-121">Nome</span><span class="sxs-lookup"><span data-stu-id="577fb-121">Name</span></span>      |<span data-ttu-id="577fb-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="577fb-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="577fb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="577fb-123">Authorization</span></span>  | <span data-ttu-id="577fb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="577fb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="577fb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="577fb-126">Request body</span></span>

<span data-ttu-id="577fb-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="577fb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="577fb-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="577fb-128">Response</span></span>

<span data-ttu-id="577fb-129">Se bem-sucedido, este método retorna o `200 OK` código de resposta e o objeto [Contract](../resources/contract.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="577fb-129">If successful, this method returns a `200 OK` response code and [Contract](../resources/contract.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="577fb-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="577fb-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="577fb-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="577fb-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="577fb-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="577fb-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contracts/{id}
```
# <a name="c"></a>[<span data-ttu-id="577fb-133">C#</span><span class="sxs-lookup"><span data-stu-id="577fb-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contract-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="577fb-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="577fb-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contract-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="577fb-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="577fb-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contract-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="577fb-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="577fb-136">Response</span></span>
<span data-ttu-id="577fb-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="577fb-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Contract"
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
<!--
{
  "type": "#page.annotation",
  "description": "Get Contract",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


