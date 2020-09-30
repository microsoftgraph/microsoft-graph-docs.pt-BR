---
title: 'impressora: GetCapabilities'
description: Obtenha uma lista de recursos para a impressora.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: a41f6c945191dcae01eceb95e45074603c30c754
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48315581"
---
# <a name="printer-getcapabilities"></a><span data-ttu-id="38f7e-103">impressora: GetCapabilities</span><span class="sxs-lookup"><span data-stu-id="38f7e-103">printer: getCapabilities</span></span>

<span data-ttu-id="38f7e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38f7e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38f7e-105">Obtenha uma lista de recursos para a [impressora](../resources/printer.md).</span><span class="sxs-lookup"><span data-stu-id="38f7e-105">Get a list of capabilities for the [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="38f7e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="38f7e-106">Permissions</span></span>
<span data-ttu-id="38f7e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38f7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="38f7e-109">Para usar o serviço de impressão universal, o usuário ou o locatário do aplicativo deve ter uma assinatura de impressão universal ativa, além das permissões listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="38f7e-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="38f7e-110">O usuário conectado deve ser um [administrador da impressora](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="38f7e-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="38f7e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38f7e-111">Permission type</span></span> | <span data-ttu-id="38f7e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="38f7e-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="38f7e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38f7e-113">Delegated (work or school account)</span></span>| <span data-ttu-id="38f7e-114">Printer. Read. All, Printer. ReadWrite. All, Printer. FullControl. All</span><span class="sxs-lookup"><span data-stu-id="38f7e-114">Printer.Read.All, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="38f7e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38f7e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38f7e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38f7e-116">Not Supported.</span></span>|
|<span data-ttu-id="38f7e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38f7e-117">Application</span></span>| <span data-ttu-id="38f7e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38f7e-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="38f7e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38f7e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/getCapabilities
```
## <a name="request-headers"></a><span data-ttu-id="38f7e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38f7e-120">Request headers</span></span>
| <span data-ttu-id="38f7e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="38f7e-121">Name</span></span>          | <span data-ttu-id="38f7e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="38f7e-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="38f7e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="38f7e-123">Authorization</span></span> | <span data-ttu-id="38f7e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38f7e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="38f7e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38f7e-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="38f7e-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="38f7e-127">Response</span></span>
<span data-ttu-id="38f7e-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [printerCapabilities](../resources/printercapabilities.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38f7e-128">If successful, this method returns a `200 OK` response code and a [printerCapabilities](../resources/printercapabilities.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38f7e-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="38f7e-129">Example</span></span>
<span data-ttu-id="38f7e-130">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="38f7e-130">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="38f7e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38f7e-131">Request</span></span>
<span data-ttu-id="38f7e-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="38f7e-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="38f7e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="38f7e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printer-getCapabilities"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/getCapabilities
```
# <a name="c"></a>[<span data-ttu-id="38f7e-134">C#</span><span class="sxs-lookup"><span data-stu-id="38f7e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printer-getcapabilities-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="38f7e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="38f7e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printer-getcapabilities-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="38f7e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="38f7e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printer-getcapabilities-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="38f7e-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="38f7e-137">Response</span></span>
<span data-ttu-id="38f7e-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="38f7e-138">The following is an example of the response.</span></span>
><span data-ttu-id="38f7e-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="38f7e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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