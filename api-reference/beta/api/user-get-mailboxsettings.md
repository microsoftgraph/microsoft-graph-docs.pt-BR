---
title: Obter as configurações da caixa de correio do usuário
description: 'Obtenha as configurações de caixa de correio do usuário. Isso inclui configurações para respostas automáticas (notificar pessoas automaticamente quando '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9cf98ffc7e0824737239868bbaadb3b2c4bead0f
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637350"
---
# <a name="get-user-mailbox-settings"></a><span data-ttu-id="fd5f2-104">Obter as configurações da caixa de correio do usuário</span><span class="sxs-lookup"><span data-stu-id="fd5f2-104">Get user mailbox settings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd5f2-105">Obtenha as [mailboxSettings](../resources/mailboxsettings.md) do usuário.</span><span class="sxs-lookup"><span data-stu-id="fd5f2-105">Get the user's [mailboxSettings](../resources/mailboxsettings.md).</span></span> <span data-ttu-id="fd5f2-106">Isso inclui as configurações para respostas automáticas (notificar as pessoas automaticamente no recebimento de seus emails), localidade (idioma e país/região), fuso horário e horário de trabalho.</span><span class="sxs-lookup"><span data-stu-id="fd5f2-106">This includes settings for automatic replies (notify people automatically upon receipt of their email), locale (language and country/region), time zone, and working hours.</span></span>

<span data-ttu-id="fd5f2-107">Você pode exibir todas as configurações de caixa de correio ou obter configurações específicas.</span><span class="sxs-lookup"><span data-stu-id="fd5f2-107">You can view all mailbox settings, or, get specific settings.</span></span>

<span data-ttu-id="fd5f2-108">O fuso horário é uma das configurações de preferência que um usuário pode fazer na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="fd5f2-108">Time zone is one of the preferred settings a user can set up for the user's mailbox.</span></span> <span data-ttu-id="fd5f2-109">O usuário escolhe-o dos [fusos horários com suporte](outlookuser-supportedtimezones.md) que um administrador configurou para o servidor de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="fd5f2-109">The user chooses it from the [supported time zones](outlookuser-supportedtimezones.md) that an administrator has set up for the user's mailbox server.</span></span> <span data-ttu-id="fd5f2-110">O administrador configura os fusos horários no formato de fuso horário do Windows ou da [autoridade de números da Internet (IANA)](https://www.iana.org/time-zones) (também conhecido como fuso horário do Olson).</span><span class="sxs-lookup"><span data-stu-id="fd5f2-110">The administrator sets up time zones in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="fd5f2-111">O formato do Windows é o padrão.</span><span class="sxs-lookup"><span data-stu-id="fd5f2-111">The Windows format is the default.</span></span> 

<span data-ttu-id="fd5f2-112">Ao obter o fuso horário de preferência de um usuário, ele é retornado no formato em que foi configurado.</span><span class="sxs-lookup"><span data-stu-id="fd5f2-112">When you get a user's preferred time zone, the time zone is returned in the format that it was set up.</span></span> <span data-ttu-id="fd5f2-113">Se quiser que o fuso horário esteja em um formato específico (Windows ou IANA), você pode primeiro [atualizar o fuso horário de preferência nesse formato como uma configuração de caixa de correio](user-update-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="fd5f2-113">If you want that time zone to be in a specific format (Windows or IANA), you can first [update the preferred time zone in that format as a mailbox setting](user-update-mailboxsettings.md).</span></span> <span data-ttu-id="fd5f2-114">Posteriormente, você poderá obter o fuso horário nesse formato.</span><span class="sxs-lookup"><span data-stu-id="fd5f2-114">Subsequently you will be able to get the time zone in that format.</span></span> <span data-ttu-id="fd5f2-115">Como alternativa, você pode gerenciar a conversão de formato separadamente no seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fd5f2-115">Alternatively, you can manage the format conversion separately in your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd5f2-116">Permissões</span><span class="sxs-lookup"><span data-stu-id="fd5f2-116">Permissions</span></span>
<span data-ttu-id="fd5f2-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd5f2-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd5f2-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fd5f2-119">Permission type</span></span>      | <span data-ttu-id="fd5f2-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fd5f2-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd5f2-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fd5f2-121">Delegated (work or school account)</span></span> | <span data-ttu-id="fd5f2-122">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd5f2-122">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="fd5f2-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fd5f2-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd5f2-124">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd5f2-124">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="fd5f2-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fd5f2-125">Application</span></span> | <span data-ttu-id="fd5f2-126">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd5f2-126">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd5f2-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fd5f2-127">HTTP request</span></span>
<span data-ttu-id="fd5f2-128">Para obter todas as configurações de caixa de correio de um usuário:</span><span class="sxs-lookup"><span data-stu-id="fd5f2-128">To get all the mailbox settings for a user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

<span data-ttu-id="fd5f2-129">Para obter configurações específicas – somente as configurações de respostas automáticas, localidade, fuso horário ou horário de trabalho:</span><span class="sxs-lookup"><span data-stu-id="fd5f2-129">To get specific settings - only the automatic replies settings, locale, time zone, or working hours:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings/automaticRepliesSetting
GET /users/{id|userPrincipalName}/mailboxSettings/automaticRepliesSetting

GET /me/mailboxSettings/language
GET /users/{id|userPrincipalName}/mailboxSettings/language

GET /me/mailboxSettings/timeZone
GET /users/{id|userPrincipalName}/mailboxSettings/timeZone

GET /me/mailboxSettings/workingHours
GET /users/{id|userPrincipalName}/mailboxSettings/workingHours
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fd5f2-130">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fd5f2-130">Optional query parameters</span></span>
<span data-ttu-id="fd5f2-131">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fd5f2-131">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fd5f2-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fd5f2-132">Request headers</span></span>
| <span data-ttu-id="fd5f2-133">Nome</span><span class="sxs-lookup"><span data-stu-id="fd5f2-133">Name</span></span>       | <span data-ttu-id="fd5f2-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="fd5f2-134">Type</span></span> | <span data-ttu-id="fd5f2-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="fd5f2-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fd5f2-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="fd5f2-136">Authorization</span></span>  | <span data-ttu-id="fd5f2-137">string</span><span class="sxs-lookup"><span data-stu-id="fd5f2-137">string</span></span>  | <span data-ttu-id="fd5f2-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fd5f2-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fd5f2-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fd5f2-140">Request body</span></span>
<span data-ttu-id="fd5f2-141">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fd5f2-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd5f2-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="fd5f2-142">Response</span></span>

<span data-ttu-id="fd5f2-143">Se for bem-sucedido, este método retornará um código de resposta `200 OK` e um dos seguintes objetos solicitados no corpo da resposta:</span><span class="sxs-lookup"><span data-stu-id="fd5f2-143">If successful, this method returns a `200 OK` response code and one of the following requested objects in the response body:</span></span>

- <span data-ttu-id="fd5f2-144">Objeto [mailboxSettings](../resources/mailboxsettings.md)</span><span class="sxs-lookup"><span data-stu-id="fd5f2-144">[mailboxSettings](../resources/mailboxsettings.md) object</span></span>
- <span data-ttu-id="fd5f2-145">Objeto [automaticRepliesSetting](../resources/automaticrepliessetting.md)</span><span class="sxs-lookup"><span data-stu-id="fd5f2-145">[automaticRepliesSetting](../resources/automaticrepliessetting.md) object</span></span>
- <span data-ttu-id="fd5f2-146">Objeto [localeInfo](../resources/localeinfo.md)</span><span class="sxs-lookup"><span data-stu-id="fd5f2-146">[localeInfo](../resources/localeinfo.md) object</span></span>
- <span data-ttu-id="fd5f2-147">cadeia de caracteres (para **timeZone**)</span><span class="sxs-lookup"><span data-stu-id="fd5f2-147">string (for **timeZone**)</span></span>
- [<span data-ttu-id="fd5f2-148">workingHours</span><span class="sxs-lookup"><span data-stu-id="fd5f2-148">workingHours</span></span>](../resources/workinghours.md)

## <a name="example"></a><span data-ttu-id="fd5f2-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fd5f2-149">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="fd5f2-150">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="fd5f2-150">Request 1</span></span>
<span data-ttu-id="fd5f2-151">O primeiro exemplo obtém todas as configurações da caixa de correio do usuário conectado, que incluem configurações de fuso horário, respostas automáticas, localidade (idioma e país/região) e horário de trabalho.</span><span class="sxs-lookup"><span data-stu-id="fd5f2-151">The first example gets all the mailbox settings of the signed-in user's mailbox, which include settings for time zone, automatic replies, locale (language and country/region), and working hours.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings
```
##### <a name="response-1"></a><span data-ttu-id="fd5f2-152">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="fd5f2-152">Response 1</span></span>
<span data-ttu-id="fd5f2-153">A resposta inclui todas as configurações de caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="fd5f2-153">The response includes all the mailbox settings of the signed-in user.</span></span> <span data-ttu-id="fd5f2-154">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="fd5f2-154">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="fd5f2-155">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fd5f2-155">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/mailboxSettings",
    "automaticRepliesSetting": {
        "status": "Scheduled",
        "externalAudience": "All",
        "scheduledStartDateTime": {
            "dateTime": "2016-03-14T07:00:00.0000000",
            "timeZone": "UTC"
        },
        "scheduledEndDateTime": {
            "dateTime": "2016-03-28T07:00:00.0000000",
            "timeZone": "UTC"
        },
        "internalReplyMessage": "<html>\n<body>\n<p>I'm at our company's worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n",
        "externalReplyMessage": "<html>\n<body>\n<p>I'm at the Contoso worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n"
    },
    "timeZone":"UTC",
    "language":{
      "locale":"en-US",
      "displayName":"English (United States)"
    },
    "workingHours":{
        "daysOfWeek":[
            "monday",
            "tuesday",
            "wednesday",
            "thursday",
            "friday"
        ],
        "startTime":"08:00:00.0000000",
        "endTime":"17:00:00.0000000",
        "timeZone":{
            "name":"Pacific Standard Time"
        }
    }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="fd5f2-156">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="fd5f2-156">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fd5f2-157">Basic</span><span class="sxs-lookup"><span data-stu-id="fd5f2-157">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_mailboxsettings_1-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fd5f2-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fd5f2-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_mailboxsettings_1-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-2"></a><span data-ttu-id="fd5f2-159">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="fd5f2-159">Request 2</span></span>
<span data-ttu-id="fd5f2-160">O segundo exemplo obtém especificamente as configurações de respostas automáticas da caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="fd5f2-160">The second example gets specifically the automatic replies settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings/automaticRepliesSetting
```
##### <a name="response-2"></a><span data-ttu-id="fd5f2-161">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="fd5f2-161">Response 2</span></span>
<span data-ttu-id="fd5f2-p108">A resposta inclui apenas as configurações de respostas automáticas. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fd5f2-p108">The response includes only the automatic replies settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/mailboxSettings/automaticRepliesSetting",
    "status": "alwaysEnabled",
    "externalAudience": "None",
    "scheduledStartDateTime": {
        "dateTime": "2016-03-19T02:00:00.0000000",
        "timeZone": "UTC"
    },
    "scheduledEndDateTime": {
        "dateTime": "2016-03-20T02:00:00.0000000",
        "timeZone": "UTC"
    },
    "internalReplyMessage": "<html>\n<body>\n<p>I'm at our company's worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n",
    "externalReplyMessage": "<html>\n<body>\n<p>I'm at the Contoso worldwide reunion and will respond to your message as soon as I return.<br>\n</p></body>\n</html>\n"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="fd5f2-165">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="fd5f2-165">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="fd5f2-166">Basic</span><span class="sxs-lookup"><span data-stu-id="fd5f2-166">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_mailboxsettings_2-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fd5f2-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fd5f2-167">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_mailboxsettings_2-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


##### <a name="request-3"></a><span data-ttu-id="fd5f2-168">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="fd5f2-168">Request 3</span></span>
<span data-ttu-id="fd5f2-169">O terceiro exemplo obtém especificamente as configurações de horário de trabalho da caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="fd5f2-169">The third example gets specifically the working hour settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_mailboxsettings_3"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings/workingHours
```
##### <a name="response-3"></a><span data-ttu-id="fd5f2-170">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="fd5f2-170">Response 3</span></span>
<span data-ttu-id="fd5f2-171">A resposta inclui apenas as configurações de horário de trabalho.</span><span class="sxs-lookup"><span data-stu-id="fd5f2-171">The response includes only the working hours settings.</span></span> <span data-ttu-id="fd5f2-172">As horas de trabalho do usuário estão em um [fuso horário personalizado](../resources/customtimezone.md).</span><span class="sxs-lookup"><span data-stu-id="fd5f2-172">Notice that the user's work hours are in a [custom time zone](../resources/customtimezone.md).</span></span> <span data-ttu-id="fd5f2-173">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="fd5f2-173">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="fd5f2-174">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fd5f2-174">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_mailboxsettings_3",
  "truncated": true,
  "@odata.type": "microsoft.graph.workingHours"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('94447c6e-ea4c-494c-a9ed-d905e366c5cb')/mailboxSettings/workingHours",
    "daysOfWeek":[
        "monday",
        "tuesday",
        "wednesday",
        "thursday",
        "friday",
        "saturday"
    ],
    "startTime":"09:00:00.0000000",
    "endTime":"18:30:00.0000000",
    "timeZone":{
        "@odata.type":"#microsoft.graph.customTimeZone",
        "bias":-200,
        "name":"Customized Time Zone",
        "standardOffset":{
            "time":"02:00:00.0000000",
            "dayOccurrence":4,
            "dayOfWeek":"sunday",
            "month":5,
            "year":0
        },
        "daylightOffset":{
            "daylightBias":-100,
            "time":"02:00:00.0000000",
            "dayOccurrence":2,
            "dayOfWeek":"sunday",
            "month":10,
            "year":0
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get mailbox settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-get-mailboxsettings.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-get-mailboxsettings.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/user-get-mailboxsettings.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-get-mailboxsettings.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
