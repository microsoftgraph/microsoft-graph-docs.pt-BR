---
title: 'outlookUser: supportedTimeZones'
description: Obtenha a lista de fusos horários com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 4fe5c0b66a6c5b1a4574a0bfeb578808195fe38b
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35269129"
---
# <a name="outlookuser-supportedtimezones"></a><span data-ttu-id="5d22c-103">outlookUser: supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="5d22c-103">outlookUser: supportedTimeZones</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d22c-104">Obtenha a lista de fusos horários com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="5d22c-104">Get the list of time zones that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="5d22c-105">É possível especificar explicitamente que os fusos horário sejam retornados no formato do Windows ou da [Autoridade para Atribuição de Números na Internet (IANA)](https://www.iana.org/time-zones) (também conhecido como fuso horário de Olson).</span><span class="sxs-lookup"><span data-stu-id="5d22c-105">You can explicitly specify to have time zones returned in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="5d22c-106">O formato do Windows é o padrão.</span><span class="sxs-lookup"><span data-stu-id="5d22c-106">The Windows format is the default.</span></span>

<span data-ttu-id="5d22c-107">Ao configurar um cliente do Outlook, o usuário seleciona o fuso horário na lista compatível.</span><span class="sxs-lookup"><span data-stu-id="5d22c-107">When setting up an Outlook client, the user selects the preferred time zone from this supported list.</span></span> <span data-ttu-id="5d22c-108">Posteriormente, é possível obter o fuso horário de sua preferência [acessando as configurações da caixa de correio do usuário](user-get-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="5d22c-108">You can subsequently get the preferred time zone by [getting the user's mailbox settings](user-get-mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="5d22c-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="5d22c-109">Permissions</span></span>
<span data-ttu-id="5d22c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5d22c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d22c-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5d22c-112">Permission type</span></span>      | <span data-ttu-id="5d22c-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5d22c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d22c-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5d22c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5d22c-115">User.Read, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="5d22c-115">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="5d22c-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5d22c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d22c-117">User.Read</span><span class="sxs-lookup"><span data-stu-id="5d22c-117">User.Read</span></span>    |
|<span data-ttu-id="5d22c-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5d22c-118">Application</span></span> | <span data-ttu-id="5d22c-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d22c-119">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d22c-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5d22c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedTimeZones
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones

GET /me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
```

## <a name="function-parameters"></a><span data-ttu-id="5d22c-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="5d22c-121">Function parameters</span></span>
| <span data-ttu-id="5d22c-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="5d22c-122">Parameter</span></span>      | <span data-ttu-id="5d22c-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="5d22c-123">Type</span></span>    | <span data-ttu-id="5d22c-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d22c-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5d22c-125">TimeZoneStandard</span><span class="sxs-lookup"><span data-stu-id="5d22c-125">TimeZoneStandard</span></span>  | <span data-ttu-id="5d22c-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5d22c-126">String</span></span>  | <span data-ttu-id="5d22c-127">Um formato de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="5d22c-127">A time zone format.</span></span> <span data-ttu-id="5d22c-128">Os valores com suporte são: `Windows` e `Iana`.</span><span class="sxs-lookup"><span data-stu-id="5d22c-128">Supported values are: `Windows`, and `Iana`.</span></span> <span data-ttu-id="5d22c-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="5d22c-129">Optional.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="5d22c-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5d22c-130">Request headers</span></span>
| <span data-ttu-id="5d22c-131">Nome</span><span class="sxs-lookup"><span data-stu-id="5d22c-131">Name</span></span>       | <span data-ttu-id="5d22c-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="5d22c-132">Type</span></span> | <span data-ttu-id="5d22c-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d22c-133">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5d22c-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="5d22c-134">Authorization</span></span>  | <span data-ttu-id="5d22c-135">string</span><span class="sxs-lookup"><span data-stu-id="5d22c-135">string</span></span>  | <span data-ttu-id="5d22c-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5d22c-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d22c-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5d22c-138">Request body</span></span>
<span data-ttu-id="5d22c-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5d22c-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d22c-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="5d22c-140">Response</span></span>
<span data-ttu-id="5d22c-141">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [timeZoneInformation](../resources/timezoneinformation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d22c-141">If successful, this method returns `200 OK` response code and a collection of [timeZoneInformation](../resources/timezoneinformation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d22c-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5d22c-142">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="5d22c-143">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="5d22c-143">Request 1</span></span>
<span data-ttu-id="5d22c-144">O exemplo a seguir não especifica o parâmetro `timeZoneStandard` e obtém a lista de fusos horários compatíveis representados no formato do Windows.</span><span class="sxs-lookup"><span data-stu-id="5d22c-144">The following example does not specify the `timeZoneStandard` parameter, and gets the list of supported time zones represented in the Windows time zone format.</span></span> 
<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_default"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/supportedTimeZones
```

##### <a name="response-1"></a><span data-ttu-id="5d22c-145">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="5d22c-145">Response 1</span></span>
<span data-ttu-id="5d22c-146">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d22c-146">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "user_supportedtimezones_default",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeZoneInformation",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.timeZoneInformation)",
  "value":[
    {
      "alias":"Dateline Standard Time",
      "displayName":"(UTC-12:00) International Date Line West"
    },
    {
      "alias":"Samoa Standard Time",
      "displayName":"(UTC+13:00) Samoa"
    },
    {
       "alias":"UTC-11",
       "displayName":"(UTC-11:00) Coordinated Universal Time-11"
    },
    {
      "alias":"Aleutian Standard Time",
      "displayName":"(UTC-10:00) Aleutian Islands"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5d22c-147">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="5d22c-147">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5d22c-148">C#</span><span class="sxs-lookup"><span data-stu-id="5d22c-148">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_supportedtimezones_default-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5d22c-149">Javascript</span><span class="sxs-lookup"><span data-stu-id="5d22c-149">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_supportedtimezones_default-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="5d22c-150">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5d22c-150">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/user_supportedtimezones_default-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-2"></a><span data-ttu-id="5d22c-151">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="5d22c-151">Request 2</span></span>
<span data-ttu-id="5d22c-152">O exemplo a seguir especifica `Iana` para o parâmetro `TimeZoneStandard` e obtém a lista de fusos horários compatíveis representados no formato da IANA.</span><span class="sxs-lookup"><span data-stu-id="5d22c-152">The following example specifies `Iana` for the `TimeZoneStandard` parameter, and gets the list of supported time zones represented in IANA format.</span></span> 

<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_iana"
} -->

```http
GET https://graph.microsoft.com/beta/me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'Iana')
```

##### <a name="response-2"></a><span data-ttu-id="5d22c-153">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="5d22c-153">Response 2</span></span>
<span data-ttu-id="5d22c-154">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d22c-154">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "name": "user_supportedtimezones_iana",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeZoneInformation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.timeZoneInformation)",
  "value":[
    {
      "alias":"Etc/GMT+12",
      "displayName":"Etc/GMT+12"
    },
    {
      "alias":"US/Samoa",
      "displayName":"US/Samoa"
    },
    {
      "alias":"Etc/GMT+11",
      "displayName":"Etc/GMT+11"
    },
    {
      "alias":"US/Aleutian",
      "displayName":"US/Aleutian"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5d22c-155">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="5d22c-155">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="5d22c-156">C#</span><span class="sxs-lookup"><span data-stu-id="5d22c-156">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_supportedtimezones_iana-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5d22c-157">Javascript</span><span class="sxs-lookup"><span data-stu-id="5d22c-157">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_supportedtimezones_iana-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="5d22c-158">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5d22c-158">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/user_supportedtimezones_iana-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: supportedTimeZones",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlookuser-supportedtimezones.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/outlookuser-supportedtimezones.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlookuser-supportedtimezones.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/outlookuser-supportedtimezones.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlookuser-supportedtimezones.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
