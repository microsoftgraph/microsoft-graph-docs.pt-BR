---
title: 'printer: getCapabilities'
description: Obter uma lista de recursos para a impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 2e3720014b3094d8d8696b6931f37586590b7d8a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049909"
---
# <a name="printer-getcapabilities"></a><span data-ttu-id="206fe-103">printer: getCapabilities</span><span class="sxs-lookup"><span data-stu-id="206fe-103">printer: getCapabilities</span></span>

<span data-ttu-id="206fe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="206fe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="206fe-105">Obter uma lista de recursos para a [impressora](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="206fe-105">Get a list of capabilities for the [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="206fe-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="206fe-106">Permissions</span></span>
<span data-ttu-id="206fe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="206fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="206fe-109">Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="206fe-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="206fe-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="206fe-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="206fe-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="206fe-111">Permission type</span></span> | <span data-ttu-id="206fe-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="206fe-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="206fe-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="206fe-113">Delegated (work or school account)</span></span>| <span data-ttu-id="206fe-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="206fe-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="206fe-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="206fe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="206fe-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="206fe-116">Not Supported.</span></span>|
|<span data-ttu-id="206fe-117">Application</span><span class="sxs-lookup"><span data-stu-id="206fe-117">Application</span></span>| <span data-ttu-id="206fe-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="206fe-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="206fe-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="206fe-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /print/printers/{id}/getCapabilities
```
## <a name="request-headers"></a><span data-ttu-id="206fe-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="206fe-120">Request headers</span></span>
| <span data-ttu-id="206fe-121">Nome</span><span class="sxs-lookup"><span data-stu-id="206fe-121">Name</span></span>          | <span data-ttu-id="206fe-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="206fe-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="206fe-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="206fe-123">Authorization</span></span> | <span data-ttu-id="206fe-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="206fe-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="206fe-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="206fe-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="206fe-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="206fe-127">Response</span></span>
<span data-ttu-id="206fe-128">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [printerCapabilities](../resources/printercapabilities.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="206fe-128">If successful, this method returns a `200 OK` response code and a [printerCapabilities](../resources/printercapabilities.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="206fe-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="206fe-129">Example</span></span>
<span data-ttu-id="206fe-130">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="206fe-130">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="206fe-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="206fe-131">Request</span></span>
<span data-ttu-id="206fe-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="206fe-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="206fe-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="206fe-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printer-getCapabilities"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/print/printers/{id}/getCapabilities
```
# <a name="c"></a>[<span data-ttu-id="206fe-134">C#</span><span class="sxs-lookup"><span data-stu-id="206fe-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printer-getcapabilities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="206fe-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="206fe-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printer-getcapabilities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="206fe-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="206fe-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printer-getcapabilities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="206fe-137">Java</span><span class="sxs-lookup"><span data-stu-id="206fe-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printer-getcapabilities-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="206fe-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="206fe-138">Response</span></span>
<span data-ttu-id="206fe-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="206fe-139">The following is an example of the response.</span></span>
><span data-ttu-id="206fe-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="206fe-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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
