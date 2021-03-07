---
title: Lista de impressoras
description: Recupere a lista de impressoras registradas no locatário.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: ff93eb5c598458c57126f0e8edda2a4f440dfc65
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516885"
---
# <a name="list-printers"></a><span data-ttu-id="606d9-103">Lista de impressoras</span><span class="sxs-lookup"><span data-stu-id="606d9-103">List printers</span></span>
<span data-ttu-id="606d9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="606d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="606d9-105">Recupere a lista de **impressoras registradas** no locatário.</span><span class="sxs-lookup"><span data-stu-id="606d9-105">Retrieve the list of **printers** that are registered in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="606d9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="606d9-106">Permissions</span></span>
<span data-ttu-id="606d9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="606d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="606d9-109">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="606d9-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="606d9-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="606d9-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="606d9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="606d9-111">Permission type</span></span> | <span data-ttu-id="606d9-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="606d9-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="606d9-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="606d9-113">Delegated (work or school account)</span></span>| <span data-ttu-id="606d9-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="606d9-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="606d9-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="606d9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="606d9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="606d9-116">Not Supported.</span></span>|
|<span data-ttu-id="606d9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="606d9-117">Application</span></span>| <span data-ttu-id="606d9-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="606d9-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="606d9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="606d9-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/printers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="606d9-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="606d9-120">Optional query parameters</span></span>
<span data-ttu-id="606d9-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="606d9-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="606d9-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="606d9-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

### <a name="exceptions"></a><span data-ttu-id="606d9-123">Exceptions</span><span class="sxs-lookup"><span data-stu-id="606d9-123">Exceptions</span></span>
* <span data-ttu-id="606d9-124">Os `$expand` `select` operadores e são suportados para a `share` propriedade de navegação, mas não para `jobs` .</span><span class="sxs-lookup"><span data-stu-id="606d9-124">The `$expand` and `select` operators are supported for the `share` navigation property, but not for `jobs`.</span></span>
* <span data-ttu-id="606d9-125">Alguns operadores não têm suporte: `$count` , `$search` .</span><span class="sxs-lookup"><span data-stu-id="606d9-125">Some operators are not supported: `$count`, `$search`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="606d9-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="606d9-126">Request headers</span></span>
|<span data-ttu-id="606d9-127">Nome</span><span class="sxs-lookup"><span data-stu-id="606d9-127">Name</span></span>|<span data-ttu-id="606d9-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="606d9-128">Description</span></span>|
|:---|:---|
|<span data-ttu-id="606d9-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="606d9-129">Authorization</span></span>|<span data-ttu-id="606d9-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="606d9-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="606d9-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="606d9-132">Request body</span></span>
<span data-ttu-id="606d9-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="606d9-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="606d9-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="606d9-134">Response</span></span>

<span data-ttu-id="606d9-135">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [de](../resources/printer.md) impressora no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="606d9-135">If successful, this method returns a `200 OK` response code and a collection of [printer](../resources/printer.md) objects in the response body.</span></span>

><span data-ttu-id="606d9-136">**Observação**: a resposta não conterá propriedades 'padrão' e 'capabilities'.</span><span class="sxs-lookup"><span data-stu-id="606d9-136">**Note**: The response will not contain 'defaults' and 'capabilities' properties.</span></span> <span data-ttu-id="606d9-137">Essas propriedades podem ser consultadas usando a [solicitação Obter Impressora.](printer-get.md)</span><span class="sxs-lookup"><span data-stu-id="606d9-137">These properties can be queried using [Get Printer](printer-get.md) request.</span></span>

## <a name="examples"></a><span data-ttu-id="606d9-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="606d9-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="606d9-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="606d9-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_printer"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/printers
```


### <a name="response"></a><span data-ttu-id="606d9-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="606d9-140">Response</span></span>
<span data-ttu-id="606d9-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="606d9-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.printer)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers",
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

