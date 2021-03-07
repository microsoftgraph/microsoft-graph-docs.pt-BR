---
title: Get printerShare
description: Recupere as propriedades e as relações de um compartilhamento de impressora.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 3e5bc385fb6e928ba82bb36660bb8af7bf794034
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517032"
---
# <a name="get-printershare"></a><span data-ttu-id="035da-103">Get printerShare</span><span class="sxs-lookup"><span data-stu-id="035da-103">Get printerShare</span></span>
<span data-ttu-id="035da-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="035da-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="035da-105">Recupere as propriedades e as relações de um compartilhamento de impressora.</span><span class="sxs-lookup"><span data-stu-id="035da-105">Retrieve the properties and relationships of a printer share.</span></span>

## <a name="permissions"></a><span data-ttu-id="035da-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="035da-106">Permissions</span></span>
<span data-ttu-id="035da-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="035da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="035da-109">Além das permissões a seguir, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="035da-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="035da-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="035da-110">Permission type</span></span> | <span data-ttu-id="035da-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="035da-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="035da-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="035da-112">Delegated (work or school account)</span></span>| <span data-ttu-id="035da-113">PrinterShare.ReadBasic.All, PrinterShare.Read.All, PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="035da-113">PrinterShare.ReadBasic.All, PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="035da-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="035da-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="035da-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="035da-115">Not Supported.</span></span>|
|<span data-ttu-id="035da-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="035da-116">Application</span></span>|<span data-ttu-id="035da-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="035da-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="035da-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="035da-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/shares/{printerShareId}
GET /print/printers/{printerId}/shares/{printerShareId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="035da-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="035da-119">Optional query parameters</span></span>
<span data-ttu-id="035da-120">Este método dá suporte a alguns dos parâmetros de consulta OData, incluindo `$select` e , para ajudar a personalizar a `$expand` resposta.</span><span class="sxs-lookup"><span data-stu-id="035da-120">This method supports some of the OData query parameters, including `$select` and `$expand`, to help customize the response.</span></span> <span data-ttu-id="035da-121">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="035da-121">For example:</span></span> 

<span data-ttu-id="035da-122">por exemplo,</span><span class="sxs-lookup"><span data-stu-id="035da-122">e.g.</span></span> 
```http
GET /print/printers/{id}?$select=id,displayName,capabilities
```
<span data-ttu-id="035da-123">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="035da-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="035da-124">Exceptions</span><span class="sxs-lookup"><span data-stu-id="035da-124">Exceptions</span></span>
* <span data-ttu-id="035da-125">O `$count` operador não tem suporte.</span><span class="sxs-lookup"><span data-stu-id="035da-125">The `$count` operator is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="035da-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="035da-126">Request headers</span></span>
|<span data-ttu-id="035da-127">Nome</span><span class="sxs-lookup"><span data-stu-id="035da-127">Name</span></span>|<span data-ttu-id="035da-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="035da-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="035da-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="035da-129">Authorization</span></span>|<span data-ttu-id="035da-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="035da-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="035da-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="035da-132">Request body</span></span>
<span data-ttu-id="035da-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="035da-133">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="035da-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="035da-134">Response</span></span>
<span data-ttu-id="035da-135">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [printerShare](../resources/printershare.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="035da-135">If successful, this method returns a `200 OK` response code and a [printerShare](../resources/printershare.md) object in the response body.</span></span>
<span data-ttu-id="035da-136">Por padrão, a resposta não conterá [printerCapabilities](../resources/printerCapabilities.md).</span><span class="sxs-lookup"><span data-stu-id="035da-136">By default, the response will not contain [printerCapabilities](../resources/printerCapabilities.md).</span></span> <span data-ttu-id="035da-137">Para obter **printerCapabilities**, use `$select` o parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="035da-137">To get **printerCapabilities**, use the `$select` query parameter.</span></span> 

## <a name="response"></a><span data-ttu-id="035da-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="035da-138">Response</span></span>

<span data-ttu-id="035da-139">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [printerShare](../resources/printershare.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="035da-139">If successful, this method returns a `200 OK` response code and a [printerShare](../resources/printershare.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="035da-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="035da-140">Examples</span></span>

### <a name="example-1-get-a-printershare"></a><span data-ttu-id="035da-141">Exemplo 1: Obter uma printerShare</span><span class="sxs-lookup"><span data-stu-id="035da-141">Example 1: Get a printerShare</span></span>

#### <a name="request"></a><span data-ttu-id="035da-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="035da-142">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printershare"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/shares/{printerShareId}
```

#### <a name="response"></a><span data-ttu-id="035da-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="035da-143">Response</span></span>
<span data-ttu-id="035da-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="035da-144">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-get-a-printershare-and-its-capabilities"></a><span data-ttu-id="035da-145">Exemplo 2: Obter um printerShare e seus recursos</span><span class="sxs-lookup"><span data-stu-id="035da-145">Example 2: Get a printerShare and its capabilities</span></span>

#### <a name="request"></a><span data-ttu-id="035da-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="035da-146">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printershare_capabilities"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/shares/{printerShareId}?$select=id,displayName,capabilities
```

#### <a name="response"></a><span data-ttu-id="035da-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="035da-147">Response</span></span>

<span data-ttu-id="035da-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="035da-148">**Note:** The response object shown here might be shortened for readability.</span></span>
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
