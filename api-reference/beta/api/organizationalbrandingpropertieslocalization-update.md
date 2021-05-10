---
title: Atualizar organizacionais localizadasproperties
description: Atualize as propriedades do objeto organizationalbrandingproperties para uma localização específica.
localization_priority: Normal
author: almars
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 693d42f81b5115b9b818e8495e320e127cd66262
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52298502"
---
# <a name="update-localized-organizationalbrandingproperties"></a><span data-ttu-id="282a7-103">Atualizar organizacionais de marca organizacional localizadas</span><span class="sxs-lookup"><span data-stu-id="282a7-103">Update Localized organizationalbrandingproperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="282a7-104">Atualize as propriedades do [objeto organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) para uma localização específica.</span><span class="sxs-lookup"><span data-stu-id="282a7-104">Update the properties of the [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object for a specific localization.</span></span>

## <a name="permissions"></a><span data-ttu-id="282a7-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="282a7-105">Permissions</span></span>

<span data-ttu-id="282a7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="282a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="282a7-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="282a7-108">Permission type</span></span>                        | <span data-ttu-id="282a7-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="282a7-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="282a7-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="282a7-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="282a7-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="282a7-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="282a7-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="282a7-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="282a7-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="282a7-113">Not supported.</span></span> |
| <span data-ttu-id="282a7-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="282a7-114">Application</span></span>                            | <span data-ttu-id="282a7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="282a7-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="282a7-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="282a7-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{tenant id}/branding/localizations/{locale}
PUT /organization/{tenant id}/branding/localizations/{locale}
```

## <a name="request-headers"></a><span data-ttu-id="282a7-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="282a7-117">Request headers</span></span>

| <span data-ttu-id="282a7-118">Nome</span><span class="sxs-lookup"><span data-stu-id="282a7-118">Name</span></span>       | <span data-ttu-id="282a7-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="282a7-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="282a7-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="282a7-120">Authorization</span></span> | <span data-ttu-id="282a7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="282a7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="282a7-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="282a7-123">Content-Type</span></span>  | <span data-ttu-id="282a7-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="282a7-p103">application/json. Required.</span></span>  |
| <span data-ttu-id="282a7-126">Content-Language</span><span class="sxs-lookup"><span data-stu-id="282a7-126">Content-Language</span></span>  | <span data-ttu-id="282a7-127">Localidade.</span><span class="sxs-lookup"><span data-stu-id="282a7-127">Locale.</span></span> <span data-ttu-id="282a7-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="282a7-128">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="282a7-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="282a7-129">Request body</span></span>

<span data-ttu-id="282a7-130">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="282a7-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="282a7-131">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="282a7-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="282a7-132">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="282a7-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="282a7-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="282a7-133">Property</span></span>     | <span data-ttu-id="282a7-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="282a7-134">Type</span></span>        | <span data-ttu-id="282a7-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="282a7-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="282a7-136">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="282a7-136">backgroundColor</span></span>|<span data-ttu-id="282a7-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="282a7-137">String</span></span>|<span data-ttu-id="282a7-138">Cor que aparecerá no lugar da imagem de plano de fundo em conexões de baixa largura de banda.</span><span class="sxs-lookup"><span data-stu-id="282a7-138">Color that will appear in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="282a7-139">A cor primária do logotipo da faixa ou da cor da sua organização é recomendada para ser usada aqui.</span><span class="sxs-lookup"><span data-stu-id="282a7-139">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="282a7-140">Especifique isso em hexadecimal (por exemplo, branco é #FFFFFF).</span><span class="sxs-lookup"><span data-stu-id="282a7-140">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span>|
|<span data-ttu-id="282a7-141">backgroundImage</span><span class="sxs-lookup"><span data-stu-id="282a7-141">backgroundImage</span></span>|<span data-ttu-id="282a7-142">Stream</span><span class="sxs-lookup"><span data-stu-id="282a7-142">Stream</span></span>|<span data-ttu-id="282a7-143">Imagem que aparece como o plano de fundo da página de logom.</span><span class="sxs-lookup"><span data-stu-id="282a7-143">Image that appears as the background of the sign in page.</span></span> <span data-ttu-id="282a7-144">.png ou .jpg maior que 1920x1080 e menor que 300kb.</span><span class="sxs-lookup"><span data-stu-id="282a7-144">.png or .jpg not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="282a7-145">Uma imagem menor reduzirá os requisitos de largura de banda e tornará as cargas de página mais performant.</span><span class="sxs-lookup"><span data-stu-id="282a7-145">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span>|
|<span data-ttu-id="282a7-146">bannerLogo</span><span class="sxs-lookup"><span data-stu-id="282a7-146">bannerLogo</span></span>|<span data-ttu-id="282a7-147">Stream</span><span class="sxs-lookup"><span data-stu-id="282a7-147">Stream</span></span>|<span data-ttu-id="282a7-148">Uma versão em faixa do logotipo da sua empresa que aparece na página de entrada.</span><span class="sxs-lookup"><span data-stu-id="282a7-148">A banner version of your company logo which appears appears on the sign-in page.</span></span> <span data-ttu-id="282a7-149">.png ou .jpg maior que 36x245px.</span><span class="sxs-lookup"><span data-stu-id="282a7-149">.png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="282a7-150">Recomendamos usar uma imagem transparente sem preenchimento ao redor do logotipo.</span><span class="sxs-lookup"><span data-stu-id="282a7-150">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="282a7-151">signInPageText</span><span class="sxs-lookup"><span data-stu-id="282a7-151">signInPageText</span></span>|<span data-ttu-id="282a7-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="282a7-152">String</span></span>|<span data-ttu-id="282a7-153">Texto que aparece na parte inferior da caixa de login.</span><span class="sxs-lookup"><span data-stu-id="282a7-153">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="282a7-154">Você pode usar isso para comunicar informações adicionais, como o número de telefone para o seu help desk ou uma declaração legal.</span><span class="sxs-lookup"><span data-stu-id="282a7-154">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="282a7-155">Este texto deve ser Unicode e não exceder 1024 caracteres.</span><span class="sxs-lookup"><span data-stu-id="282a7-155">This text must be Unicode and not exceed 1024 characters.</span></span>|
|<span data-ttu-id="282a7-156">squareLogo</span><span class="sxs-lookup"><span data-stu-id="282a7-156">squareLogo</span></span>|<span data-ttu-id="282a7-157">Stream</span><span class="sxs-lookup"><span data-stu-id="282a7-157">Stream</span></span>|<span data-ttu-id="282a7-158">Versão quadrada do logotipo da sua empresa.</span><span class="sxs-lookup"><span data-stu-id="282a7-158">Square version of your company logo.</span></span> <span data-ttu-id="282a7-159">Isso aparece em Windows 10 experiências OOBE (out-of-box) e quando Windows Autopilot está habilitado para implantação.</span><span class="sxs-lookup"><span data-stu-id="282a7-159">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="282a7-160">.png ou .jpg maior que 240x240px e não mais de 10kb de tamanho.</span><span class="sxs-lookup"><span data-stu-id="282a7-160">.png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="282a7-161">Recomendamos usar uma imagem transparente sem preenchimento ao redor do logotipo.</span><span class="sxs-lookup"><span data-stu-id="282a7-161">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="282a7-162">usernameHintText</span><span class="sxs-lookup"><span data-stu-id="282a7-162">usernameHintText</span></span>|<span data-ttu-id="282a7-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="282a7-163">String</span></span>|<span data-ttu-id="282a7-164">Cadeia de caracteres que mostra como a dica na caixa de texto do nome de usuário na tela de entrada.</span><span class="sxs-lookup"><span data-stu-id="282a7-164">String that shows as the hint in the username textbox on the sign in screen.</span></span> <span data-ttu-id="282a7-165">Este texto deve ser Unicode, sem links ou código, e não pode exceder 64 caracteres.</span><span class="sxs-lookup"><span data-stu-id="282a7-165">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span>|
|<span data-ttu-id="282a7-166">id</span><span class="sxs-lookup"><span data-stu-id="282a7-166">id</span></span>|<span data-ttu-id="282a7-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="282a7-167">String</span></span>|<span data-ttu-id="282a7-168">Localidade para atualizar a identidade visual para</span><span class="sxs-lookup"><span data-stu-id="282a7-168">Locale to update branding for</span></span>|


## <a name="response"></a><span data-ttu-id="282a7-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="282a7-169">Response</span></span>

<span data-ttu-id="282a7-170">Se tiver êxito, este método retornará um código de resposta `204 OK`.</span><span class="sxs-lookup"><span data-stu-id="282a7-170">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="282a7-171">Exemplos</span><span class="sxs-lookup"><span data-stu-id="282a7-171">Examples</span></span>

### <a name="example-1-setting-bannerlogo-for-the-fr-localization-using-put"></a><span data-ttu-id="282a7-172">Exemplo 1: **Configurando bannerLogo** para a localização fr usando PUT</span><span class="sxs-lookup"><span data-stu-id="282a7-172">Example 1: Setting **bannerLogo** for the fr localization using PUT</span></span>

<span data-ttu-id="282a7-173">A solicitação a seguir atualiza o logotipo da faixa para a localização fr.</span><span class="sxs-lookup"><span data-stu-id="282a7-173">The following request updates the banner logo for the fr localization.</span></span> <span data-ttu-id="282a7-174">Usando PUT, se a localização fr não existir, "404 não encontrado" será retornado.</span><span class="sxs-lookup"><span data-stu-id="282a7-174">Using PUT, if the fr localization does not exist, "404 not found" is returned.</span></span> <span data-ttu-id="282a7-175">Se a carga contiver uma propriedade id ou um header content-Language e eles não corresponderem à ID na URL, uma Solicitação Ruim será retornada.</span><span class="sxs-lookup"><span data-stu-id="282a7-175">If the payload contains an id property or Content-Language header, and they don't match id in URL, a Bad Request is returned.</span></span>

#### <a name="request"></a><span data-ttu-id="282a7-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="282a7-176">Request</span></span>

<span data-ttu-id="282a7-177">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="282a7-177">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="282a7-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="282a7-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties_5"
}-->

```http
PUT https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo
Content-Type: image/jpeg

<Image>
```
# <a name="c"></a>[<span data-ttu-id="282a7-179">C#</span><span class="sxs-lookup"><span data-stu-id="282a7-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandingproperties-5-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="282a7-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="282a7-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandingproperties-5-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="282a7-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="282a7-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="282a7-182">Java</span><span class="sxs-lookup"><span data-stu-id="282a7-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandingproperties-5-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="282a7-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="282a7-183">Response</span></span>

<span data-ttu-id="282a7-184">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="282a7-184">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 NO CONTENT
```

### <a name="example-2-update-bannerlogo-for-the-fr-localization-using-patch"></a><span data-ttu-id="282a7-185">Exemplo 2: Atualizar **bannerLogo** para a localização fr usando PATCH</span><span class="sxs-lookup"><span data-stu-id="282a7-185">Example 2: Update **bannerLogo** for the fr localization using PATCH</span></span>

<span data-ttu-id="282a7-186">A solicitação a seguir atualiza o logotipo da faixa para a localização fr.</span><span class="sxs-lookup"><span data-stu-id="282a7-186">The following request updates the banner logo for the fr localization.</span></span>  <span data-ttu-id="282a7-187">Usando PATCH, se a localização especificada ainda não existir, ela será criada e a propriedade será escrita nele.</span><span class="sxs-lookup"><span data-stu-id="282a7-187">Using PATCH, if the specified localization does not already exist, it is created and the property is written to it.</span></span>

#### <a name="request"></a><span data-ttu-id="282a7-188">Solicitação</span><span class="sxs-lookup"><span data-stu-id="282a7-188">Request</span></span>

<span data-ttu-id="282a7-189">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="282a7-189">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="282a7-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="282a7-190">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties_6"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "signInPageText": "fr"
}
```
# <a name="c"></a>[<span data-ttu-id="282a7-191">C#</span><span class="sxs-lookup"><span data-stu-id="282a7-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandingproperties-6-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="282a7-192">JavaScript</span><span class="sxs-lookup"><span data-stu-id="282a7-192">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandingproperties-6-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="282a7-193">Objective-C</span><span class="sxs-lookup"><span data-stu-id="282a7-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandingproperties-6-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="282a7-194">Java</span><span class="sxs-lookup"><span data-stu-id="282a7-194">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandingproperties-6-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="282a7-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="282a7-195">Response</span></span>
<span data-ttu-id="282a7-196">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="282a7-196">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```



### <a name="example-3-override-default-branding-value-with-a-blank-string"></a><span data-ttu-id="282a7-197">Exemplo 3: Substituir o valor de identidade visual padrão por uma cadeia de caracteres em branco</span><span class="sxs-lookup"><span data-stu-id="282a7-197">Example 3: Override default branding value with a blank string</span></span>

<span data-ttu-id="282a7-198">Se o valor de uma propriedade em uma localização for nulo, o valor será herdado da identidade visual padrão.</span><span class="sxs-lookup"><span data-stu-id="282a7-198">If the value of a property in a localization is null, the value will be inherited from the default branding.</span></span> <span data-ttu-id="282a7-199">Para impedir que isso aconteça, de definir uma cadeia de caracteres ou cadeia de caracteres vazia que contenha apenas o espaço em branco na identidade visual localizada.</span><span class="sxs-lookup"><span data-stu-id="282a7-199">To prevent this from happening, set an empty string or string containing only whitespace in the localized branding.</span></span>

#### <a name="request"></a><span data-ttu-id="282a7-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="282a7-200">Request</span></span>

<span data-ttu-id="282a7-201">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="282a7-201">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties_7"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
Content-Type: application/json

{
    "signInPageText": "French sign-in text.",
    "usernameHintText":" "
}
```

#### <a name="response"></a><span data-ttu-id="282a7-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="282a7-202">Response</span></span>

<span data-ttu-id="282a7-203">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="282a7-203">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="282a7-204">Após essa solicitação, usernameHintText para a localização fr estará vazio em vez de herdar o valor da identidade visual padrão.</span><span class="sxs-lookup"><span data-stu-id="282a7-204">Following this request, usernameHintText for the fr localization will be empty instead of inheriting the value from default branding.</span></span>

### <a name="example-4-replace-french-localization-with-put"></a><span data-ttu-id="282a7-205">Exemplo 4: Substitua a localização francesa por PUT</span><span class="sxs-lookup"><span data-stu-id="282a7-205">Example 4: Replace French localization with PUT</span></span>

<span data-ttu-id="282a7-206">Para fazer uma atualização sobre a localização usando PUT, devemos adicionar todas as propriedades no corpo juntamente com a propriedade que precisa ser atualizada à medida que PUT substitui o objeto existente pelo novo.</span><span class="sxs-lookup"><span data-stu-id="282a7-206">To make an update on localization using PUT, we should add all properties in body along with the property that needs to be updated as PUT replaces existing object with the new one.</span></span> <span data-ttu-id="282a7-207">As outras propriedades que não estão no corpo da carga de PUT serão definidas como NULL.</span><span class="sxs-lookup"><span data-stu-id="282a7-207">The other properties which are not in the payload body of PUT will be set to NULL.</span></span> <span data-ttu-id="282a7-208">Aqui no exemplo abaixo, somente a propriedade backgroundColor é mantida e signInPageText é atualizada enquanto outras são definidas como nulas.</span><span class="sxs-lookup"><span data-stu-id="282a7-208">Here in example below, only backgroundColor property is retained and signInPageText is updated while others are set to null.</span></span>
<span data-ttu-id="282a7-209">Se a localização especificada ainda não existir, PUT para a URL especificando que a localização a cria.</span><span class="sxs-lookup"><span data-stu-id="282a7-209">If the specified localization does not already exist, PUT to the URL specifying that localization creates it.</span></span>
<span data-ttu-id="282a7-210">Se a carga contiver uma propriedade ID ou um header content-Language e eles não corresponderem à ID na URL, lançaremos a solicitação Desa resposta.</span><span class="sxs-lookup"><span data-stu-id="282a7-210">If the payload contains an id property or a Content-Language header, and they don't match id in URL, we throw Bad request.</span></span>

#### <a name="request"></a><span data-ttu-id="282a7-211">Solicitação</span><span class="sxs-lookup"><span data-stu-id="282a7-211">Request</span></span>

<span data-ttu-id="282a7-212">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="282a7-212">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="282a7-213">HTTP</span><span class="sxs-lookup"><span data-stu-id="282a7-213">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties_8"
}-->

```http
PUT https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "signInPageText": "fr"
}
```
# <a name="c"></a>[<span data-ttu-id="282a7-214">C#</span><span class="sxs-lookup"><span data-stu-id="282a7-214">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandingproperties-8-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="282a7-215">JavaScript</span><span class="sxs-lookup"><span data-stu-id="282a7-215">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandingproperties-8-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="282a7-216">Objective-C</span><span class="sxs-lookup"><span data-stu-id="282a7-216">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandingproperties-8-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="282a7-217">Java</span><span class="sxs-lookup"><span data-stu-id="282a7-217">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandingproperties-8-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="282a7-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="282a7-218">Response</span></span>
<span data-ttu-id="282a7-219">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="282a7-219">The following is an example of the response.</span></span>

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
