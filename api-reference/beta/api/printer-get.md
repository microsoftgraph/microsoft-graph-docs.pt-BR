---
title: Obter impressora
description: Recupere as propriedades e os relacionamentos de um objeto Printer.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: c98ecee9c0dfa075831c0df5cee9142540b58e1a
ms.sourcegitcommit: 5c3f4a3e2620d1d9e635e09231bbaa73cb0c3cdd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/14/2020
ms.locfileid: "46674439"
---
# <a name="get-printer"></a><span data-ttu-id="87732-103">Obter impressora</span><span class="sxs-lookup"><span data-stu-id="87732-103">Get printer</span></span>

<span data-ttu-id="87732-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87732-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87732-105">Recupere as propriedades e os relacionamentos de um objeto [Printer](../resources/printer.md) .</span><span class="sxs-lookup"><span data-stu-id="87732-105">Retrieve the properties and relationships of a [printer](../resources/printer.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="87732-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="87732-106">Permissions</span></span>
<span data-ttu-id="87732-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87732-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="87732-109">Para usar o serviço de impressão universal, o usuário ou o locatário do aplicativo deve ter uma assinatura de impressão universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="87732-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="87732-110">O usuário conectado deve ser um [administrador da impressora](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="87732-110">The signed in user must be a [Printer Administrator](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="87732-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87732-111">Permission type</span></span> | <span data-ttu-id="87732-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="87732-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="87732-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87732-113">Delegated (work or school account)</span></span>| <span data-ttu-id="87732-114">Printer. Read. All, Printer. ReadWrite. All, Printer. FullControl. All</span><span class="sxs-lookup"><span data-stu-id="87732-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="87732-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87732-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87732-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87732-116">Not Supported.</span></span>|
|<span data-ttu-id="87732-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87732-117">Application</span></span>| <span data-ttu-id="87732-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87732-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="87732-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87732-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}
GET /print/shares/{id}/printer
```

## <a name="optional-query-parameters"></a><span data-ttu-id="87732-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="87732-120">Optional query parameters</span></span>
<span data-ttu-id="87732-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="87732-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="87732-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="87732-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="87732-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87732-123">Request headers</span></span>
| <span data-ttu-id="87732-124">Nome</span><span class="sxs-lookup"><span data-stu-id="87732-124">Name</span></span>      |<span data-ttu-id="87732-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="87732-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="87732-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="87732-126">Authorization</span></span> | <span data-ttu-id="87732-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87732-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="87732-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87732-129">Request body</span></span>
<span data-ttu-id="87732-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="87732-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="87732-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="87732-131">Response</span></span>
<span data-ttu-id="87732-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [Printer](../resources/printer.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87732-132">If successful, this method returns a `200 OK` response code and [printer](../resources/printer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="87732-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87732-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="87732-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87732-134">Request</span></span>
<span data-ttu-id="87732-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="87732-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="87732-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="87732-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printer"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}
```
# <a name="c"></a>[<span data-ttu-id="87732-137">C#</span><span class="sxs-lookup"><span data-stu-id="87732-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="87732-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="87732-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="87732-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="87732-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="87732-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="87732-140">Response</span></span>
<span data-ttu-id="87732-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="87732-141">The following is an example of the response.</span></span>
><span data-ttu-id="87732-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="87732-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get printer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
