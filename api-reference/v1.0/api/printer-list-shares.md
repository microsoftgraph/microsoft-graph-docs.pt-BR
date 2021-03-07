---
title: Listar printerShares para uma impressora
description: Recupere uma lista de printerShares associada à impressora.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 7e03ae03b239bc7a538f8d488b8b244952b40bf3
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516925"
---
# <a name="list-printershares-for-a-printer"></a><span data-ttu-id="5f4c4-103">Listar printerShares para uma impressora</span><span class="sxs-lookup"><span data-stu-id="5f4c4-103">List printerShares for a printer</span></span>
<span data-ttu-id="5f4c4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f4c4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="5f4c4-105">Recupere uma lista de compartilhamentos de impressora associados à [impressora](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="5f4c4-105">Retrieve a list of printer shares associated with the [printer](../resources/printer.md).</span></span>
><span data-ttu-id="5f4c4-106">**Observação:** Atualmente, há suporte **para apenas um compartilhamento** de impressora por impressora.</span><span class="sxs-lookup"><span data-stu-id="5f4c4-106">**Note:** Currently, only **one** printer share per printer is supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f4c4-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="5f4c4-107">Permissions</span></span>
<span data-ttu-id="5f4c4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f4c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="5f4c4-110">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve [](printer-get.md) ter uma assinatura de Impressão Universal ativa, uma permissão que concede acesso a Obter impressora e uma das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="5f4c4-110">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, a permission that grants [Get printer](printer-get.md) access, and one of the permissions listed in the following table.</span></span>

|<span data-ttu-id="5f4c4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5f4c4-111">Permission type</span></span> | <span data-ttu-id="5f4c4-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5f4c4-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="5f4c4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5f4c4-113">Delegated (work or school account)</span></span>| <span data-ttu-id="5f4c4-114">PrinterShare.ReadBasic.All, PrinterShare.Read.All, PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f4c4-114">PrinterShare.ReadBasic.All, PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="5f4c4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5f4c4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f4c4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f4c4-116">Not Supported.</span></span>|
|<span data-ttu-id="5f4c4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5f4c4-117">Application</span></span>| <span data-ttu-id="5f4c4-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5f4c4-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f4c4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5f4c4-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/printers/{printerId}/shares
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5f4c4-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5f4c4-120">Optional query parameters</span></span>
<span data-ttu-id="5f4c4-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5f4c4-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="5f4c4-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5f4c4-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5f4c4-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5f4c4-123">Request headers</span></span>
|<span data-ttu-id="5f4c4-124">Nome</span><span class="sxs-lookup"><span data-stu-id="5f4c4-124">Name</span></span>|<span data-ttu-id="5f4c4-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f4c4-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5f4c4-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="5f4c4-126">Authorization</span></span>|<span data-ttu-id="5f4c4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5f4c4-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f4c4-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5f4c4-129">Request body</span></span>
<span data-ttu-id="5f4c4-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5f4c4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f4c4-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f4c4-131">Response</span></span>

<span data-ttu-id="5f4c4-132">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos printerShare](../resources/printershare.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5f4c4-132">If successful, this method returns a `200 OK` response code and a collection of [printerShare](../resources/printershare.md) objects in the response body.</span></span>

><span data-ttu-id="5f4c4-133">**Observação**: a resposta não conterá as **propriedades padrão** **e de** recursos.</span><span class="sxs-lookup"><span data-stu-id="5f4c4-133">**Note**: The response will not contain the **defaults** and **capabilities** properties.</span></span> <span data-ttu-id="5f4c4-134">Essas propriedades podem ser consultadas usando uma [solicitação Get printerShare.](printerShare-get.md)</span><span class="sxs-lookup"><span data-stu-id="5f4c4-134">These properties can be queried using a [Get printerShare](printerShare-get.md) request.</span></span>

## <a name="examples"></a><span data-ttu-id="5f4c4-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5f4c4-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5f4c4-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5f4c4-136">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_printershare"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/printers/{printerId}/shares
```


### <a name="response"></a><span data-ttu-id="5f4c4-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="5f4c4-137">Response</span></span>
<span data-ttu-id="5f4c4-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5f4c4-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.printerShare)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers('2f3453b7-4686-4b5b-9575-4f1e5b909ba7')/shares",
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
  ]
}
```

