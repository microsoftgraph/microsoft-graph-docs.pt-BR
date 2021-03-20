---
title: Obter custodiatário
description: Leia as propriedades e as relações de um objeto custodiante.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 18fc6d6bb852b8615c3b30e34bd88789c026390d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946303"
---
# <a name="get-custodian"></a><span data-ttu-id="cda72-103">Obter custodiatário</span><span class="sxs-lookup"><span data-stu-id="cda72-103">Get custodian</span></span>

<span data-ttu-id="cda72-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="cda72-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cda72-105">Leia as propriedades e as relações de um [objeto custodiante.](../resources/ediscovery-custodian.md)</span><span class="sxs-lookup"><span data-stu-id="cda72-105">Read the properties and relationships of a [custodian](../resources/ediscovery-custodian.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cda72-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cda72-106">Permissions</span></span>

<span data-ttu-id="cda72-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cda72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cda72-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cda72-109">Permission type</span></span>|<span data-ttu-id="cda72-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cda72-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cda72-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cda72-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cda72-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cda72-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="cda72-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cda72-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cda72-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cda72-114">Not supported.</span></span>|
|<span data-ttu-id="cda72-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cda72-115">Application</span></span>|<span data-ttu-id="cda72-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cda72-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cda72-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cda72-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caesId}/custodians/{custodianId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cda72-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cda72-118">Optional query parameters</span></span>

<span data-ttu-id="cda72-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cda72-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="cda72-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="cda72-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="cda72-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cda72-121">Request headers</span></span>

|<span data-ttu-id="cda72-122">Nome</span><span class="sxs-lookup"><span data-stu-id="cda72-122">Name</span></span>|<span data-ttu-id="cda72-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="cda72-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cda72-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="cda72-124">Authorization</span></span>|<span data-ttu-id="cda72-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cda72-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cda72-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cda72-127">Request body</span></span>

<span data-ttu-id="cda72-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cda72-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cda72-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="cda72-129">Response</span></span>

<span data-ttu-id="cda72-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cda72-130">If successful, this method returns a `200 OK` response code and a [microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cda72-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cda72-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cda72-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cda72-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="cda72-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="cda72-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_custodian_2"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians/45454331323337443946343043464239
```
# <a name="c"></a>[<span data-ttu-id="cda72-134">C#</span><span class="sxs-lookup"><span data-stu-id="cda72-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-custodian-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cda72-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cda72-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-custodian-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cda72-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cda72-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-custodian-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cda72-137">Java</span><span class="sxs-lookup"><span data-stu-id="cda72-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-custodian-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cda72-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="cda72-138">Response</span></span>

<span data-ttu-id="cda72-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cda72-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.custodian"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians/$entity",
    "email": "AdeleV@contoso.com",
    "applyHoldToSources": true,
    "status": "active",
    "createdDateTime": "2020-10-30T20:59:54.9900703Z",
    "lastModifiedDateTime": "2020-10-30T20:59:55.1400013Z",
    "releasedDateTime": null,
    "acknowledgedDateTime": null,
    "id": "45454331323337443946343043464239",
    "displayName": "Adele Vance"
}
```
