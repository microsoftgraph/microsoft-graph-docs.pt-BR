---
title: 'outlookUser: supportedTimeZones'
description: Obtenha a lista de fusos horários com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 53bdd461051f2a137c0a9b04b82a0d9acc254065
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128299"
---
# <a name="outlookuser-supportedtimezones"></a><span data-ttu-id="cefbe-103">outlookUser: supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="cefbe-103">outlookUser: supportedTimeZones</span></span>

<span data-ttu-id="cefbe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cefbe-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cefbe-105">Obtenha a lista de fusos horários com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="cefbe-105">Get the list of time zones that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="cefbe-106">É possível especificar explicitamente que os fusos horário sejam retornados no formato do Windows ou da [Autoridade para Atribuição de Números na Internet (IANA)](https://www.iana.org/time-zones) (também conhecido como fuso horário de Olson).</span><span class="sxs-lookup"><span data-stu-id="cefbe-106">You can explicitly specify to have time zones returned in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="cefbe-107">O formato do Windows é o padrão.</span><span class="sxs-lookup"><span data-stu-id="cefbe-107">The Windows format is the default.</span></span>

<span data-ttu-id="cefbe-108">Ao configurar um cliente do Outlook, o usuário seleciona o fuso horário na lista compatível.</span><span class="sxs-lookup"><span data-stu-id="cefbe-108">When setting up an Outlook client, the user selects the preferred time zone from this supported list.</span></span> <span data-ttu-id="cefbe-109">Posteriormente, é possível obter o fuso horário de sua preferência [acessando as configurações da caixa de correio do usuário](user-get-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="cefbe-109">You can subsequently get the preferred time zone by [getting the user's mailbox settings](user-get-mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="cefbe-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="cefbe-110">Permissions</span></span>
<span data-ttu-id="cefbe-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cefbe-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cefbe-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cefbe-113">Permission type</span></span>      | <span data-ttu-id="cefbe-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cefbe-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cefbe-115">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cefbe-115">Delegated (work or school account)</span></span> | <span data-ttu-id="cefbe-116">User.Read, User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="cefbe-116">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="cefbe-117">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cefbe-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cefbe-118">User.Read</span><span class="sxs-lookup"><span data-stu-id="cefbe-118">User.Read</span></span>    |
|<span data-ttu-id="cefbe-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cefbe-119">Application</span></span> | <span data-ttu-id="cefbe-120">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="cefbe-120">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cefbe-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cefbe-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedTimeZones
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones

GET /me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
```

## <a name="function-parameters"></a><span data-ttu-id="cefbe-122">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="cefbe-122">Function parameters</span></span>
| <span data-ttu-id="cefbe-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="cefbe-123">Parameter</span></span>       | <span data-ttu-id="cefbe-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="cefbe-124">Type</span></span> | <span data-ttu-id="cefbe-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="cefbe-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cefbe-126">TimeZoneStandard</span><span class="sxs-lookup"><span data-stu-id="cefbe-126">TimeZoneStandard</span></span>  | <span data-ttu-id="cefbe-127">timeZoneStandard</span><span class="sxs-lookup"><span data-stu-id="cefbe-127">timeZoneStandard</span></span>  | <span data-ttu-id="cefbe-128">Um formato de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="cefbe-128">A time zone format.</span></span> <span data-ttu-id="cefbe-129">Os valores com suporte são: `Windows` e `Iana`.</span><span class="sxs-lookup"><span data-stu-id="cefbe-129">Supported values are: `Windows`, and `Iana`.</span></span> <span data-ttu-id="cefbe-130">Opcional.</span><span class="sxs-lookup"><span data-stu-id="cefbe-130">Optional.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="cefbe-131">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cefbe-131">Request headers</span></span>
| <span data-ttu-id="cefbe-132">Nome</span><span class="sxs-lookup"><span data-stu-id="cefbe-132">Name</span></span>       | <span data-ttu-id="cefbe-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="cefbe-133">Type</span></span> | <span data-ttu-id="cefbe-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="cefbe-134">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cefbe-135">Autorização</span><span class="sxs-lookup"><span data-stu-id="cefbe-135">Authorization</span></span>  | <span data-ttu-id="cefbe-136">string</span><span class="sxs-lookup"><span data-stu-id="cefbe-136">string</span></span>  | <span data-ttu-id="cefbe-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cefbe-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cefbe-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cefbe-139">Request body</span></span>
<span data-ttu-id="cefbe-140">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cefbe-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cefbe-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="cefbe-141">Response</span></span>
<span data-ttu-id="cefbe-142">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [timeZoneInformation](../resources/timezoneinformation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cefbe-142">If successful, this method returns `200 OK` response code and a collection of [timeZoneInformation](../resources/timezoneinformation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cefbe-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cefbe-143">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="cefbe-144">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="cefbe-144">Request 1</span></span>
<span data-ttu-id="cefbe-145">O exemplo a seguir não especifica o parâmetro `timeZoneStandard` e obtém a lista de fusos horários compatíveis representados no formato do Windows.</span><span class="sxs-lookup"><span data-stu-id="cefbe-145">The following example does not specify the `timeZoneStandard` parameter, and gets the list of supported time zones represented in the Windows time zone format.</span></span> 

# <a name="http"></a>[<span data-ttu-id="cefbe-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="cefbe-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_default"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/outlook/supportedTimeZones
```
# <a name="c"></a>[<span data-ttu-id="cefbe-147">C#</span><span class="sxs-lookup"><span data-stu-id="cefbe-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-supportedtimezones-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cefbe-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cefbe-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-supportedtimezones-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cefbe-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cefbe-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-supportedtimezones-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cefbe-150">Java</span><span class="sxs-lookup"><span data-stu-id="cefbe-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-supportedtimezones-default-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="cefbe-151">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="cefbe-151">Response 1</span></span>
<span data-ttu-id="cefbe-152">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cefbe-152">Here is an example of the response.</span></span> 
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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.timeZoneInformation)",
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

##### <a name="request-2"></a><span data-ttu-id="cefbe-153">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="cefbe-153">Request 2</span></span>
<span data-ttu-id="cefbe-154">O exemplo a seguir especifica `Iana` para o parâmetro `TimeZoneStandard` e obtém a lista de fusos horários compatíveis representados no formato da IANA.</span><span class="sxs-lookup"><span data-stu-id="cefbe-154">The following example specifies `Iana` for the `TimeZoneStandard` parameter, and gets the list of supported time zones represented in IANA format.</span></span> 


# <a name="http"></a>[<span data-ttu-id="cefbe-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="cefbe-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_iana"
} -->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'Iana')
```
# <a name="c"></a>[<span data-ttu-id="cefbe-156">C#</span><span class="sxs-lookup"><span data-stu-id="cefbe-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-supportedtimezones-iana-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cefbe-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cefbe-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-supportedtimezones-iana-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cefbe-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cefbe-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-supportedtimezones-iana-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cefbe-159">Java</span><span class="sxs-lookup"><span data-stu-id="cefbe-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-supportedtimezones-iana-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a><span data-ttu-id="cefbe-160">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="cefbe-160">Response 2</span></span>
<span data-ttu-id="cefbe-161">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cefbe-161">Here is an example of the response.</span></span> 

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
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.timeZoneInformation)",
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
<!-- {
  "type": "#page.annotation",
  "description": "user: supportedTimeZones",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

