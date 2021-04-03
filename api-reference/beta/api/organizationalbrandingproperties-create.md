---
title: Criar organizationalBrandingProperties
description: Criar identidade visual da organização.
localization_priority: Normal
author: almars
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 848f2dbdc03f08671f2105c52da3ffaa3bd79929
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582736"
---
# <a name="create-organizationalbrandingproperties"></a><span data-ttu-id="fe8e5-103">Criar organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="fe8e5-103">Create organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe8e5-104">Crie um [objeto organizationalBrandingProperties.](../resources/organizationalbrandingproperties.md)</span><span class="sxs-lookup"><span data-stu-id="fe8e5-104">Create an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span> <span data-ttu-id="fe8e5-105">Isso cria a identidade visual padrão e, opcionalmente, uma identidade visual localizada ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-105">This creates the default branding and optionally a localized branding at the same time.</span></span> <span data-ttu-id="fe8e5-106">A identidade visual padrão é carregada quando um conjunto de identidade visual localizado não é configurado para o idioma do navegador do usuário.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-106">The default branding is loaded when a localized branding set isn't configured for the user's browser language.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe8e5-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="fe8e5-107">Permissions</span></span>

<span data-ttu-id="fe8e5-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe8e5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fe8e5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe8e5-110">Permission type</span></span>                        | <span data-ttu-id="fe8e5-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fe8e5-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fe8e5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe8e5-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="fe8e5-113">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe8e5-113">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="fe8e5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe8e5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe8e5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-115">Not supported.</span></span> |
| <span data-ttu-id="fe8e5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe8e5-116">Application</span></span>                            | <span data-ttu-id="fe8e5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe8e5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe8e5-118">HTTP request</span></span>

<span data-ttu-id="fe8e5-119">Uma identidade visual é criada para uma organização, se ainda não existir, usando PUT ou PATCH.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-119">A branding is created for an organization, if one does not already exist, using PUT or PATCH.</span></span>

<span data-ttu-id="fe8e5-120">Se a identidade visual já estiver configurada, PUT substituirá todos os valores existentes independentemente do que está no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-120">If branding is already configured, PUT will overwrite all existing values regardless of what's in the request body.</span></span> <span data-ttu-id="fe8e5-121">PATCH só sobressá os valores incluídos no corpo da solicitação, deixando os valores não incluídos inalterados.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-121">PATCH will only overite the values that are included in the request body, leaving the values not included unchanged.</span></span>

<span data-ttu-id="fe8e5-122">A **propriedade id** é ignorada em PUT/PATCH no singleton /branding.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-122">The **id** property is ignored on PUT/PATCH to the /branding singleton.</span></span> <span data-ttu-id="fe8e5-123">Se Content-Language não for especificado, a identidade visual padrão será criada, o que corresponde a **uma id** de `und` .</span><span class="sxs-lookup"><span data-stu-id="fe8e5-123">If Content-Language is not specified, the default branding is created, which corresponds to an **id** of `und`.</span></span> <span data-ttu-id="fe8e5-124">Se Content-Language for especificado, a identidade visual será criada para essa localidade.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-124">If Content-Language is specified, branding is created for that locale.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PUT /organization/{id}/branding
PATCH /organization/{id}/branding
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fe8e5-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fe8e5-125">Optional query parameters</span></span>

<span data-ttu-id="fe8e5-126">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-126">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="fe8e5-127">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="fe8e5-127">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="fe8e5-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe8e5-128">Request headers</span></span>

| <span data-ttu-id="fe8e5-129">Nome</span><span class="sxs-lookup"><span data-stu-id="fe8e5-129">Name</span></span>      |<span data-ttu-id="fe8e5-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe8e5-130">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fe8e5-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe8e5-131">Authorization</span></span> | <span data-ttu-id="fe8e5-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fe8e5-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fe8e5-134">Content-Type</span></span>  | <span data-ttu-id="fe8e5-p107">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-p107">application/json. Required.</span></span>  |
| <span data-ttu-id="fe8e5-137">Content-Language</span><span class="sxs-lookup"><span data-stu-id="fe8e5-137">Content-Language</span></span>  | <span data-ttu-id="fe8e5-138">Localidade.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-138">Locale.</span></span> <span data-ttu-id="fe8e5-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-139">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fe8e5-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe8e5-140">Request body</span></span>

| <span data-ttu-id="fe8e5-141">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fe8e5-141">Property</span></span>     | <span data-ttu-id="fe8e5-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="fe8e5-142">Type</span></span>        | <span data-ttu-id="fe8e5-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe8e5-143">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fe8e5-144">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="fe8e5-144">backgroundColor</span></span>|<span data-ttu-id="fe8e5-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe8e5-145">String</span></span>|<span data-ttu-id="fe8e5-146">Cor que aparecerá no lugar da imagem de plano de fundo em conexões de baixa largura de banda.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-146">Color that will appear in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="fe8e5-147">A cor primária do logotipo da faixa ou da cor da sua organização é recomendada para ser usada aqui.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-147">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="fe8e5-148">Especifique isso em hexadecimal (por exemplo, branco é #FFFFFF).</span><span class="sxs-lookup"><span data-stu-id="fe8e5-148">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span>|
|<span data-ttu-id="fe8e5-149">backgroundImage</span><span class="sxs-lookup"><span data-stu-id="fe8e5-149">backgroundImage</span></span>|<span data-ttu-id="fe8e5-150">Stream</span><span class="sxs-lookup"><span data-stu-id="fe8e5-150">Stream</span></span>|<span data-ttu-id="fe8e5-151">Imagem que aparece como o plano de fundo da página de logom.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-151">Image that appears as the background of the sign in page.</span></span> <span data-ttu-id="fe8e5-152">.png ou .jpg não maior que 1920x1080 e menor que 300kb.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-152">.png or .jpg not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="fe8e5-153">Uma imagem menor reduzirá os requisitos de largura de banda e tornará as cargas de página mais performant.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-153">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span>|
|<span data-ttu-id="fe8e5-154">bannerLogo</span><span class="sxs-lookup"><span data-stu-id="fe8e5-154">bannerLogo</span></span>|<span data-ttu-id="fe8e5-155">Stream</span><span class="sxs-lookup"><span data-stu-id="fe8e5-155">Stream</span></span>|<span data-ttu-id="fe8e5-156">Uma versão em faixa do logotipo da sua empresa que aparece na página de entrada.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-156">A banner version of your company logo which appears appears on the sign-in page.</span></span> <span data-ttu-id="fe8e5-157">.png ou .jpg não maior que 36x245px.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-157">.png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="fe8e5-158">Recomendamos usar uma imagem transparente sem preenchimento ao redor do logotipo.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-158">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="fe8e5-159">signInPageText</span><span class="sxs-lookup"><span data-stu-id="fe8e5-159">signInPageText</span></span>|<span data-ttu-id="fe8e5-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe8e5-160">String</span></span>|<span data-ttu-id="fe8e5-161">Texto que aparece na parte inferior da caixa de login.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-161">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="fe8e5-162">Você pode usar isso para comunicar informações adicionais, como o número de telefone para o seu help desk ou uma declaração legal.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-162">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="fe8e5-163">Este texto deve ser Unicode e não exceder 1024 caracteres.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-163">This text must be Unicode and not exceed 1024 characters.</span></span>|
|<span data-ttu-id="fe8e5-164">squareLogo</span><span class="sxs-lookup"><span data-stu-id="fe8e5-164">squareLogo</span></span>|<span data-ttu-id="fe8e5-165">Stream</span><span class="sxs-lookup"><span data-stu-id="fe8e5-165">Stream</span></span>|<span data-ttu-id="fe8e5-166">Versão quadrada do logotipo da sua empresa.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-166">Square version of your company logo.</span></span> <span data-ttu-id="fe8e5-167">Isso aparece nas experiências OOBE (windows 10 out-of-box) e quando o Windows Autopilot está habilitado para implantação.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-167">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="fe8e5-168">.png ou .jpg não maior do que 240x240px e no máximo 10kb de tamanho.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-168">.png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="fe8e5-169">Recomendamos usar uma imagem transparente sem preenchimento ao redor do logotipo.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-169">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="fe8e5-170">usernameHintText</span><span class="sxs-lookup"><span data-stu-id="fe8e5-170">usernameHintText</span></span>|<span data-ttu-id="fe8e5-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fe8e5-171">String</span></span>|<span data-ttu-id="fe8e5-172">Cadeia de caracteres que mostra como a dica na caixa de texto do nome de usuário na tela de entrada.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-172">String that shows as the hint in the username textbox on the sign in screen.</span></span> <span data-ttu-id="fe8e5-173">Este texto deve ser Unicode, sem links ou código, e não pode exceder 64 caracteres.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-173">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span>|

## <a name="response"></a><span data-ttu-id="fe8e5-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe8e5-174">Response</span></span>

<span data-ttu-id="fe8e5-175">Se tiver êxito, este método retornará um código `201 Created` de resposta e o objeto [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) criado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-175">If successful, this method returns a `201 Created` response code and the created [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fe8e5-176">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fe8e5-176">Examples</span></span>

<span data-ttu-id="fe8e5-177">O exemplo a seguir cria a identidade visual e a localização padrão para en-US.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-177">The following example creates default branding and localization for en-US.</span></span>

### <a name="request"></a><span data-ttu-id="fe8e5-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe8e5-178">Request</span></span>

<span data-ttu-id="fe8e5-179">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-179">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fe8e5-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="fe8e5-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_1"
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
# <a name="c"></a>[<span data-ttu-id="fe8e5-181">C#</span><span class="sxs-lookup"><span data-stu-id="fe8e5-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fe8e5-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe8e5-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fe8e5-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fe8e5-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fe8e5-184">Java</span><span class="sxs-lookup"><span data-stu-id="fe8e5-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fe8e5-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe8e5-185">Response</span></span>

<span data-ttu-id="fe8e5-186">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-186">The following is an example of the response.</span></span>

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

<span data-ttu-id="fe8e5-187">Nesse caso, o objeto de identidade visual padrão é definido.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-187">In this case, the default branding object is set.</span></span> <span data-ttu-id="fe8e5-188">A identidade visual localizada para en-US também é definida devido ao Content-Language no header, mesmo que o conjunto de identidade visual en-US não seja retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-188">Localized branding for en-US is also set due to the Content-Language in the header, even though the en-US branding set is not returned in the response.</span></span> <span data-ttu-id="fe8e5-189">Observe que Content-Language na solicitação é opcional e, se não estiver presente, definirá apenas a identidade visual padrão.</span><span class="sxs-lookup"><span data-stu-id="fe8e5-189">Note that Content-Language in the request is optional, and if not present, will only set default branding.</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
