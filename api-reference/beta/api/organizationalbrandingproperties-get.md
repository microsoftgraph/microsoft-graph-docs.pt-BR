---
title: Obter organizationalBrandingProperties
description: Recupere as propriedades e as relações de um objeto organizationalBrandingProperties.
localization_priority: Normal
author: almars
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d5193b03bdf820b2a8142dd23c6dce1a742314ef
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582722"
---
# <a name="get-organizationalbrandingproperties"></a><span data-ttu-id="dcbe5-103">Obter organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="dcbe5-103">Get organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dcbe5-104">Recupere as propriedades e as relações de um [objeto organizationalBrandingProperties.](../resources/organizationalbrandingproperties.md)</span><span class="sxs-lookup"><span data-stu-id="dcbe5-104">Retrieve the properties and relationships of an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dcbe5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="dcbe5-105">Permissions</span></span>

<span data-ttu-id="dcbe5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dcbe5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dcbe5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dcbe5-108">Permission type</span></span>                        | <span data-ttu-id="dcbe5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dcbe5-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dcbe5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dcbe5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="dcbe5-111">Organization.Read.All, User.Read, User.Read.All, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="dcbe5-111">Organization.Read.All, User.Read, User.Read.All, User.ReadBasic.All</span></span> |
| <span data-ttu-id="dcbe5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dcbe5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dcbe5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dcbe5-113">Not supported.</span></span> |
| <span data-ttu-id="dcbe5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dcbe5-114">Application</span></span>                            | <span data-ttu-id="dcbe5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dcbe5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dcbe5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dcbe5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/branding
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dcbe5-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dcbe5-117">Optional query parameters</span></span>

<span data-ttu-id="dcbe5-118">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dcbe5-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="dcbe5-119">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="dcbe5-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="dcbe5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dcbe5-120">Request headers</span></span>

| <span data-ttu-id="dcbe5-121">Nome</span><span class="sxs-lookup"><span data-stu-id="dcbe5-121">Name</span></span>      |<span data-ttu-id="dcbe5-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="dcbe5-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dcbe5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dcbe5-123">Authorization</span></span> | <span data-ttu-id="dcbe5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dcbe5-p103">Bearer {token}. Required.</span></span> |

>[!NOTE]
><span data-ttu-id="dcbe5-126">Se você tentar a consulta no Graph Explorer, também deverá incluir o Accept-Language de solicitação com uma localidade ISO-639 válida.</span><span class="sxs-lookup"><span data-stu-id="dcbe5-126">If you try the query in Graph Explorer, you must also include the Accept-Language request header with a valid ISO-639 locale.</span></span>

## <a name="request-body"></a><span data-ttu-id="dcbe5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dcbe5-127">Request body</span></span>

<span data-ttu-id="dcbe5-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dcbe5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dcbe5-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcbe5-129">Response</span></span>

<span data-ttu-id="dcbe5-130">Se tiver êxito, este método retornará um código de `200 OK` resposta e o objeto [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dcbe5-130">If successful, this method returns a `200 OK` response code and the requested [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dcbe5-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="dcbe5-131">Examples</span></span>

### <a name="example-1-get-the-default-branding"></a><span data-ttu-id="dcbe5-132">Exemplo 1: Obter a identidade visual padrão</span><span class="sxs-lookup"><span data-stu-id="dcbe5-132">Example 1: Get the default branding</span></span>

>[!NOTE]
><span data-ttu-id="dcbe5-133">Se você tentar o exemplo no Graph Explorer, também deverá incluir o header de solicitação Accept-Language com uma localidade ISO-639 válida para evitar obter um erro "Valor de id de localidade inválido en-US,en;q=0,9.</span><span class="sxs-lookup"><span data-stu-id="dcbe5-133">If you try the example in Graph Explorer, you must also include the Accept-Language request header with a valid ISO-639 locale to avoid getting an error "Invalid locale id value en-US,en;q=0.9.</span></span> <span data-ttu-id="dcbe5-134">Deve ser uma localidade ISO-639 válida."</span><span class="sxs-lookup"><span data-stu-id="dcbe5-134">It must be a valid ISO-639 locale."</span></span>

#### <a name="request"></a><span data-ttu-id="dcbe5-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dcbe5-135">Request</span></span>

<span data-ttu-id="dcbe5-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dcbe5-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dcbe5-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="dcbe5-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
```
# <a name="c"></a>[<span data-ttu-id="dcbe5-138">C#</span><span class="sxs-lookup"><span data-stu-id="dcbe5-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dcbe5-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dcbe5-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dcbe5-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dcbe5-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dcbe5-141">Java</span><span class="sxs-lookup"><span data-stu-id="dcbe5-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="dcbe5-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcbe5-142">Response</span></span>

<span data-ttu-id="dcbe5-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dcbe5-143">The following is an example of the response.</span></span>

> <span data-ttu-id="dcbe5-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dcbe5-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "backgroundColor":"#FFFF33",
  "backgroundImage@odata.mediaContentType":"image/*",
  "backgroundImage@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/backgroundImage",
  "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/backgroundImage",
  "bannerLogo@odata.mediaContentType":"image/*",
  "bannerLogo@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo",
  "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo",
  "id": "und",
  "squareLogo@odata.mediaContentType":"image/*",
  "squareLogo@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/squareLogo",
  "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/squareLogo",
  "signInPageText":"Default",
  "usernameHintText":"DefaultHint"
}
```

<span data-ttu-id="dcbe5-146">As solicitações de /branding sempre retornam as **propriedades mediaContentType,** **mediaReadLink** e **mediaEditLink.**</span><span class="sxs-lookup"><span data-stu-id="dcbe5-146">Requests for /branding always return the **mediaContentType**, **mediaReadLink**, and **mediaEditLink** properties.</span></span> <span data-ttu-id="dcbe5-147">Se uma localidade tiver sido aplicada, **mediaEditLink** será o **mediaEditLink** para a localidade (que sempre não é nulo), e **mediaReadLink** e **mediaContentType** serão **mediaReadLink** e **mediaContentType** da localidade se **o mediaReadLink** da localidade não for nulo; caso contrário, o **mediaReadLink** padrão e **mediaContentType**.</span><span class="sxs-lookup"><span data-stu-id="dcbe5-147">If a locale has been applied, the **mediaEditLink** is the **mediaEditLink** for the locale (which is always non-null), and the **mediaReadLink** and **mediaContentType** are the **mediaReadLink** and **mediaContentType** of the locale if the **mediaReadLink** of the locale is non-null; otherwise, the default **mediaReadLink** and **mediaContentType**.</span></span>

### <a name="example-2-get-organizational-branding-but-no-branding-configured"></a><span data-ttu-id="dcbe5-148">Exemplo 2: Obter identidade visual organizacional, mas nenhuma identidade visual configurada</span><span class="sxs-lookup"><span data-stu-id="dcbe5-148">Example 2: Get organizational branding but no branding configured</span></span>

#### <a name="request"></a><span data-ttu-id="dcbe5-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dcbe5-149">Request</span></span>

<span data-ttu-id="dcbe5-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dcbe5-150">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_3"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
```

#### <a name="response"></a><span data-ttu-id="dcbe5-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcbe5-151">Response</span></span>

<span data-ttu-id="dcbe5-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dcbe5-152">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 404 NOT FOUND
```

### <a name="example-3-get-organizational-branding-for-the-french-locale"></a><span data-ttu-id="dcbe5-153">Exemplo 3: Obter identidade visual organizacional para a localidade francesa</span><span class="sxs-lookup"><span data-stu-id="dcbe5-153">Example 3: Get organizational branding for the French locale</span></span>
<span data-ttu-id="dcbe5-154">O Accept-Langauge é usado para aplicar uma localização específica à identidade visual.</span><span class="sxs-lookup"><span data-stu-id="dcbe5-154">The Accept-Langauge header is used to apply a particular localization to the branding.</span></span> <span data-ttu-id="dcbe5-155">As propriedades que são nulas na localização especificada são retornadas da identidade visual padrão.</span><span class="sxs-lookup"><span data-stu-id="dcbe5-155">Properties that are null in the specified localization are returned from the default branding.</span></span> <span data-ttu-id="dcbe5-156">Se o Accept-Language for especificado na solicitação, a resposta incluirá o header Content-Language, a menos que seja `und` .</span><span class="sxs-lookup"><span data-stu-id="dcbe5-156">If the Accept-Language header is specified in the request, the response will include the Content-Language header, unless it is `und`.</span></span>

#### <a name="request"></a><span data-ttu-id="dcbe5-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dcbe5-157">Request</span></span>

<span data-ttu-id="dcbe5-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dcbe5-158">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_4"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Accept-Language: fr
```

#### <a name="response"></a><span data-ttu-id="dcbe5-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcbe5-159">Response</span></span>

<span data-ttu-id="dcbe5-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dcbe5-160">The following is an example of the response.</span></span>

> <span data-ttu-id="dcbe5-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dcbe5-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Language: fr

{
    "backgroundColor":"#00000F",
    "backgroundImage@odata.mediaContentType":"image/*",
    "backgroundImage@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/backgroundImage",
    "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/backgroundImage",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo",
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
    "id": "und",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/squareLogo",
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/squareLogo",
    "signInPageText":"Default",
    "usernameHintText":"DefaultHint"
}
```

### <a name="example-4-get-bannerlogo-for-the-french-locale"></a><span data-ttu-id="dcbe5-163">Exemplo 4: Obter bannerLogo para a localidade francesa</span><span class="sxs-lookup"><span data-stu-id="dcbe5-163">Example 4: Get bannerLogo for the French locale</span></span>
<span data-ttu-id="dcbe5-164">Retorna **bannerLogo** para a localidade fr se existir.</span><span class="sxs-lookup"><span data-stu-id="dcbe5-164">Returns **bannerLogo** for the fr locale if it exists.</span></span> <span data-ttu-id="dcbe5-165">Se a localização não existir, retornará o **bannerLogo padrão**.</span><span class="sxs-lookup"><span data-stu-id="dcbe5-165">If the localization does not exist, returns the default **bannerLogo**.</span></span>

#### <a name="request"></a><span data-ttu-id="dcbe5-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dcbe5-166">Request</span></span>

<span data-ttu-id="dcbe5-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dcbe5-167">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dcbe5-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="dcbe5-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_5"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Accept-Language: fr
```
# <a name="c"></a>[<span data-ttu-id="dcbe5-169">C#</span><span class="sxs-lookup"><span data-stu-id="dcbe5-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-5-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dcbe5-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dcbe5-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-5-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dcbe5-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dcbe5-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-5-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dcbe5-172">Java</span><span class="sxs-lookup"><span data-stu-id="dcbe5-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-5-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="dcbe5-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcbe5-173">Response</span></span>

<span data-ttu-id="dcbe5-174">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dcbe5-174">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo",
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
}
```

### <a name="example-5-get-bannerlogo-when-no-bannerlogo-is-configured"></a><span data-ttu-id="dcbe5-175">Exemplo 5: Obter bannerLogo quando nenhum bannerLogo estiver configurado</span><span class="sxs-lookup"><span data-stu-id="dcbe5-175">Example 5: Get bannerLogo when no bannerLogo is configured</span></span>

<span data-ttu-id="dcbe5-176">Este exemplo mostra uma solicitação para uma propriedade que não existe na identidade visual padrão ou no idioma especificado no Accept-Language de usuário.</span><span class="sxs-lookup"><span data-stu-id="dcbe5-176">This example shows a request for a property that does not exist on the default branding or the language specified in the Accept-Language header.</span></span>

#### <a name="request"></a><span data-ttu-id="dcbe5-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dcbe5-177">Request</span></span>

<span data-ttu-id="dcbe5-178">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dcbe5-178">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dcbe5-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="dcbe5-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties_6"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Accept-Language: de
```
# <a name="c"></a>[<span data-ttu-id="dcbe5-180">C#</span><span class="sxs-lookup"><span data-stu-id="dcbe5-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-6-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dcbe5-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dcbe5-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-6-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dcbe5-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dcbe5-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-6-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dcbe5-183">Java</span><span class="sxs-lookup"><span data-stu-id="dcbe5-183">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-6-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="dcbe5-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcbe5-184">Response</span></span>

<span data-ttu-id="dcbe5-185">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dcbe5-185">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 NO CONTENT
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
