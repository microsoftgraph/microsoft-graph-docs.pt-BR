---
title: 'impressora: GetCapabilities'
description: Obtenha uma lista de recursos para a impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: d3ed6f5f57bc528abaec2661d7bd8d88cba7d75e
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947971"
---
# <a name="printer-getcapabilities"></a><span data-ttu-id="5dd99-103">impressora: GetCapabilities</span><span class="sxs-lookup"><span data-stu-id="5dd99-103">printer: getCapabilities</span></span>

<span data-ttu-id="5dd99-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5dd99-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5dd99-105">Obtenha uma lista de recursos para a [impressora](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="5dd99-105">Get a list of capabilities for the [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5dd99-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5dd99-106">Permissions</span></span>
<span data-ttu-id="5dd99-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5dd99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="5dd99-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="5dd99-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="5dd99-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5dd99-110">Permission type</span></span> | <span data-ttu-id="5dd99-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5dd99-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="5dd99-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5dd99-112">Delegated (work or school account)</span></span>| <span data-ttu-id="5dd99-113">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="5dd99-113">Users.Read.All</span></span> |
|<span data-ttu-id="5dd99-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5dd99-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5dd99-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5dd99-115">Not Supported.</span></span>|
|<span data-ttu-id="5dd99-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5dd99-116">Application</span></span>|<span data-ttu-id="5dd99-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5dd99-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5dd99-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5dd99-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/getCapabilities
```
## <a name="request-headers"></a><span data-ttu-id="5dd99-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5dd99-119">Request headers</span></span>
| <span data-ttu-id="5dd99-120">Nome</span><span class="sxs-lookup"><span data-stu-id="5dd99-120">Name</span></span>          | <span data-ttu-id="5dd99-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="5dd99-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="5dd99-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5dd99-122">Authorization</span></span> | <span data-ttu-id="5dd99-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5dd99-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5dd99-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5dd99-125">Request body</span></span>

## <a name="response"></a><span data-ttu-id="5dd99-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dd99-126">Response</span></span>
<span data-ttu-id="5dd99-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [printerCapabilities](../resources/printercapabilities.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5dd99-127">If successful, this method returns a `200 OK` response code and a [printerCapabilities](../resources/printercapabilities.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5dd99-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5dd99-128">Example</span></span>
<span data-ttu-id="5dd99-129">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="5dd99-129">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="5dd99-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5dd99-130">Request</span></span>
<span data-ttu-id="5dd99-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5dd99-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5dd99-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="5dd99-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printer-getCapabilities"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/getCapabilities
```
# <a name="c"></a>[<span data-ttu-id="5dd99-133">C#</span><span class="sxs-lookup"><span data-stu-id="5dd99-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printer-getcapabilities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5dd99-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5dd99-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printer-getcapabilities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5dd99-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5dd99-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printer-getcapabilities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="5dd99-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="5dd99-136">Response</span></span>
<span data-ttu-id="5dd99-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5dd99-137">The following is an example of the response.</span></span>
><span data-ttu-id="5dd99-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5dd99-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerCapabilities"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1159

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.printerCapabilities",
    "isColorPrintingSupported": true,
    "supportsFitPdfToPage": false,
    "supportedDocumentMimeTypes": [
        "application/oxps"
    ],
    "supportedFinishings": [
        "none"
    ],
    "supportedMediaColors": [],
    "supportedMediaTypes": [],
    "supportedMediaSizes": [
        "North America Letter",
        "North America Ledger",
        "North America Legal",
        "North America Invoice",
        "North America Executive",
        "A3",
        "A4",
        "A5",
        "JIS B4",
        "JIS B5"
    ],
    "supportedOrientations": [
        "portrait",
        "landscape"
    ],
    "supportedOutputBins": [
        "tray-1"
    ],
    "supportedDuplexConfigurations": [
        "oneSided"
    ],
    "supportedPresentationDirections": [],
    "supportedColorConfigurations": [
        "color"
    ],
    "supportedPrintQualities": [
        "medium"
    ],
    "supportedPagesPerSheet": null,
    "supportedCopiesPerJob": {
        "minimum": 1,
        "maximum": 1
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printer: getCapabilities",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
