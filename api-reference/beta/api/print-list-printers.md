---
title: Obter impressoras
description: Recupere a lista de impressoras registradas no locatário.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 38f742b4013f01b150ee5b653d341dd2e8ca5991
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766508"
---
# <a name="list-printers"></a><span data-ttu-id="00e93-103">Lista de impressoras</span><span class="sxs-lookup"><span data-stu-id="00e93-103">List printers</span></span>

<span data-ttu-id="00e93-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00e93-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00e93-105">Recupere a lista de **impressoras registradas** no locatário.</span><span class="sxs-lookup"><span data-stu-id="00e93-105">Retrieve the list of **printers** that are registered in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="00e93-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="00e93-106">Permissions</span></span>
<span data-ttu-id="00e93-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00e93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="00e93-109">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="00e93-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="00e93-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="00e93-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="00e93-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="00e93-111">Permission type</span></span> | <span data-ttu-id="00e93-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="00e93-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="00e93-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="00e93-113">Delegated (work or school account)</span></span>| <span data-ttu-id="00e93-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="00e93-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="00e93-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="00e93-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00e93-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="00e93-116">Not Supported.</span></span>|
|<span data-ttu-id="00e93-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="00e93-117">Application</span></span>| <span data-ttu-id="00e93-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="00e93-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="00e93-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="00e93-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="00e93-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="00e93-120">Optional query parameters</span></span>
<span data-ttu-id="00e93-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="00e93-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="00e93-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="00e93-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="00e93-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="00e93-123">Exceptions</span></span>
* <span data-ttu-id="00e93-124">Os `$expand` `select` operadores e são suportados para a `share` propriedade de navegação, mas não para `jobs` .</span><span class="sxs-lookup"><span data-stu-id="00e93-124">The `$expand` and `select` operators are supported for the `share` navigation property, but not for `jobs`.</span></span>
* <span data-ttu-id="00e93-125">Alguns operadores não têm suporte: `$count` , `$search` .</span><span class="sxs-lookup"><span data-stu-id="00e93-125">Some operators are not supported: `$count`, `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="00e93-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="00e93-126">Request headers</span></span>
| <span data-ttu-id="00e93-127">Nome</span><span class="sxs-lookup"><span data-stu-id="00e93-127">Name</span></span>      |<span data-ttu-id="00e93-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="00e93-128">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="00e93-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="00e93-129">Authorization</span></span> | <span data-ttu-id="00e93-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="00e93-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="00e93-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="00e93-132">Request body</span></span>
<span data-ttu-id="00e93-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="00e93-133">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="00e93-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="00e93-134">Response</span></span>
<span data-ttu-id="00e93-135">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [de](../resources/printer.md) impressora no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="00e93-135">If successful, this method returns a `200 OK` response code and a collection of [printer](../resources/printer.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="00e93-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="00e93-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="00e93-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="00e93-137">Request</span></span>
<span data-ttu-id="00e93-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="00e93-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="00e93-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="00e93-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers
```
# <a name="c"></a>[<span data-ttu-id="00e93-140">C#</span><span class="sxs-lookup"><span data-stu-id="00e93-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="00e93-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="00e93-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="00e93-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="00e93-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="00e93-143">Java</span><span class="sxs-lookup"><span data-stu-id="00e93-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="00e93-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="00e93-144">Response</span></span>
<span data-ttu-id="00e93-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="00e93-145">The following is an example of the response.</span></span>
><span data-ttu-id="00e93-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="00e93-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
