---
title: Atualização da impressora
description: Atualiza as propriedades de um objeto Printer.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 95af5526edbbd40a65e3356efa7cee76cf135c14
ms.sourcegitcommit: a9720ab80625a4692f7d2450164717853535d0b0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/11/2020
ms.locfileid: "48993966"
---
# <a name="update-printer"></a><span data-ttu-id="59058-103">Atualização da impressora</span><span class="sxs-lookup"><span data-stu-id="59058-103">Update printer</span></span>

<span data-ttu-id="59058-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59058-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59058-105">Atualiza as propriedades de um objeto [Printer](../resources/printer.md) .</span><span class="sxs-lookup"><span data-stu-id="59058-105">Update the properties of a [printer](../resources/printer.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="59058-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="59058-106">Permissions</span></span>
<span data-ttu-id="59058-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59058-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="59058-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura universal de impressão.</span><span class="sxs-lookup"><span data-stu-id="59058-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="59058-110">O usuário conectado deve ser um [administrador da impressora](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span><span class="sxs-lookup"><span data-stu-id="59058-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

<span data-ttu-id="59058-111">Somente o aplicativo que registrou a impressora tem permissão para atualizar a impressora usando permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="59058-111">Only the app that registered the printer is allowed to update the printer using application permissions.</span></span>

|<span data-ttu-id="59058-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59058-112">Permission type</span></span> | <span data-ttu-id="59058-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="59058-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="59058-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59058-114">Delegated (work or school account)</span></span>| <span data-ttu-id="59058-115">Printer. ReadWrite. All, Printer. FullControl. All</span><span class="sxs-lookup"><span data-stu-id="59058-115">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="59058-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59058-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="59058-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="59058-117">Not Supported.</span></span>|
|<span data-ttu-id="59058-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59058-118">Application</span></span>| <span data-ttu-id="59058-119">Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59058-119">Printer.ReadWrite.All</span></span> |

><span data-ttu-id="59058-120">**Observação:** No momento, apenas impressoras que não têm dispositivo físico podem ser atualizadas usando permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="59058-120">**Note:** Right now, only printers that don't have physical device can be updated using application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="59058-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59058-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/printers/{id}
```
## <a name="request-headers"></a><span data-ttu-id="59058-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59058-122">Request headers</span></span>
| <span data-ttu-id="59058-123">Nome</span><span class="sxs-lookup"><span data-stu-id="59058-123">Name</span></span>       | <span data-ttu-id="59058-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="59058-124">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="59058-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="59058-125">Authorization</span></span> | <span data-ttu-id="59058-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59058-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="59058-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="59058-128">Content-type</span></span>  | <span data-ttu-id="59058-129">`application/json` ao usar permissões delegadas, `application/ipp` ao usar permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="59058-129">`application/json` when using delegated permissions, `application/ipp` when using application permissions.</span></span> <span data-ttu-id="59058-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59058-130">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="59058-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59058-131">Request body</span></span>

### <a name="delegated-permissions-and-json-payload"></a><span data-ttu-id="59058-132">Permissões delegadas e carga JSON</span><span class="sxs-lookup"><span data-stu-id="59058-132">Delegated permissions and JSON payload</span></span>

<span data-ttu-id="59058-133">Se estiver usando permissões delegadas, no corpo da solicitação, forneça os valores para os campos de [impressora](../resources/printer.md) relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="59058-133">If using delegated permissions, in the request body, supply the values for the relevant [printer](../resources/printer.md) fields that should be updated.</span></span> <span data-ttu-id="59058-134">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="59058-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="59058-135">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="59058-135">For best performance, don't include existing values that haven't changed.</span></span> 

<span data-ttu-id="59058-136">As propriedades a seguir podem ser atualizadas usando permissões delegadas.</span><span class="sxs-lookup"><span data-stu-id="59058-136">The following properties can be updated using delegated permissions.</span></span>

| <span data-ttu-id="59058-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="59058-137">Property</span></span>     | <span data-ttu-id="59058-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="59058-138">Type</span></span>        | <span data-ttu-id="59058-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="59058-139">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="59058-140">defaults</span><span class="sxs-lookup"><span data-stu-id="59058-140">defaults</span></span>|[<span data-ttu-id="59058-141">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="59058-141">printerDefaults</span></span>](../resources/printerdefaults.md)|<span data-ttu-id="59058-142">As configurações de impressão padrão da impressora.</span><span class="sxs-lookup"><span data-stu-id="59058-142">The printer's default print settings.</span></span>|
|<span data-ttu-id="59058-143">localização</span><span class="sxs-lookup"><span data-stu-id="59058-143">location</span></span>|[<span data-ttu-id="59058-144">printerLocation</span><span class="sxs-lookup"><span data-stu-id="59058-144">printerLocation</span></span>](../resources/printerlocation.md)|<span data-ttu-id="59058-145">O local físico e/ou organizacional da impressora.</span><span class="sxs-lookup"><span data-stu-id="59058-145">The physical and/or organizational location of the printer.</span></span>|
|<span data-ttu-id="59058-146">displayName</span><span class="sxs-lookup"><span data-stu-id="59058-146">displayName</span></span>|<span data-ttu-id="59058-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59058-147">String</span></span>|<span data-ttu-id="59058-148">O nome da impressora.</span><span class="sxs-lookup"><span data-stu-id="59058-148">The name of the printer.</span></span>|

### <a name="application-permissions-and-json-payload"></a><span data-ttu-id="59058-149">Permissões de aplicativo e carga JSON</span><span class="sxs-lookup"><span data-stu-id="59058-149">Application permissions and JSON payload</span></span>
<span data-ttu-id="59058-150">No corpo da solicitação, forneça os valores para os campos de [impressora](../resources/printer.md) relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="59058-150">In the request body, supply the values for the relevant [printer](../resources/printer.md) fields that should be updated.</span></span> <span data-ttu-id="59058-151">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="59058-151">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="59058-152">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="59058-152">For best performance, don't include existing values that haven't changed.</span></span> 

<span data-ttu-id="59058-153">As propriedades a seguir podem ser atualizadas usando permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="59058-153">The following properties can be updated using application permissions.</span></span>

| <span data-ttu-id="59058-154">Propriedade</span><span class="sxs-lookup"><span data-stu-id="59058-154">Property</span></span>     | <span data-ttu-id="59058-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="59058-155">Type</span></span>        | <span data-ttu-id="59058-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="59058-156">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="59058-157">defaults</span><span class="sxs-lookup"><span data-stu-id="59058-157">defaults</span></span>|[<span data-ttu-id="59058-158">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="59058-158">printerDefaults</span></span>](../resources/printerdefaults.md)|<span data-ttu-id="59058-159">As configurações de impressão padrão da impressora.</span><span class="sxs-lookup"><span data-stu-id="59058-159">The printer's default print settings.</span></span>|
|<span data-ttu-id="59058-160">capabilities</span><span class="sxs-lookup"><span data-stu-id="59058-160">capabilities</span></span>|[<span data-ttu-id="59058-161">printerCapabilities</span><span class="sxs-lookup"><span data-stu-id="59058-161">printerCapabilities</span></span>](../resources/printerCapabilities.md)|<span data-ttu-id="59058-162">Os recursos da impressora associada a este compartilhamento de impressora.</span><span class="sxs-lookup"><span data-stu-id="59058-162">The capabilities of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="59058-163">displayName</span><span class="sxs-lookup"><span data-stu-id="59058-163">displayName</span></span>|<span data-ttu-id="59058-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="59058-164">String</span></span>|<span data-ttu-id="59058-165">O nome da impressora.</span><span class="sxs-lookup"><span data-stu-id="59058-165">The name of the printer.</span></span>|
|<span data-ttu-id="59058-166">fabricante</span><span class="sxs-lookup"><span data-stu-id="59058-166">manufacturer</span></span>|<span data-ttu-id="59058-167">String</span><span class="sxs-lookup"><span data-stu-id="59058-167">String</span></span>|<span data-ttu-id="59058-168">O fabricante da impressora.</span><span class="sxs-lookup"><span data-stu-id="59058-168">The manufacturer of the printer.</span></span>|
|<span data-ttu-id="59058-169">modelo</span><span class="sxs-lookup"><span data-stu-id="59058-169">model</span></span>|<span data-ttu-id="59058-170">String</span><span class="sxs-lookup"><span data-stu-id="59058-170">String</span></span>|<span data-ttu-id="59058-171">O nome do modelo da impressora.</span><span class="sxs-lookup"><span data-stu-id="59058-171">The model name of the printer.</span></span>|
|<span data-ttu-id="59058-172">status</span><span class="sxs-lookup"><span data-stu-id="59058-172">status</span></span>|[<span data-ttu-id="59058-173">printerStatus</span><span class="sxs-lookup"><span data-stu-id="59058-173">printerStatus</span></span>](../resources/printerstatus.md)|<span data-ttu-id="59058-174">O status de processamento da impressora, incluindo erros.</span><span class="sxs-lookup"><span data-stu-id="59058-174">The processing status of the printer, including any errors.</span></span>|
|<span data-ttu-id="59058-175">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="59058-175">isAcceptingJobs</span></span>|<span data-ttu-id="59058-176">Booliano</span><span class="sxs-lookup"><span data-stu-id="59058-176">Boolean</span></span>|<span data-ttu-id="59058-177">Se a impressora está atualmente aceitando novos trabalhos de impressão.</span><span class="sxs-lookup"><span data-stu-id="59058-177">Whether the printer is currently accepting new print jobs.</span></span>|

### <a name="application-permissions-and-ipp-payload"></a><span data-ttu-id="59058-178">Permissões de aplicativo e carga IPP</span><span class="sxs-lookup"><span data-stu-id="59058-178">Application permissions and IPP payload</span></span>

<span data-ttu-id="59058-179">Com permissões de aplicativo, uma impressora também pode ser atualizada usando uma carga do protocolo IPP (Internet Printing Protocol).</span><span class="sxs-lookup"><span data-stu-id="59058-179">With application permissions, a printer can also be updated using an Internet Printing Protocol (IPP) payload.</span></span> <span data-ttu-id="59058-180">Nesse caso, o corpo da solicitação contém um fluxo binário que representa o grupo de atributos da impressora na [codificação IPP](https://tools.ietf.org/html/rfc8010).</span><span class="sxs-lookup"><span data-stu-id="59058-180">In this case, the request body contains a binary stream that represents the Printer Attributes group in [IPP encoding](https://tools.ietf.org/html/rfc8010).</span></span>

<span data-ttu-id="59058-181">O cliente deve fornecer um conjunto de atributos de impressora com um ou mais valores (incluindo valores fora de banda explicitamente permitidos), conforme definido na [seção RFC8011 5,2](https://tools.ietf.org/html/rfc8011#section-5.2) atributos de modelo de trabalho ("XXX-default", "XXX-supported" e "XXX-Ready" Attributes), [seção 5,4](https://tools.ietf.org/html/rfc8011#section-5.4) atributos de descrição da impressora e quaisquer extensões de atributo compatíveis com a impressora.</span><span class="sxs-lookup"><span data-stu-id="59058-181">The client MUST supply a set of Printer attributes with one or more values (including explicitly allowed out-of-band values) as defined in [RFC8011 section 5.2](https://tools.ietf.org/html/rfc8011#section-5.2) Job Template Attributes ("xxx-default", "xxx-supported", and "xxx-ready" attributes), [Section 5.4](https://tools.ietf.org/html/rfc8011#section-5.4) Printer Description Attributes, and any attribute extensions supported by the Printer.</span></span> <span data-ttu-id="59058-182">O (s) valor (es) de cada atributo de impressora fornecido substitui o (s) valor (es) do atributo de impressora correspondente no objeto de impressora de destino.</span><span class="sxs-lookup"><span data-stu-id="59058-182">The value(s) of each Printer attribute supplied replaces the value(s) of the corresponding Printer attribute on the target Printer object.</span></span> <span data-ttu-id="59058-183">Para atributos que podem ter vários valores (1setOf), todos os valores fornecidos pelo cliente substituem todos os valores do atributo de objeto Printer correspondente.</span><span class="sxs-lookup"><span data-stu-id="59058-183">For attributes that can have multiple values (1setOf), all values supplied by the client replace all values of the corresponding Printer object attribute.</span></span>

## <a name="response"></a><span data-ttu-id="59058-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="59058-184">Response</span></span>

### <a name="delegated-permissions-and-json-payload"></a><span data-ttu-id="59058-185">Permissões delegadas e carga JSON</span><span class="sxs-lookup"><span data-stu-id="59058-185">Delegated permissions and JSON payload</span></span>

<span data-ttu-id="59058-186">Se usar permissões delegadas, se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [Printer](../resources/printer.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59058-186">If using delegated permissions, if successful, this method returns a `200 OK` response code and an updated [printer](../resources/printer.md) object in the response body.</span></span>

### <a name="application-permissions-and-json-payload"></a><span data-ttu-id="59058-187">Permissões de aplicativo e carga JSON</span><span class="sxs-lookup"><span data-stu-id="59058-187">Application permissions and JSON payload</span></span>

<span data-ttu-id="59058-188">Se usar permissões delegadas, se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [Printer](../resources/printer.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59058-188">If using delegated permissions, if successful, this method returns a `200 OK` response code and an updated [printer](../resources/printer.md) object in the response body.</span></span>

### <a name="application-permissions-and-ipp-payload"></a><span data-ttu-id="59058-189">Permissões de aplicativo e carga IPP</span><span class="sxs-lookup"><span data-stu-id="59058-189">Application permissions and IPP payload</span></span>

<span data-ttu-id="59058-190">Se o uso de permissões de aplicativo for bem-sucedido, este método retornará um `204 No content` código de resposta.</span><span class="sxs-lookup"><span data-stu-id="59058-190">If using application permissions, if successful, this method returns `204 No content` response code.</span></span> <span data-ttu-id="59058-191">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="59058-191">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59058-192">Exemplo</span><span class="sxs-lookup"><span data-stu-id="59058-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="59058-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59058-193">Request</span></span>
<span data-ttu-id="59058-194">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="59058-194">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="59058-195">HTTP</span><span class="sxs-lookup"><span data-stu-id="59058-195">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="59058-196">C#</span><span class="sxs-lookup"><span data-stu-id="59058-196">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-printer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="59058-197">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59058-197">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="59058-198">Objective-C</span><span class="sxs-lookup"><span data-stu-id="59058-198">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-printer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="59058-199">Java</span><span class="sxs-lookup"><span data-stu-id="59058-199">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-printer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="59058-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="59058-200">Response</span></span>
<span data-ttu-id="59058-201">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="59058-201">The following is an example of the response.</span></span>
><span data-ttu-id="59058-p110">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="59058-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
