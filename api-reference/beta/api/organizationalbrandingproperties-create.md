---
title: Criar organizationalBrandingProperties
description: Criar identidade visual da organização.
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: adf9a1e6b3f0bb01cbe028b27822b139d736d42e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49524614"
---
# <a name="create-organizationalbrandingproperties"></a><span data-ttu-id="30037-103">Criar organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="30037-103">Create organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30037-104">Criar um objeto [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) .</span><span class="sxs-lookup"><span data-stu-id="30037-104">Create an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span> <span data-ttu-id="30037-105">Isso cria a identidade visual padrão e, opcionalmente, uma identidade visual localizada ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="30037-105">This creates the default branding and optionally a localized branding at the same time.</span></span> <span data-ttu-id="30037-106">A identidade visual padrão é carregada quando um conjunto de identidade visual localizado não é configurado para o idioma do navegador do usuário.</span><span class="sxs-lookup"><span data-stu-id="30037-106">The default branding is loaded when a localized branding set isn't configured for the user's browser language.</span></span>

## <a name="permissions"></a><span data-ttu-id="30037-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="30037-107">Permissions</span></span>

<span data-ttu-id="30037-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30037-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="30037-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="30037-110">Permission type</span></span>                        | <span data-ttu-id="30037-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="30037-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="30037-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="30037-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="30037-113">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30037-113">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="30037-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="30037-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30037-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30037-115">Not supported.</span></span> |
| <span data-ttu-id="30037-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="30037-116">Application</span></span>                            | <span data-ttu-id="30037-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30037-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="30037-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="30037-118">HTTP request</span></span>

<span data-ttu-id="30037-119">Uma identidade visual é criada para uma organização, se ainda não existir uma, usando PUT ou PATCH.</span><span class="sxs-lookup"><span data-stu-id="30037-119">A branding is created for an organization, if one does not already exist, using PUT or PATCH.</span></span>

<span data-ttu-id="30037-120">Se a identidade visual já estiver configurada, PUT substituirá todos os valores existentes, independentemente do que está no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="30037-120">If branding is already configured, PUT will overwrite all existing values regardless of what's in the request body.</span></span> <span data-ttu-id="30037-121">O PATCH só overite os valores que estão incluídos no corpo da solicitação, deixando os valores não incluídos inalterados.</span><span class="sxs-lookup"><span data-stu-id="30037-121">PATCH will only overite the values that are included in the request body, leaving the values not included unchanged.</span></span>

<span data-ttu-id="30037-122">A propriedade **ID** é ignorada em Put/patch para o singleton/branding.</span><span class="sxs-lookup"><span data-stu-id="30037-122">The **id** property is ignored on PUT/PATCH to the /branding singleton.</span></span> <span data-ttu-id="30037-123">Se Content-Language não for especificado, a identidade visual padrão será criada, o que corresponde a uma **ID** de `und` .</span><span class="sxs-lookup"><span data-stu-id="30037-123">If Content-Language is not specified, the default branding is created, which corresponds to an **id** of `und`.</span></span> <span data-ttu-id="30037-124">Se o idioma de conteúdo for especificado, a identidade visual será criada para essa localidade.</span><span class="sxs-lookup"><span data-stu-id="30037-124">If Content-Language is specified, branding is created for that locale.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PUT /organization/{id}/branding
PATCH /organization/{id}/branding
```

## <a name="optional-query-parameters"></a><span data-ttu-id="30037-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="30037-125">Optional query parameters</span></span>

<span data-ttu-id="30037-126">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="30037-126">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="30037-127">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="30037-127">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="30037-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="30037-128">Request headers</span></span>

| <span data-ttu-id="30037-129">Nome</span><span class="sxs-lookup"><span data-stu-id="30037-129">Name</span></span>      |<span data-ttu-id="30037-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="30037-130">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="30037-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="30037-131">Authorization</span></span> | <span data-ttu-id="30037-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30037-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="30037-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="30037-134">Content-Type</span></span>  | <span data-ttu-id="30037-p107">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30037-p107">application/json. Required.</span></span>  |
| <span data-ttu-id="30037-137">Conteúdo-idioma</span><span class="sxs-lookup"><span data-stu-id="30037-137">Content-Language</span></span>  | <span data-ttu-id="30037-138">LCID.</span><span class="sxs-lookup"><span data-stu-id="30037-138">Locale.</span></span> <span data-ttu-id="30037-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="30037-139">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="30037-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="30037-140">Request body</span></span>

| <span data-ttu-id="30037-141">Propriedade</span><span class="sxs-lookup"><span data-stu-id="30037-141">Property</span></span>     | <span data-ttu-id="30037-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="30037-142">Type</span></span>        | <span data-ttu-id="30037-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="30037-143">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="30037-144">CorDoFundo</span><span class="sxs-lookup"><span data-stu-id="30037-144">backgroundColor</span></span>|<span data-ttu-id="30037-145">String</span><span class="sxs-lookup"><span data-stu-id="30037-145">String</span></span>|<span data-ttu-id="30037-146">Cor que aparecerá no lugar da imagem de plano de fundo em conexões de baixa largura de banda.</span><span class="sxs-lookup"><span data-stu-id="30037-146">Color that will appear in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="30037-147">É recomendável usar a cor principal do logotipo de faixa ou a cor da sua organização aqui.</span><span class="sxs-lookup"><span data-stu-id="30037-147">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="30037-148">Especifique isso em hexadecimal (por exemplo, branco é #FFFFFF).</span><span class="sxs-lookup"><span data-stu-id="30037-148">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span>|
|<span data-ttu-id="30037-149">backgroundImage</span><span class="sxs-lookup"><span data-stu-id="30037-149">backgroundImage</span></span>|<span data-ttu-id="30037-150">Stream</span><span class="sxs-lookup"><span data-stu-id="30037-150">Stream</span></span>|<span data-ttu-id="30037-151">Imagem que aparece como plano de fundo da página de entrada.</span><span class="sxs-lookup"><span data-stu-id="30037-151">Image that appears as the background of the sign in page.</span></span> <span data-ttu-id="30037-152">. png ou. jpg não é maior do que 1920 x 1080 e menor do que 300kb.</span><span class="sxs-lookup"><span data-stu-id="30037-152">.png or .jpg not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="30037-153">Uma imagem menor reduzirá os requisitos de largura de banda e fará com que as cargas de página mais tenham mais desempenho.</span><span class="sxs-lookup"><span data-stu-id="30037-153">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span>|
|<span data-ttu-id="30037-154">bannerLogo</span><span class="sxs-lookup"><span data-stu-id="30037-154">bannerLogo</span></span>|<span data-ttu-id="30037-155">Stream</span><span class="sxs-lookup"><span data-stu-id="30037-155">Stream</span></span>|<span data-ttu-id="30037-156">Uma versão de banner do logotipo da empresa que aparece aparece na página de entrada.</span><span class="sxs-lookup"><span data-stu-id="30037-156">A banner version of your company logo which appears appears on the sign-in page.</span></span> <span data-ttu-id="30037-157">. png ou. jpg não maior do que 36x245px.</span><span class="sxs-lookup"><span data-stu-id="30037-157">.png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="30037-158">Recomendamos usar uma imagem transparente sem preenchimento em torno do logotipo.</span><span class="sxs-lookup"><span data-stu-id="30037-158">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="30037-159">signInPageText</span><span class="sxs-lookup"><span data-stu-id="30037-159">signInPageText</span></span>|<span data-ttu-id="30037-160">String</span><span class="sxs-lookup"><span data-stu-id="30037-160">String</span></span>|<span data-ttu-id="30037-161">Texto que aparece na parte inferior da caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="30037-161">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="30037-162">Você pode usá-lo para comunicar informações adicionais, como o número de telefone para o suporte técnico ou uma instrução legal.</span><span class="sxs-lookup"><span data-stu-id="30037-162">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="30037-163">Este texto deve ser Unicode e não exceder 1024 caracteres.</span><span class="sxs-lookup"><span data-stu-id="30037-163">This text must be Unicode and not exceed 1024 characters.</span></span>|
|<span data-ttu-id="30037-164">squareLogo</span><span class="sxs-lookup"><span data-stu-id="30037-164">squareLogo</span></span>|<span data-ttu-id="30037-165">Stream</span><span class="sxs-lookup"><span data-stu-id="30037-165">Stream</span></span>|<span data-ttu-id="30037-166">Versão quadrada do logotipo da sua empresa.</span><span class="sxs-lookup"><span data-stu-id="30037-166">Square version of your company logo.</span></span> <span data-ttu-id="30037-167">Isso aparece nas experiências de uso (OOBE) do Windows 10 e quando o Windows AutoPilot está habilitado para implantação.</span><span class="sxs-lookup"><span data-stu-id="30037-167">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="30037-168">. png ou. jpg não maior do que 240x240px e não mais do que 10 KB em tamanho.</span><span class="sxs-lookup"><span data-stu-id="30037-168">.png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="30037-169">Recomendamos usar uma imagem transparente sem preenchimento em torno do logotipo.</span><span class="sxs-lookup"><span data-stu-id="30037-169">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="30037-170">usernameHintText</span><span class="sxs-lookup"><span data-stu-id="30037-170">usernameHintText</span></span>|<span data-ttu-id="30037-171">String</span><span class="sxs-lookup"><span data-stu-id="30037-171">String</span></span>|<span data-ttu-id="30037-172">Cadeia de caracteres que mostra como a dica na caixa de texto username na tela de entrada.</span><span class="sxs-lookup"><span data-stu-id="30037-172">String that shows as the hint in the username textbox on the sign in screen.</span></span> <span data-ttu-id="30037-173">Este texto deve ser Unicode, sem links ou código, e não pode exceder 64 caracteres.</span><span class="sxs-lookup"><span data-stu-id="30037-173">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span>|

## <a name="response"></a><span data-ttu-id="30037-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="30037-174">Response</span></span>

<span data-ttu-id="30037-175">Se tiver êxito, este método retornará um `201 Created` código de resposta e o objeto [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) criado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="30037-175">If successful, this method returns a `201 Created` response code and the created [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="30037-176">Exemplos</span><span class="sxs-lookup"><span data-stu-id="30037-176">Examples</span></span>

<span data-ttu-id="30037-177">O exemplo a seguir cria a identidade visual e a localização padrão para en-US.</span><span class="sxs-lookup"><span data-stu-id="30037-177">The following example creates default branding and localization for en-US.</span></span>

### <a name="request"></a><span data-ttu-id="30037-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="30037-178">Request</span></span>

<span data-ttu-id="30037-179">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="30037-179">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="30037-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="30037-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
PUT https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json
Content-Language: en-US

{
    "backgroundColor":"#FFFF33",
    "signInPageText":"Welcome",
    "usernameHintText":"hint"
}
```
# <a name="c"></a>[<span data-ttu-id="30037-181">C#</span><span class="sxs-lookup"><span data-stu-id="30037-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="30037-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="30037-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="30037-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="30037-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="30037-184">Java</span><span class="sxs-lookup"><span data-stu-id="30037-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="30037-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="30037-185">Response</span></span>

<span data-ttu-id="30037-186">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="30037-186">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Language: en-US

{
    "backgroundColor":"#FFFF33",
    "backgroundImage@odata.mediaContentType":"image/*",
    "backgroundImage@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/backgroundImage",
    "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/backgroundImage",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo",
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/bannerLogo",
    "id": "und",
    "signInPageText":"Welcome",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/squareLogo",
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/squareLogo",
    "usernameHintText":"hint"
}
```

<span data-ttu-id="30037-187">Nesse caso, o objeto de identidade visual padrão é definido.</span><span class="sxs-lookup"><span data-stu-id="30037-187">In this case, the default branding object is set.</span></span> <span data-ttu-id="30037-188">A identidade visual localizada para en-US também é definida devido ao idioma do conteúdo no cabeçalho, mesmo que o conjunto de marcas en-US não seja retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="30037-188">Localized branding for en-US is also set due to the Content-Language in the header, even though the en-US branding set is not returned in the response.</span></span> <span data-ttu-id="30037-189">Observe que o idioma de conteúdo na solicitação é opcional e, se não estiver presente, só definirá a identidade visual padrão.</span><span class="sxs-lookup"><span data-stu-id="30037-189">Note that Content-Language in the request is optional, and if not present, will only set default branding.</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
