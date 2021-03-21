---
title: Obter organizationalBrandingProperties localizadas
description: Recupere o objeto organizationalbrandingproperties para uma localidade específica.
localization_priority: Normal
author: kexia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 17d55e9c98eedad91b544c16b2e3ca39163adbe0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963070"
---
# <a name="get-localized-organizationalbrandingproperties"></a><span data-ttu-id="8e3e0-103">Get Localized organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="8e3e0-103">Get Localized organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e3e0-104">Recupere as propriedades do [objeto organizationalBrandingProperties.](../resources/organizationalbrandingproperties.md)</span><span class="sxs-lookup"><span data-stu-id="8e3e0-104">Retrieve the properties of the [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8e3e0-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8e3e0-105">Permissions</span></span>

<span data-ttu-id="8e3e0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e3e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8e3e0-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8e3e0-108">Permission type</span></span>                        | <span data-ttu-id="8e3e0-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8e3e0-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8e3e0-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8e3e0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="8e3e0-111">Organization.Read.All, User.Read, User.Read.All, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="8e3e0-111">Organization.Read.All, User.Read, User.Read.All, User.ReadBasic.All</span></span> |
| <span data-ttu-id="8e3e0-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8e3e0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8e3e0-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e3e0-113">Not supported.</span></span> |
| <span data-ttu-id="8e3e0-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8e3e0-114">Application</span></span>                            | <span data-ttu-id="8e3e0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8e3e0-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8e3e0-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8e3e0-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/branding/localizations/{locale}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8e3e0-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8e3e0-117">Optional query parameters</span></span>

<span data-ttu-id="8e3e0-118">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8e3e0-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="8e3e0-119">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8e3e0-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8e3e0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e3e0-120">Request headers</span></span>

| <span data-ttu-id="8e3e0-121">Nome</span><span class="sxs-lookup"><span data-stu-id="8e3e0-121">Name</span></span>      |<span data-ttu-id="8e3e0-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e3e0-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8e3e0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8e3e0-123">Authorization</span></span> | <span data-ttu-id="8e3e0-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e3e0-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8e3e0-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8e3e0-126">Content-Type</span></span>  | <span data-ttu-id="8e3e0-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8e3e0-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8e3e0-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8e3e0-129">Request body</span></span>

<span data-ttu-id="8e3e0-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8e3e0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8e3e0-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e3e0-131">Response</span></span>

<span data-ttu-id="8e3e0-132">Se tiver êxito, este método retornará um código de `200 OK` resposta e o objeto [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8e3e0-132">If successful, this method returns a `200 OK` response code and the requested [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span> <span data-ttu-id="8e3e0-133">O valor de "id" corresponde à localização solicitada.</span><span class="sxs-lookup"><span data-stu-id="8e3e0-133">The value of "id" corresponds to the localization requested.</span></span>

## <a name="examples"></a><span data-ttu-id="8e3e0-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8e3e0-134">Examples</span></span>
### <a name="example-1-get-the-localized-branding-for-a-specific-locale-fr"></a><span data-ttu-id="8e3e0-135">Exemplo 1: Obter a identidade visual localizada para uma localidade específica (fr)</span><span class="sxs-lookup"><span data-stu-id="8e3e0-135">Example 1: Get the localized branding for a specific locale (fr)</span></span>
<span data-ttu-id="8e3e0-136">Uma solicitação GET para uma localização específica retorna apenas os valores dessa localização.</span><span class="sxs-lookup"><span data-stu-id="8e3e0-136">A GET request to a particular localization returns only the values for that localization.</span></span> <span data-ttu-id="8e3e0-137">Os valores nulos não serão substituídos por aqueles da identidade visual padrão.</span><span class="sxs-lookup"><span data-stu-id="8e3e0-137">Null values will not be replaced by those from the default branding.</span></span>
#### <a name="request"></a><span data-ttu-id="8e3e0-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e3e0-138">Request</span></span>

<span data-ttu-id="8e3e0-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e3e0-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8e3e0-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e3e0-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_8"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
```
# <a name="c"></a>[<span data-ttu-id="8e3e0-141">C#</span><span class="sxs-lookup"><span data-stu-id="8e3e0-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-8-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e3e0-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e3e0-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-8-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e3e0-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e3e0-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-8-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e3e0-144">Java</span><span class="sxs-lookup"><span data-stu-id="8e3e0-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-8-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8e3e0-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e3e0-145">Response</span></span>

<span data-ttu-id="8e3e0-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8e3e0-146">The following is an example of the response.</span></span>

> <span data-ttu-id="8e3e0-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8e3e0-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
"backgroundColor":"#00000F",
"backgroundImage@odata.mediaContentType":"image/*",
"backgroundImage@odata.mediaReadLink": null,
"backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/backgroundImage",
"bannerLogo@odata.mediaContentType":"image/*",
"bannerLogo@odata.mediaReadLink": null,
"bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
"id":"fr",
"squareLogo@odata.mediaContentType":"image/*",
"squareLogo@odata.mediaReadLink": null,
"squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/squareLogo",
"signInPageText":null,
"usernameHintText":null
}
```

### <a name="example-2-get-all-language-specific-localizations-that-have-been-configured"></a><span data-ttu-id="8e3e0-149">Exemplo 2: Obter todas as localizações específicas do idioma que foram configuradas</span><span class="sxs-lookup"><span data-stu-id="8e3e0-149">Example 2: Get all language-specific localizations that have been configured</span></span>
#### <a name="request"></a><span data-ttu-id="8e3e0-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e3e0-150">Request</span></span>

<span data-ttu-id="8e3e0-151">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e3e0-151">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8e3e0-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e3e0-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_9"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations
```
# <a name="c"></a>[<span data-ttu-id="8e3e0-153">C#</span><span class="sxs-lookup"><span data-stu-id="8e3e0-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-9-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e3e0-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e3e0-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-9-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e3e0-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e3e0-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-9-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e3e0-156">Java</span><span class="sxs-lookup"><span data-stu-id="8e3e0-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-9-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8e3e0-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e3e0-157">Response</span></span>

<span data-ttu-id="8e3e0-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8e3e0-158">The following is an example of the response.</span></span>

> <span data-ttu-id="8e3e0-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8e3e0-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
 "values": [
   {
    "backgroundColor":"#FFFF33",
    "backgroundImage@odata.mediaContentType":"image/*",
    "backgroundImage@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/backgroundImage",
    "backgroundImage@odata.mediaEditLink":"https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/backgroundImage",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": null,
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/bannerLogo",
    "id":"en-us",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": null,
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/squareLogo",
    "signInPageText":"Welcome",
    "usernameHintText":"hint"
   },
   {
    "backgroundColor":"#00000F",
    "backgroundImage@odata.mediaContentType":"image/*",
    "backgroundImage@odata.mediaReadLink": null,
    "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": null,
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
    "id":"fr",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": null,
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/squareLogo",
    "signInPageText":null,
    "usernameHintText":null
   }
 ]
}
```

### <a name="example-3-get-the-value-of-signinpagetext-for-a-specific-locale"></a><span data-ttu-id="8e3e0-161">Exemplo 3: Obter o valor de signInPageText para uma localidade específica</span><span class="sxs-lookup"><span data-stu-id="8e3e0-161">Example 3: Get the value of signInPageText for a specific locale</span></span>
<span data-ttu-id="8e3e0-162">Solicitar uma propriedade de uma localização retorna esse valor ou 204 se o valor for nulo.</span><span class="sxs-lookup"><span data-stu-id="8e3e0-162">Requesting a property of a localization returns that value, or 204 if the value is null.</span></span>
#### <a name="request"></a><span data-ttu-id="8e3e0-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8e3e0-163">Request</span></span>

<span data-ttu-id="8e3e0-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8e3e0-164">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8e3e0-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="8e3e0-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_10"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/signInPageText
```
# <a name="c"></a>[<span data-ttu-id="8e3e0-166">C#</span><span class="sxs-lookup"><span data-stu-id="8e3e0-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-10-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8e3e0-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8e3e0-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-10-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8e3e0-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8e3e0-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-10-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8e3e0-169">Java</span><span class="sxs-lookup"><span data-stu-id="8e3e0-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-10-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8e3e0-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="8e3e0-170">Response</span></span>

<span data-ttu-id="8e3e0-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8e3e0-171">The following is an example of the response.</span></span>

> <span data-ttu-id="8e3e0-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8e3e0-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
"value":"Welcome"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
