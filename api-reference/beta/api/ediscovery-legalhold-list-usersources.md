---
title: Listar legalHold userSources
description: Obter os recursos userSource da propriedade de navegação userSources.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 447b33207596e2d438ae635e5e8050e63a4076a5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773029"
---
# <a name="list-legalhold-usersources"></a><span data-ttu-id="ccd2e-103">Listar legalHold userSources</span><span class="sxs-lookup"><span data-stu-id="ccd2e-103">List legalHold userSources</span></span>

<span data-ttu-id="ccd2e-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="ccd2e-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ccd2e-105">Obter a lista de [objetos userSource](../resources/ediscovery-usersource.md) associados a uma responsabilidade legal.</span><span class="sxs-lookup"><span data-stu-id="ccd2e-105">Get the list of [userSource](../resources/ediscovery-usersource.md) objects associated with a legal hold.</span></span>

## <a name="permissions"></a><span data-ttu-id="ccd2e-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="ccd2e-106">Permissions</span></span>

<span data-ttu-id="ccd2e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccd2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ccd2e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ccd2e-109">Permission type</span></span>|<span data-ttu-id="ccd2e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ccd2e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ccd2e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ccd2e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ccd2e-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ccd2e-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="ccd2e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ccd2e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ccd2e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ccd2e-114">Not supported.</span></span>|
|<span data-ttu-id="ccd2e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ccd2e-115">Application</span></span>|<span data-ttu-id="ccd2e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ccd2e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ccd2e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ccd2e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/legalHolds/{legalholdId}/userSources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ccd2e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ccd2e-118">Optional query parameters</span></span>

<span data-ttu-id="ccd2e-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ccd2e-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ccd2e-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ccd2e-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ccd2e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ccd2e-121">Request headers</span></span>

|<span data-ttu-id="ccd2e-122">Nome</span><span class="sxs-lookup"><span data-stu-id="ccd2e-122">Name</span></span>|<span data-ttu-id="ccd2e-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccd2e-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ccd2e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ccd2e-124">Authorization</span></span>|<span data-ttu-id="ccd2e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ccd2e-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ccd2e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ccd2e-127">Request body</span></span>

<span data-ttu-id="ccd2e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ccd2e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ccd2e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccd2e-129">Response</span></span>

<span data-ttu-id="ccd2e-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ccd2e-130">If successful, this method returns a `200 OK` response code and a collection of [microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ccd2e-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ccd2e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ccd2e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ccd2e-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ccd2e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ccd2e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_usersource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/c816dd6f-5af8-40c5-a760-331361e05c60/legalHolds/277107ff-fee3-41a0-a665-a9d7f6c4824f/userSources
```
# <a name="c"></a>[<span data-ttu-id="ccd2e-134">C#</span><span class="sxs-lookup"><span data-stu-id="ccd2e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-usersource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ccd2e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ccd2e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-usersource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ccd2e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ccd2e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-usersource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ccd2e-137">Java</span><span class="sxs-lookup"><span data-stu-id="ccd2e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-usersource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ccd2e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccd2e-138">Response</span></span>

<span data-ttu-id="ccd2e-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ccd2e-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.userSource)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('c816dd6f-5af8-40c5-a760-331361e05c60')/legalholds('277107ff-fee3-41a0-a665-a9d7f6c4824f')/userSources",
    "value": [
        {
            "displayName": "Adele Vance",
            "createdDateTime": "2020-10-30T21:02:41.887Z",
            "id": "2f279b24-2142-435d-97c5-0d42220ba453",
            "email": "AdeleV@contoso.com",
            "includedSources": "mailbox",
            "createdBy": {
                "user": {
                    "id": null,
                    "displayName": "eDiscovery admin"
                }
            }
        }
    ]
}
```
