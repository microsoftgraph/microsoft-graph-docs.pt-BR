---
title: Atualizar regionalAndLanguageSettings
description: Atualizar as configurações regionais e de idioma de um usuário
author: jasonbro
localization_priority: Normal
ms.prod: settings
doc_type: apiPageType
ms.openlocfilehash: 2af80fb6261d04e2aa35a6fe3ea20ce30c63842f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971976"
---
# <a name="update-regionalandlanguagesettings"></a><span data-ttu-id="54a71-103">Atualizar regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="54a71-103">Update regionalAndLanguageSettings</span></span>

<span data-ttu-id="54a71-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54a71-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54a71-105">Atualizar algumas ou todas as propriedades de um objeto [regionalAndLanguageSettings](../resources/regionalAndLanguageSettings.md) .</span><span class="sxs-lookup"><span data-stu-id="54a71-105">Update some or all of the properties of a [regionalAndLanguageSettings](../resources/regionalAndLanguageSettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="54a71-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="54a71-106">Permissions</span></span>
<span data-ttu-id="54a71-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54a71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54a71-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="54a71-109">Permission Type</span></span>                   |<span data-ttu-id="54a71-110">Permissão (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="54a71-110">Permission (from least to most privileged)</span></span>     |
|----------------------------------|---------------------------------------------- |
|<span data-ttu-id="54a71-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="54a71-111">Delegated (work or school account)</span></span>|<span data-ttu-id="54a71-112">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="54a71-112">User.ReadWrite, User.ReadWrite.All</span></span>             |
|<span data-ttu-id="54a71-113">Delegado (conta pessoal)</span><span class="sxs-lookup"><span data-stu-id="54a71-113">Delegated (personal account)</span></span>      |<span data-ttu-id="54a71-114">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="54a71-114">User.ReadWrite, User.ReadWrite.All</span></span>             |
|<span data-ttu-id="54a71-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="54a71-115">Application</span></span>                       |<span data-ttu-id="54a71-116">User. ReadWrite, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="54a71-116">User.ReadWrite, User.ReadWrite.All</span></span>             |

## <a name="http-request"></a><span data-ttu-id="54a71-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54a71-117">HTTP request</span></span>

<span data-ttu-id="54a71-118">Para atualizar todas as configurações regionais e de idioma de um usuário:</span><span class="sxs-lookup"><span data-stu-id="54a71-118">To update all of a user's regional and language settings:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /settings/regionalAndLanguageSettings
```

<span data-ttu-id="54a71-119">Para atualizar um subconjunto das propriedades das configurações regionais e de idioma de um usuário:</span><span class="sxs-lookup"><span data-stu-id="54a71-119">To update a subset of the properties of a user's regional and language settings:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /settings/regionalAndLanguageSettings
```

## <a name="request-headers"></a><span data-ttu-id="54a71-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54a71-120">Request headers</span></span>
| <span data-ttu-id="54a71-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="54a71-121">Header</span></span>       | <span data-ttu-id="54a71-122">Valor</span><span class="sxs-lookup"><span data-stu-id="54a71-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="54a71-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="54a71-123">Authorization</span></span>  | <span data-ttu-id="54a71-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54a71-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="54a71-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="54a71-126">Content-Type</span></span>  | <span data-ttu-id="54a71-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54a71-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="54a71-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54a71-129">Request body</span></span>
 <span data-ttu-id="54a71-130">**Put**: no corpo da solicitação, forneça um objeto [regionalAndLanguageSettings](../resources/regionalAndLanguageSettings.md) .</span><span class="sxs-lookup"><span data-stu-id="54a71-130">**PUT**: In the request body, supply a [regionalAndLanguageSettings](../resources/regionalAndLanguageSettings.md) object.</span></span>
 
 <span data-ttu-id="54a71-131">**Patch**: forneça apenas os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="54a71-131">**PATCH**: Only supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="54a71-132">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="54a71-132">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="54a71-133">Para obter um melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="54a71-133">For best performance you shouldn't include existing values that haven't changed.</span></span>
 
## <a name="response"></a><span data-ttu-id="54a71-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="54a71-134">Response</span></span>

<span data-ttu-id="54a71-135">Se tiver êxito, este método retornará um código de resposta 200 e o objeto regionalAndLanguageSettings atualizado.</span><span class="sxs-lookup"><span data-stu-id="54a71-135">If successful, this method returns a 200 response code and the updated regionalAndLanguageSettings object</span></span>

## <a name="example"></a><span data-ttu-id="54a71-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="54a71-136">Example</span></span>

### <a name="example-1-update-the-entire-regionalandlanguagesettings-object-of-the-signed-in-user"></a><span data-ttu-id="54a71-137">Exemplo 1: atualizar todo o objeto regionalAndLanguageSettings do usuário conectado</span><span class="sxs-lookup"><span data-stu-id="54a71-137">Example 1: Update the entire regionalAndLanguageSettings object of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="54a71-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54a71-138">Request</span></span>

<span data-ttu-id="54a71-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="54a71-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="54a71-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="54a71-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "put_regionalAndLanguageSettings"
}-->
```http
PUT https://graph.microsoft.com/beta/me/settings/regionalandlanguagesettings
Content-type: application/json

{
    "defaultDisplayLanguage": {
        "locale": "en-US"
    },
    "authoringLanguages": [
        {
            "locale": "fr-FR"
        },
        {
            "locale": "de-DE"
        }
    ],
    "defaultTranslationLanguage": {
        "locale": "en-US"
    },
    "defaultSpeechInputLanguage": {
        "locale": "en-US"
    },
    "defaultRegionalFormat": {
        "locale": "en-GB"
    },
    "regionalFormatOverrides": {
        "calendar": "Gregorian Calendar",
        "firstDayOfWeek": "Sunday",
        "shortDateFormat": "yyyy-MM-dd",
        "longDateFormat": "dddd, MMMM d, yyyy",
        "shortTimeFormat": "HH:mm",
        "longTimeFormat": "h:mm:ss tt",
        "timeZone": "Pacific Standard Time"
    }
}
```
# <a name="c"></a>[<span data-ttu-id="54a71-141">C#</span><span class="sxs-lookup"><span data-stu-id="54a71-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/put-regionalandlanguagesettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="54a71-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54a71-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-regionalandlanguagesettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="54a71-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="54a71-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/put-regionalandlanguagesettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="54a71-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="54a71-144">Response</span></span>

<span data-ttu-id="54a71-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="54a71-145">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.regionalAndLanguageSettings",
  "name": "put_regionalAndLanguageSettings"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-selected-properties-of-the-signed-in-user"></a><span data-ttu-id="54a71-146">Exemplo 2: atualizar propriedades selecionadas do usuário conectado</span><span class="sxs-lookup"><span data-stu-id="54a71-146">Example 2: Update selected properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="54a71-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54a71-147">Request</span></span>

<span data-ttu-id="54a71-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="54a71-148">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="54a71-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="54a71-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_regionalAndLanguageSettings"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/settings/regionalandlanguagesettings
Content-type: application/json

{
  "authoringLanguages": [
    {
     "locale": "en-US" },
    {
     "locale": "es-MX" }
  ],
  "defaultRegionalFormat": {
     "locale": "en-US"
   }
}
```
# <a name="c"></a>[<span data-ttu-id="54a71-150">C#</span><span class="sxs-lookup"><span data-stu-id="54a71-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/patch-regionalandlanguagesettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="54a71-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54a71-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/patch-regionalandlanguagesettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="54a71-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="54a71-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-regionalandlanguagesettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="54a71-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="54a71-153">Response</span></span>

<span data-ttu-id="54a71-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="54a71-154">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.regionalAndLanguageSettings",
  "name": "patch_regionalAndLanguageSettings"
} -->
```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Update regionalAndLanguageSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


