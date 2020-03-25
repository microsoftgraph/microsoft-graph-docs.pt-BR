---
title: Obter impressora
description: Recupere as propriedades e os relacionamentos de um objeto Printer.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: faa68c631ff498892934b35dec24f5940736d025
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947999"
---
# <a name="get-printer"></a><span data-ttu-id="8ace6-103">Obter impressora</span><span class="sxs-lookup"><span data-stu-id="8ace6-103">Get printer</span></span>

<span data-ttu-id="8ace6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ace6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ace6-105">Recupere as propriedades e os relacionamentos de um objeto [Printer](../resources/printer.md) .</span><span class="sxs-lookup"><span data-stu-id="8ace6-105">Retrieve the properties and relationships of a [printer](../resources/printer.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ace6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8ace6-106">Permissions</span></span>
<span data-ttu-id="8ace6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ace6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="8ace6-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="8ace6-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="8ace6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ace6-110">Permission type</span></span> | <span data-ttu-id="8ace6-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8ace6-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="8ace6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ace6-112">Delegated (work or school account)</span></span>| <span data-ttu-id="8ace6-113">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="8ace6-113">Users.Read.All</span></span> |
|<span data-ttu-id="8ace6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ace6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ace6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ace6-115">Not Supported.</span></span>|
|<span data-ttu-id="8ace6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ace6-116">Application</span></span>|<span data-ttu-id="8ace6-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ace6-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ace6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ace6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}
GET /print/printerShares/{id}/printer
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8ace6-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8ace6-119">Optional query parameters</span></span>
<span data-ttu-id="8ace6-120">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8ace6-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="8ace6-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8ace6-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8ace6-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ace6-122">Request headers</span></span>
| <span data-ttu-id="8ace6-123">Nome</span><span class="sxs-lookup"><span data-stu-id="8ace6-123">Name</span></span>      |<span data-ttu-id="8ace6-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ace6-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8ace6-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ace6-125">Authorization</span></span> | <span data-ttu-id="8ace6-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ace6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ace6-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ace6-128">Request body</span></span>
<span data-ttu-id="8ace6-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8ace6-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8ace6-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ace6-130">Response</span></span>
<span data-ttu-id="8ace6-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [Printer](../resources/printer.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ace6-131">If successful, this method returns a `200 OK` response code and [printer](../resources/printer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8ace6-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8ace6-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8ace6-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ace6-133">Request</span></span>
<span data-ttu-id="8ace6-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ace6-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8ace6-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="8ace6-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printer"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}
```
# <a name="c"></a>[<span data-ttu-id="8ace6-136">C#</span><span class="sxs-lookup"><span data-stu-id="8ace6-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8ace6-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8ace6-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8ace6-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8ace6-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8ace6-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ace6-139">Response</span></span>
<span data-ttu-id="8ace6-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8ace6-140">The following is an example of the response.</span></span>
><span data-ttu-id="8ace6-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8ace6-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "registeredBy": {},
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
