---
title: Criar organizationalBrandingProperties localizados
description: Crie a identidade visual da organização para uma localidade específica.
localization_priority: Normal
author: almars
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 4d06254d44f42ec7460d51f571fd5fe9b62e3b71
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52298488"
---
# <a name="create-localized-organizationalbrandingproperties"></a><span data-ttu-id="97585-103">Criar organizationalBrandingProperties localizados</span><span class="sxs-lookup"><span data-stu-id="97585-103">Create localized organizationalBrandingProperties</span></span>

<span data-ttu-id="97585-104">Crie um [objeto organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) para uma localidade específica.</span><span class="sxs-lookup"><span data-stu-id="97585-104">Create an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object for a specific locale.</span></span>

## <a name="permissions"></a><span data-ttu-id="97585-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="97585-105">Permissions</span></span>

<span data-ttu-id="97585-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97585-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="97585-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97585-108">Permission type</span></span>                        | <span data-ttu-id="97585-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="97585-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="97585-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97585-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="97585-111">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97585-111">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="97585-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97585-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97585-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97585-113">Not supported.</span></span> |
| <span data-ttu-id="97585-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97585-114">Application</span></span>                            | <span data-ttu-id="97585-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97585-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="97585-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97585-116">HTTP request</span></span>

<span data-ttu-id="97585-117">POST para identidade visual/localizações para criar uma nova localização.</span><span class="sxs-lookup"><span data-stu-id="97585-117">POST to branding/localizations to create a new localization.</span></span> <span data-ttu-id="97585-118">A id especificada no corpo é a localidade da localização.</span><span class="sxs-lookup"><span data-stu-id="97585-118">The id specified in the body is the locale for the localization.</span></span> <span data-ttu-id="97585-119">Se nenhuma id for especificada, o valor do header Content-Language, se especificado, será usado como id. Se nenhuma id e nenhum header content-Language for especificado, um erro será retornado.</span><span class="sxs-lookup"><span data-stu-id="97585-119">If no id is specified, then the value of the Content-Language header, if specified, is used as the id. If no id and no Content-Language header is specified, then an error is returned.</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /organization/{tenant id}/branding/localizations
```

## <a name="request-headers"></a><span data-ttu-id="97585-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97585-120">Request headers</span></span>

| <span data-ttu-id="97585-121">Nome</span><span class="sxs-lookup"><span data-stu-id="97585-121">Name</span></span>      |<span data-ttu-id="97585-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="97585-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="97585-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="97585-123">Authorization</span></span> | <span data-ttu-id="97585-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97585-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="97585-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="97585-126">Content-Type</span></span>  | <span data-ttu-id="97585-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97585-p104">application/json. Required.</span></span>  |
| <span data-ttu-id="97585-129">Content-Language</span><span class="sxs-lookup"><span data-stu-id="97585-129">Content-Language</span></span>  | <span data-ttu-id="97585-130">Localidade.</span><span class="sxs-lookup"><span data-stu-id="97585-130">Locale.</span></span> <span data-ttu-id="97585-131">Opcional.</span><span class="sxs-lookup"><span data-stu-id="97585-131">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="97585-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97585-132">Request body</span></span>

<span data-ttu-id="97585-133">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="97585-133">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="97585-134">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="97585-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="97585-135">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="97585-135">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="97585-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97585-136">Property</span></span>     | <span data-ttu-id="97585-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="97585-137">Type</span></span>        | <span data-ttu-id="97585-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="97585-138">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="97585-139">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="97585-139">backgroundColor</span></span>|<span data-ttu-id="97585-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="97585-140">String</span></span>|<span data-ttu-id="97585-141">Cor que aparecerá no lugar da imagem de plano de fundo em conexões de baixa largura de banda.</span><span class="sxs-lookup"><span data-stu-id="97585-141">Color that will appear in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="97585-142">A cor primária do logotipo da faixa ou da cor da sua organização é recomendada para ser usada aqui.</span><span class="sxs-lookup"><span data-stu-id="97585-142">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="97585-143">Especifique isso em hexadecimal (por exemplo, branco é #FFFFFF).</span><span class="sxs-lookup"><span data-stu-id="97585-143">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span>|
|<span data-ttu-id="97585-144">backgroundImage</span><span class="sxs-lookup"><span data-stu-id="97585-144">backgroundImage</span></span>|<span data-ttu-id="97585-145">Stream</span><span class="sxs-lookup"><span data-stu-id="97585-145">Stream</span></span>|<span data-ttu-id="97585-146">Imagem que aparece como o plano de fundo da página de logom.</span><span class="sxs-lookup"><span data-stu-id="97585-146">Image that appears as the background of the sign in page.</span></span> <span data-ttu-id="97585-147">.png ou .jpg maior que 1920x1080 e menor que 300kb.</span><span class="sxs-lookup"><span data-stu-id="97585-147">.png or .jpg not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="97585-148">Uma imagem menor reduzirá os requisitos de largura de banda e tornará as cargas de página mais performant.</span><span class="sxs-lookup"><span data-stu-id="97585-148">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span>|
|<span data-ttu-id="97585-149">bannerLogo</span><span class="sxs-lookup"><span data-stu-id="97585-149">bannerLogo</span></span>|<span data-ttu-id="97585-150">Stream</span><span class="sxs-lookup"><span data-stu-id="97585-150">Stream</span></span>|<span data-ttu-id="97585-151">Uma versão em faixa do logotipo da sua empresa que aparece na página de entrada.</span><span class="sxs-lookup"><span data-stu-id="97585-151">A banner version of your company logo which appears appears on the sign-in page.</span></span> <span data-ttu-id="97585-152">.png ou .jpg maior que 36x245px.</span><span class="sxs-lookup"><span data-stu-id="97585-152">.png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="97585-153">Recomendamos usar uma imagem transparente sem preenchimento ao redor do logotipo.</span><span class="sxs-lookup"><span data-stu-id="97585-153">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="97585-154">signInPageText</span><span class="sxs-lookup"><span data-stu-id="97585-154">signInPageText</span></span>|<span data-ttu-id="97585-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="97585-155">String</span></span>|<span data-ttu-id="97585-156">Texto que aparece na parte inferior da caixa de login.</span><span class="sxs-lookup"><span data-stu-id="97585-156">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="97585-157">Você pode usar isso para comunicar informações adicionais, como o número de telefone para o seu help desk ou uma declaração legal.</span><span class="sxs-lookup"><span data-stu-id="97585-157">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="97585-158">Este texto deve ser Unicode e não exceder 1024 caracteres.</span><span class="sxs-lookup"><span data-stu-id="97585-158">This text must be Unicode and not exceed 1024 characters.</span></span>|
|<span data-ttu-id="97585-159">squareLogo</span><span class="sxs-lookup"><span data-stu-id="97585-159">squareLogo</span></span>|<span data-ttu-id="97585-160">Stream</span><span class="sxs-lookup"><span data-stu-id="97585-160">Stream</span></span>|<span data-ttu-id="97585-161">Versão quadrada do logotipo da sua empresa.</span><span class="sxs-lookup"><span data-stu-id="97585-161">Square version of your company logo.</span></span> <span data-ttu-id="97585-162">Isso aparece em Windows 10 experiências OOBE (out-of-box) e quando Windows Autopilot está habilitado para implantação.</span><span class="sxs-lookup"><span data-stu-id="97585-162">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="97585-163">.png ou .jpg maior que 240x240px e não mais de 10kb de tamanho.</span><span class="sxs-lookup"><span data-stu-id="97585-163">.png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="97585-164">Recomendamos usar uma imagem transparente sem preenchimento ao redor do logotipo.</span><span class="sxs-lookup"><span data-stu-id="97585-164">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="97585-165">usernameHintText</span><span class="sxs-lookup"><span data-stu-id="97585-165">usernameHintText</span></span>|<span data-ttu-id="97585-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="97585-166">String</span></span>|<span data-ttu-id="97585-167">Cadeia de caracteres que mostra como a dica na caixa de texto do nome de usuário na tela de entrada.</span><span class="sxs-lookup"><span data-stu-id="97585-167">String that shows as the hint in the username textbox on the sign in screen.</span></span> <span data-ttu-id="97585-168">Este texto deve ser Unicode, sem links ou código, e não pode exceder 64 caracteres.</span><span class="sxs-lookup"><span data-stu-id="97585-168">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span>|
|<span data-ttu-id="97585-169">id</span><span class="sxs-lookup"><span data-stu-id="97585-169">id</span></span>|<span data-ttu-id="97585-170">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="97585-170">String</span></span>|<span data-ttu-id="97585-171">Localidade para criar identidade visual para</span><span class="sxs-lookup"><span data-stu-id="97585-171">Locale to create branding for</span></span>|

## <a name="response"></a><span data-ttu-id="97585-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="97585-172">Response</span></span>

<span data-ttu-id="97585-173">Se tiver êxito, este método retornará um código `201 Created` de resposta e o objeto [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) criado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97585-173">If successful, this method returns a `201 Created` response code and the created [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="97585-174">Exemplos</span><span class="sxs-lookup"><span data-stu-id="97585-174">Examples</span></span>

<span data-ttu-id="97585-175">O exemplo a seguir cria uma localização de identidade visual para francês (fr).</span><span class="sxs-lookup"><span data-stu-id="97585-175">The following example creates a branding localization for French (fr).</span></span>

### <a name="request"></a><span data-ttu-id="97585-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97585-176">Request</span></span>

<span data-ttu-id="97585-177">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="97585-177">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="97585-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="97585-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_7"
}-->

```http
POST https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "id": "fr"
}
```
# <a name="c"></a>[<span data-ttu-id="97585-179">C#</span><span class="sxs-lookup"><span data-stu-id="97585-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-7-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="97585-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="97585-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-7-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="97585-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="97585-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-7-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="97585-182">Java</span><span class="sxs-lookup"><span data-stu-id="97585-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-7-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="97585-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="97585-183">Response</span></span>

<span data-ttu-id="97585-184">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="97585-184">The following is an example of the response.</span></span>

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
    "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/backgroundImage",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": null,
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
    "id": "fr",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": null,
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/squareLogo"
}
```
<span data-ttu-id="97585-185">O **mediaEditLink** especifica onde a mídia localizada é escrita.</span><span class="sxs-lookup"><span data-stu-id="97585-185">The **mediaEditLink** specifies where the localized media is written.</span></span> <span data-ttu-id="97585-186">O mediaReadLink é nulo porque nenhuma mídia foi definida para a localização.</span><span class="sxs-lookup"><span data-stu-id="97585-186">The mediaReadLink is null because no media has been set for the localization.</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
