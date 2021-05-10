---
title: Criar organizationalBrandingProperties
description: Criar identidade visual da organização.
localization_priority: Normal
author: almars
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 4443c6608d83b8c61f5116d6823a41db9058f757
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52298699"
---
# <a name="create-organizationalbrandingproperties"></a><span data-ttu-id="73a89-103">Criar organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="73a89-103">Create organizationalBrandingProperties</span></span>

<span data-ttu-id="73a89-104">Crie um [objeto organizationalBrandingProperties.](../resources/organizationalbrandingproperties.md)</span><span class="sxs-lookup"><span data-stu-id="73a89-104">Create an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span> <span data-ttu-id="73a89-105">Isso cria a identidade visual padrão e, opcionalmente, uma identidade visual localizada.</span><span class="sxs-lookup"><span data-stu-id="73a89-105">This creates the default branding and optionally a localized branding.</span></span> <span data-ttu-id="73a89-106">A identidade visual padrão é carregada quando um conjunto de identidade visual localizado não é configurado para o idioma do navegador do usuário.</span><span class="sxs-lookup"><span data-stu-id="73a89-106">The default branding is loaded when a localized branding set isn't configured for the user's browser language.</span></span>

## <a name="permissions"></a><span data-ttu-id="73a89-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="73a89-107">Permissions</span></span>

<span data-ttu-id="73a89-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73a89-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="73a89-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="73a89-110">Permission type</span></span>                        | <span data-ttu-id="73a89-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="73a89-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="73a89-112">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="73a89-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="73a89-113">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73a89-113">Organization.ReadWrite.All</span></span> |
| <span data-ttu-id="73a89-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="73a89-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73a89-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73a89-115">Not supported.</span></span> |
| <span data-ttu-id="73a89-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="73a89-116">Application</span></span>                            | <span data-ttu-id="73a89-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73a89-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="73a89-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="73a89-118">HTTP request</span></span>

<span data-ttu-id="73a89-119">Uma identidade visual é criada para uma organização, se ainda não existir, usando PUT ou PATCH.</span><span class="sxs-lookup"><span data-stu-id="73a89-119">A branding is created for an organization, if one does not already exist, using PUT or PATCH.</span></span>

<span data-ttu-id="73a89-120">Se a identidade visual já estiver configurada, PUT substituirá todos os valores existentes independentemente do que está no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="73a89-120">If branding is already configured, PUT overwrites all existing values regardless of what's in the request body.</span></span> <span data-ttu-id="73a89-121">PATCH apenas substitui os valores incluídos no corpo da solicitação, deixando os valores não incluídos inalterados.</span><span class="sxs-lookup"><span data-stu-id="73a89-121">PATCH only overwrites the values that are included in the request body, leaving the values not included unchanged.</span></span>

<span data-ttu-id="73a89-122">A `id` propriedade é ignorada em PUT/PATCH no singleton /branding.</span><span class="sxs-lookup"><span data-stu-id="73a89-122">The `id` property is ignored on PUT/PATCH to the /branding singleton.</span></span> <span data-ttu-id="73a89-123">Se **Content-Language** não for especificado, a identidade visual padrão será criada, o que corresponde a `id` um de `und` .</span><span class="sxs-lookup"><span data-stu-id="73a89-123">If **Content-Language** is not specified, the default branding is created, which corresponds to an `id` of `und`.</span></span> <span data-ttu-id="73a89-124">Se **Content-Language** for especificado, a identidade visual será criada para essa localidade.</span><span class="sxs-lookup"><span data-stu-id="73a89-124">If **Content-Language** is specified, branding is created for that locale.</span></span>
<!-- { "blockType": "ignored" } -->

```http
PUT /organization/{tenant id}/branding
PATCH /organization/{tenant id}/branding
```

## <a name="request-headers"></a><span data-ttu-id="73a89-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="73a89-125">Request headers</span></span>

| <span data-ttu-id="73a89-126">Nome</span><span class="sxs-lookup"><span data-stu-id="73a89-126">Name</span></span>      |<span data-ttu-id="73a89-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="73a89-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="73a89-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="73a89-128">Authorization</span></span> | <span data-ttu-id="73a89-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73a89-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="73a89-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="73a89-131">Content-Type</span></span>  | <span data-ttu-id="73a89-p106">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73a89-p106">application/json. Required.</span></span>  |
| <span data-ttu-id="73a89-134">Content-Language</span><span class="sxs-lookup"><span data-stu-id="73a89-134">Content-Language</span></span>  | <span data-ttu-id="73a89-135">Localidade.</span><span class="sxs-lookup"><span data-stu-id="73a89-135">Locale.</span></span> <span data-ttu-id="73a89-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="73a89-136">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="73a89-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="73a89-137">Request body</span></span>

<span data-ttu-id="73a89-138">No corpo da solicitação, inclua uma representação JSON de um [objeto organizationalBrandingProperties.](../resources/organizationalbrandingproperties.md)</span><span class="sxs-lookup"><span data-stu-id="73a89-138">In the request body, include a JSON representation of an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span> <span data-ttu-id="73a89-139">A tabela a seguir lista as propriedades necessárias.</span><span class="sxs-lookup"><span data-stu-id="73a89-139">The following table lists the required properties.</span></span>

| <span data-ttu-id="73a89-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73a89-140">Property</span></span>     | <span data-ttu-id="73a89-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="73a89-141">Type</span></span>        | <span data-ttu-id="73a89-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="73a89-142">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="73a89-143">backgroundColor</span><span class="sxs-lookup"><span data-stu-id="73a89-143">backgroundColor</span></span>|<span data-ttu-id="73a89-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73a89-144">String</span></span>|<span data-ttu-id="73a89-145">Cor que aparece no lugar da imagem de plano de fundo em conexões de baixa largura de banda.</span><span class="sxs-lookup"><span data-stu-id="73a89-145">Color that appears in place of the background image in low-bandwidth connections.</span></span> <span data-ttu-id="73a89-146">A cor primária do logotipo da faixa ou da cor da sua organização é recomendada para ser usada aqui.</span><span class="sxs-lookup"><span data-stu-id="73a89-146">The primary color of your banner logo or your organization color is recommended to be used here.</span></span> <span data-ttu-id="73a89-147">Especifique isso em hexadecimal (por exemplo, branco é #FFFFFF).</span><span class="sxs-lookup"><span data-stu-id="73a89-147">Specify this in hexadecimal (for example, white is #FFFFFF).</span></span>|
|<span data-ttu-id="73a89-148">backgroundImage</span><span class="sxs-lookup"><span data-stu-id="73a89-148">backgroundImage</span></span>|<span data-ttu-id="73a89-149">Stream</span><span class="sxs-lookup"><span data-stu-id="73a89-149">Stream</span></span>|<span data-ttu-id="73a89-150">Imagem que aparece como o plano de fundo da página de login.</span><span class="sxs-lookup"><span data-stu-id="73a89-150">Image that appears as the background of the sign-in page.</span></span> <span data-ttu-id="73a89-151">A imagem é uma .png ou .jpg que não é maior que 1920x1080 e menor que 300kb.</span><span class="sxs-lookup"><span data-stu-id="73a89-151">The image is a .png or .jpg that is not larger than 1920x1080 and smaller than 300kb.</span></span> <span data-ttu-id="73a89-152">Uma imagem menor reduzirá os requisitos de largura de banda e tornará as cargas de página mais performant.</span><span class="sxs-lookup"><span data-stu-id="73a89-152">A smaller image will reduce bandwidth requirements and make page loads more performant.</span></span>|
|<span data-ttu-id="73a89-153">bannerLogo</span><span class="sxs-lookup"><span data-stu-id="73a89-153">bannerLogo</span></span>|<span data-ttu-id="73a89-154">Stream</span><span class="sxs-lookup"><span data-stu-id="73a89-154">Stream</span></span>|<span data-ttu-id="73a89-155">Uma versão em faixa do logotipo da sua empresa que aparece na página de entrada.</span><span class="sxs-lookup"><span data-stu-id="73a89-155">A banner version of your company logo that appears on the sign-in page.</span></span> <span data-ttu-id="73a89-156">O banner é um .png ou .jpg não maior que 36x245px.</span><span class="sxs-lookup"><span data-stu-id="73a89-156">The banner is a .png or .jpg no larger than 36x245px.</span></span> <span data-ttu-id="73a89-157">Recomendamos usar uma imagem transparente sem preenchimento ao redor do logotipo.</span><span class="sxs-lookup"><span data-stu-id="73a89-157">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="73a89-158">signInPageText</span><span class="sxs-lookup"><span data-stu-id="73a89-158">signInPageText</span></span>|<span data-ttu-id="73a89-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73a89-159">String</span></span>|<span data-ttu-id="73a89-160">Texto que aparece na parte inferior da caixa de login.</span><span class="sxs-lookup"><span data-stu-id="73a89-160">Text that appears at the bottom of the sign-in box.</span></span> <span data-ttu-id="73a89-161">Você pode usar isso para comunicar informações adicionais, como o número de telefone para o seu help desk ou uma declaração legal.</span><span class="sxs-lookup"><span data-stu-id="73a89-161">You can use this to communicate additional information, such as the phone number to your help desk or a legal statement.</span></span> <span data-ttu-id="73a89-162">Este texto deve ser Unicode e não exceder 1024 caracteres.</span><span class="sxs-lookup"><span data-stu-id="73a89-162">This text must be Unicode and not exceed 1024 characters.</span></span>|
|<span data-ttu-id="73a89-163">squareLogo</span><span class="sxs-lookup"><span data-stu-id="73a89-163">squareLogo</span></span>|<span data-ttu-id="73a89-164">Stream</span><span class="sxs-lookup"><span data-stu-id="73a89-164">Stream</span></span>|<span data-ttu-id="73a89-165">Versão quadrada do logotipo da sua empresa.</span><span class="sxs-lookup"><span data-stu-id="73a89-165">Square version of your company logo.</span></span> <span data-ttu-id="73a89-166">Isso aparece em Windows 10 experiências OOBE (out-of-box) e quando Windows Autopilot está habilitado para implantação.</span><span class="sxs-lookup"><span data-stu-id="73a89-166">This appears in Windows 10 out-of-box (OOBE) experiences and when Windows Autopilot is enabled for deployment.</span></span> <span data-ttu-id="73a89-167">O logotipo é um .png ou .jpg não maior que 240x240px e não mais de 10kb de tamanho.</span><span class="sxs-lookup"><span data-stu-id="73a89-167">The logo is a .png or .jpg no larger than 240x240px and no more than 10kb in size.</span></span> <span data-ttu-id="73a89-168">Recomendamos usar uma imagem transparente sem preenchimento ao redor do logotipo.</span><span class="sxs-lookup"><span data-stu-id="73a89-168">We recommend using a transparent image with no padding around the logo.</span></span>|
|<span data-ttu-id="73a89-169">usernameHintText</span><span class="sxs-lookup"><span data-stu-id="73a89-169">usernameHintText</span></span>|<span data-ttu-id="73a89-170">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73a89-170">String</span></span>|<span data-ttu-id="73a89-171">A dica na caixa de texto nome de usuário na tela de entrada.</span><span class="sxs-lookup"><span data-stu-id="73a89-171">The hint in the username textbox on the sign-in screen.</span></span> <span data-ttu-id="73a89-172">Este texto deve ser Unicode, sem links ou código, e não pode exceder 64 caracteres.</span><span class="sxs-lookup"><span data-stu-id="73a89-172">This text must be Unicode, without links or code, and can't exceed 64 characters.</span></span>|

## <a name="response"></a><span data-ttu-id="73a89-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="73a89-173">Response</span></span>

<span data-ttu-id="73a89-174">Se tiver êxito, este método retornará um código `201 Created` de resposta e o objeto [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) criado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="73a89-174">If successful, this method returns a `201 Created` response code and the created [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="73a89-175">Exemplos</span><span class="sxs-lookup"><span data-stu-id="73a89-175">Examples</span></span>

<span data-ttu-id="73a89-176">O exemplo a seguir cria a identidade visual padrão e a localização onde **Content-Language** é `en-US` .</span><span class="sxs-lookup"><span data-stu-id="73a89-176">The following example creates default branding and localization where **Content-Language** is `en-US`.</span></span>

### <a name="request"></a><span data-ttu-id="73a89-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73a89-177">Request</span></span>

<span data-ttu-id="73a89-178">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="73a89-178">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="73a89-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="73a89-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_1"
}-->

```http
PUT https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json
Content-Language: en-US

{
    "backgroundColor":"#FFFF33",
    "signInPageText":"Welcome",
    "usernameHintText":"hint"
}
```
# <a name="c"></a>[<span data-ttu-id="73a89-180">C#</span><span class="sxs-lookup"><span data-stu-id="73a89-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="73a89-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73a89-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="73a89-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73a89-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="73a89-183">Java</span><span class="sxs-lookup"><span data-stu-id="73a89-183">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="73a89-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="73a89-184">Response</span></span>

<span data-ttu-id="73a89-185">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="73a89-185">The following is an example of the response.</span></span>

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
    "backgroundImage@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/backgroundImage",
    "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/backgroundImage",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo",
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/bannerLogo",
    "id": "und",
    "signInPageText":"Welcome",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/squareLogo",
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/squareLogo",
    "usernameHintText":"hint"
}
```

<span data-ttu-id="73a89-186">Nesse caso, o objeto de identidade visual padrão é definido.</span><span class="sxs-lookup"><span data-stu-id="73a89-186">In this case, the default branding object is set.</span></span> <span data-ttu-id="73a89-187">A identidade visual localizada para também é definida devido ao `en-US` header **Content-Language,** mesmo que o conjunto de identidade visual não seja `en-US` retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="73a89-187">Localized branding for `en-US` is also set due to the **Content-Language** header, even though the `en-US` branding set is not returned in the response.</span></span> <span data-ttu-id="73a89-188">O **header Content-Language** na solicitação é opcional e, se não estiver presente, define apenas a identidade visual padrão.</span><span class="sxs-lookup"><span data-stu-id="73a89-188">The **Content-Language** header in the request is optional, and if not present, only sets the default branding.</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
