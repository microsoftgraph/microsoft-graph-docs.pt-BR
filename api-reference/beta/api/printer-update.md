---
title: Atualização da impressora
description: Atualize as propriedades de um objeto printer.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 2a0d40490365a2974a83683f7b9564063f8e25c0
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766221"
---
# <a name="update-printer"></a><span data-ttu-id="b0d5e-103">Atualização da impressora</span><span class="sxs-lookup"><span data-stu-id="b0d5e-103">Update printer</span></span>

<span data-ttu-id="b0d5e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0d5e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b0d5e-105">Atualize as propriedades de um [objeto printer.](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="b0d5e-105">Update the properties of a [printer](../resources/printer.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b0d5e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b0d5e-106">Permissions</span></span>
<span data-ttu-id="b0d5e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0d5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="b0d5e-109">Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.</span><span class="sxs-lookup"><span data-stu-id="b0d5e-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="b0d5e-110">O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="b0d5e-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

<span data-ttu-id="b0d5e-111">Somente o aplicativo que registrou a impressora tem permissão para atualizar a impressora usando permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b0d5e-111">Only the app that registered the printer is allowed to update the printer using application permissions.</span></span>

|<span data-ttu-id="b0d5e-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0d5e-112">Permission type</span></span> | <span data-ttu-id="b0d5e-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b0d5e-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="b0d5e-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0d5e-114">Delegated (work or school account)</span></span>| <span data-ttu-id="b0d5e-115">Printer.ReadWrite.All, Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="b0d5e-115">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="b0d5e-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b0d5e-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0d5e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0d5e-117">Not Supported.</span></span>|
|<span data-ttu-id="b0d5e-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0d5e-118">Application</span></span>| <span data-ttu-id="b0d5e-119">Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0d5e-119">Printer.ReadWrite.All</span></span> |

><span data-ttu-id="b0d5e-120">**Observação:** No momento, somente as impressoras que não têm dispositivo físico podem ser atualizadas usando permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b0d5e-120">**Note:** Right now, only printers that don't have physical device can be updated using application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="b0d5e-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b0d5e-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/printers/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b0d5e-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b0d5e-122">Request headers</span></span>
| <span data-ttu-id="b0d5e-123">Nome</span><span class="sxs-lookup"><span data-stu-id="b0d5e-123">Name</span></span>       | <span data-ttu-id="b0d5e-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0d5e-124">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b0d5e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b0d5e-125">Authorization</span></span> | <span data-ttu-id="b0d5e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0d5e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b0d5e-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="b0d5e-128">Content-type</span></span>  | <span data-ttu-id="b0d5e-129">`application/json` ao usar permissões delegadas `application/ipp` ou ao usar permissões de `application/json` aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b0d5e-129">`application/json` when using delegated permissions, `application/ipp` or `application/json` when using application permissions.</span></span> <span data-ttu-id="b0d5e-130">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0d5e-130">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0d5e-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b0d5e-131">Request body</span></span>

### <a name="delegated-permissions-and-json-payload"></a><span data-ttu-id="b0d5e-132">Permissões delegadas e carga JSON</span><span class="sxs-lookup"><span data-stu-id="b0d5e-132">Delegated permissions and JSON payload</span></span>

<span data-ttu-id="b0d5e-133">Se estiver usando permissões delegadas, no corpo da solicitação, forneça os valores para os campos de [impressora relevantes](../resources/printer.md) que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="b0d5e-133">If using delegated permissions, in the request body, supply the values for the relevant [printer](../resources/printer.md) fields that should be updated.</span></span> <span data-ttu-id="b0d5e-134">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="b0d5e-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b0d5e-135">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="b0d5e-135">For best performance, don't include existing values that haven't changed.</span></span> 

<span data-ttu-id="b0d5e-136">As propriedades a seguir podem ser atualizadas usando permissões delegadas.</span><span class="sxs-lookup"><span data-stu-id="b0d5e-136">The following properties can be updated using delegated permissions.</span></span>

| <span data-ttu-id="b0d5e-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0d5e-137">Property</span></span>     | <span data-ttu-id="b0d5e-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0d5e-138">Type</span></span>        | <span data-ttu-id="b0d5e-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0d5e-139">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b0d5e-140">defaults</span><span class="sxs-lookup"><span data-stu-id="b0d5e-140">defaults</span></span>|[<span data-ttu-id="b0d5e-141">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="b0d5e-141">printerDefaults</span></span>](../resources/printerdefaults.md)|<span data-ttu-id="b0d5e-142">As configurações de impressão padrão da impressora.</span><span class="sxs-lookup"><span data-stu-id="b0d5e-142">The printer's default print settings.</span></span>|
|<span data-ttu-id="b0d5e-143">localização</span><span class="sxs-lookup"><span data-stu-id="b0d5e-143">location</span></span>|[<span data-ttu-id="b0d5e-144">printerLocation</span><span class="sxs-lookup"><span data-stu-id="b0d5e-144">printerLocation</span></span>](../resources/printerlocation.md)|<span data-ttu-id="b0d5e-145">O local físico e/ou organizacional da impressora.</span><span class="sxs-lookup"><span data-stu-id="b0d5e-145">The physical and/or organizational location of the printer.</span></span>|
|<span data-ttu-id="b0d5e-146">displayName</span><span class="sxs-lookup"><span data-stu-id="b0d5e-146">displayName</span></span>|<span data-ttu-id="b0d5e-147">String</span><span class="sxs-lookup"><span data-stu-id="b0d5e-147">String</span></span>|<span data-ttu-id="b0d5e-148">O nome da impressora.</span><span class="sxs-lookup"><span data-stu-id="b0d5e-148">The name of the printer.</span></span>|

### <a name="application-permissions-and-json-payload"></a><span data-ttu-id="b0d5e-149">Permissões de aplicativo e carga JSON</span><span class="sxs-lookup"><span data-stu-id="b0d5e-149">Application permissions and JSON payload</span></span>
<span data-ttu-id="b0d5e-150">No corpo da solicitação, fornece os valores para os campos de [impressora relevantes](../resources/printer.md) que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="b0d5e-150">In the request body, supply the values for the relevant [printer](../resources/printer.md) fields that should be updated.</span></span> <span data-ttu-id="b0d5e-151">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="b0d5e-151">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b0d5e-152">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="b0d5e-152">For best performance, don't include existing values that haven't changed.</span></span> 

<span data-ttu-id="b0d5e-153">As propriedades a seguir podem ser atualizadas usando permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b0d5e-153">The following properties can be updated using application permissions.</span></span>

| <span data-ttu-id="b0d5e-154">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0d5e-154">Property</span></span>     | <span data-ttu-id="b0d5e-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0d5e-155">Type</span></span>        | <span data-ttu-id="b0d5e-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0d5e-156">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b0d5e-157">defaults</span><span class="sxs-lookup"><span data-stu-id="b0d5e-157">defaults</span></span>|[<span data-ttu-id="b0d5e-158">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="b0d5e-158">printerDefaults</span></span>](../resources/printerdefaults.md)|<span data-ttu-id="b0d5e-159">As configurações de impressão padrão da impressora.</span><span class="sxs-lookup"><span data-stu-id="b0d5e-159">The printer's default print settings.</span></span>|
|<span data-ttu-id="b0d5e-160">capabilities</span><span class="sxs-lookup"><span data-stu-id="b0d5e-160">capabilities</span></span>|[<span data-ttu-id="b0d5e-161">printerCapabilities</span><span class="sxs-lookup"><span data-stu-id="b0d5e-161">printerCapabilities</span></span>](../resources/printerCapabilities.md)|<span data-ttu-id="b0d5e-162">Os recursos da impressora associados a esse compartilhamento de impressora.</span><span class="sxs-lookup"><span data-stu-id="b0d5e-162">The capabilities of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="b0d5e-163">displayName</span><span class="sxs-lookup"><span data-stu-id="b0d5e-163">displayName</span></span>|<span data-ttu-id="b0d5e-164">String</span><span class="sxs-lookup"><span data-stu-id="b0d5e-164">String</span></span>|<span data-ttu-id="b0d5e-165">O nome da impressora.</span><span class="sxs-lookup"><span data-stu-id="b0d5e-165">The name of the printer.</span></span>|
|<span data-ttu-id="b0d5e-166">fabricante</span><span class="sxs-lookup"><span data-stu-id="b0d5e-166">manufacturer</span></span>|<span data-ttu-id="b0d5e-167">String</span><span class="sxs-lookup"><span data-stu-id="b0d5e-167">String</span></span>|<span data-ttu-id="b0d5e-168">O fabricante da impressora.</span><span class="sxs-lookup"><span data-stu-id="b0d5e-168">The manufacturer of the printer.</span></span>|
|<span data-ttu-id="b0d5e-169">modelo</span><span class="sxs-lookup"><span data-stu-id="b0d5e-169">model</span></span>|<span data-ttu-id="b0d5e-170">String</span><span class="sxs-lookup"><span data-stu-id="b0d5e-170">String</span></span>|<span data-ttu-id="b0d5e-171">O nome do modelo da impressora.</span><span class="sxs-lookup"><span data-stu-id="b0d5e-171">The model name of the printer.</span></span>|
|<span data-ttu-id="b0d5e-172">status</span><span class="sxs-lookup"><span data-stu-id="b0d5e-172">status</span></span>|[<span data-ttu-id="b0d5e-173">printerStatus</span><span class="sxs-lookup"><span data-stu-id="b0d5e-173">printerStatus</span></span>](../resources/printerstatus.md)|<span data-ttu-id="b0d5e-174">O status de processamento da impressora, incluindo quaisquer erros.</span><span class="sxs-lookup"><span data-stu-id="b0d5e-174">The processing status of the printer, including any errors.</span></span>|
|<span data-ttu-id="b0d5e-175">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="b0d5e-175">isAcceptingJobs</span></span>|<span data-ttu-id="b0d5e-176">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0d5e-176">Boolean</span></span>|<span data-ttu-id="b0d5e-177">Se a impressora está aceitando novos trabalhos de impressão no momento.</span><span class="sxs-lookup"><span data-stu-id="b0d5e-177">Whether the printer is currently accepting new print jobs.</span></span>|

### <a name="application-permissions-and-ipp-payload"></a><span data-ttu-id="b0d5e-178">Permissões de aplicativo e carga IPP</span><span class="sxs-lookup"><span data-stu-id="b0d5e-178">Application permissions and IPP payload</span></span>

<span data-ttu-id="b0d5e-179">Com permissões de aplicativo, uma impressora também pode ser atualizada usando uma carga IPP (Internet Printing Protocol).</span><span class="sxs-lookup"><span data-stu-id="b0d5e-179">With application permissions, a printer can also be updated using an Internet Printing Protocol (IPP) payload.</span></span> <span data-ttu-id="b0d5e-180">Nesse caso, o corpo da solicitação contém um fluxo binário que representa o grupo Atributos da Impressora na [codificação IPP.](https://tools.ietf.org/html/rfc8010)</span><span class="sxs-lookup"><span data-stu-id="b0d5e-180">In this case, the request body contains a binary stream that represents the Printer Attributes group in [IPP encoding](https://tools.ietf.org/html/rfc8010).</span></span>

<span data-ttu-id="b0d5e-181">O cliente DEVE fornecer um conjunto de atributos printer com um ou mais valores (incluindo valores fora de banda explicitamente permitidos), conforme definido em Atributos de Descrição da Impressora [RFC8011 seção 5.2](https://tools.ietf.org/html/rfc8011#section-5.2) Atributos de Modelo de Trabalho ("xxx-default", "xxx-supported" e "xxx-ready"), Atributos de Descrição da Impressora da Seção [5.4](https://tools.ietf.org/html/rfc8011#section-5.4) e quaisquer extensões de atributo suportadas pela Impressora.</span><span class="sxs-lookup"><span data-stu-id="b0d5e-181">The client MUST supply a set of Printer attributes with one or more values (including explicitly allowed out-of-band values) as defined in [RFC8011 section 5.2](https://tools.ietf.org/html/rfc8011#section-5.2) Job Template Attributes ("xxx-default", "xxx-supported", and "xxx-ready" attributes), [Section 5.4](https://tools.ietf.org/html/rfc8011#section-5.4) Printer Description Attributes, and any attribute extensions supported by the Printer.</span></span> <span data-ttu-id="b0d5e-182">Os valores de cada atributo Printer fornecido substituem os valores do atributo Printer correspondente no objeto Printer de destino.</span><span class="sxs-lookup"><span data-stu-id="b0d5e-182">The value(s) of each Printer attribute supplied replaces the value(s) of the corresponding Printer attribute on the target Printer object.</span></span> <span data-ttu-id="b0d5e-183">Para atributos que podem ter vários valores (1setOf), todos os valores fornecidos pelo cliente substituem todos os valores do atributo de objeto Printer correspondente.</span><span class="sxs-lookup"><span data-stu-id="b0d5e-183">For attributes that can have multiple values (1setOf), all values supplied by the client replace all values of the corresponding Printer object attribute.</span></span>

> <span data-ttu-id="b0d5e-184">**Observação:** Não passe atributos de operação no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0d5e-184">**Note:** Do not pass operation attributes in the request body.</span></span> <span data-ttu-id="b0d5e-185">O corpo da solicitação deve conter apenas atributos de impressora.</span><span class="sxs-lookup"><span data-stu-id="b0d5e-185">The request body should only contain printer attributes.</span></span>


> <span data-ttu-id="b0d5e-186">**Observação:** Para que as impressoras funcionem com uma plataforma específica, ela deve atender aos requisitos dessa plataforma.</span><span class="sxs-lookup"><span data-stu-id="b0d5e-186">**Note:** For printers to work with a particular platform, it should meet the requirements of that platform.</span></span> <span data-ttu-id="b0d5e-187">Por exemplo, no cliente windows, é esperado que a impressora especifique todos os atributos considerados obrigatórios de acordo com as especificações [MOPRIA.](https://mopria.org)</span><span class="sxs-lookup"><span data-stu-id="b0d5e-187">For example, on windows client, it is expected that printer specifies all attributes that are considered mandatory as per [MOPRIA](https://mopria.org) specs.</span></span> <span data-ttu-id="b0d5e-188">Observe que as especificações MOPRIA estão disponíveis apenas para os membros pagos da MOPRIA.</span><span class="sxs-lookup"><span data-stu-id="b0d5e-188">Please note MOPRIA specs are available to only the paid members of MOPRIA.</span></span>

## <a name="response"></a><span data-ttu-id="b0d5e-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0d5e-189">Response</span></span>

### <a name="delegated-permissions-and-json-payload"></a><span data-ttu-id="b0d5e-190">Permissões delegadas e carga JSON</span><span class="sxs-lookup"><span data-stu-id="b0d5e-190">Delegated permissions and JSON payload</span></span>

<span data-ttu-id="b0d5e-191">Se estiver usando permissões delegadas, se bem-sucedido, este método retornará um código de resposta e um objeto de impressora `200 OK` atualizado no corpo da resposta. [](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="b0d5e-191">If using delegated permissions, if successful, this method returns a `200 OK` response code and an updated [printer](../resources/printer.md) object in the response body.</span></span>

### <a name="application-permissions-and-json-payload"></a><span data-ttu-id="b0d5e-192">Permissões de aplicativo e carga JSON</span><span class="sxs-lookup"><span data-stu-id="b0d5e-192">Application permissions and JSON payload</span></span>

<span data-ttu-id="b0d5e-193">Se estiver usando permissões delegadas, se bem-sucedido, este método retornará um código de resposta e um objeto de impressora `200 OK` atualizado no corpo da resposta. [](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="b0d5e-193">If using delegated permissions, if successful, this method returns a `200 OK` response code and an updated [printer](../resources/printer.md) object in the response body.</span></span>

### <a name="application-permissions-and-ipp-payload"></a><span data-ttu-id="b0d5e-194">Permissões de aplicativo e carga IPP</span><span class="sxs-lookup"><span data-stu-id="b0d5e-194">Application permissions and IPP payload</span></span>

<span data-ttu-id="b0d5e-195">Se estiver usando permissões de aplicativo, se bem-sucedido, este método retornará `204 No content` o código de resposta.</span><span class="sxs-lookup"><span data-stu-id="b0d5e-195">If using application permissions, if successful, this method returns `204 No content` response code.</span></span> <span data-ttu-id="b0d5e-196">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0d5e-196">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0d5e-197">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b0d5e-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0d5e-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0d5e-198">Request</span></span>
<span data-ttu-id="b0d5e-199">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0d5e-199">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b0d5e-200">HTTP</span><span class="sxs-lookup"><span data-stu-id="b0d5e-200">HTTP</span></span>](#tab/http)
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

---

### <a name="response"></a><span data-ttu-id="b0d5e-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0d5e-201">Response</span></span>
<span data-ttu-id="b0d5e-202">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b0d5e-202">The following is an example of the response.</span></span>
><span data-ttu-id="b0d5e-p112">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b0d5e-p112">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update printer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
