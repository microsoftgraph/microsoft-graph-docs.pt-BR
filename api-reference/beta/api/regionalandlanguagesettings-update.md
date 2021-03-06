---
title: Atualizar regionalAndLanguageSettings
description: Atualize as configurações regionais e de idioma de um usuário.
author: jasonbro
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 82f33ae2b4165586ccb4a3d55873e1e6ff6c1765
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516616"
---
# <a name="update-regionalandlanguagesettings"></a><span data-ttu-id="e1214-103">Atualizar regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="e1214-103">Update regionalAndLanguageSettings</span></span>

<span data-ttu-id="e1214-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1214-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1214-105">Atualize algumas ou todas as propriedades de um [objeto regionalAndLanguageSettings.](../resources/regionalAndLanguageSettings.md)</span><span class="sxs-lookup"><span data-stu-id="e1214-105">Update some or all of the properties of a [regionalAndLanguageSettings](../resources/regionalAndLanguageSettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1214-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e1214-106">Permissions</span></span>
<span data-ttu-id="e1214-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1214-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1214-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1214-109">Permission Type</span></span>                   |<span data-ttu-id="e1214-110">Permissão (do mínimo para o mais privilegiado)</span><span class="sxs-lookup"><span data-stu-id="e1214-110">Permission (from least to most privileged)</span></span>     |
|----------------------------------|---------------------------------------------- |
|<span data-ttu-id="e1214-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1214-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e1214-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1214-112">User.ReadWrite, User.ReadWrite.All</span></span>             |
|<span data-ttu-id="e1214-113">Delegada (conta pessoal)</span><span class="sxs-lookup"><span data-stu-id="e1214-113">Delegated (personal account)</span></span>      |<span data-ttu-id="e1214-114">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1214-114">User.ReadWrite, User.ReadWrite.All</span></span>             |
|<span data-ttu-id="e1214-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1214-115">Application</span></span>                       |<span data-ttu-id="e1214-116">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1214-116">User.ReadWrite, User.ReadWrite.All</span></span>             |

## <a name="http-request"></a><span data-ttu-id="e1214-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1214-117">HTTP request</span></span>

<span data-ttu-id="e1214-118">Para atualizar todas as configurações regionais e de idioma de um usuário:</span><span class="sxs-lookup"><span data-stu-id="e1214-118">To update all of a user's regional and language settings:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /settings/regionalAndLanguageSettings
```

<span data-ttu-id="e1214-119">Para atualizar um subconjunto das propriedades das configurações regionais e de idioma de um usuário:</span><span class="sxs-lookup"><span data-stu-id="e1214-119">To update a subset of the properties of a user's regional and language settings:</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /settings/regionalAndLanguageSettings
```

## <a name="request-headers"></a><span data-ttu-id="e1214-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1214-120">Request headers</span></span>
| <span data-ttu-id="e1214-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e1214-121">Header</span></span>       | <span data-ttu-id="e1214-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e1214-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="e1214-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1214-123">Authorization</span></span>  | <span data-ttu-id="e1214-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1214-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e1214-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e1214-126">Content-Type</span></span>  | <span data-ttu-id="e1214-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1214-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e1214-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1214-129">Request body</span></span>
 <span data-ttu-id="e1214-130">**PUT**: No corpo da solicitação, fornece um [objeto regionalAndLanguageSettings.](../resources/regionalAndLanguageSettings.md)</span><span class="sxs-lookup"><span data-stu-id="e1214-130">**PUT**: In the request body, supply a [regionalAndLanguageSettings](../resources/regionalAndLanguageSettings.md) object.</span></span>
 
 <span data-ttu-id="e1214-131">**PATCH**: fornece somente os valores para campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="e1214-131">**PATCH**: Only supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="e1214-132">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="e1214-132">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e1214-133">Para obter um melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="e1214-133">For best performance you shouldn't include existing values that haven't changed.</span></span>
 
## <a name="response"></a><span data-ttu-id="e1214-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1214-134">Response</span></span>

<span data-ttu-id="e1214-135">Se tiver êxito, este método retornará um código de resposta 200 e o **objeto regionalAndLanguageSettings** atualizado.</span><span class="sxs-lookup"><span data-stu-id="e1214-135">If successful, this method returns a 200 response code and the updated **regionalAndLanguageSettings** object.</span></span>

## <a name="example"></a><span data-ttu-id="e1214-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1214-136">Example</span></span>

### <a name="example-1-update-the-entire-regionalandlanguagesettings-object-of-the-signed-in-user"></a><span data-ttu-id="e1214-137">Exemplo 1: Atualizar todo o objeto regionalAndLanguageSettings do usuário in-loca</span><span class="sxs-lookup"><span data-stu-id="e1214-137">Example 1: Update the entire regionalAndLanguageSettings object of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="e1214-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1214-138">Request</span></span>

<span data-ttu-id="e1214-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1214-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e1214-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1214-140">HTTP</span></span>](#tab/http)
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
    },
    "translationPreferences": {
        "translationBehavior": "Yes",
        "languageOverrides": [
            {
                "languageTag": "fr",
                "translationBehavior": "Yes" 
            }
        ]
     }
}
```
# <a name="c"></a>[<span data-ttu-id="e1214-141">C#</span><span class="sxs-lookup"><span data-stu-id="e1214-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/put-regionalandlanguagesettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e1214-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1214-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/put-regionalandlanguagesettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e1214-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e1214-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/put-regionalandlanguagesettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e1214-144">Java</span><span class="sxs-lookup"><span data-stu-id="e1214-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/put-regionalandlanguagesettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="e1214-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1214-145">Response</span></span>

<span data-ttu-id="e1214-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e1214-146">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.regionalAndLanguageSettings",
  "name": "put_regionalAndLanguageSettings"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-selected-properties-of-the-signed-in-user"></a><span data-ttu-id="e1214-147">Exemplo 2: Atualizar propriedades selecionadas do usuário in-locar</span><span class="sxs-lookup"><span data-stu-id="e1214-147">Example 2: Update selected properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="e1214-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1214-148">Request</span></span>

<span data-ttu-id="e1214-149">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1214-149">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e1214-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1214-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="e1214-151">C#</span><span class="sxs-lookup"><span data-stu-id="e1214-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/patch-regionalandlanguagesettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e1214-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1214-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/patch-regionalandlanguagesettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e1214-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e1214-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-regionalandlanguagesettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e1214-154">Java</span><span class="sxs-lookup"><span data-stu-id="e1214-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/patch-regionalandlanguagesettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="e1214-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1214-155">Response</span></span>

<span data-ttu-id="e1214-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e1214-156">The following is an example of the response.</span></span>
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


