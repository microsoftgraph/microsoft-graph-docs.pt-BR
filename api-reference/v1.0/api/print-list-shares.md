---
title: Listar shares
description: Recupere uma lista de compartilhamentos de impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 1841f80be8d5062419f4b12d98f25e062e91ed49
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777156"
---
# <a name="list-shares"></a><span data-ttu-id="39335-103">Listar shares</span><span class="sxs-lookup"><span data-stu-id="39335-103">List shares</span></span>
<span data-ttu-id="39335-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39335-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="39335-105">Recuperar uma lista de **printerShares**.</span><span class="sxs-lookup"><span data-stu-id="39335-105">Retrieve a list of **printerShares**.</span></span>

## <a name="permissions"></a><span data-ttu-id="39335-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="39335-106">Permissions</span></span>
<span data-ttu-id="39335-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39335-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="39335-109">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="39335-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span>

|<span data-ttu-id="39335-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="39335-110">Permission type</span></span> | <span data-ttu-id="39335-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="39335-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="39335-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="39335-112">Delegated (work or school account)</span></span>| <span data-ttu-id="39335-113">PrinterShare.Read.All, PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39335-113">PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="39335-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="39335-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39335-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39335-115">Not Supported.</span></span>|
|<span data-ttu-id="39335-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="39335-116">Application</span></span>|<span data-ttu-id="39335-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39335-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="39335-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="39335-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/shares
```

## <a name="optional-query-parameters"></a><span data-ttu-id="39335-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="39335-119">Optional query parameters</span></span>
<span data-ttu-id="39335-120">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="39335-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="39335-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="39335-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="39335-122">Para ver uma lista dos recursos de cada compartilhamento de impressora, inclua o parâmetro `$select=capabilities` de consulta opcional.</span><span class="sxs-lookup"><span data-stu-id="39335-122">To see a list of each printer share's capabilities, include the optional `$select=capabilities` query parameter.</span></span>

### <a name="exceptions"></a><span data-ttu-id="39335-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="39335-123">Exceptions</span></span>
<span data-ttu-id="39335-124">Alguns operadores não têm suporte: `$count` , `$orderby` , `$search` .</span><span class="sxs-lookup"><span data-stu-id="39335-124">Some operators are not supported: `$count`, `$orderby`, `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="39335-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="39335-125">Request headers</span></span>
|<span data-ttu-id="39335-126">Nome</span><span class="sxs-lookup"><span data-stu-id="39335-126">Name</span></span>|<span data-ttu-id="39335-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="39335-127">Description</span></span>|
|:---|:---|
|<span data-ttu-id="39335-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="39335-128">Authorization</span></span>|<span data-ttu-id="39335-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="39335-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="39335-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="39335-131">Request body</span></span>
<span data-ttu-id="39335-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="39335-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39335-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="39335-133">Response</span></span>

<span data-ttu-id="39335-134">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos printerShare](../resources/printershare.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="39335-134">If successful, this method returns a `200 OK` response code and a collection of [printerShare](../resources/printershare.md) objects in the response body.</span></span>

><span data-ttu-id="39335-135">**Observação**: a resposta não conterá as **propriedades padrão** **e de** recursos.</span><span class="sxs-lookup"><span data-stu-id="39335-135">**Note**: The response will not contain the **defaults** and **capabilities** properties.</span></span> <span data-ttu-id="39335-136">Você pode obter essas propriedades por meio de uma [solicitação Get printerShare.](printershare-get.md)</span><span class="sxs-lookup"><span data-stu-id="39335-136">You can get these properties via a [Get printerShare](printershare-get.md) request.</span></span>

## <a name="examples"></a><span data-ttu-id="39335-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="39335-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="39335-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="39335-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="39335-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="39335-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_printershare"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/shares
```
# <a name="c"></a>[<span data-ttu-id="39335-140">C#</span><span class="sxs-lookup"><span data-stu-id="39335-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-printershare-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39335-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39335-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-printershare-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39335-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39335-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-printershare-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="39335-143">Java</span><span class="sxs-lookup"><span data-stu-id="39335-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-printershare-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="39335-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="39335-144">Response</span></span>
<span data-ttu-id="39335-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="39335-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.printerShare)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/shares",
      "id": "d837c17b-3296-4384-a053-828d56e10f50",
      "displayName": "PrinterShare Name",
      "createdDateTime": "2020-02-04T00:00:00.0000000Z",
      "isAcceptingJobs": true,
      "allowAllUsers": false,
      "status": {
        "state": "stopped",
        "details": [
          "disconnected"
        ],
        "description": ""
      },
      "defaults": {
        "copiesPerJob": 1,
        "finishings": [
          "none"
        ],
        "mediaColor": "Unknown",
        "mediaType": "stationery",
        "mediaSize": "North America Letter",
        "pagesPerSheet": 1,
        "orientation": "portrait",
        "outputBin": "auto",
        "inputBin": "auto",
        "contentType": "application/oxps",
        "fitPdfToPage": false,
        "multipageLayout": null,
        "colorMode": "color",
        "quality": "medium",
        "duplexMode": "oneSided",
        "dpi": 600,
        "scaling": null
      },
      "location": {
        "latitude": 47.6450,
        "longitude": -122.1409,
        "altitudeInMeters": 3,
        "streetAddress": "One Microsoft Way",
        "subUnit": [
          "Main Plaza",
          "Unit 400"
        ],
        "city": "Redmond",
        "postalCode": "98052",
        "countryOrRegion": "USA",
        "site": "Puget Sound",
        "building": "Studio E",
        "floor": "1",
        "floorDescription": "First Floor",
        "roomName": "1234",
        "roomDescription": "First floor copy room",
        "organization": [
          "C+AI",
          "Microsoft Graph"
        ],
        "subdivision": [
          "King County",
          "Red West"
        ],
        "stateOrProvince": "Washington"
      }
    }
  ]
}
```

