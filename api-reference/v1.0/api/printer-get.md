---
title: Obter impressora
description: Recupere as propriedades e as relações de um objeto printer.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 547cde8d31870fcc2b0d73c1021f5628ce74c19b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776918"
---
# <a name="get-printer"></a><span data-ttu-id="17b14-103">Obter impressora</span><span class="sxs-lookup"><span data-stu-id="17b14-103">Get printer</span></span>
<span data-ttu-id="17b14-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17b14-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="17b14-105">Recupere as propriedades e as relações de um [objeto printer.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="17b14-105">Retrieve the properties and relationships of a [printer](../resources/printer.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="17b14-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="17b14-106">Permissions</span></span>
<span data-ttu-id="17b14-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="17b14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="17b14-109">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="17b14-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="17b14-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="17b14-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="17b14-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="17b14-111">Permission type</span></span> | <span data-ttu-id="17b14-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="17b14-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="17b14-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="17b14-113">Delegated (work or school account)</span></span>| <span data-ttu-id="17b14-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="17b14-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="17b14-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="17b14-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17b14-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="17b14-116">Not Supported.</span></span>|
|<span data-ttu-id="17b14-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="17b14-117">Application</span></span>| <span data-ttu-id="17b14-118">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17b14-118">Printer.Read.All, Printer.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="17b14-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="17b14-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/printers/{id}
GET /print/shares/{id}/printer
```

## <a name="optional-query-parameters"></a><span data-ttu-id="17b14-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="17b14-120">Optional query parameters</span></span>
<span data-ttu-id="17b14-121">Este método dá suporte a alguns dos parâmetros de consulta OData, incluindo `$select` e , para ajudar a personalizar a `$expand` resposta.</span><span class="sxs-lookup"><span data-stu-id="17b14-121">This method supports some of the OData query parameters, including `$select` and `$expand`, to help customize the response.</span></span> <span data-ttu-id="17b14-122">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="17b14-122">For example:</span></span>

```http
GET /print/printers/{id}?$select=id,displayName,capabilities
```
<span data-ttu-id="17b14-123">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="17b14-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="17b14-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="17b14-124">Request headers</span></span>
|<span data-ttu-id="17b14-125">Nome</span><span class="sxs-lookup"><span data-stu-id="17b14-125">Name</span></span>|<span data-ttu-id="17b14-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="17b14-126">Description</span></span>|
|:---|:---|
|<span data-ttu-id="17b14-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="17b14-127">Authorization</span></span>|<span data-ttu-id="17b14-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17b14-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="17b14-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="17b14-130">Request body</span></span>
<span data-ttu-id="17b14-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="17b14-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17b14-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="17b14-132">Response</span></span>
<span data-ttu-id="17b14-133">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [printer](../resources/printer.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="17b14-133">If successful, this method returns a `200 OK` response code and a [printer](../resources/printer.md) object in the response body.</span></span>
<span data-ttu-id="17b14-134">Por padrão, a resposta não conterá [printerCapabilities](../resources/printerCapabilities.md).</span><span class="sxs-lookup"><span data-stu-id="17b14-134">By default, the response will not contain [printerCapabilities](../resources/printerCapabilities.md).</span></span> <span data-ttu-id="17b14-135">Para obter **printerCapabilities**, use `$select` o parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="17b14-135">To get **printerCapabilities**, use the `$select` query parameter.</span></span> 

## <a name="examples"></a><span data-ttu-id="17b14-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="17b14-136">Examples</span></span>

### <a name="example-1-get-a-printer"></a><span data-ttu-id="17b14-137">Exemplo 1: Obter uma impressora</span><span class="sxs-lookup"><span data-stu-id="17b14-137">Example 1: Get a printer</span></span>

#### <a name="request"></a><span data-ttu-id="17b14-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17b14-138">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="17b14-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="17b14-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printer"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}
```
# <a name="c"></a>[<span data-ttu-id="17b14-140">C#</span><span class="sxs-lookup"><span data-stu-id="17b14-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="17b14-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="17b14-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="17b14-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="17b14-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="17b14-143">Java</span><span class="sxs-lookup"><span data-stu-id="17b14-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="17b14-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="17b14-144">Response</span></span>
<span data-ttu-id="17b14-145">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="17b14-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printer"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers/$entity",
  "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
  "displayName": "PrinterName",
  "manufacturer": "PrinterManufacturer",
  "model": "PrinterModel",
  "isShared": true,
  "registeredDateTime": "2020-02-04T00:00:00.0000000Z",
  "isAcceptingJobs": true,
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
    "latitude": 1.1,
    "longitude": 2.2,
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

### <a name="example-2-get-a-printer-and-its-capabilities"></a><span data-ttu-id="17b14-146">Exemplo 2: obter uma impressora e seus recursos</span><span class="sxs-lookup"><span data-stu-id="17b14-146">Example 2: Get a printer and its capabilities</span></span>

#### <a name="request"></a><span data-ttu-id="17b14-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="17b14-147">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="17b14-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="17b14-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printer_capabilities"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}?$select=id,displayName,capabilities
```
# <a name="c"></a>[<span data-ttu-id="17b14-149">C#</span><span class="sxs-lookup"><span data-stu-id="17b14-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printer-capabilities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="17b14-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="17b14-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printer-capabilities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="17b14-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="17b14-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printer-capabilities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="17b14-152">Java</span><span class="sxs-lookup"><span data-stu-id="17b14-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printer-capabilities-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="17b14-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="17b14-153">Response</span></span>

<span data-ttu-id="17b14-154">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="17b14-154">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printer"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers/$entity",
  "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
  "displayName": "PrinterName",
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

