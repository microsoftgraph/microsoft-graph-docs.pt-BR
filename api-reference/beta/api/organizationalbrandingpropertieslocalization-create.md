---
title: Criar organizationalBrandingProperties localizados
description: Crie a identidade visual da organização para uma localidade específica.
localization_priority: Normal
author: kexia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e072be81f10b56802d648501e56d3d2b88ef9c0c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943881"
---
# <a name="create-localized-organizationalbrandingproperties"></a><span data-ttu-id="52f84-103">Criar organizationalBrandingProperties localizados</span><span class="sxs-lookup"><span data-stu-id="52f84-103">Create localized organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52f84-104">Crie um [objeto organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) para uma localidade específica.</span><span class="sxs-lookup"><span data-stu-id="52f84-104">Create an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object for a specific locale.</span></span>

## <a name="permissions"></a><span data-ttu-id="52f84-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="52f84-105">Permissions</span></span>

<span data-ttu-id="52f84-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52f84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="52f84-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52f84-108">Permission type</span></span>                        | <span data-ttu-id="52f84-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="52f84-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="52f84-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52f84-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="52f84-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52f84-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="52f84-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52f84-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52f84-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52f84-113">Not supported.</span></span> |
| <span data-ttu-id="52f84-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52f84-114">Application</span></span>                            | <span data-ttu-id="52f84-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52f84-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="52f84-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52f84-116">HTTP request</span></span>

<span data-ttu-id="52f84-117">POST para identidade visual/localizações para criar uma nova localização.</span><span class="sxs-lookup"><span data-stu-id="52f84-117">POST to branding/localizations to create a new localization.</span></span> <span data-ttu-id="52f84-118">A id especificada no corpo é a localidade da localização.</span><span class="sxs-lookup"><span data-stu-id="52f84-118">The id specified in the body is the locale for the localization.</span></span> <span data-ttu-id="52f84-119">Se nenhuma id for especificada, o valor do header Content-Language, se especificado, será usado como id. Se nenhuma id e nenhum header content-Language for especificado, um erro será retornado.</span><span class="sxs-lookup"><span data-stu-id="52f84-119">If no id is specified, then the value of the Content-Language header, if specified, is used as the id. If no id and no Content-Language header is specified, then an error is returned.</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /organization/{id}/branding/localizations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="52f84-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="52f84-120">Optional query parameters</span></span>

<span data-ttu-id="52f84-121">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="52f84-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="52f84-122">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="52f84-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="52f84-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52f84-123">Request headers</span></span>

| <span data-ttu-id="52f84-124">Nome</span><span class="sxs-lookup"><span data-stu-id="52f84-124">Name</span></span>      |<span data-ttu-id="52f84-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="52f84-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="52f84-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="52f84-126">Authorization</span></span> | <span data-ttu-id="52f84-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52f84-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="52f84-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="52f84-129">Content-Type</span></span>  | <span data-ttu-id="52f84-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52f84-p105">application/json. Required.</span></span>  |
| <span data-ttu-id="52f84-132">Content-Language</span><span class="sxs-lookup"><span data-stu-id="52f84-132">Content-Language</span></span>  | <span data-ttu-id="52f84-133">Localidade.</span><span class="sxs-lookup"><span data-stu-id="52f84-133">Locale.</span></span> <span data-ttu-id="52f84-134">Opcional.</span><span class="sxs-lookup"><span data-stu-id="52f84-134">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="52f84-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52f84-135">Request body</span></span>

<span data-ttu-id="52f84-136">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="52f84-136">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="52f84-137">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="52f84-137">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="52f84-138">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="52f84-138">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="52f84-139">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52f84-139">Property</span></span>     | <span data-ttu-id="52f84-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="52f84-140">Type</span></span>        | <span data-ttu-id="52f84-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="52f84-141">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="52f84-142">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="52f84-142">backgroundColor</span></span>|<span data-ttu-id="52f84-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52f84-143">String</span></span>|<span data-ttu-id="52f84-144">Cor que aparecerá no lugar da imagem de plano de fundo em conexões de baixa largura de banda.</span><span class="sxs-lookup"><span data-stu-id="52f84-144">Color that will appear in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="52f84-145">A cor primária do logotipo da faixa ou da cor da sua organização é recomendada para ser usada aqui.</span><span class="sxs-lookup"><span data-stu-id="52f84-145">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="52f84-146">Especifique isso em hexadecimal (por exemplo, branco é #FFFFFF).</span><span class="sxs-lookup"><span data-stu-id="52f84-146">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span>|
|<span data-ttu-id="52f84-147">backgroundImage</span><span class="sxs-lookup"><span data-stu-id="52f84-147">backgroundImage</span></span>|<span data-ttu-id="52f84-148">Stream</span><span class="sxs-lookup"><span data-stu-id="52f84-148">Stream</span></span>|<span data-ttu-id="52f84-149">Imagem que aparece como o plano de fundo da página de logom.</span><span class="sxs-lookup"><span data-stu-id="52f84-149">Image that appears as the background of the sign in page.</span></span> <span data-ttu-id="52f84-150">.png ou .jpg não maior que 1920x1080 e menor que 300kb.</span><span class="sxs-lookup"><span data-stu-id="52f84-150">.png or .jpg not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="52f84-151">Uma imagem menor reduzirá os requisitos de largura de banda e tornará as cargas de página mais performant.</span><span class="sxs-lookup"><span data-stu-id="52f84-151">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span>|
|<span data-ttu-id="52f84-152">bannerLogo</span><span class="sxs-lookup"><span data-stu-id="52f84-152">bannerLogo</span></span>|<span data-ttu-id="52f84-153">Stream</span><span class="sxs-lookup"><span data-stu-id="52f84-153">Stream</span></span>|<span data-ttu-id="52f84-154">Uma versão em faixa do logotipo da sua empresa que aparece na página de entrada.</span><span class="sxs-lookup"><span data-stu-id="52f84-154">A banner version of your company logo which appears appears on the sign-in page.</span></span> <span data-ttu-id="52f84-155">.png ou .jpg não maior que 36x245px.</span><span class="sxs-lookup"><span data-stu-id="52f84-155">.png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="52f84-156">Recomendamos usar uma imagem transparente sem preenchimento ao redor do logotipo.</span><span class="sxs-lookup"><span data-stu-id="52f84-156">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="52f84-157">signInPageText</span><span class="sxs-lookup"><span data-stu-id="52f84-157">signInPageText</span></span>|<span data-ttu-id="52f84-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52f84-158">String</span></span>|<span data-ttu-id="52f84-159">Texto que aparece na parte inferior da caixa de login.</span><span class="sxs-lookup"><span data-stu-id="52f84-159">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="52f84-160">Você pode usar isso para comunicar informações adicionais, como o número de telefone para o seu help desk ou uma declaração legal.</span><span class="sxs-lookup"><span data-stu-id="52f84-160">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="52f84-161">Este texto deve ser Unicode e não exceder 1024 caracteres.</span><span class="sxs-lookup"><span data-stu-id="52f84-161">This text must be Unicode and not exceed 1024 characters.</span></span>|
|<span data-ttu-id="52f84-162">squareLogo</span><span class="sxs-lookup"><span data-stu-id="52f84-162">squareLogo</span></span>|<span data-ttu-id="52f84-163">Stream</span><span class="sxs-lookup"><span data-stu-id="52f84-163">Stream</span></span>|<span data-ttu-id="52f84-164">Versão quadrada do logotipo da sua empresa.</span><span class="sxs-lookup"><span data-stu-id="52f84-164">Square version of your company logo.</span></span> <span data-ttu-id="52f84-165">Isso aparece nas experiências OOBE (windows 10 out-of-box) e quando o Windows Autopilot está habilitado para implantação.</span><span class="sxs-lookup"><span data-stu-id="52f84-165">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="52f84-166">.png ou .jpg não maior do que 240x240px e no máximo 10kb de tamanho.</span><span class="sxs-lookup"><span data-stu-id="52f84-166">.png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="52f84-167">Recomendamos usar uma imagem transparente sem preenchimento ao redor do logotipo.</span><span class="sxs-lookup"><span data-stu-id="52f84-167">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="52f84-168">usernameHintText</span><span class="sxs-lookup"><span data-stu-id="52f84-168">usernameHintText</span></span>|<span data-ttu-id="52f84-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52f84-169">String</span></span>|<span data-ttu-id="52f84-170">Cadeia de caracteres que mostra como a dica na caixa de texto do nome de usuário na tela de entrada.</span><span class="sxs-lookup"><span data-stu-id="52f84-170">String that shows as the hint in the username textbox on the sign in screen.</span></span> <span data-ttu-id="52f84-171">Este texto deve ser Unicode, sem links ou código, e não pode exceder 64 caracteres.</span><span class="sxs-lookup"><span data-stu-id="52f84-171">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span>|
|<span data-ttu-id="52f84-172">id</span><span class="sxs-lookup"><span data-stu-id="52f84-172">id</span></span>|<span data-ttu-id="52f84-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52f84-173">String</span></span>|<span data-ttu-id="52f84-174">Localidade para criar identidade visual para</span><span class="sxs-lookup"><span data-stu-id="52f84-174">Locale to create branding for</span></span>|

## <a name="response"></a><span data-ttu-id="52f84-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="52f84-175">Response</span></span>

<span data-ttu-id="52f84-176">Se tiver êxito, este método retornará um código `201 CREATED` de resposta e o objeto [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) criado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52f84-176">If successful, this method returns a `201 CREATED` response code and the created [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="52f84-177">Exemplos</span><span class="sxs-lookup"><span data-stu-id="52f84-177">Examples</span></span>

<span data-ttu-id="52f84-178">O exemplo a seguir cria uma localização de identidade visual para francês (fr).</span><span class="sxs-lookup"><span data-stu-id="52f84-178">The following example creates a branding localization for French (fr).</span></span>

### <a name="request"></a><span data-ttu-id="52f84-179">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52f84-179">Request</span></span>

<span data-ttu-id="52f84-180">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="52f84-180">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="52f84-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="52f84-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_7"
}-->

```http
POST https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "id": "fr"
}
```
# <a name="c"></a>[<span data-ttu-id="52f84-182">C#</span><span class="sxs-lookup"><span data-stu-id="52f84-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-7-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="52f84-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52f84-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-7-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="52f84-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="52f84-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-7-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="52f84-185">Java</span><span class="sxs-lookup"><span data-stu-id="52f84-185">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-7-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="52f84-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="52f84-186">Response</span></span>

<span data-ttu-id="52f84-187">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="52f84-187">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "backgroundImage@odata.mediaContentType":"image/*",
    "backgroundImage@odata.mediaReadLink": null,
    "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/backgroundImage",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": null,
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
    "id": "fr",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": null,
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/squareLogo"
}
```
<span data-ttu-id="52f84-188">O **mediaEditLink** especifica onde a mídia localizada é escrita.</span><span class="sxs-lookup"><span data-stu-id="52f84-188">The **mediaEditLink** specifies where the localized media is written.</span></span> <span data-ttu-id="52f84-189">O mediaReadLink é nulo porque nenhuma mídia foi definida para a localização.</span><span class="sxs-lookup"><span data-stu-id="52f84-189">The mediaReadLink is null because no media has been set for the localization.</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
