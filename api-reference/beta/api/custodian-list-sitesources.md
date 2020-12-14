---
title: Listar siteSources
description: Obter uma lista dos objetos SiteName e suas propriedades.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 7510efdde8cbf248643bfa0429d63e05f2bc8dea
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659335"
---
# <a name="list-sitesources"></a><span data-ttu-id="c18ff-103">Listar siteSources</span><span class="sxs-lookup"><span data-stu-id="c18ff-103">List siteSources</span></span>

<span data-ttu-id="c18ff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c18ff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c18ff-105">Obter uma lista de objetos de [site de site](../resources/sitesource.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="c18ff-105">Get a list of [siteSource](../resources/sitesource.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="c18ff-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c18ff-106">Permissions</span></span>

<span data-ttu-id="c18ff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c18ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c18ff-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c18ff-109">Permission type</span></span>|<span data-ttu-id="c18ff-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c18ff-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c18ff-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c18ff-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c18ff-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="c18ff-112">User.Read</span></span>|
|<span data-ttu-id="c18ff-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c18ff-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c18ff-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c18ff-114">Not supported.</span></span>|
|<span data-ttu-id="c18ff-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c18ff-115">Application</span></span>|<span data-ttu-id="c18ff-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c18ff-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c18ff-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c18ff-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/siteSources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c18ff-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c18ff-118">Optional query parameters</span></span>

<span data-ttu-id="c18ff-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c18ff-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c18ff-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c18ff-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c18ff-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c18ff-121">Request headers</span></span>

|<span data-ttu-id="c18ff-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c18ff-122">Name</span></span>|<span data-ttu-id="c18ff-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c18ff-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c18ff-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c18ff-124">Authorization</span></span>|<span data-ttu-id="c18ff-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c18ff-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c18ff-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c18ff-127">Request body</span></span>

<span data-ttu-id="c18ff-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c18ff-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c18ff-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="c18ff-129">Response</span></span>

<span data-ttu-id="c18ff-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [sitery](../resources/sitesource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c18ff-130">If successful, this method returns a `200 OK` response code and a collection of [siteSource](../resources/sitesource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c18ff-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c18ff-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c18ff-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c18ff-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c18ff-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c18ff-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_sitesource"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/siteSources
```
# <a name="c"></a>[<span data-ttu-id="c18ff-134">C#</span><span class="sxs-lookup"><span data-stu-id="c18ff-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-sitesource-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c18ff-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c18ff-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-sitesource-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c18ff-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c18ff-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-sitesource-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c18ff-137">Java</span><span class="sxs-lookup"><span data-stu-id="c18ff-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-sitesource-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c18ff-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="c18ff-138">Response</span></span>

<span data-ttu-id="c18ff-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c18ff-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.siteSource)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians('2192ca408ea2410eba3bec8ae873be6b')/siteSources",
    "value": [
        {
            "displayName": "Microsoft Team Site",
            "createdDateTime": "2020-10-27T15:14:11.0048392Z",
            "id": "38304445-3741-3333-4233-344238454333",
            "createdBy": {
                "user": {
                    "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
                    "displayName": null
                }
            }
        }
    ]
}
```
