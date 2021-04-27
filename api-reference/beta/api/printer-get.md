---
title: Obter impressora
description: Recupere as propriedades e as relações de um objeto printer.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 00cdebef99cc27de862b88768c725dd5e0a92372
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049132"
---
# <a name="get-printer"></a><span data-ttu-id="37e26-103">Obter impressora</span><span class="sxs-lookup"><span data-stu-id="37e26-103">Get printer</span></span>

<span data-ttu-id="37e26-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37e26-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37e26-105">Recupere as propriedades e as relações de um [objeto printer.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="37e26-105">Retrieve the properties and relationships of a [printer](../resources/printer.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="37e26-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="37e26-106">Permissions</span></span>
<span data-ttu-id="37e26-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37e26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="37e26-109">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="37e26-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="37e26-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="37e26-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="37e26-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37e26-111">Permission type</span></span> | <span data-ttu-id="37e26-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="37e26-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="37e26-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37e26-113">Delegated (work or school account)</span></span>| <span data-ttu-id="37e26-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="37e26-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="37e26-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37e26-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37e26-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="37e26-116">Not Supported.</span></span>|
|<span data-ttu-id="37e26-117">Application</span><span class="sxs-lookup"><span data-stu-id="37e26-117">Application</span></span>| <span data-ttu-id="37e26-118">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37e26-118">Printer.Read.All, Printer.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="37e26-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37e26-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}
GET /print/shares/{id}/printer
```

## <a name="optional-query-parameters"></a><span data-ttu-id="37e26-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="37e26-120">Optional query parameters</span></span>
<span data-ttu-id="37e26-121">Este método dá suporte a alguns dos parâmetros de consulta OData, incluindo $select, $expand ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="37e26-121">This method supports some of the OData query parameters including $select, $expand to help customize the response.</span></span> <span data-ttu-id="37e26-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="37e26-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="37e26-123">por exemplo,</span><span class="sxs-lookup"><span data-stu-id="37e26-123">e.g.</span></span> 
```http
GET /print/printers/{id}?$select=id,displayName,capabilities
```
## <a name="request-headers"></a><span data-ttu-id="37e26-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37e26-124">Request headers</span></span>
| <span data-ttu-id="37e26-125">Nome</span><span class="sxs-lookup"><span data-stu-id="37e26-125">Name</span></span>      |<span data-ttu-id="37e26-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="37e26-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="37e26-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="37e26-127">Authorization</span></span> | <span data-ttu-id="37e26-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37e26-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="37e26-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37e26-130">Request body</span></span>
<span data-ttu-id="37e26-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="37e26-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="37e26-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="37e26-132">Response</span></span>
<span data-ttu-id="37e26-133">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [printer](../resources/printer.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37e26-133">If successful, this method returns a `200 OK` response code and a [printer](../resources/printer.md) object in the response body.</span></span>
<span data-ttu-id="37e26-134">Por padrão, a resposta não conterá [printerCapabilities](../resources/printerCapabilities.md).</span><span class="sxs-lookup"><span data-stu-id="37e26-134">By default, the response will not contain [printerCapabilities](../resources/printerCapabilities.md).</span></span> <span data-ttu-id="37e26-135">Para obter **printerCapabilities**, use `$select` o parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="37e26-135">To get **printerCapabilities**, use the `$select` query parameter.</span></span> 

## <a name="example"></a><span data-ttu-id="37e26-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="37e26-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="37e26-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37e26-137">Request</span></span>
<span data-ttu-id="37e26-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="37e26-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="37e26-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="37e26-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printer"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}
```
# <a name="c"></a>[<span data-ttu-id="37e26-140">C#</span><span class="sxs-lookup"><span data-stu-id="37e26-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37e26-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37e26-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37e26-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37e26-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="37e26-143">Java</span><span class="sxs-lookup"><span data-stu-id="37e26-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="37e26-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="37e26-144">Response</span></span>
<span data-ttu-id="37e26-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="37e26-145">The following is an example of the response.</span></span>
><span data-ttu-id="37e26-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="37e26-146">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printer"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1313

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers/$entity",
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

<span data-ttu-id="37e26-147">A seguir, um exemplo da resposta, ao usar $select=id,displayName,capabilities</span><span class="sxs-lookup"><span data-stu-id="37e26-147">The following is an example of the response, when using $select=id,displayName,capabilities</span></span>
><span data-ttu-id="37e26-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="37e26-148">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printer"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1313

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers/$entity",
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
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
