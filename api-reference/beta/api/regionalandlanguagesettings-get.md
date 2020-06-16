---
title: Obter recurso regionalAndLanguageSettings
description: Recuperar as propriedades do regionalAndLanguageSettings de um usuário
author: jasonbro
localization_priority: Normal
ms.prod: settings
doc_type: apiPageType
ms.openlocfilehash: 493af1c75e20552e9fb420402365894a04717e17
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/16/2020
ms.locfileid: "44744203"
---
# <a name="get-regionalandlanguagesettings"></a><span data-ttu-id="be87c-103">Obter regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="be87c-103">Get regionalAndLanguageSettings</span></span>

<span data-ttu-id="be87c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be87c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be87c-105">Obter as propriedades de um objeto [regionalAndLanguageSettings](../resources/regionalAndLanguageSettings.md) .</span><span class="sxs-lookup"><span data-stu-id="be87c-105">Get the properties of a [regionalAndLanguageSettings](../resources/regionalAndLanguageSettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="be87c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="be87c-106">Permissions</span></span>
<span data-ttu-id="be87c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="be87c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be87c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="be87c-109">Permission Type</span></span>                   |<span data-ttu-id="be87c-110">Permissão (de menos para mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="be87c-110">Permission (from least to most privileged)</span></span>     |
|----------------------------------|---------------------------------------------- |
|<span data-ttu-id="be87c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="be87c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="be87c-112">User. Read, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="be87c-112">User.Read, User.Read.All</span></span>                        |
|<span data-ttu-id="be87c-113">Delegado (conta pessoal)</span><span class="sxs-lookup"><span data-stu-id="be87c-113">Delegated (personal account)</span></span>      |<span data-ttu-id="be87c-114">User. Read, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="be87c-114">User.Read, User.Read.All</span></span>              |
|<span data-ttu-id="be87c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="be87c-115">Application</span></span>                       |<span data-ttu-id="be87c-116">User. Read, User. Read. All</span><span class="sxs-lookup"><span data-stu-id="be87c-116">User.Read, User.Read.All</span></span>              |

## <a name="http-request"></a><span data-ttu-id="be87c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="be87c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /settings/regionalAndLanguageSettings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="be87c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="be87c-118">Optional query parameters</span></span>
<span data-ttu-id="be87c-119">Você pode usar o `$select` para obter propriedades específicas do regionalAndLanguageSettings, incluindo aquelas que não são retornadas por padrão.</span><span class="sxs-lookup"><span data-stu-id="be87c-119">You can use `$select` to get specific regionalAndLanguageSettings properties, including those that are not returned by default.</span></span>

<span data-ttu-id="be87c-120">Para saber mais sobre as opções de consulta do OData, confira [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="be87c-120">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="be87c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="be87c-121">Request headers</span></span>
| <span data-ttu-id="be87c-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="be87c-122">Header</span></span>       | <span data-ttu-id="be87c-123">Valor</span><span class="sxs-lookup"><span data-stu-id="be87c-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="be87c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="be87c-124">Authorization</span></span>  | <span data-ttu-id="be87c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="be87c-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="be87c-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="be87c-127">Content-Type</span></span>   | <span data-ttu-id="be87c-128">application/json</span><span class="sxs-lookup"><span data-stu-id="be87c-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="be87c-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="be87c-129">Request body</span></span>
<span data-ttu-id="be87c-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="be87c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be87c-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="be87c-131">Response</span></span>

<span data-ttu-id="be87c-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="be87c-132">If successful, this method returns a `200 OK` response code and [regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be87c-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="be87c-133">Example</span></span>

### <a name="example-1-get-the-properties-of-the-signed-in-user"></a><span data-ttu-id="be87c-134">Exemplo 1: Obter as propriedades do usuário conectado</span><span class="sxs-lookup"><span data-stu-id="be87c-134">Example 1: Get the properties of the signed-in user</span></span>

#### <a name="request"></a><span data-ttu-id="be87c-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="be87c-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="be87c-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="be87c-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_regionalAndLanguageSettings"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/settings/regionalAndLanguageSettings
```

##### <a name="response"></a><span data-ttu-id="be87c-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="be87c-137">Response</span></span>
<span data-ttu-id="be87c-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="be87c-138">Here is an example of the response.</span></span> <span data-ttu-id="be87c-139">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="be87c-139">Note: The response object shown here may be truncated for brevity.</span></span> 

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
