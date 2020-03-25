---
title: Obter impressoras
description: Recupere a lista de impressoras registradas no locatário.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 1e0c9e97904df35c5d8383d77a1b37441a96abb5
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2020
ms.locfileid: "42948309"
---
# <a name="list-printers"></a><span data-ttu-id="b5563-103">Listar impressoras</span><span class="sxs-lookup"><span data-stu-id="b5563-103">List printers</span></span>

<span data-ttu-id="b5563-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5563-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5563-105">Recupere a lista de **impressoras** registradas no locatário.</span><span class="sxs-lookup"><span data-stu-id="b5563-105">Retrieve the list of **printers** that are registered in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5563-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b5563-106">Permissions</span></span>
<span data-ttu-id="b5563-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5563-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5563-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b5563-109">Permission type</span></span> | <span data-ttu-id="b5563-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b5563-110">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="b5563-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b5563-111">Delegated (work or school account)</span></span>| <span data-ttu-id="b5563-112">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="b5563-112">Users.Read.All</span></span> |
|<span data-ttu-id="b5563-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b5563-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5563-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5563-114">Not Supported.</span></span>|
|<span data-ttu-id="b5563-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b5563-115">Application</span></span>|<span data-ttu-id="b5563-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5563-116">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5563-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5563-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b5563-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b5563-118">Optional query parameters</span></span>
<span data-ttu-id="b5563-119">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b5563-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b5563-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b5563-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="b5563-121">Exceções</span><span class="sxs-lookup"><span data-stu-id="b5563-121">Exceptions</span></span>
* <span data-ttu-id="b5563-122">Os `$expand` operadores `select` e têm suporte para a `share` propriedade de navegação, mas não `jobs`para.</span><span class="sxs-lookup"><span data-stu-id="b5563-122">The `$expand` and `select` operators are supported for the `share` navigation property, but not for `jobs`.</span></span>
* <span data-ttu-id="b5563-123">Não `$count` há suporte para o operador.</span><span class="sxs-lookup"><span data-stu-id="b5563-123">The `$count` operator is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b5563-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b5563-124">Request headers</span></span>
| <span data-ttu-id="b5563-125">Nome</span><span class="sxs-lookup"><span data-stu-id="b5563-125">Name</span></span>      |<span data-ttu-id="b5563-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5563-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b5563-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="b5563-127">Authorization</span></span> | <span data-ttu-id="b5563-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5563-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5563-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b5563-130">Request body</span></span>
<span data-ttu-id="b5563-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b5563-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="b5563-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5563-132">Response</span></span>
<span data-ttu-id="b5563-133">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [Printer](../resources/printer.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b5563-133">If successful, this method returns a `200 OK` response code and a collection of [printer](../resources/printer.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b5563-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b5563-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b5563-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5563-135">Request</span></span>
<span data-ttu-id="b5563-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5563-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b5563-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5563-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers
```
# <a name="c"></a>[<span data-ttu-id="b5563-138">C#</span><span class="sxs-lookup"><span data-stu-id="b5563-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b5563-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5563-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b5563-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5563-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b5563-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5563-141">Response</span></span>
<span data-ttu-id="b5563-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b5563-142">The following is an example of the response.</span></span>
><span data-ttu-id="b5563-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b5563-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printer",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1526

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers",
  "value": [
    {
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List printers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
