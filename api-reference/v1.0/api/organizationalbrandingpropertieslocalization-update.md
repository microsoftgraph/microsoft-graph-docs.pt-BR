---
title: Atualizar organizacionais localizadasproperties
description: Atualize as propriedades do objeto organizationalbrandingproperties para uma localização específica.
localization_priority: Normal
author: kexia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 0c38656b71c2fdc5b3832a106effecfe9970c811
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722502"
---
# <a name="update-localized-organizationalbrandingproperties"></a><span data-ttu-id="14050-103">Atualizar organizacionais localizadasproperties</span><span class="sxs-lookup"><span data-stu-id="14050-103">Update localized organizationalbrandingproperties</span></span>

<span data-ttu-id="14050-104">Atualize as propriedades do [objeto organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) para uma localização específica.</span><span class="sxs-lookup"><span data-stu-id="14050-104">Update the properties of the [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object for a specific localization.</span></span>

## <a name="permissions"></a><span data-ttu-id="14050-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="14050-105">Permissions</span></span>

<span data-ttu-id="14050-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14050-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="14050-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14050-108">Permission type</span></span>                        | <span data-ttu-id="14050-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="14050-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="14050-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14050-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="14050-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14050-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="14050-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14050-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14050-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14050-113">Not supported.</span></span> |
| <span data-ttu-id="14050-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="14050-114">Application</span></span>                            | <span data-ttu-id="14050-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14050-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="14050-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14050-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}/branding/localizations/{locale}/{property name}
PUT /organization/{id}/branding/localizations/{locale}/{property name}
```

## <a name="request-headers"></a><span data-ttu-id="14050-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14050-117">Request headers</span></span>

| <span data-ttu-id="14050-118">Nome</span><span class="sxs-lookup"><span data-stu-id="14050-118">Name</span></span>       | <span data-ttu-id="14050-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="14050-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="14050-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="14050-120">Authorization</span></span> | <span data-ttu-id="14050-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14050-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="14050-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="14050-123">Content-Type</span></span>  | <span data-ttu-id="14050-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14050-p103">application/json. Required.</span></span>  |
| <span data-ttu-id="14050-126">Content-Language</span><span class="sxs-lookup"><span data-stu-id="14050-126">Content-Language</span></span>  | <span data-ttu-id="14050-127">Localidade.</span><span class="sxs-lookup"><span data-stu-id="14050-127">Locale.</span></span> <span data-ttu-id="14050-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="14050-128">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="14050-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="14050-129">Request body</span></span>

<span data-ttu-id="14050-130">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="14050-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="14050-131">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="14050-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="14050-132">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="14050-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="14050-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14050-133">Property</span></span>     | <span data-ttu-id="14050-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="14050-134">Type</span></span>        | <span data-ttu-id="14050-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="14050-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="14050-136">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="14050-136">backgroundColor</span></span>|<span data-ttu-id="14050-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14050-137">String</span></span>|<span data-ttu-id="14050-138">Cor que aparecerá no lugar da imagem de plano de fundo em conexões de baixa largura de banda.</span><span class="sxs-lookup"><span data-stu-id="14050-138">Color that will appear in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="14050-139">A cor primária do logotipo da faixa ou da cor da sua organização é recomendada para ser usada aqui.</span><span class="sxs-lookup"><span data-stu-id="14050-139">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="14050-140">Especifique isso em hexadecimal (por exemplo, branco é #FFFFFF).</span><span class="sxs-lookup"><span data-stu-id="14050-140">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span>|
|<span data-ttu-id="14050-141">backgroundImage</span><span class="sxs-lookup"><span data-stu-id="14050-141">backgroundImage</span></span>|<span data-ttu-id="14050-142">Fluxo</span><span class="sxs-lookup"><span data-stu-id="14050-142">Stream</span></span>|<span data-ttu-id="14050-143">Imagem que aparece como o plano de fundo da página de logom.</span><span class="sxs-lookup"><span data-stu-id="14050-143">Image that appears as the background of the sign in page.</span></span> <span data-ttu-id="14050-144">.png ou .jpg não maior que 1920x1080 e menor que 300kb.</span><span class="sxs-lookup"><span data-stu-id="14050-144">.png or .jpg not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="14050-145">Uma imagem menor reduzirá os requisitos de largura de banda e tornará as cargas de página mais performant.</span><span class="sxs-lookup"><span data-stu-id="14050-145">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span>|
|<span data-ttu-id="14050-146">bannerLogo</span><span class="sxs-lookup"><span data-stu-id="14050-146">bannerLogo</span></span>|<span data-ttu-id="14050-147">Fluxo</span><span class="sxs-lookup"><span data-stu-id="14050-147">Stream</span></span>|<span data-ttu-id="14050-148">Uma versão em faixa do logotipo da sua empresa que aparece na página de entrada.</span><span class="sxs-lookup"><span data-stu-id="14050-148">A banner version of your company logo which appears appears on the sign-in page.</span></span> <span data-ttu-id="14050-149">.png ou .jpg não maior que 36x245px.</span><span class="sxs-lookup"><span data-stu-id="14050-149">.png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="14050-150">Recomendamos usar uma imagem transparente sem preenchimento ao redor do logotipo.</span><span class="sxs-lookup"><span data-stu-id="14050-150">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="14050-151">signInPageText</span><span class="sxs-lookup"><span data-stu-id="14050-151">signInPageText</span></span>|<span data-ttu-id="14050-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14050-152">String</span></span>|<span data-ttu-id="14050-153">Texto que aparece na parte inferior da caixa de login.</span><span class="sxs-lookup"><span data-stu-id="14050-153">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="14050-154">Você pode usar isso para comunicar informações adicionais, como o número de telefone para o seu help desk ou uma declaração legal.</span><span class="sxs-lookup"><span data-stu-id="14050-154">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="14050-155">Este texto deve ser Unicode e não exceder 1024 caracteres.</span><span class="sxs-lookup"><span data-stu-id="14050-155">This text must be Unicode and not exceed 1024 characters.</span></span>|
|<span data-ttu-id="14050-156">squareLogo</span><span class="sxs-lookup"><span data-stu-id="14050-156">squareLogo</span></span>|<span data-ttu-id="14050-157">Fluxo</span><span class="sxs-lookup"><span data-stu-id="14050-157">Stream</span></span>|<span data-ttu-id="14050-158">Versão quadrada do logotipo da sua empresa.</span><span class="sxs-lookup"><span data-stu-id="14050-158">Square version of your company logo.</span></span> <span data-ttu-id="14050-159">Isso aparece nas experiências OOBE (windows 10 out-of-box) e quando o Windows Autopilot está habilitado para implantação.</span><span class="sxs-lookup"><span data-stu-id="14050-159">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="14050-160">.png ou .jpg não maior do que 240x240px e no máximo 10kb de tamanho.</span><span class="sxs-lookup"><span data-stu-id="14050-160">.png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="14050-161">Recomendamos usar uma imagem transparente sem preenchimento ao redor do logotipo.</span><span class="sxs-lookup"><span data-stu-id="14050-161">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="14050-162">usernameHintText</span><span class="sxs-lookup"><span data-stu-id="14050-162">usernameHintText</span></span>|<span data-ttu-id="14050-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14050-163">String</span></span>|<span data-ttu-id="14050-164">Cadeia de caracteres que mostra como a dica na caixa de texto do nome de usuário na tela de entrada.</span><span class="sxs-lookup"><span data-stu-id="14050-164">String that shows as the hint in the username textbox on the sign in screen.</span></span> <span data-ttu-id="14050-165">Este texto deve ser Unicode, sem links ou código, e não pode exceder 64 caracteres.</span><span class="sxs-lookup"><span data-stu-id="14050-165">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span>|
|<span data-ttu-id="14050-166">id</span><span class="sxs-lookup"><span data-stu-id="14050-166">id</span></span>|<span data-ttu-id="14050-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14050-167">String</span></span>|<span data-ttu-id="14050-168">Localidade para atualizar a identidade visual para</span><span class="sxs-lookup"><span data-stu-id="14050-168">Locale to update branding for</span></span>|


## <a name="response"></a><span data-ttu-id="14050-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="14050-169">Response</span></span>

<span data-ttu-id="14050-170">Se tiver êxito, este método retornará um código de resposta `204 OK`.</span><span class="sxs-lookup"><span data-stu-id="14050-170">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="14050-171">Exemplos</span><span class="sxs-lookup"><span data-stu-id="14050-171">Examples</span></span>

### <a name="example-1-setting-bannerlogo-for-the-fr-localization-using-put"></a><span data-ttu-id="14050-172">Exemplo 1: **Configurando bannerLogo** para a localização fr usando PUT</span><span class="sxs-lookup"><span data-stu-id="14050-172">Example 1: Setting **bannerLogo** for the fr localization using PUT</span></span>

<span data-ttu-id="14050-173">A solicitação a seguir atualiza o logotipo da faixa para `fr` a localização.</span><span class="sxs-lookup"><span data-stu-id="14050-173">The following request updates the banner logo for the `fr` localization.</span></span> <span data-ttu-id="14050-174">Usando PUT, se a localização fr não existir, um `404 not found` erro será retornado.</span><span class="sxs-lookup"><span data-stu-id="14050-174">Using PUT, if the fr localization does not exist, a `404 not found` error is returned.</span></span> <span data-ttu-id="14050-175">Se a carga contiver uma propriedade ou um `id` header **content-Language** e eles não corresponderem `id` na URL, um `Bad Request` erro será retornado.</span><span class="sxs-lookup"><span data-stu-id="14050-175">If the payload contains an `id` property or **Content-Language** header, and they don't match `id` in URL, a `Bad Request` error is returned.</span></span>

#### <a name="request"></a><span data-ttu-id="14050-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14050-176">Request</span></span>

<span data-ttu-id="14050-177">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="14050-177">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PUT https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo
Content-Type: image/jpeg

<Image>
```

#### <a name="response"></a><span data-ttu-id="14050-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="14050-178">Response</span></span>

<span data-ttu-id="14050-179">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="14050-179">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-bannerlogo-for-the-fr-localization-using-patch"></a><span data-ttu-id="14050-180">Exemplo 2: Atualizar **bannerLogo** para a localização fr usando PATCH</span><span class="sxs-lookup"><span data-stu-id="14050-180">Example 2: Update **bannerLogo** for the fr localization using PATCH</span></span>

<span data-ttu-id="14050-181">A solicitação a seguir atualiza o logotipo da faixa para a localização fr.</span><span class="sxs-lookup"><span data-stu-id="14050-181">The following request updates the banner logo for the fr localization.</span></span>  <span data-ttu-id="14050-182">Usando PATCH, se a localização especificada ainda não existir, ela será criada e a propriedade será escrita nele.</span><span class="sxs-lookup"><span data-stu-id="14050-182">Using PATCH, if the specified localization does not already exist, it is created and the property is written to it.</span></span>

#### <a name="request"></a><span data-ttu-id="14050-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14050-183">Request</span></span>

<span data-ttu-id="14050-184">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="14050-184">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "signInPageText": "fr"
}
```

#### <a name="response"></a><span data-ttu-id="14050-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="14050-185">Response</span></span>
<span data-ttu-id="14050-186">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="14050-186">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-override-default-branding-value-with-a-blank-string"></a><span data-ttu-id="14050-187">Exemplo 3: Substituir o valor de identidade visual padrão por uma cadeia de caracteres em branco</span><span class="sxs-lookup"><span data-stu-id="14050-187">Example 3: Override default branding value with a blank string</span></span>

<span data-ttu-id="14050-188">Se o valor de uma propriedade em uma localização for nulo, o valor será herdado da identidade visual padrão.</span><span class="sxs-lookup"><span data-stu-id="14050-188">If the value of a property in a localization is null, the value will be inherited from the default branding.</span></span> <span data-ttu-id="14050-189">Para impedir que isso aconteça, de definir uma cadeia de caracteres ou cadeia de caracteres vazia que contenha apenas o espaço em branco na identidade visual localizada.</span><span class="sxs-lookup"><span data-stu-id="14050-189">To prevent this from happening, set an empty string or string containing only whitespace in the localized branding.</span></span>

#### <a name="request"></a><span data-ttu-id="14050-190">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14050-190">Request</span></span>

<span data-ttu-id="14050-191">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="14050-191">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
Content-Type: application/json

{
    "signInPageText": "French sign-in text.",
    "usernameHintText":" "
}
```

#### <a name="response"></a><span data-ttu-id="14050-192">Resposta</span><span class="sxs-lookup"><span data-stu-id="14050-192">Response</span></span>

<span data-ttu-id="14050-193">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="14050-193">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="14050-194">Após essa solicitação, usernameHintText para a localização fr estará vazio em vez de herdar o valor da identidade visual padrão.</span><span class="sxs-lookup"><span data-stu-id="14050-194">Following this request, usernameHintText for the fr localization will be empty instead of inheriting the value from default branding.</span></span>

### <a name="example-4-replace-french-localization-with-put"></a><span data-ttu-id="14050-195">Exemplo 4: Substitua a localização francesa por PUT</span><span class="sxs-lookup"><span data-stu-id="14050-195">Example 4: Replace French localization with PUT</span></span>

<span data-ttu-id="14050-196">Para fazer uma atualização sobre a localização usando PUT, devemos adicionar todas as propriedades no corpo juntamente com a propriedade que precisa ser atualizada à medida que PUT substitui o objeto existente pelo novo.</span><span class="sxs-lookup"><span data-stu-id="14050-196">To make an update on localization using PUT, we should add all properties in body along with the property that needs to be updated as PUT replaces existing object with the new one.</span></span> <span data-ttu-id="14050-197">As outras propriedades que não estão no corpo da carga de PUT serão definidas como NULL.</span><span class="sxs-lookup"><span data-stu-id="14050-197">The other properties which are not in the payload body of PUT will be set to NULL.</span></span> <span data-ttu-id="14050-198">Aqui no exemplo abaixo, somente a propriedade backgroundColor é mantida e signInPageText é atualizada enquanto outras são definidas como nulas.</span><span class="sxs-lookup"><span data-stu-id="14050-198">Here in example below, only backgroundColor property is retained and signInPageText is updated while others are set to null.</span></span>
<span data-ttu-id="14050-199">Se a localização especificada ainda não existir, PUT para a URL especificando que a localização a cria.</span><span class="sxs-lookup"><span data-stu-id="14050-199">If the specified localization does not already exist, PUT to the URL specifying that localization creates it.</span></span>
<span data-ttu-id="14050-200">Se a carga contiver uma propriedade ID ou um header content-Language e eles não corresponderem à ID na URL, lançaremos a solicitação Desa resposta.</span><span class="sxs-lookup"><span data-stu-id="14050-200">If the payload contains an id property or a Content-Language header, and they don't match id in URL, we throw Bad request.</span></span>

#### <a name="request"></a><span data-ttu-id="14050-201">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14050-201">Request</span></span>

<span data-ttu-id="14050-202">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="14050-202">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PUT https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "signInPageText": "fr"
}
```

#### <a name="response"></a><span data-ttu-id="14050-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="14050-203">Response</span></span>
<span data-ttu-id="14050-204">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="14050-204">The following is an example of the response.</span></span>

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
