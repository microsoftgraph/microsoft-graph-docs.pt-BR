---
title: Atualizar organizationalBrandingProperties
description: Atualize as propriedades de um objeto organizationalBrandingProperties.
localization_priority: Normal
author: almars
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: b39e11c4ff864cbd62fc2b1fd6eb567306b46c3c
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52298226"
---
# <a name="update-organizationalbrandingproperties"></a><span data-ttu-id="51e83-103">Atualizar organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="51e83-103">Update organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51e83-104">Atualize as propriedades de [um objeto organizationalBrandingProperties.](../resources/organizationalbrandingproperties.md)</span><span class="sxs-lookup"><span data-stu-id="51e83-104">Update the properties of an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="51e83-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="51e83-105">Permissions</span></span>

<span data-ttu-id="51e83-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51e83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="51e83-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51e83-108">Permission type</span></span>                        | <span data-ttu-id="51e83-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="51e83-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="51e83-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51e83-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="51e83-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51e83-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="51e83-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="51e83-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51e83-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51e83-113">Not supported.</span></span> |
| <span data-ttu-id="51e83-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="51e83-114">Application</span></span>                            | <span data-ttu-id="51e83-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51e83-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="51e83-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51e83-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{tenant id}/branding
PUT /organization/{tenant id}/branding
```

## <a name="request-headers"></a><span data-ttu-id="51e83-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51e83-117">Request headers</span></span>

| <span data-ttu-id="51e83-118">Nome</span><span class="sxs-lookup"><span data-stu-id="51e83-118">Name</span></span>       | <span data-ttu-id="51e83-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="51e83-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="51e83-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="51e83-120">Authorization</span></span> | <span data-ttu-id="51e83-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51e83-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="51e83-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="51e83-123">Content-Type</span></span>  | <span data-ttu-id="51e83-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51e83-p103">application/json. Required.</span></span>  |
| <span data-ttu-id="51e83-126">Content-Language</span><span class="sxs-lookup"><span data-stu-id="51e83-126">Content-Language</span></span>  | <span data-ttu-id="51e83-127">Localidade.</span><span class="sxs-lookup"><span data-stu-id="51e83-127">Locale.</span></span> <span data-ttu-id="51e83-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="51e83-128">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="51e83-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51e83-129">Request body</span></span>

<span data-ttu-id="51e83-130">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="51e83-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="51e83-131">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="51e83-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="51e83-132">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="51e83-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="51e83-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="51e83-133">Property</span></span>     | <span data-ttu-id="51e83-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="51e83-134">Type</span></span>        | <span data-ttu-id="51e83-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="51e83-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="51e83-136">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="51e83-136">backgroundColor</span></span>|<span data-ttu-id="51e83-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51e83-137">String</span></span>|<span data-ttu-id="51e83-138">Cor que aparecerá no lugar da imagem de plano de fundo em conexões de baixa largura de banda.</span><span class="sxs-lookup"><span data-stu-id="51e83-138">Color that will appear in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="51e83-139">A cor primária do logotipo da faixa ou da cor da sua organização é recomendada para ser usada aqui.</span><span class="sxs-lookup"><span data-stu-id="51e83-139">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="51e83-140">Especifique isso em hexadecimal (por exemplo, branco é #FFFFFF).</span><span class="sxs-lookup"><span data-stu-id="51e83-140">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span>|
|<span data-ttu-id="51e83-141">backgroundImage</span><span class="sxs-lookup"><span data-stu-id="51e83-141">backgroundImage</span></span>|<span data-ttu-id="51e83-142">Stream</span><span class="sxs-lookup"><span data-stu-id="51e83-142">Stream</span></span>|<span data-ttu-id="51e83-143">Imagem que aparece como o plano de fundo da página de logom.</span><span class="sxs-lookup"><span data-stu-id="51e83-143">Image that appears as the background of the sign in page.</span></span> <span data-ttu-id="51e83-144">.png ou .jpg maior que 1920x1080 e menor que 300kb.</span><span class="sxs-lookup"><span data-stu-id="51e83-144">.png or .jpg not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="51e83-145">Uma imagem menor reduzirá os requisitos de largura de banda e tornará as cargas de página mais performant.</span><span class="sxs-lookup"><span data-stu-id="51e83-145">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span>|
|<span data-ttu-id="51e83-146">bannerLogo</span><span class="sxs-lookup"><span data-stu-id="51e83-146">bannerLogo</span></span>|<span data-ttu-id="51e83-147">Stream</span><span class="sxs-lookup"><span data-stu-id="51e83-147">Stream</span></span>|<span data-ttu-id="51e83-148">Uma versão em faixa do logotipo da sua empresa que aparece na página de entrada.</span><span class="sxs-lookup"><span data-stu-id="51e83-148">A banner version of your company logo which appears appears on the sign-in page.</span></span> <span data-ttu-id="51e83-149">.png ou .jpg maior que 36x245px.</span><span class="sxs-lookup"><span data-stu-id="51e83-149">.png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="51e83-150">Recomendamos usar uma imagem transparente sem preenchimento ao redor do logotipo.</span><span class="sxs-lookup"><span data-stu-id="51e83-150">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="51e83-151">signInPageText</span><span class="sxs-lookup"><span data-stu-id="51e83-151">signInPageText</span></span>|<span data-ttu-id="51e83-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51e83-152">String</span></span>|<span data-ttu-id="51e83-153">Texto que aparece na parte inferior da caixa de login.</span><span class="sxs-lookup"><span data-stu-id="51e83-153">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="51e83-154">Você pode usar isso para comunicar informações adicionais, como o número de telefone para o seu help desk ou uma declaração legal.</span><span class="sxs-lookup"><span data-stu-id="51e83-154">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="51e83-155">Este texto deve ser Unicode e não exceder 1024 caracteres.</span><span class="sxs-lookup"><span data-stu-id="51e83-155">This text must be Unicode and not exceed 1024 characters.</span></span>|
|<span data-ttu-id="51e83-156">squareLogo</span><span class="sxs-lookup"><span data-stu-id="51e83-156">squareLogo</span></span>|<span data-ttu-id="51e83-157">Stream</span><span class="sxs-lookup"><span data-stu-id="51e83-157">Stream</span></span>|<span data-ttu-id="51e83-158">Versão quadrada do logotipo da sua empresa.</span><span class="sxs-lookup"><span data-stu-id="51e83-158">Square version of your company logo.</span></span> <span data-ttu-id="51e83-159">Isso aparece em Windows 10 experiências OOBE (out-of-box) e quando Windows Autopilot está habilitado para implantação.</span><span class="sxs-lookup"><span data-stu-id="51e83-159">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="51e83-160">.png ou .jpg maior que 240x240px e não mais de 10kb de tamanho.</span><span class="sxs-lookup"><span data-stu-id="51e83-160">.png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="51e83-161">Recomendamos usar uma imagem transparente sem preenchimento ao redor do logotipo.</span><span class="sxs-lookup"><span data-stu-id="51e83-161">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="51e83-162">usernameHintText</span><span class="sxs-lookup"><span data-stu-id="51e83-162">usernameHintText</span></span>|<span data-ttu-id="51e83-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51e83-163">String</span></span>|<span data-ttu-id="51e83-164">Cadeia de caracteres que mostra como a dica na caixa de texto do nome de usuário na tela de entrada.</span><span class="sxs-lookup"><span data-stu-id="51e83-164">String that shows as the hint in the username textbox on the sign in screen.</span></span> <span data-ttu-id="51e83-165">Este texto deve ser Unicode, sem links ou código, e não pode exceder 64 caracteres.</span><span class="sxs-lookup"><span data-stu-id="51e83-165">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span>|

<span data-ttu-id="51e83-166">A **propriedade id** é ignorada quando passada.</span><span class="sxs-lookup"><span data-stu-id="51e83-166">The **id** property is ignored when passed in.</span></span>

## <a name="response"></a><span data-ttu-id="51e83-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="51e83-167">Response</span></span>

<span data-ttu-id="51e83-168">Se tiver êxito, este método retornará um código de resposta `204 OK`.</span><span class="sxs-lookup"><span data-stu-id="51e83-168">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="51e83-169">Exemplos</span><span class="sxs-lookup"><span data-stu-id="51e83-169">Examples</span></span>
### <a name="example-1-update-default-branding"></a><span data-ttu-id="51e83-170">Exemplo 1: atualizar a identidade visual padrão</span><span class="sxs-lookup"><span data-stu-id="51e83-170">Example 1: Update default branding</span></span>
<span data-ttu-id="51e83-171">Se a identidade visual já existir, substituirá apenas as propriedades especificadas, deixando propriedades não `PATCH` especificadas inalteradas.</span><span class="sxs-lookup"><span data-stu-id="51e83-171">If the branding already exists, `PATCH` will replace only the specified properties, leaving unspecified properties unchanged.</span></span> 
#### <a name="request"></a><span data-ttu-id="51e83-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51e83-172">Request</span></span>

<span data-ttu-id="51e83-173">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="51e83-173">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="51e83-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="51e83-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties_1"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json

{
    "signInPageText":"Default",
    "usernameHintText":"DefaultHint"
}
```
# <a name="c"></a>[<span data-ttu-id="51e83-175">C#</span><span class="sxs-lookup"><span data-stu-id="51e83-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandingproperties-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51e83-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51e83-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandingproperties-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51e83-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51e83-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandingproperties-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="51e83-178">Java</span><span class="sxs-lookup"><span data-stu-id="51e83-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandingproperties-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="51e83-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="51e83-179">Response</span></span>
<span data-ttu-id="51e83-180">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="51e83-180">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 OK
```

<span data-ttu-id="51e83-181">Nesse caso, os valores da identidade visual padrão são atualizados, mas nenhum valor é alterado em qualquer localização.</span><span class="sxs-lookup"><span data-stu-id="51e83-181">In this case, the values of the default branding are updated but no values are changed on any localization.</span></span>

### <a name="example-2-update-bannerlogo-for-default-branding"></a><span data-ttu-id="51e83-182">Exemplo 2: Atualizar bannerLogo para identidade visual padrão</span><span class="sxs-lookup"><span data-stu-id="51e83-182">Example 2: Update bannerLogo for default branding</span></span>
<span data-ttu-id="51e83-183">A solicitação a seguir atualiza o logotipo da faixa para a identidade visual padrão.</span><span class="sxs-lookup"><span data-stu-id="51e83-183">The following request updates the banner logo for the default branding.</span></span>
#### <a name="request"></a><span data-ttu-id="51e83-184">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51e83-184">Request</span></span>

<span data-ttu-id="51e83-185">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="51e83-185">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties_2"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Content-Type: image/jpeg

<Image>
```

#### <a name="response"></a><span data-ttu-id="51e83-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="51e83-186">Response</span></span>
<span data-ttu-id="51e83-187">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="51e83-187">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-update-localized-branding"></a><span data-ttu-id="51e83-188">Exemplo 3: atualizar a identidade visual localizada</span><span class="sxs-lookup"><span data-stu-id="51e83-188">Example 3: Update localized branding</span></span>
<span data-ttu-id="51e83-189">Se o header **Content-Language** for especificado, a localização associada ao **Content-Language** será criada primeiro se ainda não existir e, em seguida, atualizada usando os valores especificados.</span><span class="sxs-lookup"><span data-stu-id="51e83-189">If **Content-Language** header is specified, the localization associated with **Content-Language** is first created if it doesn't already exist, and then updated using the specified values.</span></span> <span data-ttu-id="51e83-190">A identidade visual padrão não foi alterada.</span><span class="sxs-lookup"><span data-stu-id="51e83-190">The default branding is not changed.</span></span>
#### <a name="request"></a><span data-ttu-id="51e83-191">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51e83-191">Request</span></span>

<span data-ttu-id="51e83-192">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="51e83-192">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties_3"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json
Content-Language: fr

{
    "backgroundColor":"#FFFF33"
}
```

#### <a name="response"></a><span data-ttu-id="51e83-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="51e83-193">Response</span></span>
<span data-ttu-id="51e83-194">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="51e83-194">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="51e83-195">Após essa solicitação, a localização é atualizada com o novo valor de backgroundColor , mas nenhuma alteração é feita para a `fr` identidade visual padrão. </span><span class="sxs-lookup"><span data-stu-id="51e83-195">Following this request, the `fr` localization is updated with the new value of **backgroundColor**, but no change is made to the default branding.</span></span>

### <a name="example-4-replace-default-branding-and-all-localizations"></a><span data-ttu-id="51e83-196">Exemplo 4: Substituir a identidade visual padrão e todas as localizações</span><span class="sxs-lookup"><span data-stu-id="51e83-196">Example 4: Replace default branding and all localizations</span></span>
<span data-ttu-id="51e83-197">Se a identidade visual já existir, `PUT` substituirá a identidade visual padrão e quaisquer localizações.</span><span class="sxs-lookup"><span data-stu-id="51e83-197">If the branding already exists, `PUT` will replace the default branding and any localizations.</span></span>
#### <a name="request"></a><span data-ttu-id="51e83-198">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51e83-198">Request</span></span>

<span data-ttu-id="51e83-199">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="51e83-199">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="51e83-200">HTTP</span><span class="sxs-lookup"><span data-stu-id="51e83-200">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties_4"
}-->

```http
PUT https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json
Content-Language: fr

{
    "backgroundColor":"#FFFF33"
}
```
# <a name="c"></a>[<span data-ttu-id="51e83-201">C#</span><span class="sxs-lookup"><span data-stu-id="51e83-201">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandingproperties-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51e83-202">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51e83-202">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandingproperties-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51e83-203">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51e83-203">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandingproperties-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="51e83-204">Java</span><span class="sxs-lookup"><span data-stu-id="51e83-204">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandingproperties-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="51e83-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="51e83-205">Response</span></span>
<span data-ttu-id="51e83-206">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="51e83-206">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="51e83-207">Após essa solicitação, a identidade visual padrão tem apenas o **backgroundColor** especificado e tem exatamente uma localização com a **id** , também com o `fr` conjunto **backgroundColor.**</span><span class="sxs-lookup"><span data-stu-id="51e83-207">Following this request, the default branding has only the **backgroundColor** specified and has exactly one localization with the **id** `fr`, also with the **backgroundColor** set.</span></span>
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organizationalbrandingproperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
