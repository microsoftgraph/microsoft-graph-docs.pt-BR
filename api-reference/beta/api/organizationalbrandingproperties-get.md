---
title: Obter organizationalBrandingProperties
description: Recupere as propriedades e os relacionamentos de um objeto organizationalBrandingProperties.
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f46f6487fc067aaab780f06395f5ff2b5b682f80
ms.sourcegitcommit: 40b0e58312819b69567f35ab894ee0d2989837ab
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/13/2020
ms.locfileid: "49031896"
---
# <a name="get-organizationalbrandingproperties"></a><span data-ttu-id="ccda2-103">Obter organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="ccda2-103">Get organizationalBrandingProperties</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ccda2-104">Recupere as propriedades e os relacionamentos de um objeto [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) .</span><span class="sxs-lookup"><span data-stu-id="ccda2-104">Retrieve the properties and relationships of an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ccda2-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ccda2-105">Permissions</span></span>

<span data-ttu-id="ccda2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ccda2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ccda2-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ccda2-108">Permission type</span></span>                        | <span data-ttu-id="ccda2-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ccda2-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ccda2-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ccda2-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ccda2-111">Organization. Read. All, User. Read, User. Read. All, User. ReadBasic. All</span><span class="sxs-lookup"><span data-stu-id="ccda2-111">Organization.Read.All, User.Read, User.Read.All, User.ReadBasic.All</span></span> |
| <span data-ttu-id="ccda2-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ccda2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ccda2-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ccda2-113">Not supported.</span></span> |
| <span data-ttu-id="ccda2-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ccda2-114">Application</span></span>                            | <span data-ttu-id="ccda2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ccda2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ccda2-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ccda2-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/branding/{property name}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ccda2-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ccda2-117">Optional query parameters</span></span>

<span data-ttu-id="ccda2-118">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ccda2-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ccda2-119">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ccda2-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ccda2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ccda2-120">Request headers</span></span>

| <span data-ttu-id="ccda2-121">Nome</span><span class="sxs-lookup"><span data-stu-id="ccda2-121">Name</span></span>      |<span data-ttu-id="ccda2-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccda2-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ccda2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ccda2-123">Authorization</span></span> | <span data-ttu-id="ccda2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ccda2-p103">Bearer {token}. Required.</span></span> |

>[!NOTE]
><span data-ttu-id="ccda2-126">Se você tentar a consulta no explorador do Graph, você também deve incluir o Accept-Language cabeçalho de solicitação com uma localidade ISO-639 válida.</span><span class="sxs-lookup"><span data-stu-id="ccda2-126">If you try the query in Graph Explorer, you must also include the Accept-Language request header with a valid ISO-639 locale.</span></span>

## <a name="request-body"></a><span data-ttu-id="ccda2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ccda2-127">Request body</span></span>

<span data-ttu-id="ccda2-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ccda2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ccda2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccda2-129">Response</span></span>

<span data-ttu-id="ccda2-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ccda2-130">If successful, this method returns a `200 OK` response code and the requested [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ccda2-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ccda2-131">Examples</span></span>

### <a name="example-1-get-the-default-branding"></a><span data-ttu-id="ccda2-132">Exemplo 1: obter a identidade visual padrão</span><span class="sxs-lookup"><span data-stu-id="ccda2-132">Example 1: Get the default branding</span></span>

>[!NOTE]
><span data-ttu-id="ccda2-133">Se você tentar usar o exemplo no explorador do Graph, também deverá incluir o Accept-Language cabeçalho de solicitação com uma localidade ISO-639 válida para evitar obter um erro "valor de ID de localidade inválido en-US, en; q = 0,9.</span><span class="sxs-lookup"><span data-stu-id="ccda2-133">If you try the example in Graph Explorer, you must also include the Accept-Language request header with a valid ISO-639 locale to avoid getting an error "Invalid locale id value en-US,en;q=0.9.</span></span> <span data-ttu-id="ccda2-134">Deve ser uma localidade ISO-639 válida. "</span><span class="sxs-lookup"><span data-stu-id="ccda2-134">It must be a valid ISO-639 locale."</span></span>

#### <a name="request"></a><span data-ttu-id="ccda2-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ccda2-135">Request</span></span>

<span data-ttu-id="ccda2-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ccda2-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
```

#### <a name="response"></a><span data-ttu-id="ccda2-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccda2-137">Response</span></span>

<span data-ttu-id="ccda2-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ccda2-138">The following is an example of the response.</span></span>

> <span data-ttu-id="ccda2-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ccda2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

<span data-ttu-id="ccda2-141">As solicitações para/branding sempre retornam as propriedades **mediaContentType** , **mediaReadLink** e **mediaEditLink** .</span><span class="sxs-lookup"><span data-stu-id="ccda2-141">Requests for /branding always return the **mediaContentType** , **mediaReadLink** , and **mediaEditLink** properties.</span></span> <span data-ttu-id="ccda2-142">Se uma localidade tiver sido aplicada, **mediaEditLink** será o **mediaEditLink** para a localidade (que é sempre não nulo) e o **mediaReadLink** e o **mediaContentType** serão os **mediaReadLink** e **mediaContentType** da localidade se o **mediaReadLink** da localidade for não nulo; caso contrário, o padrão **mediaReadLink** e **mediaContentType**.</span><span class="sxs-lookup"><span data-stu-id="ccda2-142">If a locale has been applied, the **mediaEditLink** is the **mediaEditLink** for the locale (which is always non-null), and the **mediaReadLink** and **mediaContentType** are the **mediaReadLink** and **mediaContentType** of the locale if the **mediaReadLink** of the locale is non-null; otherwise, the default **mediaReadLink** and **mediaContentType**.</span></span>

### <a name="example-2-get-organizational-branding-but-no-branding-configured"></a><span data-ttu-id="ccda2-143">Exemplo 2: obter a identidade visual organizacional mas nenhuma identidade visual configurada</span><span class="sxs-lookup"><span data-stu-id="ccda2-143">Example 2: Get organizational branding but no branding configured</span></span>

#### <a name="request"></a><span data-ttu-id="ccda2-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ccda2-144">Request</span></span>

<span data-ttu-id="ccda2-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ccda2-145">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
```

#### <a name="response"></a><span data-ttu-id="ccda2-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccda2-146">Response</span></span>

<span data-ttu-id="ccda2-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ccda2-147">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 404 NOT FOUND
```

### <a name="example-3-get-organizational-branding-for-the-french-locale"></a><span data-ttu-id="ccda2-148">Exemplo 3: obter a identidade visual organizacional para a localidade francês</span><span class="sxs-lookup"><span data-stu-id="ccda2-148">Example 3: Get organizational branding for the French locale</span></span>
<span data-ttu-id="ccda2-149">O cabeçalho Accept-Langauge é usado para aplicar uma determinada localização à identidade visual.</span><span class="sxs-lookup"><span data-stu-id="ccda2-149">The Accept-Langauge header is used to apply a particular localization to the branding.</span></span> <span data-ttu-id="ccda2-150">As propriedades que são nulas na localização especificada são retornadas da identidade visual padrão.</span><span class="sxs-lookup"><span data-stu-id="ccda2-150">Properties that are null in the specified localization are returned from the default branding.</span></span> <span data-ttu-id="ccda2-151">Se o cabeçalho Accept-Language for especificado na solicitação, a resposta incluirá o cabeçalho do idioma de conteúdo, a menos que seja `und` .</span><span class="sxs-lookup"><span data-stu-id="ccda2-151">If the Accept-Language header is specified in the request, the response will include the Content-Language header, unless it is `und`.</span></span>

#### <a name="request"></a><span data-ttu-id="ccda2-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ccda2-152">Request</span></span>

<span data-ttu-id="ccda2-153">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ccda2-153">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Accept-Language: fr
```

#### <a name="response"></a><span data-ttu-id="ccda2-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccda2-154">Response</span></span>

<span data-ttu-id="ccda2-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ccda2-155">The following is an example of the response.</span></span>

> <span data-ttu-id="ccda2-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ccda2-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-get-bannerlogo-for-the-french-locale"></a><span data-ttu-id="ccda2-158">Exemplo 4: obter bannerLogo para a localidade francês</span><span class="sxs-lookup"><span data-stu-id="ccda2-158">Example 4: Get bannerLogo for the French locale</span></span>
<span data-ttu-id="ccda2-159">Retorna **bannerLogo** para a localidade fr se ela existir.</span><span class="sxs-lookup"><span data-stu-id="ccda2-159">Returns **bannerLogo** for the fr locale if it exists.</span></span> <span data-ttu-id="ccda2-160">Se a localização não existir, retornará o **bannerLogo** padrão.</span><span class="sxs-lookup"><span data-stu-id="ccda2-160">If the localization does not exist, returns the default **bannerLogo**.</span></span>

#### <a name="request"></a><span data-ttu-id="ccda2-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ccda2-161">Request</span></span>

<span data-ttu-id="ccda2-162">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ccda2-162">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Accept-Language: fr
```

#### <a name="response"></a><span data-ttu-id="ccda2-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccda2-163">Response</span></span>

<span data-ttu-id="ccda2-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ccda2-164">The following is an example of the response.</span></span>

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

### <a name="example-5-get-bannerlogo-when-no-bannerlogo-is-configured"></a><span data-ttu-id="ccda2-165">Exemplo 5: obter bannerLogo quando nenhum bannerLogo estiver configurado</span><span class="sxs-lookup"><span data-stu-id="ccda2-165">Example 5: Get bannerLogo when no bannerLogo is configured</span></span>

<span data-ttu-id="ccda2-166">Este exemplo mostra uma solicitação para uma propriedade que não existe na identidade visual padrão ou o idioma especificado no cabeçalho Accept-Language.</span><span class="sxs-lookup"><span data-stu-id="ccda2-166">This example shows a request for a property that does not exist on the default branding or the language specified in the Accept-Language header.</span></span>

#### <a name="request"></a><span data-ttu-id="ccda2-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ccda2-167">Request</span></span>

<span data-ttu-id="ccda2-168">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ccda2-168">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
GET https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Accept-Language: de
```

#### <a name="response"></a><span data-ttu-id="ccda2-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="ccda2-169">Response</span></span>

<span data-ttu-id="ccda2-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ccda2-170">The following is an example of the response.</span></span>

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
