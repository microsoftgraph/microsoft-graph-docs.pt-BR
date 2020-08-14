---
title: Atualizar impressora
description: Atualiza as propriedades de um objeto Printer.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 4040174e1f1ad0278dcdfcd1dd94dbe9b6d94b27
ms.sourcegitcommit: 5c3f4a3e2620d1d9e635e09231bbaa73cb0c3cdd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/14/2020
ms.locfileid: "46674397"
---
# <a name="update-printer"></a><span data-ttu-id="39053-103">Atualizar impressora</span><span class="sxs-lookup"><span data-stu-id="39053-103">Update printer</span></span>

<span data-ttu-id="39053-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39053-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39053-105">Atualiza as propriedades de um objeto [Printer](../resources/printer.md) .</span><span class="sxs-lookup"><span data-stu-id="39053-105">Update the properties of a [printer](../resources/printer.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="39053-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="39053-106">Permissions</span></span>
<span data-ttu-id="39053-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39053-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="39053-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="39053-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="39053-110">O usuário conectado deve ser um [administrador da impressora](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="39053-110">The signed in user must be a [Printer Administrator](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

<span data-ttu-id="39053-111">Somente o aplicativo que registrou a impressora tem permissão para atualizar a impressora usando permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="39053-111">Only the app that registered the printer is allowed to update the printer using application permissions.</span></span>

|<span data-ttu-id="39053-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="39053-112">Permission type</span></span> | <span data-ttu-id="39053-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="39053-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="39053-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="39053-114">Delegated (work or school account)</span></span>| <span data-ttu-id="39053-115">Printer. ReadWrite. All, Printer. FullControl. All</span><span class="sxs-lookup"><span data-stu-id="39053-115">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="39053-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="39053-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39053-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="39053-117">Not Supported.</span></span>|
|<span data-ttu-id="39053-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="39053-118">Application</span></span>| <span data-ttu-id="39053-119">Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39053-119">Printer.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="39053-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="39053-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/printers/{id}
```
## <a name="request-headers"></a><span data-ttu-id="39053-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="39053-121">Request headers</span></span>
| <span data-ttu-id="39053-122">Nome</span><span class="sxs-lookup"><span data-stu-id="39053-122">Name</span></span>       | <span data-ttu-id="39053-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="39053-123">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="39053-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="39053-124">Authorization</span></span> | <span data-ttu-id="39053-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="39053-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="39053-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="39053-127">Content-type</span></span>  | <span data-ttu-id="39053-128">`application/json` ao usar permissões delegadas, `application/ipp` ao usar permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="39053-128">`application/json` when using delegated permissions, `application/ipp` when using application permissions.</span></span> <span data-ttu-id="39053-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="39053-129">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="39053-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="39053-130">Request body</span></span>

### <a name="delegated-permissions-and-json-payload"></a><span data-ttu-id="39053-131">Permissões delegadas e carga JSON</span><span class="sxs-lookup"><span data-stu-id="39053-131">Delegated permissions and JSON payload</span></span>

<span data-ttu-id="39053-132">Se estiver usando permissões delegadas, no corpo da solicitação, forneça os valores para os campos de [impressora](../resources/printer.md) relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="39053-132">If using delegated permissions, in the request body, supply the values for the relevant [printer](../resources/printer.md) fields that should be updated.</span></span> <span data-ttu-id="39053-133">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="39053-133">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="39053-134">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="39053-134">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="39053-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="39053-135">Property</span></span>     | <span data-ttu-id="39053-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="39053-136">Type</span></span>        | <span data-ttu-id="39053-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="39053-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="39053-138">location</span><span class="sxs-lookup"><span data-stu-id="39053-138">location</span></span>|[<span data-ttu-id="39053-139">printerLocation</span><span class="sxs-lookup"><span data-stu-id="39053-139">printerLocation</span></span>](../resources/printerlocation.md)|<span data-ttu-id="39053-140">O local físico e/ou organizacional da impressora.</span><span class="sxs-lookup"><span data-stu-id="39053-140">The physical and/or organizational location of the printer.</span></span>|
|<span data-ttu-id="39053-141">nome</span><span class="sxs-lookup"><span data-stu-id="39053-141">name</span></span>|<span data-ttu-id="39053-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="39053-142">String</span></span>|<span data-ttu-id="39053-143">O nome da impressora.</span><span class="sxs-lookup"><span data-stu-id="39053-143">The name of the printer.</span></span>|

### <a name="application-permissions-and-ipp-payload"></a><span data-ttu-id="39053-144">Permissões de aplicativo e carga IPP</span><span class="sxs-lookup"><span data-stu-id="39053-144">Application permissions and IPP payload</span></span>

<span data-ttu-id="39053-145">Se estiver usando permissões de aplicativo, o corpo da solicitação contém um fluxo binário que representa o grupo de atributos da impressora na [codificação IPP](https://tools.ietf.org/html/rfc8010).</span><span class="sxs-lookup"><span data-stu-id="39053-145">If using application permissions, the request body contains a binary stream representing the Printer Attributes group in [IPP encoding](https://tools.ietf.org/html/rfc8010).</span></span>

<span data-ttu-id="39053-146">O cliente deve fornecer um conjunto de atributos de impressora com um ou mais valores (incluindo valores fora de banda explicitamente permitidos), conforme definido na [seção RFC8011 4,2](https://tools.ietf.org/html/rfc8011#section-4.2) atributos de modelo de trabalho ("XXX-default", "XXX-supported" e "XXX-Ready" Attributes), [seção 4,4](https://tools.ietf.org/html/rfc8011#section-4.4) atributos de descrição da impressora e quaisquer extensões de atributo compatíveis com a impressora.</span><span class="sxs-lookup"><span data-stu-id="39053-146">The client MUST supply a set of Printer attributes with one or more values (including explicitly allowed out-of-band values) as defined in [RFC8011 section 4.2](https://tools.ietf.org/html/rfc8011#section-4.2) Job Template Attributes ("xxx-default", "xxx-supported", and "xxx-ready" attributes), [Section 4.4](https://tools.ietf.org/html/rfc8011#section-4.4) Printer Description Attributes, and any attribute extensions supported by the Printer.</span></span> <span data-ttu-id="39053-147">O (s) valor (es) de cada atributo de impressora fornecido substitui o (s) valor (es) do atributo de impressora correspondente no objeto de impressora de destino.</span><span class="sxs-lookup"><span data-stu-id="39053-147">The value(s) of each Printer attribute supplied replaces the value(s) of the corresponding Printer attribute on the target Printer object.</span></span> <span data-ttu-id="39053-148">Para atributos que podem ter vários valores (1setOf), todos os valores fornecidos pelo cliente substituem todos os valores do atributo de objeto Printer correspondente.</span><span class="sxs-lookup"><span data-stu-id="39053-148">For attributes that can have multiple values (1setOf), all values supplied by the client replace all values of the corresponding Printer object attribute.</span></span>

## <a name="response"></a><span data-ttu-id="39053-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="39053-149">Response</span></span>

### <a name="delegated-permissions-and-json-payload"></a><span data-ttu-id="39053-150">Permissões delegadas e carga JSON</span><span class="sxs-lookup"><span data-stu-id="39053-150">Delegated permissions and JSON payload</span></span>

<span data-ttu-id="39053-151">Se usar permissões delegadas, se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [Printer](../resources/printer.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="39053-151">If using delegated permissions, if successful, this method returns a `200 OK` response code and an updated [printer](../resources/printer.md) object in the response body.</span></span>

### <a name="application-permissions-and-ipp-payload"></a><span data-ttu-id="39053-152">Permissões de aplicativo e carga IPP</span><span class="sxs-lookup"><span data-stu-id="39053-152">Application permissions and IPP payload</span></span>

<span data-ttu-id="39053-153">Se o uso de permissões de aplicativo for bem-sucedido, este método retornará um `204 No content` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="39053-153">If using application permissions, if successful, this method returns `204 No content` response code.</span></span> <span data-ttu-id="39053-154">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="39053-154">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39053-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="39053-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="39053-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="39053-156">Request</span></span>
<span data-ttu-id="39053-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="39053-157">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="39053-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="39053-158">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="39053-159">C#</span><span class="sxs-lookup"><span data-stu-id="39053-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-printer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39053-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39053-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39053-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39053-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-printer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="39053-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="39053-162">Response</span></span>
<span data-ttu-id="39053-163">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="39053-163">The following is an example of the response.</span></span>
><span data-ttu-id="39053-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="39053-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
