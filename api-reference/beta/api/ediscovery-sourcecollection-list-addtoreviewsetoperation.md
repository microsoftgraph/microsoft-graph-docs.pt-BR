---
title: Listar addToReviewSetOperation
description: Obter o último objeto addToReviewSetOperation associado a uma coleção de origem.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: f5ef3f5831e04e125bd67de070c6089cfce90ce0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772664"
---
# <a name="list-addtoreviewsetoperation"></a><span data-ttu-id="78dec-103">Listar addToReviewSetOperation</span><span class="sxs-lookup"><span data-stu-id="78dec-103">List addToReviewSetOperation</span></span>

<span data-ttu-id="78dec-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="78dec-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78dec-105">Obter o último [objeto addToReviewSetOperation](../resources/ediscovery-addtoreviewsetoperation.md) associado a uma coleção de origem.</span><span class="sxs-lookup"><span data-stu-id="78dec-105">Get the last [addToReviewSetOperation](../resources/ediscovery-addtoreviewsetoperation.md) object associated with a source collection.</span></span> 

><span data-ttu-id="78dec-106">**Observação:** Este método lista apenas a última operação; ele não retorna um histórico de todas as operações.</span><span class="sxs-lookup"><span data-stu-id="78dec-106">**Note:** This method only lists the last operation; it does not return a history of all operations.</span></span>

## <a name="permissions"></a><span data-ttu-id="78dec-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="78dec-107">Permissions</span></span>

<span data-ttu-id="78dec-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78dec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78dec-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78dec-110">Permission type</span></span>|<span data-ttu-id="78dec-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="78dec-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78dec-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78dec-112">Delegated (work or school account)</span></span>|<span data-ttu-id="78dec-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78dec-113">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="78dec-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78dec-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78dec-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78dec-115">Not supported.</span></span>|
|<span data-ttu-id="78dec-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="78dec-116">Application</span></span>|<span data-ttu-id="78dec-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78dec-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="78dec-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78dec-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/addToReviewSetOperation
```

## <a name="optional-query-parameters"></a><span data-ttu-id="78dec-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="78dec-119">Optional query parameters</span></span>

<span data-ttu-id="78dec-120">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="78dec-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="78dec-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="78dec-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="78dec-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="78dec-122">Request headers</span></span>

|<span data-ttu-id="78dec-123">Nome</span><span class="sxs-lookup"><span data-stu-id="78dec-123">Name</span></span>|<span data-ttu-id="78dec-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="78dec-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="78dec-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="78dec-125">Authorization</span></span>|<span data-ttu-id="78dec-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78dec-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="78dec-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="78dec-128">Request body</span></span>

<span data-ttu-id="78dec-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="78dec-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78dec-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="78dec-130">Response</span></span>

<span data-ttu-id="78dec-131">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto microsoft.graph.ediscovery.addToReviewSetOperation](../resources/ediscovery-addtoreviewsetoperation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78dec-131">If successful, this method returns a `200 OK` response code and a [microsoft.graph.ediscovery.addToReviewSetOperation](../resources/ediscovery-addtoreviewsetoperation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="78dec-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="78dec-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="78dec-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78dec-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="78dec-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="78dec-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_addtoreviewsetoperation"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/sourceCollections/1a9b4145d8f84e39bc45a7f68c5c5119/addToReviewSetOperation
```
# <a name="c"></a>[<span data-ttu-id="78dec-135">C#</span><span class="sxs-lookup"><span data-stu-id="78dec-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-addtoreviewsetoperation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="78dec-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="78dec-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-addtoreviewsetoperation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="78dec-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="78dec-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-addtoreviewsetoperation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="78dec-138">Java</span><span class="sxs-lookup"><span data-stu-id="78dec-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-addtoreviewsetoperation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="78dec-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="78dec-139">Response</span></span>

<span data-ttu-id="78dec-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="78dec-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.addToReviewSetOperation)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.ediscovery.addToReviewSetOperation",
      "id": "9055c657-c657-9055-57c6-559057c65590",
      "createdDateTime": "String (timestamp)",
      "completedDateTime": "String (timestamp)",
      "percentProgress": "Integer",
      "status": "String",
      "action": "String",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "resultInfo": {
        "@odata.type": "microsoft.graph.resultInfo"
      }
    }
  ]
}
```
