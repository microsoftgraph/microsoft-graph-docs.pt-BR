---
title: Atualizar impressora
description: Atualiza as propriedades de um objeto Printer.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: d23b016bb383903f35d370c9d4afb623518e5bfd
ms.sourcegitcommit: 66a52d2e63cf3447ec50bd28e562d99e7c344814
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2020
ms.locfileid: "43062088"
---
# <a name="update-printer"></a><span data-ttu-id="73828-103">Atualizar impressora</span><span class="sxs-lookup"><span data-stu-id="73828-103">Update printer</span></span>

<span data-ttu-id="73828-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73828-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73828-105">Atualiza as propriedades de um objeto [Printer](../resources/printer.md) .</span><span class="sxs-lookup"><span data-stu-id="73828-105">Update the properties of a [printer](../resources/printer.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="73828-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="73828-106">Permissions</span></span>
<span data-ttu-id="73828-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73828-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="73828-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="73828-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="73828-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="73828-110">Permission type</span></span> | <span data-ttu-id="73828-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="73828-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="73828-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="73828-112">Delegated (work or school account)</span></span>| <span data-ttu-id="73828-113">Users. Read. All</span><span class="sxs-lookup"><span data-stu-id="73828-113">Users.Read.All</span></span> |
|<span data-ttu-id="73828-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="73828-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73828-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73828-115">Not Supported.</span></span>|
|<span data-ttu-id="73828-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="73828-116">Application</span></span>|<span data-ttu-id="73828-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73828-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73828-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="73828-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/printers/{id}
```
## <a name="request-headers"></a><span data-ttu-id="73828-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="73828-119">Request headers</span></span>
| <span data-ttu-id="73828-120">Nome</span><span class="sxs-lookup"><span data-stu-id="73828-120">Name</span></span>       | <span data-ttu-id="73828-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="73828-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="73828-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="73828-122">Authorization</span></span> | <span data-ttu-id="73828-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73828-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="73828-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="73828-125">Content-type</span></span>  | <span data-ttu-id="73828-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73828-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="73828-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="73828-128">Request body</span></span>
<span data-ttu-id="73828-129">No corpo da solicitação, forneça os valores para os campos de [impressora](../resources/printer.md) relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="73828-129">In the request body, supply the values for the relevant [printer](../resources/printer.md) fields that should be updated.</span></span> <span data-ttu-id="73828-130">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="73828-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="73828-131">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="73828-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="73828-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73828-132">Property</span></span>     | <span data-ttu-id="73828-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="73828-133">Type</span></span>        | <span data-ttu-id="73828-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="73828-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="73828-135">location</span><span class="sxs-lookup"><span data-stu-id="73828-135">location</span></span>|[<span data-ttu-id="73828-136">printerLocation</span><span class="sxs-lookup"><span data-stu-id="73828-136">printerLocation</span></span>](../resources/printerlocation.md)|<span data-ttu-id="73828-137">O local físico e/ou organizacional da impressora.</span><span class="sxs-lookup"><span data-stu-id="73828-137">The physical and/or organizational location of the printer.</span></span>|
|<span data-ttu-id="73828-138">name</span><span class="sxs-lookup"><span data-stu-id="73828-138">name</span></span>|<span data-ttu-id="73828-139">String</span><span class="sxs-lookup"><span data-stu-id="73828-139">String</span></span>|<span data-ttu-id="73828-140">O nome da impressora.</span><span class="sxs-lookup"><span data-stu-id="73828-140">The name of the printer.</span></span>|

## <a name="response"></a><span data-ttu-id="73828-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="73828-141">Response</span></span>
<span data-ttu-id="73828-142">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [Printer](../resources/printer.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="73828-142">If successful, this method returns a `200 OK` response code and an updated [printer](../resources/printer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="73828-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="73828-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="73828-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73828-144">Request</span></span>
<span data-ttu-id="73828-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="73828-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="73828-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="73828-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_printer"
}-->
```http
PATCH https://graph.microsoft.com/beta/print/printers/{id}
Content-type: application/json
Content-length: 124

{
  "name": "PrinterName",
  "location": {
    "latitude": 1.1,
    "longitude": 2.2,
    "altitudeInMeters": 3
  }
}
```
# <a name="c"></a>[<span data-ttu-id="73828-147">C#</span><span class="sxs-lookup"><span data-stu-id="73828-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-printer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="73828-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73828-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="73828-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73828-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-printer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="73828-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="73828-150">Response</span></span>
<span data-ttu-id="73828-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="73828-151">The following is an example of the response.</span></span>
><span data-ttu-id="73828-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="73828-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "processingState": "idle",
    "processingStateReasons": [],
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
  "description": "Update printer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
