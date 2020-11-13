---
title: Obter organizationalBrandingProperties localizado
description: Recupere o objeto organizationalbrandingproperties para uma localidade específica.
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 75ba4f8ef3202f95d7538ef6017d01e005db60c9
ms.sourcegitcommit: 40b0e58312819b69567f35ab894ee0d2989837ab
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/13/2020
ms.locfileid: "49031892"
---
# <a name="get-localized-organizationalbrandingproperties"></a><span data-ttu-id="b3e09-103">Obter organizationalBrandingProperties localizado</span><span class="sxs-lookup"><span data-stu-id="b3e09-103">Get Localized organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3e09-104">Recupere as propriedades do objeto [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) .</span><span class="sxs-lookup"><span data-stu-id="b3e09-104">Retrieve the properties of the [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3e09-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="b3e09-105">Permissions</span></span>

<span data-ttu-id="b3e09-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b3e09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b3e09-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b3e09-108">Permission type</span></span>                        | <span data-ttu-id="b3e09-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b3e09-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b3e09-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b3e09-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b3e09-111">Organization. Read. All, User. Read, User. Read. All, User. ReadBasic. All</span><span class="sxs-lookup"><span data-stu-id="b3e09-111">Organization.Read.All, User.Read, User.Read.All, User.ReadBasic.All</span></span> |
| <span data-ttu-id="b3e09-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b3e09-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3e09-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3e09-113">Not supported.</span></span> |
| <span data-ttu-id="b3e09-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b3e09-114">Application</span></span>                            | <span data-ttu-id="b3e09-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b3e09-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3e09-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b3e09-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/branding/localizations/{locale}/{property name}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b3e09-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b3e09-117">Optional query parameters</span></span>

<span data-ttu-id="b3e09-118">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b3e09-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b3e09-119">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b3e09-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b3e09-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b3e09-120">Request headers</span></span>

| <span data-ttu-id="b3e09-121">Nome</span><span class="sxs-lookup"><span data-stu-id="b3e09-121">Name</span></span>      |<span data-ttu-id="b3e09-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3e09-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b3e09-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b3e09-123">Authorization</span></span> | <span data-ttu-id="b3e09-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3e09-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b3e09-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b3e09-126">Content-Type</span></span>  | <span data-ttu-id="b3e09-p104">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b3e09-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b3e09-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b3e09-129">Request body</span></span>

<span data-ttu-id="b3e09-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b3e09-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3e09-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3e09-131">Response</span></span>

<span data-ttu-id="b3e09-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b3e09-132">If successful, this method returns a `200 OK` response code and the requested [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span> <span data-ttu-id="b3e09-133">O valor de "ID" corresponde à localização solicitada.</span><span class="sxs-lookup"><span data-stu-id="b3e09-133">The value of "id" corresponds to the localization requested.</span></span>

## <a name="examples"></a><span data-ttu-id="b3e09-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b3e09-134">Examples</span></span>
### <a name="example-1-get-the-localized-branding-for-a-specific-locale-fr"></a><span data-ttu-id="b3e09-135">Exemplo 1: obter a identidade visual localizada para uma localidade específica (FR)</span><span class="sxs-lookup"><span data-stu-id="b3e09-135">Example 1: Get the localized branding for a specific locale (fr)</span></span>
<span data-ttu-id="b3e09-136">Uma solicitação GET para uma determinada localização retorna apenas os valores dessa localização.</span><span class="sxs-lookup"><span data-stu-id="b3e09-136">A GET request to a particular localization returns only the values for that localization.</span></span> <span data-ttu-id="b3e09-137">Valores nulos não serão substituídos por aqueles da identidade visual padrão.</span><span class="sxs-lookup"><span data-stu-id="b3e09-137">Null values will not be replaced by those from the default branding.</span></span>
#### <a name="request"></a><span data-ttu-id="b3e09-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3e09-138">Request</span></span>

<span data-ttu-id="b3e09-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3e09-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
```

#### <a name="response"></a><span data-ttu-id="b3e09-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3e09-140">Response</span></span>

<span data-ttu-id="b3e09-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b3e09-141">The following is an example of the response.</span></span>

> <span data-ttu-id="b3e09-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b3e09-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-all-language-specific-localizations-that-have-been-configured"></a><span data-ttu-id="b3e09-144">Exemplo 2: obter todas as localizações específicas de idioma que foram configuradas</span><span class="sxs-lookup"><span data-stu-id="b3e09-144">Example 2: Get all language-specific localizations that have been configured</span></span>
#### <a name="request"></a><span data-ttu-id="b3e09-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3e09-145">Request</span></span>

<span data-ttu-id="b3e09-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3e09-146">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations
```

#### <a name="response"></a><span data-ttu-id="b3e09-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3e09-147">Response</span></span>

<span data-ttu-id="b3e09-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b3e09-148">The following is an example of the response.</span></span>

> <span data-ttu-id="b3e09-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b3e09-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-3-get-the-value-of-signinpagetext-for-a-specific-locale"></a><span data-ttu-id="b3e09-151">Exemplo 3: obter o valor de signInPageText para uma localidade específica</span><span class="sxs-lookup"><span data-stu-id="b3e09-151">Example 3: Get the value of signInPageText for a specific locale</span></span>
<span data-ttu-id="b3e09-152">A solicitação de uma propriedade de uma localização retorna o valor ou 204 se o valor for NULL.</span><span class="sxs-lookup"><span data-stu-id="b3e09-152">Requesting a property of a localization returns that value, or 204 if the value is null.</span></span>
#### <a name="request"></a><span data-ttu-id="b3e09-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b3e09-153">Request</span></span>

<span data-ttu-id="b3e09-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b3e09-154">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/signInPageText
```

#### <a name="response"></a><span data-ttu-id="b3e09-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="b3e09-155">Response</span></span>

<span data-ttu-id="b3e09-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b3e09-156">The following is an example of the response.</span></span>

> <span data-ttu-id="b3e09-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b3e09-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
