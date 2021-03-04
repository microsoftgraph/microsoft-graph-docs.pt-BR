---
title: Obter Contrato
description: Recupere as propriedades e as relações do objeto contract.
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 9e88686b3772fcd5f9c43ddd64e1c9eda865b518
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437270"
---
# <a name="get-contract"></a><span data-ttu-id="5ca99-103">Obter Contrato</span><span class="sxs-lookup"><span data-stu-id="5ca99-103">Get Contract</span></span>

<span data-ttu-id="5ca99-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ca99-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ca99-105">Recupere as propriedades e as relações do [objeto contract.](../resources/contract.md)</span><span class="sxs-lookup"><span data-stu-id="5ca99-105">Retrieve the properties and relationships of [contract](../resources/contract.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ca99-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5ca99-106">Permissions</span></span>

<span data-ttu-id="5ca99-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ca99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5ca99-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ca99-109">Permission type</span></span>      | <span data-ttu-id="5ca99-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5ca99-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ca99-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ca99-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5ca99-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5ca99-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5ca99-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ca99-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ca99-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ca99-114">Not supported.</span></span>    |
|<span data-ttu-id="5ca99-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ca99-115">Application</span></span> | <span data-ttu-id="5ca99-116">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ca99-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ca99-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ca99-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contracts/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5ca99-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5ca99-118">Optional query parameters</span></span>

<span data-ttu-id="5ca99-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5ca99-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5ca99-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ca99-120">Request headers</span></span>

| <span data-ttu-id="5ca99-121">Nome</span><span class="sxs-lookup"><span data-stu-id="5ca99-121">Name</span></span>      |<span data-ttu-id="5ca99-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ca99-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5ca99-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ca99-123">Authorization</span></span>  | <span data-ttu-id="5ca99-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ca99-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5ca99-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ca99-126">Request body</span></span>

<span data-ttu-id="5ca99-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5ca99-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ca99-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ca99-128">Response</span></span>

<span data-ttu-id="5ca99-129">Se tiver êxito, este método retornará um código de resposta e `200 OK` [um objeto Contract](../resources/contract.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ca99-129">If successful, this method returns a `200 OK` response code and [Contract](../resources/contract.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ca99-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ca99-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5ca99-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ca99-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5ca99-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ca99-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contracts/{id}
```
# <a name="c"></a>[<span data-ttu-id="5ca99-133">C#</span><span class="sxs-lookup"><span data-stu-id="5ca99-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contract-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ca99-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ca99-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contract-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ca99-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ca99-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contract-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5ca99-136">Java</span><span class="sxs-lookup"><span data-stu-id="5ca99-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contract-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5ca99-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ca99-137">Response</span></span>
<span data-ttu-id="5ca99-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ca99-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
