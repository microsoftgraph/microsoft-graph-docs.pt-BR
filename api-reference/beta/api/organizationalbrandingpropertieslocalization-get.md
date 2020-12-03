---
title: Obter organizationalBrandingProperties localizado
description: Recupere o objeto organizationalbrandingproperties para uma localidade específica.
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9ca1f3459910a41b38632acafdab79be61025da3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49523907"
---
# <a name="get-localized-organizationalbrandingproperties"></a><span data-ttu-id="22fef-103">Obter organizationalBrandingProperties localizado</span><span class="sxs-lookup"><span data-stu-id="22fef-103">Get Localized organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22fef-104">Recupere as propriedades do objeto [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) .</span><span class="sxs-lookup"><span data-stu-id="22fef-104">Retrieve the properties of the [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="22fef-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="22fef-105">Permissions</span></span>

<span data-ttu-id="22fef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22fef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="22fef-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22fef-108">Permission type</span></span>                        | <span data-ttu-id="22fef-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="22fef-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="22fef-110">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22fef-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="22fef-111">Organization. Read. All, User. Read, User. Read. All, User. ReadBasic. All</span><span class="sxs-lookup"><span data-stu-id="22fef-111">Organization.Read.All, User.Read, User.Read.All, User.ReadBasic.All</span></span> |
| <span data-ttu-id="22fef-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22fef-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22fef-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22fef-113">Not supported.</span></span> |
| <span data-ttu-id="22fef-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="22fef-114">Application</span></span>                            | <span data-ttu-id="22fef-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22fef-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="22fef-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22fef-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/branding/localizations/{locale}/{property name}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="22fef-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="22fef-117">Optional query parameters</span></span>

<span data-ttu-id="22fef-118">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="22fef-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="22fef-119">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="22fef-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="22fef-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22fef-120">Request headers</span></span>

| <span data-ttu-id="22fef-121">Nome</span><span class="sxs-lookup"><span data-stu-id="22fef-121">Name</span></span>      |<span data-ttu-id="22fef-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="22fef-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="22fef-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="22fef-123">Authorization</span></span> | <span data-ttu-id="22fef-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22fef-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="22fef-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="22fef-126">Content-Type</span></span>  | <span data-ttu-id="22fef-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22fef-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="22fef-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22fef-129">Request body</span></span>

<span data-ttu-id="22fef-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="22fef-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22fef-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="22fef-131">Response</span></span>

<span data-ttu-id="22fef-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22fef-132">If successful, this method returns a `200 OK` response code and the requested [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span> <span data-ttu-id="22fef-133">O valor de "ID" corresponde à localização solicitada.</span><span class="sxs-lookup"><span data-stu-id="22fef-133">The value of "id" corresponds to the localization requested.</span></span>

## <a name="examples"></a><span data-ttu-id="22fef-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="22fef-134">Examples</span></span>
### <a name="example-1-get-the-localized-branding-for-a-specific-locale-fr"></a><span data-ttu-id="22fef-135">Exemplo 1: obter a identidade visual localizada para uma localidade específica (FR)</span><span class="sxs-lookup"><span data-stu-id="22fef-135">Example 1: Get the localized branding for a specific locale (fr)</span></span>
<span data-ttu-id="22fef-136">Uma solicitação GET para uma determinada localização retorna apenas os valores dessa localização.</span><span class="sxs-lookup"><span data-stu-id="22fef-136">A GET request to a particular localization returns only the values for that localization.</span></span> <span data-ttu-id="22fef-137">Valores nulos não serão substituídos por aqueles da identidade visual padrão.</span><span class="sxs-lookup"><span data-stu-id="22fef-137">Null values will not be replaced by those from the default branding.</span></span>
#### <a name="request"></a><span data-ttu-id="22fef-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22fef-138">Request</span></span>

<span data-ttu-id="22fef-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="22fef-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="22fef-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="22fef-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
```
# <a name="c"></a>[<span data-ttu-id="22fef-141">C#</span><span class="sxs-lookup"><span data-stu-id="22fef-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22fef-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22fef-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22fef-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22fef-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="22fef-144">Java</span><span class="sxs-lookup"><span data-stu-id="22fef-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="22fef-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="22fef-145">Response</span></span>

<span data-ttu-id="22fef-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="22fef-146">The following is an example of the response.</span></span>

> <span data-ttu-id="22fef-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22fef-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-all-language-specific-localizations-that-have-been-configured"></a><span data-ttu-id="22fef-149">Exemplo 2: obter todas as localizações específicas de idioma que foram configuradas</span><span class="sxs-lookup"><span data-stu-id="22fef-149">Example 2: Get all language-specific localizations that have been configured</span></span>
#### <a name="request"></a><span data-ttu-id="22fef-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22fef-150">Request</span></span>

<span data-ttu-id="22fef-151">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="22fef-151">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="22fef-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="22fef-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations
```
# <a name="c"></a>[<span data-ttu-id="22fef-153">C#</span><span class="sxs-lookup"><span data-stu-id="22fef-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22fef-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22fef-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22fef-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22fef-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="22fef-156">Java</span><span class="sxs-lookup"><span data-stu-id="22fef-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="22fef-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="22fef-157">Response</span></span>

<span data-ttu-id="22fef-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="22fef-158">The following is an example of the response.</span></span>

> <span data-ttu-id="22fef-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22fef-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-get-the-value-of-signinpagetext-for-a-specific-locale"></a><span data-ttu-id="22fef-161">Exemplo 3: obter o valor de signInPageText para uma localidade específica</span><span class="sxs-lookup"><span data-stu-id="22fef-161">Example 3: Get the value of signInPageText for a specific locale</span></span>
<span data-ttu-id="22fef-162">A solicitação de uma propriedade de uma localização retorna o valor ou 204 se o valor for NULL.</span><span class="sxs-lookup"><span data-stu-id="22fef-162">Requesting a property of a localization returns that value, or 204 if the value is null.</span></span>
#### <a name="request"></a><span data-ttu-id="22fef-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22fef-163">Request</span></span>

<span data-ttu-id="22fef-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="22fef-164">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="22fef-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="22fef-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/signInPageText
```
# <a name="c"></a>[<span data-ttu-id="22fef-166">C#</span><span class="sxs-lookup"><span data-stu-id="22fef-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22fef-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22fef-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22fef-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22fef-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="22fef-169">Java</span><span class="sxs-lookup"><span data-stu-id="22fef-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="22fef-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="22fef-170">Response</span></span>

<span data-ttu-id="22fef-171">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="22fef-171">The following is an example of the response.</span></span>

> <span data-ttu-id="22fef-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22fef-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
