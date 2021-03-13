---
title: Get printerShare
description: Recupere as propriedades e as relações de um compartilhamento de impressora.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: e9a16d9d615b780d921ff49291d6b15edda2ed3f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771607"
---
# <a name="get-printershare"></a><span data-ttu-id="65d17-103">Get printerShare</span><span class="sxs-lookup"><span data-stu-id="65d17-103">Get printerShare</span></span>
<span data-ttu-id="65d17-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65d17-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="65d17-105">Recupere as propriedades e as relações de um compartilhamento de impressora.</span><span class="sxs-lookup"><span data-stu-id="65d17-105">Retrieve the properties and relationships of a printer share.</span></span>

## <a name="permissions"></a><span data-ttu-id="65d17-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="65d17-106">Permissions</span></span>
<span data-ttu-id="65d17-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65d17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="65d17-109">Além das permissões a seguir, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="65d17-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="65d17-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="65d17-110">Permission type</span></span> | <span data-ttu-id="65d17-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="65d17-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="65d17-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="65d17-112">Delegated (work or school account)</span></span>| <span data-ttu-id="65d17-113">PrinterShare.ReadBasic.All, PrinterShare.Read.All, PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65d17-113">PrinterShare.ReadBasic.All, PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="65d17-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="65d17-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65d17-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="65d17-115">Not Supported.</span></span>|
|<span data-ttu-id="65d17-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="65d17-116">Application</span></span>|<span data-ttu-id="65d17-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="65d17-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="65d17-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="65d17-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/shares/{printerShareId}
GET /print/printers/{printerId}/shares/{printerShareId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="65d17-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="65d17-119">Optional query parameters</span></span>
<span data-ttu-id="65d17-120">Este método dá suporte a alguns dos parâmetros de consulta OData, incluindo `$select` e , para ajudar a personalizar a `$expand` resposta.</span><span class="sxs-lookup"><span data-stu-id="65d17-120">This method supports some of the OData query parameters, including `$select` and `$expand`, to help customize the response.</span></span> <span data-ttu-id="65d17-121">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="65d17-121">For example:</span></span> 

<span data-ttu-id="65d17-122">por exemplo,</span><span class="sxs-lookup"><span data-stu-id="65d17-122">e.g.</span></span> 
```http
GET /print/printers/{id}?$select=id,displayName,capabilities
```
<span data-ttu-id="65d17-123">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="65d17-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="65d17-124">Exceptions</span><span class="sxs-lookup"><span data-stu-id="65d17-124">Exceptions</span></span>
* <span data-ttu-id="65d17-125">O `$count` operador não tem suporte.</span><span class="sxs-lookup"><span data-stu-id="65d17-125">The `$count` operator is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="65d17-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="65d17-126">Request headers</span></span>
|<span data-ttu-id="65d17-127">Nome</span><span class="sxs-lookup"><span data-stu-id="65d17-127">Name</span></span>|<span data-ttu-id="65d17-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="65d17-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="65d17-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="65d17-129">Authorization</span></span>|<span data-ttu-id="65d17-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="65d17-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="65d17-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="65d17-132">Request body</span></span>
<span data-ttu-id="65d17-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="65d17-133">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="65d17-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="65d17-134">Response</span></span>
<span data-ttu-id="65d17-135">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [printerShare](../resources/printershare.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="65d17-135">If successful, this method returns a `200 OK` response code and a [printerShare](../resources/printershare.md) object in the response body.</span></span>
<span data-ttu-id="65d17-136">Por padrão, a resposta não conterá [printerCapabilities](../resources/printerCapabilities.md).</span><span class="sxs-lookup"><span data-stu-id="65d17-136">By default, the response will not contain [printerCapabilities](../resources/printerCapabilities.md).</span></span> <span data-ttu-id="65d17-137">Para obter **printerCapabilities**, use `$select` o parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="65d17-137">To get **printerCapabilities**, use the `$select` query parameter.</span></span> 

## <a name="response"></a><span data-ttu-id="65d17-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="65d17-138">Response</span></span>

<span data-ttu-id="65d17-139">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [printerShare](../resources/printershare.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="65d17-139">If successful, this method returns a `200 OK` response code and a [printerShare](../resources/printershare.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="65d17-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="65d17-140">Examples</span></span>

### <a name="example-1-get-a-printershare"></a><span data-ttu-id="65d17-141">Exemplo 1: Obter uma printerShare</span><span class="sxs-lookup"><span data-stu-id="65d17-141">Example 1: Get a printerShare</span></span>

#### <a name="request"></a><span data-ttu-id="65d17-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="65d17-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="65d17-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="65d17-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printershare"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/shares/{printerShareId}
```
# <a name="c"></a>[<span data-ttu-id="65d17-144">C#</span><span class="sxs-lookup"><span data-stu-id="65d17-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printershare-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="65d17-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65d17-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printershare-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="65d17-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65d17-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printershare-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="65d17-147">Java</span><span class="sxs-lookup"><span data-stu-id="65d17-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printershare-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="65d17-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="65d17-148">Response</span></span>
<span data-ttu-id="65d17-149">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="65d17-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerShare"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/shares/$entity",
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
```

### <a name="example-2-get-a-printershare-and-its-capabilities"></a><span data-ttu-id="65d17-150">Exemplo 2: Obter um printerShare e seus recursos</span><span class="sxs-lookup"><span data-stu-id="65d17-150">Example 2: Get a printerShare and its capabilities</span></span>

#### <a name="request"></a><span data-ttu-id="65d17-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="65d17-151">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="65d17-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="65d17-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printershare_capabilities"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/shares/{printerShareId}?$select=id,displayName,capabilities
```
# <a name="c"></a>[<span data-ttu-id="65d17-153">C#</span><span class="sxs-lookup"><span data-stu-id="65d17-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printershare-capabilities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="65d17-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65d17-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printershare-capabilities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="65d17-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65d17-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printershare-capabilities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="65d17-156">Java</span><span class="sxs-lookup"><span data-stu-id="65d17-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printershare-capabilities-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="65d17-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="65d17-157">Response</span></span>

<span data-ttu-id="65d17-158">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="65d17-158">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerShare"
}
--> 
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/shares/$entity",
  "id": "d837c17b-3296-4384-a053-828d56e10f50",
  "displayName": "PrinterShare Name",
  "capabilities": {
    "isColorPrintingSupported": true,
    "supportsFitPdfToPage": false,
    "contentTypes": [
      "application/pdf",
      "image/pwg-raster",
      "application/PCLm"
    ],
    "isPageRangeSupported": false,
    "qualities": [
      "medium"
    ],
    "dpis": [
      600
    ],
    "duplexModes": [
      "oneSided",
      "flipOnLongEdge",
      "flipOnShortEdge"
    ],
    "finishings": [
      "none"
    ],
    "mediaTypes": [
      "stationery"
    ],
    "mediaSizes": [
      "North America Letter"
    ],
    "outputBins": [
      "tray-1"
    ],
    "colorModes": [
      "grayscale",
      "color"
    ],
    "inputBins": [
      "tray-1"
    ],
    "collation": true,
    "scalings": [
      "fill"
    ],
    "copiesPerJob": {
      "start": 1,
      "end": 38
    }
  }
}
```
