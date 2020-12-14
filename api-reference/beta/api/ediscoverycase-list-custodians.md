---
title: Listar os responsáveis
description: Obtenha uma lista dos objetos responsáveis e suas propriedades.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: d1d387e396b8ed413cb6796c6df95058363b7e6d
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49657136"
---
# <a name="list-custodians"></a><span data-ttu-id="0dd5f-103">Listar os responsáveis</span><span class="sxs-lookup"><span data-stu-id="0dd5f-103">List custodians</span></span>

<span data-ttu-id="0dd5f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0dd5f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0dd5f-105">Obtenha uma lista dos objetos [responsáveis](../resources/custodian.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="0dd5f-105">Get a list of the [custodian](../resources/custodian.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="0dd5f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0dd5f-106">Permissions</span></span>

<span data-ttu-id="0dd5f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0dd5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0dd5f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0dd5f-109">Permission type</span></span>|<span data-ttu-id="0dd5f-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0dd5f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0dd5f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0dd5f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0dd5f-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="0dd5f-112">User.Read</span></span>|
|<span data-ttu-id="0dd5f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0dd5f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0dd5f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0dd5f-114">Not supported.</span></span>|
|<span data-ttu-id="0dd5f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0dd5f-115">Application</span></span>|<span data-ttu-id="0dd5f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0dd5f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0dd5f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0dd5f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0dd5f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0dd5f-118">Optional query parameters</span></span>

<span data-ttu-id="0dd5f-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0dd5f-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="0dd5f-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0dd5f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0dd5f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0dd5f-121">Request headers</span></span>

|<span data-ttu-id="0dd5f-122">Nome</span><span class="sxs-lookup"><span data-stu-id="0dd5f-122">Name</span></span>|<span data-ttu-id="0dd5f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="0dd5f-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0dd5f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="0dd5f-124">Authorization</span></span>|<span data-ttu-id="0dd5f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0dd5f-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0dd5f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0dd5f-127">Request body</span></span>

<span data-ttu-id="0dd5f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0dd5f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0dd5f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0dd5f-129">Response</span></span>

<span data-ttu-id="0dd5f-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [responsáveis](../resources/custodian.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0dd5f-130">If successful, this method returns a `200 OK` response code and a collection of [custodian](../resources/custodian.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0dd5f-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0dd5f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0dd5f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0dd5f-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0dd5f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0dd5f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_custodian"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians
```
# <a name="c"></a>[<span data-ttu-id="0dd5f-134">C#</span><span class="sxs-lookup"><span data-stu-id="0dd5f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-custodian-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0dd5f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0dd5f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-custodian-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0dd5f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0dd5f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-custodian-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0dd5f-137">Java</span><span class="sxs-lookup"><span data-stu-id="0dd5f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-custodian-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0dd5f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="0dd5f-138">Response</span></span>

<span data-ttu-id="0dd5f-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0dd5f-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.custodian)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians",
    "value": [
        {
            "email": "meganb@contoso.com",
            "applyHoldToSources": false,
            "status": "released",
            "createdDateTime": "2020-10-27T15:55:43.4971108Z",
            "lastModifiedDateTime": "2020-10-30T05:34:00.947558Z",
            "releasedDateTime": "2020-10-27T15:55:58.2338864Z",
            "acknowledgedDateTime": null,
            "id": "fd03ce02ecde42a58d24fcbc9ebbea3e",
            "displayName": "Megan Bowen"
        },
        {
            "email": "AdeleV@contoso.com",
            "applyHoldToSources": true,
            "status": "active",
            "createdDateTime": "2020-08-21T13:20:02.0117254Z",
            "lastModifiedDateTime": "2020-10-27T15:14:14.1244649Z",
            "releasedDateTime": null,
            "acknowledgedDateTime": null,
            "id": "2192ca408ea2410eba3bec8ae873be6b",
            "displayName": "Adele Vance"
        }
    ]
}
```
