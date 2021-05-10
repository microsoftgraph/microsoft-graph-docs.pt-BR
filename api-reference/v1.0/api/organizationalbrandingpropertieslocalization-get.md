---
title: Obter organizationalBrandingProperties localizadas
description: Recupere o objeto organizationalbrandingproperties para uma localidade específica.
localization_priority: Normal
author: almars
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8760803c6363cacfe41d239c6031a7e81c18492f
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52298720"
---
# <a name="get-localized-organizationalbrandingproperties"></a><span data-ttu-id="e5022-103">Get Localized organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="e5022-103">Get Localized organizationalBrandingProperties</span></span>

<span data-ttu-id="e5022-104">Recupere as propriedades do [objeto organizationalBrandingProperties.](../resources/organizationalbrandingproperties.md)</span><span class="sxs-lookup"><span data-stu-id="e5022-104">Retrieve the properties of the [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5022-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e5022-105">Permissions</span></span>

<span data-ttu-id="e5022-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5022-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e5022-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5022-108">Permission type</span></span>                        | <span data-ttu-id="e5022-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e5022-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e5022-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5022-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="e5022-111">Organization.Read.All, User.Read, User.Read.All, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="e5022-111">Organization.Read.All, User.Read, User.Read.All, User.ReadBasic.All</span></span> |
| <span data-ttu-id="e5022-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5022-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5022-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5022-113">Not supported.</span></span> |
| <span data-ttu-id="e5022-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5022-114">Application</span></span>                            | <span data-ttu-id="e5022-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5022-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5022-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5022-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{tenant id}/branding/localizations/{locale}
```

## <a name="request-headers"></a><span data-ttu-id="e5022-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e5022-117">Request headers</span></span>

| <span data-ttu-id="e5022-118">Nome</span><span class="sxs-lookup"><span data-stu-id="e5022-118">Name</span></span>      |<span data-ttu-id="e5022-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5022-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e5022-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="e5022-120">Authorization</span></span> | <span data-ttu-id="e5022-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e5022-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e5022-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e5022-123">Content-Type</span></span>  | <span data-ttu-id="e5022-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e5022-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e5022-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5022-126">Request body</span></span>

<span data-ttu-id="e5022-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e5022-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5022-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5022-128">Response</span></span>

<span data-ttu-id="e5022-129">Se tiver êxito, este método retornará um código de `200 OK` resposta e o objeto [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5022-129">If successful, this method returns a `200 OK` response code and the requested [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span> <span data-ttu-id="e5022-130">O valor de "id" corresponde à localização solicitada.</span><span class="sxs-lookup"><span data-stu-id="e5022-130">The value of "id" corresponds to the localization requested.</span></span>

## <a name="examples"></a><span data-ttu-id="e5022-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e5022-131">Examples</span></span>
### <a name="example-1-get-the-localized-branding-for-a-specific-locale-fr"></a><span data-ttu-id="e5022-132">Exemplo 1: Obter a identidade visual localizada para uma localidade específica (fr)</span><span class="sxs-lookup"><span data-stu-id="e5022-132">Example 1: Get the localized branding for a specific locale (fr)</span></span>
<span data-ttu-id="e5022-133">Uma solicitação GET para uma localização específica retorna apenas os valores dessa localização.</span><span class="sxs-lookup"><span data-stu-id="e5022-133">A GET request to a particular localization returns only the values for that localization.</span></span> <span data-ttu-id="e5022-134">Os valores nulos não serão substituídos por aqueles da identidade visual padrão.</span><span class="sxs-lookup"><span data-stu-id="e5022-134">Null values will not be replaced by those from the default branding.</span></span>
#### <a name="request"></a><span data-ttu-id="e5022-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5022-135">Request</span></span>

<span data-ttu-id="e5022-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5022-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e5022-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5022-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_8"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
```
# <a name="c"></a>[<span data-ttu-id="e5022-138">C#</span><span class="sxs-lookup"><span data-stu-id="e5022-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-8-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5022-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5022-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-8-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5022-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5022-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-8-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e5022-141">Java</span><span class="sxs-lookup"><span data-stu-id="e5022-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-8-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e5022-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5022-142">Response</span></span>

<span data-ttu-id="e5022-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e5022-143">The following is an example of the response.</span></span>

> <span data-ttu-id="e5022-144">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e5022-144">**Note:** The response object shown here might be shortened for readability.</span></span>

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
"backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/backgroundImage",
"bannerLogo@odata.mediaContentType":"image/*",
"bannerLogo@odata.mediaReadLink": null,
"bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
"id":"fr",
"squareLogo@odata.mediaContentType":"image/*",
"squareLogo@odata.mediaReadLink": null,
"squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/squareLogo",
"signInPageText":null,
"usernameHintText":null
}
```

### <a name="example-2-get-all-language-specific-localizations-that-have-been-configured"></a><span data-ttu-id="e5022-145">Exemplo 2: Obter todas as localizações específicas do idioma que foram configuradas</span><span class="sxs-lookup"><span data-stu-id="e5022-145">Example 2: Get all language-specific localizations that have been configured</span></span>
#### <a name="request"></a><span data-ttu-id="e5022-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5022-146">Request</span></span>

<span data-ttu-id="e5022-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5022-147">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e5022-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5022-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_9"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations
```
# <a name="c"></a>[<span data-ttu-id="e5022-149">C#</span><span class="sxs-lookup"><span data-stu-id="e5022-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-9-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5022-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5022-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-9-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5022-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5022-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-9-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e5022-152">Java</span><span class="sxs-lookup"><span data-stu-id="e5022-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-9-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e5022-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5022-153">Response</span></span>

<span data-ttu-id="e5022-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e5022-154">The following is an example of the response.</span></span>

> <span data-ttu-id="e5022-155">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e5022-155">**Note:** The response object shown here might be shortened for readability.</span></span>

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
    "backgroundImage@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/backgroundImage",
    "backgroundImage@odata.mediaEditLink":"https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/backgroundImage",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": null,
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/bannerLogo",
    "id":"en-us",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": null,
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/squareLogo",
    "signInPageText":"Welcome",
    "usernameHintText":"hint"
   },
   {
    "backgroundColor":"#00000F",
    "backgroundImage@odata.mediaContentType":"image/*",
    "backgroundImage@odata.mediaReadLink": null,
    "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": null,
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
    "id":"fr",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": null,
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/squareLogo",
    "signInPageText":null,
    "usernameHintText":null
   }
 ]
}
```

### <a name="example-3-get-the-value-of-signinpagetext-for-a-specific-locale"></a><span data-ttu-id="e5022-156">Exemplo 3: Obter o valor de signInPageText para uma localidade específica</span><span class="sxs-lookup"><span data-stu-id="e5022-156">Example 3: Get the value of signInPageText for a specific locale</span></span>
<span data-ttu-id="e5022-157">Solicitar uma propriedade de uma localização retorna esse valor ou 204 se o valor for nulo.</span><span class="sxs-lookup"><span data-stu-id="e5022-157">Requesting a property of a localization returns that value, or 204 if the value is null.</span></span>
#### <a name="request"></a><span data-ttu-id="e5022-158">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5022-158">Request</span></span>

<span data-ttu-id="e5022-159">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5022-159">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e5022-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5022-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_10"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/signInPageText
```
# <a name="c"></a>[<span data-ttu-id="e5022-161">C#</span><span class="sxs-lookup"><span data-stu-id="e5022-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-10-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5022-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5022-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-10-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5022-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5022-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-10-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e5022-164">Java</span><span class="sxs-lookup"><span data-stu-id="e5022-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-10-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e5022-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5022-165">Response</span></span>

<span data-ttu-id="e5022-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e5022-166">The following is an example of the response.</span></span>

> <span data-ttu-id="e5022-167">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e5022-167">**Note:** The response object shown here might be shortened for readability.</span></span>

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
