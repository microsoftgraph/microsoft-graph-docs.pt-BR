---
title: Atualizar organizationalBrandingProperties
description: Atualiza as propriedades de um objeto organizationalBrandingProperties.
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7655caa6e5c8eb1187bcc159f7f6d8c78641abc9
ms.sourcegitcommit: 40b0e58312819b69567f35ab894ee0d2989837ab
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/13/2020
ms.locfileid: "49031895"
---
# <a name="update-organizationalbrandingproperties"></a><span data-ttu-id="667f8-103">Atualizar organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="667f8-103">Update organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="667f8-104">Atualiza as propriedades de um objeto [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) .</span><span class="sxs-lookup"><span data-stu-id="667f8-104">Update the properties of an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="667f8-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="667f8-105">Permissions</span></span>

<span data-ttu-id="667f8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="667f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="667f8-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="667f8-108">Permission type</span></span>                        | <span data-ttu-id="667f8-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="667f8-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="667f8-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="667f8-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="667f8-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="667f8-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="667f8-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="667f8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="667f8-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="667f8-113">Not supported.</span></span> |
| <span data-ttu-id="667f8-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="667f8-114">Application</span></span>                            | <span data-ttu-id="667f8-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="667f8-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="667f8-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="667f8-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}/branding/{property name}
PUT /organization/{id}/branding/{property name}
```

## <a name="request-headers"></a><span data-ttu-id="667f8-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="667f8-117">Request headers</span></span>

| <span data-ttu-id="667f8-118">Nome</span><span class="sxs-lookup"><span data-stu-id="667f8-118">Name</span></span>       | <span data-ttu-id="667f8-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="667f8-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="667f8-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="667f8-120">Authorization</span></span> | <span data-ttu-id="667f8-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="667f8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="667f8-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="667f8-123">Content-Type</span></span>  | <span data-ttu-id="667f8-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="667f8-p103">application/json. Required.</span></span>  |
| <span data-ttu-id="667f8-126">Conteúdo-idioma</span><span class="sxs-lookup"><span data-stu-id="667f8-126">Content-Language</span></span>  | <span data-ttu-id="667f8-127">LCID.</span><span class="sxs-lookup"><span data-stu-id="667f8-127">Locale.</span></span> <span data-ttu-id="667f8-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="667f8-128">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="667f8-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="667f8-129">Request body</span></span>

<span data-ttu-id="667f8-130">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="667f8-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="667f8-131">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="667f8-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="667f8-132">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="667f8-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="667f8-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="667f8-133">Property</span></span>     | <span data-ttu-id="667f8-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="667f8-134">Type</span></span>        | <span data-ttu-id="667f8-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="667f8-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="667f8-136">CorDoFundo</span><span class="sxs-lookup"><span data-stu-id="667f8-136">backgroundColor</span></span>|<span data-ttu-id="667f8-137">String</span><span class="sxs-lookup"><span data-stu-id="667f8-137">String</span></span>|<span data-ttu-id="667f8-138">Cor que aparecerá no lugar da imagem de plano de fundo em conexões de baixa largura de banda.</span><span class="sxs-lookup"><span data-stu-id="667f8-138">Color that will appear in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="667f8-139">É recomendável usar a cor principal do logotipo de faixa ou a cor da sua organização aqui.</span><span class="sxs-lookup"><span data-stu-id="667f8-139">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="667f8-140">Especifique isso em hexadecimal (por exemplo, branco é #FFFFFF).</span><span class="sxs-lookup"><span data-stu-id="667f8-140">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span>|
|<span data-ttu-id="667f8-141">backgroundImage</span><span class="sxs-lookup"><span data-stu-id="667f8-141">backgroundImage</span></span>|<span data-ttu-id="667f8-142">Fluxo</span><span class="sxs-lookup"><span data-stu-id="667f8-142">Stream</span></span>|<span data-ttu-id="667f8-143">Imagem que aparece como plano de fundo da página de entrada.</span><span class="sxs-lookup"><span data-stu-id="667f8-143">Image that appears as the background of the sign in page.</span></span> <span data-ttu-id="667f8-144">. png ou. jpg não é maior do que 1920 x 1080 e menor do que 300kb.</span><span class="sxs-lookup"><span data-stu-id="667f8-144">.png or .jpg not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="667f8-145">Uma imagem menor reduzirá os requisitos de largura de banda e fará com que as cargas de página mais tenham mais desempenho.</span><span class="sxs-lookup"><span data-stu-id="667f8-145">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span>|
|<span data-ttu-id="667f8-146">bannerLogo</span><span class="sxs-lookup"><span data-stu-id="667f8-146">bannerLogo</span></span>|<span data-ttu-id="667f8-147">Fluxo</span><span class="sxs-lookup"><span data-stu-id="667f8-147">Stream</span></span>|<span data-ttu-id="667f8-148">Uma versão de banner do logotipo da empresa que aparece aparece na página de entrada.</span><span class="sxs-lookup"><span data-stu-id="667f8-148">A banner version of your company logo which appears appears on the sign-in page.</span></span> <span data-ttu-id="667f8-149">. png ou. jpg não maior do que 36x245px.</span><span class="sxs-lookup"><span data-stu-id="667f8-149">.png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="667f8-150">Recomendamos usar uma imagem transparente sem preenchimento em torno do logotipo.</span><span class="sxs-lookup"><span data-stu-id="667f8-150">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="667f8-151">signInPageText</span><span class="sxs-lookup"><span data-stu-id="667f8-151">signInPageText</span></span>|<span data-ttu-id="667f8-152">String</span><span class="sxs-lookup"><span data-stu-id="667f8-152">String</span></span>|<span data-ttu-id="667f8-153">Texto que aparece na parte inferior da caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="667f8-153">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="667f8-154">Você pode usá-lo para comunicar informações adicionais, como o número de telefone para o suporte técnico ou uma instrução legal.</span><span class="sxs-lookup"><span data-stu-id="667f8-154">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="667f8-155">Este texto deve ser Unicode e não exceder 1024 caracteres.</span><span class="sxs-lookup"><span data-stu-id="667f8-155">This text must be Unicode and not exceed 1024 characters.</span></span>|
|<span data-ttu-id="667f8-156">squareLogo</span><span class="sxs-lookup"><span data-stu-id="667f8-156">squareLogo</span></span>|<span data-ttu-id="667f8-157">Fluxo</span><span class="sxs-lookup"><span data-stu-id="667f8-157">Stream</span></span>|<span data-ttu-id="667f8-158">Versão quadrada do logotipo da sua empresa.</span><span class="sxs-lookup"><span data-stu-id="667f8-158">Square version of your company logo.</span></span> <span data-ttu-id="667f8-159">Isso aparece nas experiências de uso (OOBE) do Windows 10 e quando o Windows AutoPilot está habilitado para implantação.</span><span class="sxs-lookup"><span data-stu-id="667f8-159">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="667f8-160">. png ou. jpg não maior do que 240x240px e não mais do que 10 KB em tamanho.</span><span class="sxs-lookup"><span data-stu-id="667f8-160">.png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="667f8-161">Recomendamos usar uma imagem transparente sem preenchimento em torno do logotipo.</span><span class="sxs-lookup"><span data-stu-id="667f8-161">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="667f8-162">usernameHintText</span><span class="sxs-lookup"><span data-stu-id="667f8-162">usernameHintText</span></span>|<span data-ttu-id="667f8-163">String</span><span class="sxs-lookup"><span data-stu-id="667f8-163">String</span></span>|<span data-ttu-id="667f8-164">Cadeia de caracteres que mostra como a dica na caixa de texto username na tela de entrada.</span><span class="sxs-lookup"><span data-stu-id="667f8-164">String that shows as the hint in the username textbox on the sign in screen.</span></span> <span data-ttu-id="667f8-165">Este texto deve ser Unicode, sem links ou código, e não pode exceder 64 caracteres.</span><span class="sxs-lookup"><span data-stu-id="667f8-165">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span>|

<span data-ttu-id="667f8-166">A propriedade **ID** é ignorada quando passada.</span><span class="sxs-lookup"><span data-stu-id="667f8-166">The **id** property is ignored when passed in.</span></span>

## <a name="response"></a><span data-ttu-id="667f8-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="667f8-167">Response</span></span>

<span data-ttu-id="667f8-168">Se tiver êxito, este método retornará um código de resposta `204 OK`.</span><span class="sxs-lookup"><span data-stu-id="667f8-168">If successful, this method returns a `204 OK` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="667f8-169">Exemplos</span><span class="sxs-lookup"><span data-stu-id="667f8-169">Examples</span></span>
### <a name="example-1-update-default-branding"></a><span data-ttu-id="667f8-170">Exemplo 1: atualizar a identidade visual padrão</span><span class="sxs-lookup"><span data-stu-id="667f8-170">Example 1: Update default branding</span></span>
<span data-ttu-id="667f8-171">Se a identidade visual já existir, o PATCH substituirá apenas as propriedades especificadas, deixando inalteradas as propriedades não especificadas.</span><span class="sxs-lookup"><span data-stu-id="667f8-171">If the branding already exists, PATCH will replace only the specified properties, leaving unspecified properties unchanged.</span></span> 
#### <a name="request"></a><span data-ttu-id="667f8-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="667f8-172">Request</span></span>

<span data-ttu-id="667f8-173">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="667f8-173">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json

{
    "signInPageText":"Default",
    "usernameHintText":"DefaultHint"
}
```

#### <a name="response"></a><span data-ttu-id="667f8-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="667f8-174">Response</span></span>
<span data-ttu-id="667f8-175">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="667f8-175">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 OK
```

<span data-ttu-id="667f8-176">Nesse caso, os valores do/branding padrão são atualizados, mas nenhum valor é alterado em qualquer localização.</span><span class="sxs-lookup"><span data-stu-id="667f8-176">In this case, the values of the default /branding are updated but no values are changed on any localization.</span></span>

### <a name="example-2-update-bannerlogo-for-default-branding"></a><span data-ttu-id="667f8-177">Exemplo 2: atualizar bannerLogo para identidade visual padrão</span><span class="sxs-lookup"><span data-stu-id="667f8-177">Example 2: Update bannerLogo for default branding</span></span>
<span data-ttu-id="667f8-178">A solicitação a seguir atualiza o logotipo da faixa para a identidade visual padrão.</span><span class="sxs-lookup"><span data-stu-id="667f8-178">The following request updates the banner logo for the default branding.</span></span>
#### <a name="request"></a><span data-ttu-id="667f8-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="667f8-179">Request</span></span>

<span data-ttu-id="667f8-180">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="667f8-180">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Content-Type: image/jpeg

<Image>
```

#### <a name="response"></a><span data-ttu-id="667f8-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="667f8-181">Response</span></span>
<span data-ttu-id="667f8-182">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="667f8-182">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-update-localized-branding"></a><span data-ttu-id="667f8-183">Exemplo 3: atualizar a identidade visual localizada</span><span class="sxs-lookup"><span data-stu-id="667f8-183">Example 3: Update localized branding</span></span>
<span data-ttu-id="667f8-184">Se o cabeçalho de idioma de conteúdo for especificado, a localização associada ao conteúdo será criada, se ainda não existir, e atualizada com os valores especificados.</span><span class="sxs-lookup"><span data-stu-id="667f8-184">If Content-Language header is specified the localization associated with Content-Language is created, if it doesn't already exist, and then updated using the specified values.</span></span> <span data-ttu-id="667f8-185">A identidade visual padrão não é alterada.</span><span class="sxs-lookup"><span data-stu-id="667f8-185">The default branding is not changed.</span></span>
#### <a name="request"></a><span data-ttu-id="667f8-186">Solicitação</span><span class="sxs-lookup"><span data-stu-id="667f8-186">Request</span></span>

<span data-ttu-id="667f8-187">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="667f8-187">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json
Content-Language: fr

{
    "backgroundColor":"#FFFF33"
}
```

#### <a name="response"></a><span data-ttu-id="667f8-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="667f8-188">Response</span></span>
<span data-ttu-id="667f8-189">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="667f8-189">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="667f8-190">Após essa solicitação, a localização fr é atualizada com o novo valor de backgroundColor, mas nenhuma alteração é feita no padrão/branding.</span><span class="sxs-lookup"><span data-stu-id="667f8-190">Following this request, the fr localization is updated with the new value of backgroundColor, but no change is made to the default /branding.</span></span>

### <a name="example-4-replace-default-branding-and-all-localizations"></a><span data-ttu-id="667f8-191">Exemplo 4: substituir a identidade visual padrão e todas as localizações</span><span class="sxs-lookup"><span data-stu-id="667f8-191">Example 4: Replace default branding and all localizations</span></span>
<span data-ttu-id="667f8-192">Se a identidade visual já existir, PUT substituirá a identidade visual padrão e todas as localizações.</span><span class="sxs-lookup"><span data-stu-id="667f8-192">If the branding already exists, PUT will replace the default branding and any localizations.</span></span>
#### <a name="request"></a><span data-ttu-id="667f8-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="667f8-193">Request</span></span>

<span data-ttu-id="667f8-194">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="667f8-194">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PUT https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json
Content-Language: fr

{
    "backgroundColor":"#FFFF33"
}
```

#### <a name="response"></a><span data-ttu-id="667f8-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="667f8-195">Response</span></span>
<span data-ttu-id="667f8-196">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="667f8-196">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="667f8-197">Após essa solicitação, a identidade visual padrão tem apenas o backgroundColor especificado e tem exatamente uma localização com a ID fr, também com o conjunto backgroundColor.</span><span class="sxs-lookup"><span data-stu-id="667f8-197">Following this request, the default branding has only the backgroundColor specified and has exactly one localization with the id fr, also with the backgroundColor set.</span></span>
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organizationalbrandingproperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
