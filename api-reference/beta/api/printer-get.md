---
title: Obter impressora
description: Recupere as propriedades e os relacionamentos de um objeto printer.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: bfd3f6e71e8fd56c630cfcaa5b56cc32eff4e148
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034048"
---
# <a name="get-printer"></a><span data-ttu-id="dae9f-103">Obter impressora</span><span class="sxs-lookup"><span data-stu-id="dae9f-103">Get printer</span></span>

<span data-ttu-id="dae9f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dae9f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dae9f-105">Recupere as propriedades e os relacionamentos de um [objeto printer.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="dae9f-105">Retrieve the properties and relationships of a [printer](../resources/printer.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dae9f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dae9f-106">Permissions</span></span>
<span data-ttu-id="dae9f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dae9f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="dae9f-109">Para usar o serviço de Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="dae9f-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="dae9f-110">O usuário assinado deve ser um Administrador [de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="dae9f-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="dae9f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dae9f-111">Permission type</span></span> | <span data-ttu-id="dae9f-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dae9f-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="dae9f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dae9f-113">Delegated (work or school account)</span></span>| <span data-ttu-id="dae9f-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="dae9f-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="dae9f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dae9f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dae9f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dae9f-116">Not Supported.</span></span>|
|<span data-ttu-id="dae9f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dae9f-117">Application</span></span>| <span data-ttu-id="dae9f-118">Printer.Read.All, Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dae9f-118">Printer.Read.All, Printer.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dae9f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dae9f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}
GET /print/shares/{id}/printer
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dae9f-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dae9f-120">Optional query parameters</span></span>
<span data-ttu-id="dae9f-121">Esse método dá suporte a alguns dos parâmetros de consulta OData, incluindo $select, $expand para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dae9f-121">This method supports some of the OData query parameters including $select, $expand to help customize the response.</span></span> <span data-ttu-id="dae9f-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="dae9f-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="dae9f-123">por exemplo,</span><span class="sxs-lookup"><span data-stu-id="dae9f-123">e.g.</span></span> 
```http
GET /print/printers/{id}?$select=id,displayName,capabilities
```
## <a name="request-headers"></a><span data-ttu-id="dae9f-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dae9f-124">Request headers</span></span>
| <span data-ttu-id="dae9f-125">Nome</span><span class="sxs-lookup"><span data-stu-id="dae9f-125">Name</span></span>      |<span data-ttu-id="dae9f-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="dae9f-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dae9f-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="dae9f-127">Authorization</span></span> | <span data-ttu-id="dae9f-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dae9f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dae9f-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dae9f-130">Request body</span></span>
<span data-ttu-id="dae9f-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dae9f-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="dae9f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="dae9f-132">Response</span></span>
<span data-ttu-id="dae9f-133">Se bem-sucedido, este método retorna `200 OK` um código de resposta e um objeto [printer](../resources/printer.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dae9f-133">If successful, this method returns a `200 OK` response code and a [printer](../resources/printer.md) object in the response body.</span></span>
<span data-ttu-id="dae9f-134">Por padrão, a resposta não conterá [printerCapabilities](../resources/printerCapabilities.md).</span><span class="sxs-lookup"><span data-stu-id="dae9f-134">By default, the response will not contain [printerCapabilities](../resources/printerCapabilities.md).</span></span> <span data-ttu-id="dae9f-135">Para obter **printerCapabilities**, use `$select` o parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="dae9f-135">To get **printerCapabilities**, use the `$select` query parameter.</span></span> 

## <a name="example"></a><span data-ttu-id="dae9f-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dae9f-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="dae9f-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dae9f-137">Request</span></span>
<span data-ttu-id="dae9f-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dae9f-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dae9f-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="dae9f-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printer"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}
```
# <a name="c"></a>[<span data-ttu-id="dae9f-140">C#</span><span class="sxs-lookup"><span data-stu-id="dae9f-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dae9f-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dae9f-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dae9f-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dae9f-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dae9f-143">Java</span><span class="sxs-lookup"><span data-stu-id="dae9f-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="dae9f-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="dae9f-144">Response</span></span>
<span data-ttu-id="dae9f-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dae9f-145">The following is an example of the response.</span></span>
><span data-ttu-id="dae9f-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dae9f-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "name": "PrinterName",
  "manufacturer": "PrinterManufacturer",
  "model": "PrinterModel",
  "isShared": true,
  "registeredDateTime": "2020-02-04T00:00:00.0000000Z",
  "acceptingJobs": true,
  "status": {
    "processingState": "stopped",
    "processingStateReasons": ["disconnected"],
    "processingStateDescription": ""
  },
  "defaults": {
    "copiesPerJob":1,
    "documentMimeType": "application/oxps",
    "finishings": ["none"],
    "mediaType": "stationery"
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
    "floorNumber": 1,
    "floorDescription": "First Floor",
    "roomNumber": 1234,
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

<span data-ttu-id="dae9f-148">A seguir está um exemplo da resposta, ao usar $select=id,displayName,capabilities</span><span class="sxs-lookup"><span data-stu-id="dae9f-148">The following is an example of the response, when using $select=id,displayName,capabilities</span></span>
><span data-ttu-id="dae9f-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dae9f-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
