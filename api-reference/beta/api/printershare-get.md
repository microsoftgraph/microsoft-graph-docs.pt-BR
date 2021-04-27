---
title: Get printerShare
description: Recupere as propriedades e as relações de um compartilhamento de impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 046d5a107ea2b92adf17bb24f585138764757b50
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52037484"
---
# <a name="get-printershare"></a><span data-ttu-id="52f52-103">Get printerShare</span><span class="sxs-lookup"><span data-stu-id="52f52-103">Get printerShare</span></span>

<span data-ttu-id="52f52-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52f52-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52f52-105">Recupere as propriedades e as relações de um compartilhamento de impressora.</span><span class="sxs-lookup"><span data-stu-id="52f52-105">Retrieve the properties and relationships of a printer share.</span></span>

## <a name="permissions"></a><span data-ttu-id="52f52-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="52f52-106">Permissions</span></span>
<span data-ttu-id="52f52-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52f52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="52f52-109">Além das permissões a seguir, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="52f52-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="52f52-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52f52-110">Permission type</span></span> | <span data-ttu-id="52f52-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="52f52-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="52f52-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52f52-112">Delegated (work or school account)</span></span>| <span data-ttu-id="52f52-113">PrinterShare.ReadBasic.All, PrinterShare.Read.All, PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52f52-113">PrinterShare.ReadBasic.All, PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="52f52-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52f52-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52f52-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52f52-115">Not Supported.</span></span>|
|<span data-ttu-id="52f52-116">Application</span><span class="sxs-lookup"><span data-stu-id="52f52-116">Application</span></span>|<span data-ttu-id="52f52-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52f52-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="52f52-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52f52-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/shares/{printerShareId}
GET /print/printers/{printerId}/shares/{printerShareId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="52f52-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="52f52-119">Optional query parameters</span></span>
<span data-ttu-id="52f52-120">Este método dá suporte a alguns dos parâmetros de consulta OData, incluindo $select, $expand ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="52f52-120">This method supports some of the OData query parameters including $select, $expand to help customize the response.</span></span> <span data-ttu-id="52f52-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="52f52-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="52f52-122">por exemplo,</span><span class="sxs-lookup"><span data-stu-id="52f52-122">e.g.</span></span> 
```http
GET /print/printers/{id}?$select=id,displayName,capabilities
```

### <a name="exceptions"></a><span data-ttu-id="52f52-123">Exceções</span><span class="sxs-lookup"><span data-stu-id="52f52-123">Exceptions</span></span>
* <span data-ttu-id="52f52-124">O `$count` operador não tem suporte.</span><span class="sxs-lookup"><span data-stu-id="52f52-124">The `$count` operator is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="52f52-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52f52-125">Request headers</span></span>
| <span data-ttu-id="52f52-126">Nome</span><span class="sxs-lookup"><span data-stu-id="52f52-126">Name</span></span>      |<span data-ttu-id="52f52-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="52f52-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="52f52-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="52f52-128">Authorization</span></span> | <span data-ttu-id="52f52-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52f52-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="52f52-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52f52-131">Request body</span></span>
<span data-ttu-id="52f52-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="52f52-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="52f52-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="52f52-133">Response</span></span>
<span data-ttu-id="52f52-134">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [printerShare](../resources/printershare.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52f52-134">If successful, this method returns a `200 OK` response code and a [printerShare](../resources/printershare.md) object in the response body.</span></span>
<span data-ttu-id="52f52-135">Por padrão, a resposta não conterá [printerCapabilities](../resources/printerCapabilities.md).</span><span class="sxs-lookup"><span data-stu-id="52f52-135">By default, the response will not contain [printerCapabilities](../resources/printerCapabilities.md).</span></span> <span data-ttu-id="52f52-136">Para obter **printerCapabilities**, use `$select` o parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="52f52-136">To get **printerCapabilities**, use the `$select` query parameter.</span></span> 

## <a name="example"></a><span data-ttu-id="52f52-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52f52-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="52f52-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52f52-138">Request</span></span>
<span data-ttu-id="52f52-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="52f52-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="52f52-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="52f52-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printershare"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/shares/{id}
```
# <a name="c"></a>[<span data-ttu-id="52f52-141">C#</span><span class="sxs-lookup"><span data-stu-id="52f52-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printershare-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="52f52-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52f52-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printershare-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="52f52-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="52f52-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printershare-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="52f52-144">Java</span><span class="sxs-lookup"><span data-stu-id="52f52-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printershare-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="52f52-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="52f52-145">Response</span></span>
<span data-ttu-id="52f52-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="52f52-146">The following is an example of the response.</span></span>
><span data-ttu-id="52f52-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="52f52-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerShare"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 225

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/shares/$entity",
  "id": "d837c17b-3296-4384-a053-828d56e10f50",
  "displayName": "ShareName",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z"
}
```

<span data-ttu-id="52f52-148">A seguir, um exemplo da resposta, ao usar $select=id,displayName,capabilities</span><span class="sxs-lookup"><span data-stu-id="52f52-148">The following is an example of the response, when using $select=id,displayName,capabilities</span></span>
><span data-ttu-id="52f52-149">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="52f52-149">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/shares/$entity",
  "id": "d837c17b-3296-4384-a053-828d56e10f50",
  "displayName": "ShareName",
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
  "description": "Get printerShare",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


