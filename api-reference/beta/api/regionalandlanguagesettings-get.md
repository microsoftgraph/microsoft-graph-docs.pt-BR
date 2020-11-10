---
title: Obter recurso regionalAndLanguageSettings
description: Recuperar as propriedades do regionalAndLanguageSettings de um usuário
author: jasonbro
localization_priority: Normal
ms.prod: settings
doc_type: apiPageType
ms.openlocfilehash: 39b7f0afb8f7abd8bf1838465c4f51bb5336862e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981073"
---
# <a name="get-regionalandlanguagesettings"></a><span data-ttu-id="65f80-103">Obter regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="65f80-103">Get regionalAndLanguageSettings</span></span>

<span data-ttu-id="65f80-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65f80-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65f80-105">Obter as propriedades de um objeto [regionalAndLanguageSettings](../resources/regionalAndLanguageSettings.md) .</span><span class="sxs-lookup"><span data-stu-id="65f80-105">Get the properties of a [regionalAndLanguageSettings](../resources/regionalAndLanguageSettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="65f80-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="65f80-106">Permissions</span></span>
<span data-ttu-id="65f80-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65f80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65f80-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="65f80-109">Permission Type</span></span>                   |<span data-ttu-id="65f80-110">Permissão (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="65f80-110">Permission (from least to most privileged)</span></span>     |
|----------------------------------|---------------------------------------------- |
|<span data-ttu-id="65f80-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="65f80-111">Delegated (work or school account)</span></span>|<span data-ttu-id="65f80-112">User. Read, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="65f80-112">User.Read, User.Read.All</span></span>                        |
|<span data-ttu-id="65f80-113">Delegado (conta pessoal)</span><span class="sxs-lookup"><span data-stu-id="65f80-113">Delegated (personal account)</span></span>      |<span data-ttu-id="65f80-114">User. Read, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="65f80-114">User.Read, User.Read.All</span></span>              |
|<span data-ttu-id="65f80-115">Application</span><span class="sxs-lookup"><span data-stu-id="65f80-115">Application</span></span>                       |<span data-ttu-id="65f80-116">User. Read, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="65f80-116">User.Read, User.Read.All</span></span>              |

## <a name="http-request"></a><span data-ttu-id="65f80-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="65f80-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /settings/regionalAndLanguageSettings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="65f80-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="65f80-118">Optional query parameters</span></span>
<span data-ttu-id="65f80-119">Você pode usar o `$select` para obter propriedades específicas do regionalAndLanguageSettings, incluindo aquelas que não são retornadas por padrão.</span><span class="sxs-lookup"><span data-stu-id="65f80-119">You can use `$select` to get specific regionalAndLanguageSettings properties, including those that are not returned by default.</span></span>

<span data-ttu-id="65f80-120">Para saber mais sobre as opções de consulta do OData, confira [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="65f80-120">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="65f80-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="65f80-121">Request headers</span></span>
| <span data-ttu-id="65f80-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="65f80-122">Header</span></span>       | <span data-ttu-id="65f80-123">Valor</span><span class="sxs-lookup"><span data-stu-id="65f80-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="65f80-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="65f80-124">Authorization</span></span>  | <span data-ttu-id="65f80-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="65f80-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="65f80-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="65f80-127">Content-Type</span></span>   | <span data-ttu-id="65f80-128">application/json</span><span class="sxs-lookup"><span data-stu-id="65f80-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="65f80-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="65f80-129">Request body</span></span>
<span data-ttu-id="65f80-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="65f80-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65f80-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="65f80-131">Response</span></span>

<span data-ttu-id="65f80-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="65f80-132">If successful, this method returns a `200 OK` response code and [regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65f80-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="65f80-133">Example</span></span>

<span data-ttu-id="65f80-134">O exemplo a seguir obtém as propriedades do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="65f80-134">The following example gets the properties of the signed-in user.</span></span>

### <a name="request"></a><span data-ttu-id="65f80-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="65f80-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="65f80-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="65f80-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_regionalAndLanguageSettings"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/settings/regionalAndLanguageSettings
```
# <a name="c"></a>[<span data-ttu-id="65f80-137">C#</span><span class="sxs-lookup"><span data-stu-id="65f80-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-regionalandlanguagesettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="65f80-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65f80-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-regionalandlanguagesettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="65f80-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65f80-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-regionalandlanguagesettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="65f80-140">Java</span><span class="sxs-lookup"><span data-stu-id="65f80-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-regionalandlanguagesettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="65f80-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="65f80-141">Response</span></span>

><span data-ttu-id="65f80-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="65f80-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.regionalAndLanguageSettings",
  "name": "get_regionalAndLanguageSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "defaultDisplayLanguage": {
        "locale": "en-US",
        "displayName": "English (United States)"
    },
    "authoringLanguages": [
        {
            "locale": "fr-FR",
            "displayName": "French (France)"
        },
        {
            "locale": "de-DE",
            "displayName": "German (Germany)"
        },
    ],
    "defaultTranslationLanguage": {
        "locale": "en-US",
        "displayName": "English (United States)"
    },
    "defaultSpeechInputLanguage": {
        "locale": "en-US",
        "displayName": "English (United States)"
    },
    "defaultRegionalFormat": {
        "locale": "en-GB",
        "displayName": "English (United Kingdom)"
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

<!--
{
  "type": "#page.annotation",
  "description": "Get regionalAndLanguageSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


