---
title: Obter configurações
description: Leia as propriedades e as relações de um objeto settings.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: a119efd1541aef242bbe0d8ece72593d1871f012
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240861"
---
# <a name="get-settings"></a><span data-ttu-id="45a07-103">Obter configurações</span><span class="sxs-lookup"><span data-stu-id="45a07-103">Get settings</span></span>

<span data-ttu-id="45a07-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="45a07-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45a07-105">Leia as propriedades e as relações de um [objeto settings.](../resources/ediscovery-settings.md)</span><span class="sxs-lookup"><span data-stu-id="45a07-105">Read the properties and relationships of a [settings](../resources/ediscovery-settings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="45a07-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="45a07-106">Permissions</span></span>

<span data-ttu-id="45a07-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45a07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45a07-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45a07-109">Permission type</span></span>|<span data-ttu-id="45a07-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="45a07-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45a07-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45a07-111">Delegated (work or school account)</span></span>|<span data-ttu-id="45a07-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45a07-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="45a07-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45a07-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45a07-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45a07-114">Not supported.</span></span>|
|<span data-ttu-id="45a07-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45a07-115">Application</span></span>|<span data-ttu-id="45a07-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45a07-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45a07-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45a07-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /compliance/ediscovery/cases/{caseId}/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="45a07-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="45a07-118">Optional query parameters</span></span>

<span data-ttu-id="45a07-119">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="45a07-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="45a07-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="45a07-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="45a07-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45a07-121">Request headers</span></span>

|<span data-ttu-id="45a07-122">Nome</span><span class="sxs-lookup"><span data-stu-id="45a07-122">Name</span></span>|<span data-ttu-id="45a07-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="45a07-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="45a07-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="45a07-124">Authorization</span></span>|<span data-ttu-id="45a07-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45a07-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="45a07-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45a07-127">Request body</span></span>

<span data-ttu-id="45a07-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="45a07-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45a07-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="45a07-129">Response</span></span>

<span data-ttu-id="45a07-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto settings](../resources/ediscovery-settings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="45a07-130">If successful, this method returns a `200 OK` response code and a [settings](../resources/ediscovery-settings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="45a07-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="45a07-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="45a07-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45a07-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="45a07-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="45a07-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_settings"
}
-->

``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases/5b840b94-f821-4c4a-8cad-3a90062bf51a/settings
```
# <a name="c"></a>[<span data-ttu-id="45a07-134">C#</span><span class="sxs-lookup"><span data-stu-id="45a07-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="45a07-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45a07-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="45a07-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="45a07-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="45a07-137">Java</span><span class="sxs-lookup"><span data-stu-id="45a07-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-settings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="45a07-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="45a07-138">Response</span></span>

<span data-ttu-id="45a07-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="45a07-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.settings"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('5b840b94-f821-4c4a-8cad-3a90062bf51a')/settings/$entity",
    "id": "5b840b94-f821-4c4a-8cad-3a90062bf51a",
    "redundancyDetection": {
        "isEnabled": true,
        "similarityThreshold": 65,
        "minWords": 10,
        "maxWords": 500000
    },
    "topicModeling": {
        "isEnabled": true,
        "ignoreNumbers": true,
        "topicCount": 100,
        "dynamicallyAdjustTopicCount": true
    },
    "ocr": {
        "isEnabled": false,
        "maxImageSize": 24576,
        "timeout": "PT1M"
    }
}
```
