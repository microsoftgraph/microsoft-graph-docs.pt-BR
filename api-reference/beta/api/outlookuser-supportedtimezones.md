---
title: 'outlookUser: supportedTimeZones'
description: Obtenha a lista de fusos horários com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 5c661507dfa71f89a1947f33f80d26d090cfde87
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342387"
---
# <a name="outlookuser-supportedtimezones"></a><span data-ttu-id="08246-103">outlookUser: supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="08246-103">outlookUser: supportedTimeZones</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08246-104">Obtenha a lista de fusos horários com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="08246-104">Get the list of time zones that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="08246-105">É possível especificar explicitamente que os fusos horário sejam retornados no formato do Windows ou da [Autoridade para Atribuição de Números na Internet (IANA)](https://www.iana.org/time-zones) (também conhecido como fuso horário de Olson).</span><span class="sxs-lookup"><span data-stu-id="08246-105">You can explicitly specify to have time zones returned in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="08246-106">O formato do Windows é o padrão.</span><span class="sxs-lookup"><span data-stu-id="08246-106">The Windows format is the default.</span></span>

<span data-ttu-id="08246-107">Ao configurar um cliente do Outlook, o usuário seleciona o fuso horário na lista compatível.</span><span class="sxs-lookup"><span data-stu-id="08246-107">When setting up an Outlook client, the user selects the preferred time zone from this supported list.</span></span> <span data-ttu-id="08246-108">Posteriormente, é possível obter o fuso horário de sua preferência [acessando as configurações da caixa de correio do usuário](user-get-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="08246-108">You can subsequently get the preferred time zone by [getting the user's mailbox settings](user-get-mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="08246-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="08246-109">Permissions</span></span>
<span data-ttu-id="08246-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08246-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08246-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="08246-112">Permission type</span></span>      | <span data-ttu-id="08246-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="08246-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08246-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="08246-114">Delegated (work or school account)</span></span> | <span data-ttu-id="08246-115">User.Read, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="08246-115">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="08246-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="08246-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08246-117">User.Read</span><span class="sxs-lookup"><span data-stu-id="08246-117">User.Read</span></span>    |
|<span data-ttu-id="08246-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="08246-118">Application</span></span> | <span data-ttu-id="08246-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="08246-119">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="08246-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08246-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedTimeZones
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones

GET /me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
```

## <a name="function-parameters"></a><span data-ttu-id="08246-121">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="08246-121">Function parameters</span></span>
| <span data-ttu-id="08246-122">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="08246-122">Parameter</span></span>      | <span data-ttu-id="08246-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="08246-123">Type</span></span>    | <span data-ttu-id="08246-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="08246-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="08246-125">TimeZoneStandard</span><span class="sxs-lookup"><span data-stu-id="08246-125">TimeZoneStandard</span></span>  | <span data-ttu-id="08246-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="08246-126">String</span></span>  | <span data-ttu-id="08246-127">Um formato de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="08246-127">A time zone format.</span></span> <span data-ttu-id="08246-128">Os valores com suporte são: `Windows` e `Iana`.</span><span class="sxs-lookup"><span data-stu-id="08246-128">Supported values are: `Windows`, and `Iana`.</span></span> <span data-ttu-id="08246-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="08246-129">Optional.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="08246-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="08246-130">Request headers</span></span>
| <span data-ttu-id="08246-131">Nome</span><span class="sxs-lookup"><span data-stu-id="08246-131">Name</span></span>       | <span data-ttu-id="08246-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="08246-132">Type</span></span> | <span data-ttu-id="08246-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="08246-133">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="08246-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="08246-134">Authorization</span></span>  | <span data-ttu-id="08246-135">string</span><span class="sxs-lookup"><span data-stu-id="08246-135">string</span></span>  | <span data-ttu-id="08246-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08246-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="08246-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="08246-138">Request body</span></span>
<span data-ttu-id="08246-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="08246-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08246-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="08246-140">Response</span></span>
<span data-ttu-id="08246-141">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [timeZoneInformation](../resources/timezoneinformation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="08246-141">If successful, this method returns `200 OK` response code and a collection of [timeZoneInformation](../resources/timezoneinformation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08246-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="08246-142">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="08246-143">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="08246-143">Request 1</span></span>
<span data-ttu-id="08246-144">O exemplo a seguir não especifica o parâmetro `timeZoneStandard` e obtém a lista de fusos horários compatíveis representados no formato do Windows.</span><span class="sxs-lookup"><span data-stu-id="08246-144">The following example does not specify the `timeZoneStandard` parameter, and gets the list of supported time zones represented in the Windows time zone format.</span></span> 

# <a name="httptabhttp"></a>[<span data-ttu-id="08246-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="08246-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_default"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/supportedTimeZones
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="08246-146">C#</span><span class="sxs-lookup"><span data-stu-id="08246-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-supportedtimezones-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="08246-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08246-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-supportedtimezones-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="08246-148">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="08246-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-supportedtimezones-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="08246-149">Java</span><span class="sxs-lookup"><span data-stu-id="08246-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-supportedtimezones-default-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="08246-150">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="08246-150">Response 1</span></span>
<span data-ttu-id="08246-151">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="08246-151">Here is an example of the response.</span></span> 
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

##### <a name="request-2"></a><span data-ttu-id="08246-152">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="08246-152">Request 2</span></span>
<span data-ttu-id="08246-153">O exemplo a seguir especifica `Iana` para o parâmetro `TimeZoneStandard` e obtém a lista de fusos horários compatíveis representados no formato da IANA.</span><span class="sxs-lookup"><span data-stu-id="08246-153">The following example specifies `Iana` for the `TimeZoneStandard` parameter, and gets the list of supported time zones represented in IANA format.</span></span> 


# <a name="httptabhttp"></a>[<span data-ttu-id="08246-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="08246-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_iana"
} -->

```http
GET https://graph.microsoft.com/beta/me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'Iana')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="08246-155">C#</span><span class="sxs-lookup"><span data-stu-id="08246-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-supportedtimezones-iana-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="08246-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08246-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-supportedtimezones-iana-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="08246-157">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="08246-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-supportedtimezones-iana-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="08246-158">Java</span><span class="sxs-lookup"><span data-stu-id="08246-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-supportedtimezones-iana-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a><span data-ttu-id="08246-159">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="08246-159">Response 2</span></span>
<span data-ttu-id="08246-160">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="08246-160">Here is an example of the response.</span></span> 

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
  ]
}
-->
