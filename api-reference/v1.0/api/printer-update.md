---
title: Atualização da impressora
description: Atualize as propriedades de um objeto printer.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: e29335cab6d88c736825684b2ab46e65db64d563
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516838"
---
# <a name="update-printer"></a><span data-ttu-id="14303-103">Atualização da impressora</span><span class="sxs-lookup"><span data-stu-id="14303-103">Update printer</span></span>
<span data-ttu-id="14303-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14303-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="14303-105">Atualize as propriedades de um [objeto printer.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="14303-105">Update the properties of a [printer](../resources/printer.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="14303-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="14303-106">Permissions</span></span>
<span data-ttu-id="14303-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14303-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="14303-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="14303-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="14303-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="14303-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

><span data-ttu-id="14303-111">**Observação:** Somente o aplicativo que registrou a impressora tem permissão para atualizar a impressora usando permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="14303-111">**Note:** Only the app that registered the printer is allowed to update the printer using application permissions.</span></span>

|<span data-ttu-id="14303-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14303-112">Permission type</span></span> | <span data-ttu-id="14303-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="14303-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="14303-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14303-114">Delegated (work or school account)</span></span>| <span data-ttu-id="14303-115">Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="14303-115">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="14303-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14303-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14303-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14303-117">Not Supported.</span></span>|
|<span data-ttu-id="14303-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="14303-118">Application</span></span>| <span data-ttu-id="14303-119">Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14303-119">Printer.ReadWrite.All</span></span> |

><span data-ttu-id="14303-120">**Observação:** No momento, somente as impressoras que não têm dispositivo físico podem ser atualizadas usando permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="14303-120">**Note:** Right now, only printers that don't have physical device can be updated using application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="14303-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14303-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /print/printers/{printerId}
```

## <a name="request-headers"></a><span data-ttu-id="14303-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14303-122">Request headers</span></span>
|<span data-ttu-id="14303-123">Nome</span><span class="sxs-lookup"><span data-stu-id="14303-123">Name</span></span>|<span data-ttu-id="14303-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="14303-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="14303-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="14303-125">Authorization</span></span>|<span data-ttu-id="14303-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14303-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="14303-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="14303-128">Content-Type</span></span>|<span data-ttu-id="14303-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14303-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="14303-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="14303-131">Request body</span></span>

### <a name="delegated-permissions-and-json-payload"></a><span data-ttu-id="14303-132">Permissões delegadas e carga JSON</span><span class="sxs-lookup"><span data-stu-id="14303-132">Delegated permissions and JSON payload</span></span>

<span data-ttu-id="14303-133">Se estiver usando permissões delegadas, no corpo da solicitação, forneça os valores para os campos de [impressora relevantes](../resources/printer.md) que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="14303-133">If using delegated permissions, in the request body, supply the values for the relevant [printer](../resources/printer.md) fields that should be updated.</span></span> <span data-ttu-id="14303-134">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="14303-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="14303-135">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="14303-135">For best performance, don't include existing values that haven't changed.</span></span> 

<span data-ttu-id="14303-136">As propriedades a seguir podem ser atualizadas usando permissões delegadas.</span><span class="sxs-lookup"><span data-stu-id="14303-136">The following properties can be updated using delegated permissions.</span></span>

| <span data-ttu-id="14303-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14303-137">Property</span></span>     | <span data-ttu-id="14303-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="14303-138">Type</span></span>        | <span data-ttu-id="14303-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="14303-139">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="14303-140">defaults</span><span class="sxs-lookup"><span data-stu-id="14303-140">defaults</span></span>|[<span data-ttu-id="14303-141">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="14303-141">printerDefaults</span></span>](../resources/printerdefaults.md)|<span data-ttu-id="14303-142">As configurações de impressão padrão da impressora.</span><span class="sxs-lookup"><span data-stu-id="14303-142">The printer's default print settings.</span></span>|
|<span data-ttu-id="14303-143">location</span><span class="sxs-lookup"><span data-stu-id="14303-143">location</span></span>|[<span data-ttu-id="14303-144">printerLocation</span><span class="sxs-lookup"><span data-stu-id="14303-144">printerLocation</span></span>](../resources/printerlocation.md)|<span data-ttu-id="14303-145">O local físico e/ou organizacional da impressora.</span><span class="sxs-lookup"><span data-stu-id="14303-145">The physical and/or organizational location of the printer.</span></span>|
|<span data-ttu-id="14303-146">displayName</span><span class="sxs-lookup"><span data-stu-id="14303-146">displayName</span></span>|<span data-ttu-id="14303-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14303-147">String</span></span>|<span data-ttu-id="14303-148">O nome da impressora.</span><span class="sxs-lookup"><span data-stu-id="14303-148">The name of the printer.</span></span>|

### <a name="application-permissions-and-json-payload"></a><span data-ttu-id="14303-149">Permissões de aplicativo e carga JSON</span><span class="sxs-lookup"><span data-stu-id="14303-149">Application permissions and JSON payload</span></span>
<span data-ttu-id="14303-150">No corpo da solicitação, fornece os valores para os campos de [impressora relevantes](../resources/printer.md) que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="14303-150">In the request body, supply the values for the relevant [printer](../resources/printer.md) fields that should be updated.</span></span> <span data-ttu-id="14303-151">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="14303-151">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="14303-152">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="14303-152">For best performance, don't include existing values that haven't changed.</span></span> 

<span data-ttu-id="14303-153">As propriedades a seguir podem ser atualizadas usando permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="14303-153">The following properties can be updated using application permissions.</span></span>

| <span data-ttu-id="14303-154">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14303-154">Property</span></span>     | <span data-ttu-id="14303-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="14303-155">Type</span></span>        | <span data-ttu-id="14303-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="14303-156">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="14303-157">defaults</span><span class="sxs-lookup"><span data-stu-id="14303-157">defaults</span></span>|[<span data-ttu-id="14303-158">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="14303-158">printerDefaults</span></span>](../resources/printerdefaults.md)|<span data-ttu-id="14303-159">As configurações de impressão padrão da impressora.</span><span class="sxs-lookup"><span data-stu-id="14303-159">The printer's default print settings.</span></span>|
|<span data-ttu-id="14303-160">capabilities</span><span class="sxs-lookup"><span data-stu-id="14303-160">capabilities</span></span>|[<span data-ttu-id="14303-161">printerCapabilities</span><span class="sxs-lookup"><span data-stu-id="14303-161">printerCapabilities</span></span>](../resources/printerCapabilities.md)|<span data-ttu-id="14303-162">Os recursos da impressora associados a esse compartilhamento de impressora.</span><span class="sxs-lookup"><span data-stu-id="14303-162">The capabilities of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="14303-163">displayName</span><span class="sxs-lookup"><span data-stu-id="14303-163">displayName</span></span>|<span data-ttu-id="14303-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14303-164">String</span></span>|<span data-ttu-id="14303-165">O nome da impressora.</span><span class="sxs-lookup"><span data-stu-id="14303-165">The name of the printer.</span></span>|
|<span data-ttu-id="14303-166">fabricante</span><span class="sxs-lookup"><span data-stu-id="14303-166">manufacturer</span></span>|<span data-ttu-id="14303-167">String</span><span class="sxs-lookup"><span data-stu-id="14303-167">String</span></span>|<span data-ttu-id="14303-168">O fabricante da impressora.</span><span class="sxs-lookup"><span data-stu-id="14303-168">The manufacturer of the printer.</span></span>|
|<span data-ttu-id="14303-169">modelo</span><span class="sxs-lookup"><span data-stu-id="14303-169">model</span></span>|<span data-ttu-id="14303-170">String</span><span class="sxs-lookup"><span data-stu-id="14303-170">String</span></span>|<span data-ttu-id="14303-171">O nome do modelo da impressora.</span><span class="sxs-lookup"><span data-stu-id="14303-171">The model name of the printer.</span></span>|
|<span data-ttu-id="14303-172">status</span><span class="sxs-lookup"><span data-stu-id="14303-172">status</span></span>|[<span data-ttu-id="14303-173">printerStatus</span><span class="sxs-lookup"><span data-stu-id="14303-173">printerStatus</span></span>](../resources/printerstatus.md)|<span data-ttu-id="14303-174">O status de processamento da impressora, incluindo quaisquer erros.</span><span class="sxs-lookup"><span data-stu-id="14303-174">The processing status of the printer, including any errors.</span></span>|
|<span data-ttu-id="14303-175">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="14303-175">isAcceptingJobs</span></span>|<span data-ttu-id="14303-176">Booliano</span><span class="sxs-lookup"><span data-stu-id="14303-176">Boolean</span></span>|<span data-ttu-id="14303-177">Se a impressora está aceitando novos trabalhos de impressão no momento.</span><span class="sxs-lookup"><span data-stu-id="14303-177">Whether the printer is currently accepting new print jobs.</span></span>|

### <a name="application-permissions-and-ipp-payload"></a><span data-ttu-id="14303-178">Permissões de aplicativo e carga IPP</span><span class="sxs-lookup"><span data-stu-id="14303-178">Application permissions and IPP payload</span></span>

<span data-ttu-id="14303-179">Com permissões de aplicativo, uma impressora também pode ser atualizada usando uma carga IPP (Internet Printing Protocol).</span><span class="sxs-lookup"><span data-stu-id="14303-179">With application permissions, a printer can also be updated using an Internet Printing Protocol (IPP) payload.</span></span> <span data-ttu-id="14303-180">Nesse caso, o corpo da solicitação contém um fluxo binário que representa o grupo Atributos da Impressora na [codificação IPP.](https://tools.ietf.org/html/rfc8010)</span><span class="sxs-lookup"><span data-stu-id="14303-180">In this case, the request body contains a binary stream that represents the Printer Attributes group in [IPP encoding](https://tools.ietf.org/html/rfc8010).</span></span>

<span data-ttu-id="14303-181">O cliente DEVE fornecer um conjunto de atributos printer com um ou mais valores (incluindo valores fora de banda explicitamente permitidos), conforme definido em Atributos de Descrição da Impressora [RFC8011 seção 5.2](https://tools.ietf.org/html/rfc8011#section-5.2) Atributos de Modelo de Trabalho ("xxx-default", "xxx-supported" e "xxx-ready"), Atributos de Descrição da Impressora da Seção [5.4](https://tools.ietf.org/html/rfc8011#section-5.4) e quaisquer extensões de atributo suportadas pela Impressora.</span><span class="sxs-lookup"><span data-stu-id="14303-181">The client MUST supply a set of Printer attributes with one or more values (including explicitly allowed out-of-band values) as defined in [RFC8011 section 5.2](https://tools.ietf.org/html/rfc8011#section-5.2) Job Template Attributes ("xxx-default", "xxx-supported", and "xxx-ready" attributes), [Section 5.4](https://tools.ietf.org/html/rfc8011#section-5.4) Printer Description Attributes, and any attribute extensions supported by the Printer.</span></span> <span data-ttu-id="14303-182">Os valores de cada atributo Printer fornecido substituem os valores do atributo Printer correspondente no objeto Printer de destino.</span><span class="sxs-lookup"><span data-stu-id="14303-182">The value(s) of each Printer attribute supplied replaces the value(s) of the corresponding Printer attribute on the target Printer object.</span></span> <span data-ttu-id="14303-183">Para atributos que podem ter vários valores (1setOf), todos os valores fornecidos pelo cliente substituem todos os valores do atributo de objeto Printer correspondente.</span><span class="sxs-lookup"><span data-stu-id="14303-183">For attributes that can have multiple values (1setOf), all values supplied by the client replace all values of the corresponding Printer object attribute.</span></span>

## <a name="response"></a><span data-ttu-id="14303-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="14303-184">Response</span></span>

### <a name="delegated-permissions-and-json-payload"></a><span data-ttu-id="14303-185">Permissões delegadas e carga JSON</span><span class="sxs-lookup"><span data-stu-id="14303-185">Delegated permissions and JSON payload</span></span>

<span data-ttu-id="14303-186">Se estiver usando permissões delegadas, se bem-sucedido, este método retornará um código de resposta e um objeto de impressora `200 OK` atualizado no corpo da resposta. [](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="14303-186">If using delegated permissions, if successful, this method returns a `200 OK` response code and an updated [printer](../resources/printer.md) object in the response body.</span></span>

### <a name="application-permissions-and-json-payload"></a><span data-ttu-id="14303-187">Permissões de aplicativo e carga JSON</span><span class="sxs-lookup"><span data-stu-id="14303-187">Application permissions and JSON payload</span></span>

<span data-ttu-id="14303-188">Se estiver usando permissões delegadas, se bem-sucedido, este método retornará um código de resposta e um objeto de impressora `200 OK` atualizado no corpo da resposta. [](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="14303-188">If using delegated permissions, if successful, this method returns a `200 OK` response code and an updated [printer](../resources/printer.md) object in the response body.</span></span>

### <a name="application-permissions-and-ipp-payload"></a><span data-ttu-id="14303-189">Permissões de aplicativo e carga IPP</span><span class="sxs-lookup"><span data-stu-id="14303-189">Application permissions and IPP payload</span></span>

<span data-ttu-id="14303-190">Se estiver usando permissões de aplicativo, se bem-sucedido, este método retornará `204 No content` o código de resposta.</span><span class="sxs-lookup"><span data-stu-id="14303-190">If using application permissions, if successful, this method returns `204 No content` response code.</span></span> <span data-ttu-id="14303-191">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="14303-191">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="14303-192">Exemplos</span><span class="sxs-lookup"><span data-stu-id="14303-192">Examples</span></span>

### <a name="request"></a><span data-ttu-id="14303-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14303-193">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_printer"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/print/printers/{printerId}
Content-Type: application/json
Content-length: 581

{
  "name": "PrinterName",
  "location": {
    "latitude": 1.1,
    "longitude": 2.2,
    "altitudeInMeters": 3
  }
}
```


### <a name="response"></a><span data-ttu-id="14303-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="14303-194">Response</span></span>
<span data-ttu-id="14303-195">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="14303-195">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printer"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers/$entity",
  "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
  "displayName": "PrinterName",
  "manufacturer": "PrinterManufacturer",
  "model": "PrinterModel",
  "isShared": true,
  "registeredDateTime": "2020-02-04T00:00:00.0000000Z",
  "isAcceptingJobs": true,
  "status": {
    "state": "idle",
    "details": [],
    "description": ""
  },
  "defaults": {
    "copiesPerJob":1,
    "contentType": "application/oxps",
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
```

