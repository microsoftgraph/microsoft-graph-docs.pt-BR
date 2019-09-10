---
title: Obter as configurações da caixa de correio do usuário
description: 'Obtenha as configurações de caixa de correio do usuário. Isso inclui configurações para respostas automáticas (notificar pessoas automaticamente quando '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 296a5225ca924374a3c38242207f7f329b2e8401
ms.sourcegitcommit: 3e7769ad097e9c34233fa5fea83afa23c34e14a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822806"
---
# <a name="get-user-mailbox-settings"></a><span data-ttu-id="8731d-104">Obter as configurações da caixa de correio do usuário</span><span class="sxs-lookup"><span data-stu-id="8731d-104">Get user mailbox settings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8731d-105">Obtenha as [mailboxSettings](../resources/mailboxsettings.md) do usuário.</span><span class="sxs-lookup"><span data-stu-id="8731d-105">Get the user's [mailboxSettings](../resources/mailboxsettings.md).</span></span> <span data-ttu-id="8731d-106">Você pode exibir todas as configurações da caixa de correio ou obter configurações específicas.</span><span class="sxs-lookup"><span data-stu-id="8731d-106">You can view all mailbox settings, or get specific settings.</span></span>

<span data-ttu-id="8731d-107">Os usuários podem definir as seguintes configurações para suas caixas de correio por meio de um cliente do Outlook:</span><span class="sxs-lookup"><span data-stu-id="8731d-107">Users can set the following settings for their mailboxes through an Outlook client:</span></span>

- <span data-ttu-id="8731d-108">[respostas automáticas](../resources/automaticrepliessetting.md) (notificar as pessoas automaticamente no recebimento de seus emails)</span><span class="sxs-lookup"><span data-stu-id="8731d-108">[automatic replies](../resources/automaticrepliessetting.md) (notify people automatically upon receipt of their email)</span></span>
- <span data-ttu-id="8731d-109">formato de data</span><span class="sxs-lookup"><span data-stu-id="8731d-109">date format</span></span>
- <span data-ttu-id="8731d-110">[localidade](../resources/localeinfo.md) (idioma e país/região)</span><span class="sxs-lookup"><span data-stu-id="8731d-110">[locale](../resources/localeinfo.md) (language and country/region)</span></span>
- <span data-ttu-id="8731d-111">formato de hora</span><span class="sxs-lookup"><span data-stu-id="8731d-111">time format</span></span>
- <span data-ttu-id="8731d-112">fuso horário</span><span class="sxs-lookup"><span data-stu-id="8731d-112">time zone</span></span>
- [<span data-ttu-id="8731d-113">horário comercial</span><span class="sxs-lookup"><span data-stu-id="8731d-113">working hours</span></span>](../resources/workinghours.md)

<span data-ttu-id="8731d-114">Os usuários podem definir os formatos de data e hora preferidos usando o Outlook na Web.</span><span class="sxs-lookup"><span data-stu-id="8731d-114">Users can set their preferred date and time formats using Outlook on the web.</span></span> <span data-ttu-id="8731d-115">Os usuários podem escolher um dos formatos de [Data](https://docs.microsoft.com/en-us/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortDate) e [hora](https://docs.microsoft.com/en-us/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortTime) abreviados com suporte.</span><span class="sxs-lookup"><span data-stu-id="8731d-115">Users can choose one of the supported [short date](https://docs.microsoft.com/en-us/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortDate) or [short time](https://docs.microsoft.com/en-us/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortTime) formats.</span></span> <span data-ttu-id="8731d-116">Essa `GET` operação retorna o formato escolhido pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="8731d-116">This `GET` operation returns the format the user has chosen.</span></span>

<span data-ttu-id="8731d-117">Os usuários podem definir o fuso horário que eles preferem em qualquer cliente do Outlook, escolhendo dos [fusos horários com suporte](outlookuser-supportedtimezones.md) que o administrador configurou para o servidor de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="8731d-117">Users can set the time zone they prefer on any Outlook client, by choosing from the [supported time zones](outlookuser-supportedtimezones.md) that their administrator has set up for their mailbox server.</span></span> <span data-ttu-id="8731d-118">O administrador pode configurar os fusos horários no formato de fuso horário do Windows ou da [autoridade de números da Internet (IANA)](https://www.iana.org/time-zones) (também conhecido como fuso horário do Olson).</span><span class="sxs-lookup"><span data-stu-id="8731d-118">The administrator can set up time zones in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="8731d-119">O formato do Windows é o padrão.</span><span class="sxs-lookup"><span data-stu-id="8731d-119">The Windows format is the default.</span></span> 

<span data-ttu-id="8731d-120">Essa `GET` operação retorna o fuso horário preferencial do usuário no formato que o administrador configurou.</span><span class="sxs-lookup"><span data-stu-id="8731d-120">This `GET` operation returns the user's preferred time zone in the format that the administrator has set up.</span></span> <span data-ttu-id="8731d-121">Se quiser que o fuso horário esteja em um formato específico (Windows ou IANA), você pode primeiro [atualizar o fuso horário de preferência nesse formato como uma configuração de caixa de correio](user-update-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="8731d-121">If you want that time zone to be in a specific format (Windows or IANA), you can first [update the preferred time zone in that format as a mailbox setting](user-update-mailboxsettings.md).</span></span> <span data-ttu-id="8731d-122">Posteriormente, você poderá obter o fuso horário nesse formato.</span><span class="sxs-lookup"><span data-stu-id="8731d-122">Subsequently you will be able to get the time zone in that format.</span></span> <span data-ttu-id="8731d-123">Como alternativa, você pode gerenciar a conversão de formato separadamente no seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8731d-123">Alternatively, you can manage the format conversion separately in your app.</span></span> 

## <a name="permissions"></a><span data-ttu-id="8731d-124">Permissões</span><span class="sxs-lookup"><span data-stu-id="8731d-124">Permissions</span></span>
<span data-ttu-id="8731d-p106">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8731d-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8731d-127">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8731d-127">Permission type</span></span>      | <span data-ttu-id="8731d-128">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8731d-128">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8731d-129">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8731d-129">Delegated (work or school account)</span></span> | <span data-ttu-id="8731d-130">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8731d-130">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="8731d-131">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8731d-131">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8731d-132">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8731d-132">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="8731d-133">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8731d-133">Application</span></span> | <span data-ttu-id="8731d-134">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8731d-134">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8731d-135">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8731d-135">HTTP request</span></span>
<span data-ttu-id="8731d-136">Para obter todas as configurações de caixa de correio de um usuário:</span><span class="sxs-lookup"><span data-stu-id="8731d-136">To get all the mailbox settings for a user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

<span data-ttu-id="8731d-137">Para obter configurações específicas – somente as configurações de respostas automáticas, localidade, fuso horário ou horário de trabalho:</span><span class="sxs-lookup"><span data-stu-id="8731d-137">To get specific settings - only the automatic replies settings, locale, time zone, or working hours:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings/automaticRepliesSetting
GET /users/{id|userPrincipalName}/mailboxSettings/automaticRepliesSetting

GET /me/mailboxSettings/dateFormat
GET /users/{id|userPrincipalName}/mailboxSettings/dateFormat

GET /me/mailboxSettings/language
GET /users/{id|userPrincipalName}/mailboxSettings/language

GET /me/mailboxSettings/timeFormat
GET /users/{id|userPrincipalName}/mailboxSettings/timeFormat

GET /me/mailboxSettings/timeZone
GET /users/{id|userPrincipalName}/mailboxSettings/timeZone

GET /me/mailboxSettings/workingHours
GET /users/{id|userPrincipalName}/mailboxSettings/workingHours
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8731d-138">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8731d-138">Optional query parameters</span></span>
<span data-ttu-id="8731d-139">Este método oferece suporte a alguns dos [parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8731d-139">This method supports some of the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8731d-140">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8731d-140">Request headers</span></span>
| <span data-ttu-id="8731d-141">Nome</span><span class="sxs-lookup"><span data-stu-id="8731d-141">Name</span></span>       | <span data-ttu-id="8731d-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="8731d-142">Type</span></span> | <span data-ttu-id="8731d-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="8731d-143">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8731d-144">Autorização</span><span class="sxs-lookup"><span data-stu-id="8731d-144">Authorization</span></span>  | <span data-ttu-id="8731d-145">string</span><span class="sxs-lookup"><span data-stu-id="8731d-145">string</span></span>  | <span data-ttu-id="8731d-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8731d-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8731d-148">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8731d-148">Request body</span></span>
<span data-ttu-id="8731d-149">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8731d-149">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8731d-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="8731d-150">Response</span></span>

<span data-ttu-id="8731d-151">Se for bem-sucedido, este método retornará um código de resposta `200 OK` e um dos seguintes objetos solicitados no corpo da resposta:</span><span class="sxs-lookup"><span data-stu-id="8731d-151">If successful, this method returns a `200 OK` response code and one of the following requested objects in the response body:</span></span>

- <span data-ttu-id="8731d-152">Objeto [mailboxSettings](../resources/mailboxsettings.md)</span><span class="sxs-lookup"><span data-stu-id="8731d-152">[mailboxSettings](../resources/mailboxsettings.md) object</span></span>
- <span data-ttu-id="8731d-153">Objeto [automaticRepliesSetting](../resources/automaticrepliessetting.md)</span><span class="sxs-lookup"><span data-stu-id="8731d-153">[automaticRepliesSetting](../resources/automaticrepliessetting.md) object</span></span>
- <span data-ttu-id="8731d-154">Cadeia de caracteres (para **DateFormat**)</span><span class="sxs-lookup"><span data-stu-id="8731d-154">string (for **dateFormat**)</span></span>
- <span data-ttu-id="8731d-155">Objeto [localeInfo](../resources/localeinfo.md)</span><span class="sxs-lookup"><span data-stu-id="8731d-155">[localeInfo](../resources/localeinfo.md) object</span></span>
- <span data-ttu-id="8731d-156">Cadeia de caracteres (para o **formato de TimeFormat**)</span><span class="sxs-lookup"><span data-stu-id="8731d-156">string (for **timeFormat**)</span></span>
- <span data-ttu-id="8731d-157">cadeia de caracteres (para **timeZone**)</span><span class="sxs-lookup"><span data-stu-id="8731d-157">string (for **timeZone**)</span></span>
- [<span data-ttu-id="8731d-158">workingHours</span><span class="sxs-lookup"><span data-stu-id="8731d-158">workingHours</span></span>](../resources/workinghours.md)

## <a name="examples"></a><span data-ttu-id="8731d-159">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8731d-159">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="8731d-160">Exemplo 1</span><span class="sxs-lookup"><span data-stu-id="8731d-160">Example 1</span></span>
#### <a name="request"></a><span data-ttu-id="8731d-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8731d-161">Request</span></span> 
<span data-ttu-id="8731d-162">O primeiro exemplo obtém todas as configurações de caixa de correio da caixa de correio do usuário conectado, que incluem configurações de respostas automáticas, formato de data, localidade (idioma e país/região), formato de hora, fuso horário e horário de trabalho.</span><span class="sxs-lookup"><span data-stu-id="8731d-162">The first example gets all the mailbox settings of the signed-in user's mailbox, which include settings for automatic replies, date format, locale (language and country/region), time format, time zone, and working hours.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8731d-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="8731d-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailboxSettings
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8731d-164">C#</span><span class="sxs-lookup"><span data-stu-id="8731d-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailboxsettings-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8731d-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8731d-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailboxsettings-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8731d-166">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8731d-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailboxsettings-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="8731d-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="8731d-167">Response</span></span>
<span data-ttu-id="8731d-168">A resposta inclui todas as configurações de caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="8731d-168">The response includes all the mailbox settings of the signed-in user.</span></span> <span data-ttu-id="8731d-169">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="8731d-169">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8731d-170">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8731d-170">All of the properties will be returned from an actual call.</span></span>
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
    },
    "dateFormat": "MM/dd/yyyy",
    "timeFormat": "hh:mm tt"
}
```

### <a name="example-2"></a><span data-ttu-id="8731d-171">Exemplo 2</span><span class="sxs-lookup"><span data-stu-id="8731d-171">Example 2</span></span>
#### <a name="request"></a><span data-ttu-id="8731d-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8731d-172">Request</span></span>
<span data-ttu-id="8731d-173">O segundo exemplo obtém especificamente as configurações de respostas automáticas da caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="8731d-173">The second example gets specifically the automatic replies settings of the signed-in user's mailbox.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8731d-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="8731d-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailboxSettings/automaticRepliesSetting
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8731d-175">C#</span><span class="sxs-lookup"><span data-stu-id="8731d-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailboxsettings-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8731d-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8731d-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailboxsettings-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8731d-177">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="8731d-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailboxsettings-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="8731d-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="8731d-178">Response</span></span>
<span data-ttu-id="8731d-p109">A resposta inclui apenas as configurações de respostas automáticas. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8731d-p109">The response includes only the automatic replies settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-3"></a><span data-ttu-id="8731d-182">Exemplo 3</span><span class="sxs-lookup"><span data-stu-id="8731d-182">Example 3</span></span>
#### <a name="request"></a><span data-ttu-id="8731d-183">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8731d-183">Request</span></span>
<span data-ttu-id="8731d-184">O terceiro exemplo obtém especificamente as configurações de horário de trabalho da caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="8731d-184">The third example gets specifically the working hour settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_mailboxsettings_3"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings/workingHours
```
#### <a name="response"></a><span data-ttu-id="8731d-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="8731d-185">Response</span></span>
<span data-ttu-id="8731d-186">A resposta inclui apenas as configurações de horário de trabalho.</span><span class="sxs-lookup"><span data-stu-id="8731d-186">The response includes only the working hours settings.</span></span> <span data-ttu-id="8731d-187">As horas de trabalho do usuário estão em um [fuso horário personalizado](../resources/customtimezone.md).</span><span class="sxs-lookup"><span data-stu-id="8731d-187">Notice that the user's work hours are in a [custom time zone](../resources/customtimezone.md).</span></span> <span data-ttu-id="8731d-188">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="8731d-188">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8731d-189">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8731d-189">All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
