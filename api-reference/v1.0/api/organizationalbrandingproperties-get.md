---
title: Obter organizationalBrandingProperties
description: Recupere as propriedades e as relações de um objeto organizationalBrandingProperties.
localization_priority: Normal
author: kexia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: df77f6b26cab6324574ce22335e0b0c3236ee7b9
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722507"
---
# <a name="get-organizationalbrandingproperties"></a><span data-ttu-id="f028d-103">Obter organizationalBrandingProperties</span><span class="sxs-lookup"><span data-stu-id="f028d-103">Get organizationalBrandingProperties</span></span>

<span data-ttu-id="f028d-104">Recupere as propriedades e as relações de um [objeto organizationalBrandingProperties.](../resources/organizationalbrandingproperties.md)</span><span class="sxs-lookup"><span data-stu-id="f028d-104">Retrieve the properties and relationships of an [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f028d-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="f028d-105">Permissions</span></span>

<span data-ttu-id="f028d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f028d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f028d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f028d-108">Permission type</span></span>                        | <span data-ttu-id="f028d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f028d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f028d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f028d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f028d-111">Organization.Read.All, User.Read, User.Read.All, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="f028d-111">Organization.Read.All, User.Read, User.Read.All, User.ReadBasic.All</span></span> |
| <span data-ttu-id="f028d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f028d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f028d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f028d-113">Not supported.</span></span> |
| <span data-ttu-id="f028d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f028d-114">Application</span></span>                            | <span data-ttu-id="f028d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f028d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f028d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f028d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /organization/{id}/branding/{property name}
```

## <a name="request-headers"></a><span data-ttu-id="f028d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f028d-117">Request headers</span></span>

| <span data-ttu-id="f028d-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f028d-118">Name</span></span>      |<span data-ttu-id="f028d-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f028d-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f028d-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="f028d-120">Authorization</span></span> | <span data-ttu-id="f028d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f028d-p102">Bearer {token}. Required.</span></span> |

>[!NOTE]
><span data-ttu-id="f028d-123">Se você tentar a consulta no Graph Explorer, também deverá incluir o header de solicitação **Accept-Language** com uma localidade ISO-639 válida.</span><span class="sxs-lookup"><span data-stu-id="f028d-123">If you try the query in Graph Explorer, you must also include the **Accept-Language** request header with a valid ISO-639 locale.</span></span>

## <a name="request-body"></a><span data-ttu-id="f028d-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f028d-124">Request body</span></span>

<span data-ttu-id="f028d-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f028d-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f028d-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="f028d-126">Response</span></span>

<span data-ttu-id="f028d-127">Se tiver êxito, este método retornará um código de `200 OK` resposta e o objeto [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f028d-127">If successful, this method returns a `200 OK` response code and the requested [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f028d-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f028d-128">Examples</span></span>

### <a name="example-1-get-the-default-branding"></a><span data-ttu-id="f028d-129">Exemplo 1: Obter a identidade visual padrão</span><span class="sxs-lookup"><span data-stu-id="f028d-129">Example 1: Get the default branding</span></span>

>[!NOTE]
><span data-ttu-id="f028d-130">Se você tentar o exemplo no Graph Explorer, também deverá incluir o header de solicitação **Accept-Language** com uma localidade ISO-639 válida para evitar obter um erro " Valor de id de localidade inválido *en-US,en;q=0,9. Deve ser uma localidade ISO-639 válida.*"</span><span class="sxs-lookup"><span data-stu-id="f028d-130">If you try the example in Graph Explorer, you must also include the **Accept-Language** request header with a valid ISO-639 locale to avoid getting an error "*Invalid locale id value en-US,en;q=0.9. It must be a valid ISO-639 locale.*"</span></span>

#### <a name="request"></a><span data-ttu-id="f028d-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f028d-131">Request</span></span>

<span data-ttu-id="f028d-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f028d-132">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
```

#### <a name="response"></a><span data-ttu-id="f028d-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="f028d-133">Response</span></span>

<span data-ttu-id="f028d-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f028d-134">The following is an example of the response.</span></span>

> <span data-ttu-id="f028d-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f028d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "backgroundImage@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/backgroundImage",
  "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/backgroundImage",
  "bannerLogo@odata.mediaContentType":"image/*",
  "bannerLogo@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo",
  "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo",
  "id": "und",
  "squareLogo@odata.mediaContentType":"image/*",
  "squareLogo@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/squareLogo",
  "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/squareLogo",
  "signInPageText":"Default",
  "usernameHintText":"DefaultHint"
}
```

<span data-ttu-id="f028d-137">As solicitações de /branding sempre retornam as **propriedades mediaContentType,** **mediaReadLink** e **mediaEditLink.**</span><span class="sxs-lookup"><span data-stu-id="f028d-137">Requests for /branding always return the **mediaContentType**, **mediaReadLink**, and **mediaEditLink** properties.</span></span> <span data-ttu-id="f028d-138">Se uma localidade tiver sido aplicada, **mediaEditLink** será o **mediaEditLink** para a localidade (que sempre não é nulo), e **mediaReadLink** e **mediaContentType** serão **mediaReadLink** e **mediaContentType** da localidade se **o mediaReadLink** da localidade não for nulo; caso contrário, o **mediaReadLink** padrão e **mediaContentType**.</span><span class="sxs-lookup"><span data-stu-id="f028d-138">If a locale has been applied, the **mediaEditLink** is the **mediaEditLink** for the locale (which is always non-null), and the **mediaReadLink** and **mediaContentType** are the **mediaReadLink** and **mediaContentType** of the locale if the **mediaReadLink** of the locale is non-null; otherwise, the default **mediaReadLink** and **mediaContentType**.</span></span>

### <a name="example-2-get-organizational-branding-but-no-branding-configured"></a><span data-ttu-id="f028d-139">Exemplo 2: Obter identidade visual organizacional, mas nenhuma identidade visual configurada</span><span class="sxs-lookup"><span data-stu-id="f028d-139">Example 2: Get organizational branding but no branding configured</span></span>

#### <a name="request"></a><span data-ttu-id="f028d-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f028d-140">Request</span></span>

<span data-ttu-id="f028d-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f028d-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
```

#### <a name="response"></a><span data-ttu-id="f028d-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="f028d-142">Response</span></span>

<span data-ttu-id="f028d-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f028d-143">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 404 NOT FOUND
```

### <a name="example-3-get-organizational-branding-for-the-french-locale"></a><span data-ttu-id="f028d-144">Exemplo 3: Obter identidade visual organizacional para a localidade francesa</span><span class="sxs-lookup"><span data-stu-id="f028d-144">Example 3: Get organizational branding for the French locale</span></span>
<span data-ttu-id="f028d-145">O **header Accept-Language** é usado para aplicar uma localização específica à identidade visual.</span><span class="sxs-lookup"><span data-stu-id="f028d-145">The **Accept-Language** header is used to apply a particular localization to the branding.</span></span> <span data-ttu-id="f028d-146">As propriedades que `null` estão na localização especificada são retornadas da identidade visual padrão.</span><span class="sxs-lookup"><span data-stu-id="f028d-146">Properties that are `null` in the specified localization are returned from the default branding.</span></span> <span data-ttu-id="f028d-147">Se o header **Accept-Language** for especificado na solicitação, a resposta incluirá o header **Content-Language,** a menos que seja `und` .</span><span class="sxs-lookup"><span data-stu-id="f028d-147">If the **Accept-Language** header is specified in the request, the response will include the **Content-Language** header, unless it is `und`.</span></span>

#### <a name="request"></a><span data-ttu-id="f028d-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f028d-148">Request</span></span>

<span data-ttu-id="f028d-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f028d-149">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Accept-Language: fr
```

#### <a name="response"></a><span data-ttu-id="f028d-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="f028d-150">Response</span></span>

<span data-ttu-id="f028d-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f028d-151">The following is an example of the response.</span></span>

> <span data-ttu-id="f028d-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f028d-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "backgroundImage@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/backgroundImage",
    "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/backgroundImage",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo",
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
    "id": "und",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/squareLogo",
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/squareLogo",
    "signInPageText":"Default",
    "usernameHintText":"DefaultHint"
}
```

### <a name="example-4-get-bannerlogo-for-the-french-locale"></a><span data-ttu-id="f028d-154">Exemplo 4: Obter bannerLogo para a localidade francesa</span><span class="sxs-lookup"><span data-stu-id="f028d-154">Example 4: Get bannerLogo for the French locale</span></span>
<span data-ttu-id="f028d-155">Retorna **bannerLogo** para `fr` a localidade se ela existir.</span><span class="sxs-lookup"><span data-stu-id="f028d-155">Returns **bannerLogo** for the `fr` locale if it exists.</span></span> <span data-ttu-id="f028d-156">Se a localização não existir, retornará o **bannerLogo padrão**.</span><span class="sxs-lookup"><span data-stu-id="f028d-156">If the localization does not exist, returns the default **bannerLogo**.</span></span>

#### <a name="request"></a><span data-ttu-id="f028d-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f028d-157">Request</span></span>

<span data-ttu-id="f028d-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f028d-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Accept-Language: fr
```

#### <a name="response"></a><span data-ttu-id="f028d-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="f028d-159">Response</span></span>

<span data-ttu-id="f028d-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f028d-160">The following is an example of the response.</span></span>

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
    "bannerLogo@odata.mediaReadLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo",
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
}
```

### <a name="example-5-get-bannerlogo-when-no-bannerlogo-is-configured"></a><span data-ttu-id="f028d-161">Exemplo 5: Obter bannerLogo quando nenhum bannerLogo estiver configurado</span><span class="sxs-lookup"><span data-stu-id="f028d-161">Example 5: Get bannerLogo when no bannerLogo is configured</span></span>

<span data-ttu-id="f028d-162">Este exemplo mostra uma solicitação para uma propriedade que não existe na identidade visual padrão ou no idioma especificado no header **Accept-Language.**</span><span class="sxs-lookup"><span data-stu-id="f028d-162">This example shows a request for a property that does not exist on the default branding or the language specified in the **Accept-Language** header.</span></span>

#### <a name="request"></a><span data-ttu-id="f028d-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f028d-163">Request</span></span>

<span data-ttu-id="f028d-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f028d-164">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
GET https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Accept-Language: de
```

#### <a name="response"></a><span data-ttu-id="f028d-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="f028d-165">Response</span></span>

<span data-ttu-id="f028d-166">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f028d-166">The following is an example of the response.</span></span>

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
