---
title: Obter noncustodialDataSource
description: Leia as propriedades e as relações de um objeto noncustodialDataSource.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 3f943ad2390becfe50185203b278c731e24faad4
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240935"
---
# <a name="get-noncustodialdatasource"></a><span data-ttu-id="1a7ae-103">Obter noncustodialDataSource</span><span class="sxs-lookup"><span data-stu-id="1a7ae-103">Get noncustodialDataSource</span></span>

<span data-ttu-id="1a7ae-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="1a7ae-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a7ae-105">Leia as propriedades e as relações de [um objeto noncustodialDataSource.](../resources/ediscovery-noncustodialdatasource.md)</span><span class="sxs-lookup"><span data-stu-id="1a7ae-105">Read the properties and relationships of a [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a7ae-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1a7ae-106">Permissions</span></span>

<span data-ttu-id="1a7ae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a7ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a7ae-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1a7ae-109">Permission type</span></span>|<span data-ttu-id="1a7ae-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1a7ae-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a7ae-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1a7ae-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1a7ae-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a7ae-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="1a7ae-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1a7ae-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a7ae-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a7ae-114">Not supported.</span></span>|
|<span data-ttu-id="1a7ae-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1a7ae-115">Application</span></span>|<span data-ttu-id="1a7ae-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a7ae-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a7ae-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1a7ae-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/noncustodialDataSources/{noncustodialDataSourceId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1a7ae-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1a7ae-118">Optional query parameters</span></span>

<span data-ttu-id="1a7ae-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1a7ae-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1a7ae-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1a7ae-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1a7ae-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1a7ae-121">Request headers</span></span>

|<span data-ttu-id="1a7ae-122">Nome</span><span class="sxs-lookup"><span data-stu-id="1a7ae-122">Name</span></span>|<span data-ttu-id="1a7ae-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a7ae-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1a7ae-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1a7ae-124">Authorization</span></span>|<span data-ttu-id="1a7ae-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a7ae-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a7ae-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1a7ae-127">Request body</span></span>

<span data-ttu-id="1a7ae-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1a7ae-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a7ae-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a7ae-129">Response</span></span>

<span data-ttu-id="1a7ae-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1a7ae-130">If successful, this method returns a `200 OK` response code and a [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1a7ae-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1a7ae-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1a7ae-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1a7ae-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1a7ae-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a7ae-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_noncustodialdatasource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/5b840b94-f821-4c4a-8cad-3a90062bf51a/noncustodialDataSources/8b69818bf6af4f8a9dede428401c71e7
```
# <a name="c"></a>[<span data-ttu-id="1a7ae-134">C#</span><span class="sxs-lookup"><span data-stu-id="1a7ae-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-noncustodialdatasource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1a7ae-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a7ae-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-noncustodialdatasource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1a7ae-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a7ae-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-noncustodialdatasource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1a7ae-137">Java</span><span class="sxs-lookup"><span data-stu-id="1a7ae-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-noncustodialdatasource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1a7ae-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a7ae-138">Response</span></span>

<span data-ttu-id="1a7ae-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1a7ae-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.noncustodialDataSource"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('5b840b94-f821-4c4a-8cad-3a90062bf51a')/noncustodialDataSources/$entity",
    "status": "Active",
    "lastModifiedDateTime": "2021-02-17T19:41:28.8714643Z",
    "releasedDateTime": "0001-01-01T00:00:00Z",
    "id": "8b69818bf6af4f8a9dede428401c71e7",
    "displayName": null,
    "createdDateTime": "2021-02-17T19:41:22.958104Z",
    "applyHoldToSource": true
}
```
