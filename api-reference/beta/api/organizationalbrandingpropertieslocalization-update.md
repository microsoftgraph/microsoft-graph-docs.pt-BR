---
title: Atualizar organizationalbrandingproperties localizado
description: Atualize as propriedades do objeto organizationalbrandingproperties para uma localização específica.
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0b835316d611d3735a0a981fc77f58622ab89c9b
ms.sourcegitcommit: 40b0e58312819b69567f35ab894ee0d2989837ab
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/13/2020
ms.locfileid: "49031891"
---
# <a name="update-localized-organizationalbrandingproperties"></a><span data-ttu-id="cf37d-103">Atualizar organizationalbrandingproperties localizado</span><span class="sxs-lookup"><span data-stu-id="cf37d-103">Update Localized organizationalbrandingproperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf37d-104">Atualize as propriedades do objeto [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) para uma localização específica.</span><span class="sxs-lookup"><span data-stu-id="cf37d-104">Update the properties of the [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object for a specific localization.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf37d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="cf37d-105">Permissions</span></span>

<span data-ttu-id="cf37d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf37d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cf37d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf37d-108">Permission type</span></span>                        | <span data-ttu-id="cf37d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cf37d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cf37d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf37d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="cf37d-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf37d-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="cf37d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf37d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf37d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf37d-113">Not supported.</span></span> |
| <span data-ttu-id="cf37d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf37d-114">Application</span></span>                            | <span data-ttu-id="cf37d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf37d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf37d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf37d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}/branding/localizations/{locale}/{property name}
PUT /organization/{id}/branding/localizations/{locale}/{property name}
```

## <a name="request-headers"></a><span data-ttu-id="cf37d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf37d-117">Request headers</span></span>

| <span data-ttu-id="cf37d-118">Nome</span><span class="sxs-lookup"><span data-stu-id="cf37d-118">Name</span></span>       | <span data-ttu-id="cf37d-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf37d-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="cf37d-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf37d-120">Authorization</span></span> | <span data-ttu-id="cf37d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf37d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cf37d-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cf37d-123">Content-Type</span></span>  | <span data-ttu-id="cf37d-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf37d-p103">application/json. Required.</span></span>  |
| <span data-ttu-id="cf37d-126">Conteúdo-idioma</span><span class="sxs-lookup"><span data-stu-id="cf37d-126">Content-Language</span></span>  | <span data-ttu-id="cf37d-127">LCID.</span><span class="sxs-lookup"><span data-stu-id="cf37d-127">Locale.</span></span> <span data-ttu-id="cf37d-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="cf37d-128">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cf37d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf37d-129">Request body</span></span>

<span data-ttu-id="cf37d-130">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="cf37d-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="cf37d-131">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="cf37d-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="cf37d-132">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="cf37d-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="cf37d-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf37d-133">Property</span></span>     | <span data-ttu-id="cf37d-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf37d-134">Type</span></span>        | <span data-ttu-id="cf37d-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf37d-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cf37d-136">CorDoFundo</span><span class="sxs-lookup"><span data-stu-id="cf37d-136">backgroundColor</span></span>|<span data-ttu-id="cf37d-137">String</span><span class="sxs-lookup"><span data-stu-id="cf37d-137">String</span></span>|<span data-ttu-id="cf37d-138">Cor que aparecerá no lugar da imagem de plano de fundo em conexões de baixa largura de banda.</span><span class="sxs-lookup"><span data-stu-id="cf37d-138">Color that will appear in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="cf37d-139">É recomendável usar a cor principal do logotipo de faixa ou a cor da sua organização aqui.</span><span class="sxs-lookup"><span data-stu-id="cf37d-139">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="cf37d-140">Especifique isso em hexadecimal (por exemplo, branco é #FFFFFF).</span><span class="sxs-lookup"><span data-stu-id="cf37d-140">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span>|
|<span data-ttu-id="cf37d-141">backgroundImage</span><span class="sxs-lookup"><span data-stu-id="cf37d-141">backgroundImage</span></span>|<span data-ttu-id="cf37d-142">Fluxo</span><span class="sxs-lookup"><span data-stu-id="cf37d-142">Stream</span></span>|<span data-ttu-id="cf37d-143">Imagem que aparece como plano de fundo da página de entrada.</span><span class="sxs-lookup"><span data-stu-id="cf37d-143">Image that appears as the background of the sign in page.</span></span> <span data-ttu-id="cf37d-144">. png ou. jpg não é maior do que 1920 x 1080 e menor do que 300kb.</span><span class="sxs-lookup"><span data-stu-id="cf37d-144">.png or .jpg not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="cf37d-145">Uma imagem menor reduzirá os requisitos de largura de banda e fará com que as cargas de página mais tenham mais desempenho.</span><span class="sxs-lookup"><span data-stu-id="cf37d-145">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span>|
|<span data-ttu-id="cf37d-146">bannerLogo</span><span class="sxs-lookup"><span data-stu-id="cf37d-146">bannerLogo</span></span>|<span data-ttu-id="cf37d-147">Fluxo</span><span class="sxs-lookup"><span data-stu-id="cf37d-147">Stream</span></span>|<span data-ttu-id="cf37d-148">Uma versão de banner do logotipo da empresa que aparece aparece na página de entrada.</span><span class="sxs-lookup"><span data-stu-id="cf37d-148">A banner version of your company logo which appears appears on the sign-in page.</span></span> <span data-ttu-id="cf37d-149">. png ou. jpg não maior do que 36x245px.</span><span class="sxs-lookup"><span data-stu-id="cf37d-149">.png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="cf37d-150">Recomendamos usar uma imagem transparente sem preenchimento em torno do logotipo.</span><span class="sxs-lookup"><span data-stu-id="cf37d-150">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="cf37d-151">signInPageText</span><span class="sxs-lookup"><span data-stu-id="cf37d-151">signInPageText</span></span>|<span data-ttu-id="cf37d-152">String</span><span class="sxs-lookup"><span data-stu-id="cf37d-152">String</span></span>|<span data-ttu-id="cf37d-153">Texto que aparece na parte inferior da caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="cf37d-153">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="cf37d-154">Você pode usá-lo para comunicar informações adicionais, como o número de telefone para o suporte técnico ou uma instrução legal.</span><span class="sxs-lookup"><span data-stu-id="cf37d-154">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="cf37d-155">Este texto deve ser Unicode e não exceder 1024 caracteres.</span><span class="sxs-lookup"><span data-stu-id="cf37d-155">This text must be Unicode and not exceed 1024 characters.</span></span>|
|<span data-ttu-id="cf37d-156">squareLogo</span><span class="sxs-lookup"><span data-stu-id="cf37d-156">squareLogo</span></span>|<span data-ttu-id="cf37d-157">Fluxo</span><span class="sxs-lookup"><span data-stu-id="cf37d-157">Stream</span></span>|<span data-ttu-id="cf37d-158">Versão quadrada do logotipo da sua empresa.</span><span class="sxs-lookup"><span data-stu-id="cf37d-158">Square version of your company logo.</span></span> <span data-ttu-id="cf37d-159">Isso aparece nas experiências de uso (OOBE) do Windows 10 e quando o Windows AutoPilot está habilitado para implantação.</span><span class="sxs-lookup"><span data-stu-id="cf37d-159">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="cf37d-160">. png ou. jpg não maior do que 240x240px e não mais do que 10 KB em tamanho.</span><span class="sxs-lookup"><span data-stu-id="cf37d-160">.png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="cf37d-161">Recomendamos usar uma imagem transparente sem preenchimento em torno do logotipo.</span><span class="sxs-lookup"><span data-stu-id="cf37d-161">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="cf37d-162">usernameHintText</span><span class="sxs-lookup"><span data-stu-id="cf37d-162">usernameHintText</span></span>|<span data-ttu-id="cf37d-163">String</span><span class="sxs-lookup"><span data-stu-id="cf37d-163">String</span></span>|<span data-ttu-id="cf37d-164">Cadeia de caracteres que mostra como a dica na caixa de texto username na tela de entrada.</span><span class="sxs-lookup"><span data-stu-id="cf37d-164">String that shows as the hint in the username textbox on the sign in screen.</span></span> <span data-ttu-id="cf37d-165">Este texto deve ser Unicode, sem links ou código, e não pode exceder 64 caracteres.</span><span class="sxs-lookup"><span data-stu-id="cf37d-165">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span>|
|<span data-ttu-id="cf37d-166">id</span><span class="sxs-lookup"><span data-stu-id="cf37d-166">id</span></span>|<span data-ttu-id="cf37d-167">String</span><span class="sxs-lookup"><span data-stu-id="cf37d-167">String</span></span>|<span data-ttu-id="cf37d-168">Local para atualizar a identidade visual do</span><span class="sxs-lookup"><span data-stu-id="cf37d-168">Locale to update branding for</span></span>|


## <a name="response"></a><span data-ttu-id="cf37d-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf37d-169">Response</span></span>

<span data-ttu-id="cf37d-170">Se tiver êxito, este método retornará um código de resposta `204 OK`.</span><span class="sxs-lookup"><span data-stu-id="cf37d-170">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="cf37d-171">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cf37d-171">Examples</span></span>

### <a name="example-1-setting-bannerlogo-for-the-fr-localization-using-put"></a><span data-ttu-id="cf37d-172">Exemplo 1: Configurando **bannerLogo** para a localização fr usando put</span><span class="sxs-lookup"><span data-stu-id="cf37d-172">Example 1: Setting **bannerLogo** for the fr localization using PUT</span></span>

<span data-ttu-id="cf37d-173">A solicitação a seguir atualiza o logotipo do banner para a localização fr.</span><span class="sxs-lookup"><span data-stu-id="cf37d-173">The following request updates the banner logo for the fr localization.</span></span> <span data-ttu-id="cf37d-174">Usando PUT, se a localização fr não existir, "404 não encontrado" será retornado.</span><span class="sxs-lookup"><span data-stu-id="cf37d-174">Using PUT, if the fr localization does not exist, "404 not found" is returned.</span></span> <span data-ttu-id="cf37d-175">Se a carga contiver uma propriedade ID ou cabeçalho de linguagem de conteúdo e não corresponder à ID na URL, uma solicitação inválida será retornada.</span><span class="sxs-lookup"><span data-stu-id="cf37d-175">If the payload contains an id property or Content-Language header, and they don't match id in URL, a Bad Request is returned.</span></span>

#### <a name="request"></a><span data-ttu-id="cf37d-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf37d-176">Request</span></span>

<span data-ttu-id="cf37d-177">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf37d-177">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PUT https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo
Content-Type: image/jpeg

<Image>
```

#### <a name="response"></a><span data-ttu-id="cf37d-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf37d-178">Response</span></span>

<span data-ttu-id="cf37d-179">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cf37d-179">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 NO CONTENT
```

### <a name="example-2-update-bannerlogo-for-the-fr-localization-using-patch"></a><span data-ttu-id="cf37d-180">Exemplo 2: atualizar **bannerLogo** para a localização fr usando patch</span><span class="sxs-lookup"><span data-stu-id="cf37d-180">Example 2: Update **bannerLogo** for the fr localization using PATCH</span></span>

<span data-ttu-id="cf37d-181">A solicitação a seguir atualiza o logotipo do banner para a localização fr.</span><span class="sxs-lookup"><span data-stu-id="cf37d-181">The following request updates the banner logo for the fr localization.</span></span>  <span data-ttu-id="cf37d-182">Usando PATCH, se a localização especificada ainda não existir, ela será criada e a propriedade será gravada nela.</span><span class="sxs-lookup"><span data-stu-id="cf37d-182">Using PATCH, if the specified localization does not already exist, it is created and the property is written to it.</span></span>

#### <a name="request"></a><span data-ttu-id="cf37d-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf37d-183">Request</span></span>

<span data-ttu-id="cf37d-184">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf37d-184">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "signInPageText": "fr"
}
```

#### <a name="response"></a><span data-ttu-id="cf37d-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf37d-185">Response</span></span>
<span data-ttu-id="cf37d-186">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cf37d-186">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```



### <a name="example-3-override-default-branding-value-with-a-blank-string"></a><span data-ttu-id="cf37d-187">Exemplo 3: substituir o valor padrão de identidade visual por uma cadeia de caracteres em branco</span><span class="sxs-lookup"><span data-stu-id="cf37d-187">Example 3: Override default branding value with a blank string</span></span>

<span data-ttu-id="cf37d-188">Se o valor de uma propriedade em uma localização for nulo, o valor será herdado da identidade visual padrão.</span><span class="sxs-lookup"><span data-stu-id="cf37d-188">If the value of a property in a localization is null, the value will be inherited from the default branding.</span></span> <span data-ttu-id="cf37d-189">Para evitar que isso aconteça, defina uma cadeia de caracteres vazia ou uma cadeia de caracteres contendo apenas espaços em branco na identidade visual localizada.</span><span class="sxs-lookup"><span data-stu-id="cf37d-189">To prevent this from happening, set an empty string or string containing only whitespace in the localized branding.</span></span>

#### <a name="request"></a><span data-ttu-id="cf37d-190">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf37d-190">Request</span></span>

<span data-ttu-id="cf37d-191">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf37d-191">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
Content-Type: application/json

{
    "signInPageText": "French sign-in text.",
    "usernameHintText":" "
}
```

#### <a name="response"></a><span data-ttu-id="cf37d-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf37d-192">Response</span></span>

<span data-ttu-id="cf37d-193">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cf37d-193">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="cf37d-194">Após essa solicitação, usernameHintText para a localização fr estará vazia em vez de herdar o valor da identidade visual padrão.</span><span class="sxs-lookup"><span data-stu-id="cf37d-194">Following this request, usernameHintText for the fr localization will be empty instead of inheriting the value from default branding.</span></span>

### <a name="example-4-replace-french-localization-with-put"></a><span data-ttu-id="cf37d-195">Exemplo 4: substituir a localização em francês por PUT</span><span class="sxs-lookup"><span data-stu-id="cf37d-195">Example 4: Replace French localization with PUT</span></span>

<span data-ttu-id="cf37d-196">Para fazer uma atualização na localização usando PUT, devemos adicionar todas as propriedades no corpo junto com a propriedade que precisa ser atualizada conforme PUT substitui o objeto existente pelo novo.</span><span class="sxs-lookup"><span data-stu-id="cf37d-196">To make an update on localization using PUT, we should add all properties in body along with the property that needs to be updated as PUT replaces existing object with the new one.</span></span> <span data-ttu-id="cf37d-197">As outras propriedades que não estão no corpo de carga de PUT serão definidas como NULL.</span><span class="sxs-lookup"><span data-stu-id="cf37d-197">The other properties which are not in the payload body of PUT will be set to NULL.</span></span> <span data-ttu-id="cf37d-198">Aqui, no exemplo abaixo, somente a propriedade backgroundColor é mantida e o signInPageText é atualizado enquanto outros são definidos como NULL.</span><span class="sxs-lookup"><span data-stu-id="cf37d-198">Here in example below, only backgroundColor property is retained and signInPageText is updated while others are set to null.</span></span>
<span data-ttu-id="cf37d-199">Se a localização especificada ainda não existir, coloque na URL especificando que a localização a cria.</span><span class="sxs-lookup"><span data-stu-id="cf37d-199">If the specified localization does not already exist, PUT to the URL specifying that localization creates it.</span></span>
<span data-ttu-id="cf37d-200">Se a carga contiver uma propriedade ID ou um cabeçalho de idioma de conteúdo e não corresponder à ID na URL, lançamos uma solicitação incorreta.</span><span class="sxs-lookup"><span data-stu-id="cf37d-200">If the payload contains an id property or a Content-Language header, and they don't match id in URL, we throw Bad request.</span></span>

#### <a name="request"></a><span data-ttu-id="cf37d-201">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf37d-201">Request</span></span>

<span data-ttu-id="cf37d-202">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf37d-202">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PUT https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "signInPageText": "fr"
}
```

#### <a name="response"></a><span data-ttu-id="cf37d-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf37d-203">Response</span></span>
<span data-ttu-id="cf37d-204">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cf37d-204">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organizationalbrandingproperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->