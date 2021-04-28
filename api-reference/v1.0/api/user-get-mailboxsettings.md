---
title: Obter as configurações da caixa de correio do usuário
description: 'Obtenha as configurações de caixa de correio do usuário. Isso inclui configurações para respostas automáticas (notificar pessoas automaticamente quando '
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e2f697a332eb4912f0f4f442f57ccf79b86d03ca
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054305"
---
# <a name="get-user-mailbox-settings"></a><span data-ttu-id="8327c-104">Obter as configurações da caixa de correio do usuário</span><span class="sxs-lookup"><span data-stu-id="8327c-104">Get user mailbox settings</span></span>

<span data-ttu-id="8327c-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8327c-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8327c-106">Obtenha as [mailboxSettings](../resources/mailboxsettings.md) do usuário.</span><span class="sxs-lookup"><span data-stu-id="8327c-106">Get the user's [mailboxSettings](../resources/mailboxsettings.md).</span></span> <span data-ttu-id="8327c-107">Você pode exibir todas as configurações de caixa de correio ou obter configurações específicas.</span><span class="sxs-lookup"><span data-stu-id="8327c-107">You can view all mailbox settings, or get specific settings.</span></span>

<span data-ttu-id="8327c-108">Os usuários podem definir as configurações a seguir para suas caixas de correio por meio de um cliente do Outlook:</span><span class="sxs-lookup"><span data-stu-id="8327c-108">Users can set the following settings for their mailboxes through an Outlook client:</span></span>

- <span data-ttu-id="8327c-109">[respostas automáticas](../resources/automaticrepliessetting.md) (notificar pessoas automaticamente ao receber seus emails)</span><span class="sxs-lookup"><span data-stu-id="8327c-109">[automatic replies](../resources/automaticrepliessetting.md) (notify people automatically upon receipt of their email)</span></span>
- <span data-ttu-id="8327c-110">formato de data</span><span class="sxs-lookup"><span data-stu-id="8327c-110">date format</span></span>
- <span data-ttu-id="8327c-111">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="8327c-111">delegateMeetingMessageDeliveryOptions</span></span>
- <span data-ttu-id="8327c-112">[localidade](../resources/localeinfo.md) (idioma e país/região)</span><span class="sxs-lookup"><span data-stu-id="8327c-112">[locale](../resources/localeinfo.md) (language and country/region)</span></span>
- <span data-ttu-id="8327c-113">formato de hora</span><span class="sxs-lookup"><span data-stu-id="8327c-113">time format</span></span>
- <span data-ttu-id="8327c-114">fuso horário</span><span class="sxs-lookup"><span data-stu-id="8327c-114">time zone</span></span>
- [<span data-ttu-id="8327c-115">horário de trabalho</span><span class="sxs-lookup"><span data-stu-id="8327c-115">working hours</span></span>](../resources/workinghours.md)

<span data-ttu-id="8327c-116">Os usuários podem definir os formatos de data e hora preferidos usando o Outlook na Web.</span><span class="sxs-lookup"><span data-stu-id="8327c-116">Users can set their preferred date and time formats using Outlook on the web.</span></span> <span data-ttu-id="8327c-117">Os usuários podem escolher um dos formatos de [data abreviada](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortDate) ou de [tempo abreviado](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortTime) com suporte.</span><span class="sxs-lookup"><span data-stu-id="8327c-117">Users can choose one of the supported [short date](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortDate) or [short time](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortTime) formats.</span></span> <span data-ttu-id="8327c-118">Essa operação `GET` retorna o formato escolhido pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="8327c-118">This `GET` operation returns the format the user has chosen.</span></span>

<span data-ttu-id="8327c-119">Os usuários podem definir o fuso horário preferido em qualquer cliente do Outlook, escolhendo entre os [fusos horários com suporte](outlookuser-supportedtimezones.md) que o administrador configurou para o servidor da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="8327c-119">Users can set the time zone they prefer on any Outlook client, by choosing from the [supported time zones](outlookuser-supportedtimezones.md) that their administrator has set up for their mailbox server.</span></span> <span data-ttu-id="8327c-120">O administrador pode configurar os fusos horários no formato de fuso horário do Windows ou no formato de [fuso horário de Autoridade para Atribuição de Números na Internet (IANA)](https://www.iana.org/time-zones) (também conhecido como fuso horário de Olson).</span><span class="sxs-lookup"><span data-stu-id="8327c-120">The administrator can set up time zones in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="8327c-121">O formato do Windows é o padrão.</span><span class="sxs-lookup"><span data-stu-id="8327c-121">The Windows format is the default.</span></span>

<span data-ttu-id="8327c-122">Essa operação `GET` retorna o fuso horário preferido do usuário no formato configurado pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="8327c-122">This `GET` operation returns the user's preferred time zone in the format that the administrator has set up.</span></span> <span data-ttu-id="8327c-123">Se quiser que o fuso horário esteja em um formato específico (Windows ou IANA), você pode primeiro [atualizar o fuso horário de preferência nesse formato como uma configuração de caixa de correio](user-update-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="8327c-123">If you want that time zone to be in a specific format (Windows or IANA), you can first [update the preferred time zone in that format as a mailbox setting](user-update-mailboxsettings.md).</span></span> <span data-ttu-id="8327c-124">Posteriormente, você poderá obter o fuso horário nesse formato.</span><span class="sxs-lookup"><span data-stu-id="8327c-124">Subsequently you will be able to get the time zone in that format.</span></span> <span data-ttu-id="8327c-125">Como alternativa, você pode gerenciar a conversão de formato separadamente no seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8327c-125">Alternatively, you can manage the format conversion separately in your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="8327c-126">Permissões</span><span class="sxs-lookup"><span data-stu-id="8327c-126">Permissions</span></span>
<span data-ttu-id="8327c-p106">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8327c-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8327c-129">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8327c-129">Permission type</span></span>      | <span data-ttu-id="8327c-130">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8327c-130">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8327c-131">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8327c-131">Delegated (work or school account)</span></span> | <span data-ttu-id="8327c-132">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8327c-132">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="8327c-133">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8327c-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8327c-134">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8327c-134">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="8327c-135">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8327c-135">Application</span></span> | <span data-ttu-id="8327c-136">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8327c-136">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8327c-137">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8327c-137">HTTP request</span></span>
<span data-ttu-id="8327c-138">Para obter todas as configurações de caixa de correio de um usuário:</span><span class="sxs-lookup"><span data-stu-id="8327c-138">To get all the mailbox settings for a user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

<span data-ttu-id="8327c-139">Para obter configurações específicas, somente as configurações de respostas automáticas, formato de data, localidade, formato de hora, fuso horário ou horário de trabalho:</span><span class="sxs-lookup"><span data-stu-id="8327c-139">To get specific settings - only the automatic replies settings, date format, locale, time format, time zone, or working hours:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings/automaticRepliesSetting
GET /users/{id|userPrincipalName}/mailboxSettings/automaticRepliesSetting

GET /me/mailboxSettings/dateFormat
GET /users/{id|userPrincipalName}/mailboxSettings/dateFormat

GET /me/mailboxSettings/delegateMeetingMessageDeliveryOptions
GET /users/{id|userPrincipalName}/mailboxSettings/delegateMeetingMessageDeliveryOptions

GET /me/mailboxSettings/language
GET /users/{id|userPrincipalName}/mailboxSettings/language

GET /me/mailboxSettings/timeFormat
GET /users/{id|userPrincipalName}/mailboxSettings/timeFormat

GET /me/mailboxSettings/timeZone
GET /users/{id|userPrincipalName}/mailboxSettings/timeZone

GET /me/mailboxSettings/workingHours
GET /users/{id|userPrincipalName}/mailboxSettings/workingHours
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8327c-140">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8327c-140">Optional query parameters</span></span>
<span data-ttu-id="8327c-141">Este método também dá suporte a alguns [Parâmetros de Consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8327c-141">This method supports some of the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8327c-142">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8327c-142">Request headers</span></span>
| <span data-ttu-id="8327c-143">Nome</span><span class="sxs-lookup"><span data-stu-id="8327c-143">Name</span></span>       | <span data-ttu-id="8327c-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="8327c-144">Type</span></span> | <span data-ttu-id="8327c-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="8327c-145">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8327c-146">Autorização</span><span class="sxs-lookup"><span data-stu-id="8327c-146">Authorization</span></span>  | <span data-ttu-id="8327c-147">string</span><span class="sxs-lookup"><span data-stu-id="8327c-147">string</span></span>  | <span data-ttu-id="8327c-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8327c-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8327c-150">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8327c-150">Request body</span></span>
<span data-ttu-id="8327c-151">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8327c-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8327c-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="8327c-152">Response</span></span>

<span data-ttu-id="8327c-153">Se for bem-sucedido, este método retornará um código de resposta `200 OK` e um dos seguintes objetos solicitados no corpo da resposta:</span><span class="sxs-lookup"><span data-stu-id="8327c-153">If successful, this method returns a `200 OK` response code and one of the following requested objects in the response body:</span></span>

- <span data-ttu-id="8327c-154">Objeto [mailboxSettings](../resources/mailboxsettings.md)</span><span class="sxs-lookup"><span data-stu-id="8327c-154">[mailboxSettings](../resources/mailboxsettings.md) object</span></span>
- <span data-ttu-id="8327c-155">Objeto [automaticRepliesSetting](../resources/automaticrepliessetting.md)</span><span class="sxs-lookup"><span data-stu-id="8327c-155">[automaticRepliesSetting](../resources/automaticrepliessetting.md) object</span></span>
- <span data-ttu-id="8327c-156">cadeia de caracteres (para **dateFormat**)</span><span class="sxs-lookup"><span data-stu-id="8327c-156">string (for **dateFormat**)</span></span>
- <span data-ttu-id="8327c-157">string (para **delegateMeetingMessageDeliveryOptions**)</span><span class="sxs-lookup"><span data-stu-id="8327c-157">string (for **delegateMeetingMessageDeliveryOptions**)</span></span>
- <span data-ttu-id="8327c-158">Objeto [localeInfo](../resources/localeinfo.md)</span><span class="sxs-lookup"><span data-stu-id="8327c-158">[localeInfo](../resources/localeinfo.md) object</span></span>
- <span data-ttu-id="8327c-159">cadeia de caracteres (para **timeFormat**)</span><span class="sxs-lookup"><span data-stu-id="8327c-159">string (for **timeFormat**)</span></span>
- <span data-ttu-id="8327c-160">cadeia de caracteres (para **timeZone**)</span><span class="sxs-lookup"><span data-stu-id="8327c-160">string (for **timeZone**)</span></span>
- [<span data-ttu-id="8327c-161">workingHours</span><span class="sxs-lookup"><span data-stu-id="8327c-161">workingHours</span></span>](../resources/workinghours.md)

## <a name="examples"></a><span data-ttu-id="8327c-162">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8327c-162">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="8327c-163">Exemplo 1</span><span class="sxs-lookup"><span data-stu-id="8327c-163">Example 1</span></span>
#### <a name="request"></a><span data-ttu-id="8327c-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8327c-164">Request</span></span>
<span data-ttu-id="8327c-165">O primeiro exemplo obtém todas as configurações da caixa de correio do usuário conectado, que incluem configurações de respostas automáticas, formato de data, localidade (idioma e país/região), formato de hora, fuso horário e horário de trabalho.</span><span class="sxs-lookup"><span data-stu-id="8327c-165">The first example gets all the mailbox settings of the signed-in user's mailbox, which include settings for automatic replies, date format, locale (language and country/region), time format, time zone, and working hours.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailboxSettings
```

#### <a name="response"></a><span data-ttu-id="8327c-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="8327c-166">Response</span></span>
<span data-ttu-id="8327c-167">A resposta inclui todas as configurações da caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="8327c-167">The response includes all the mailbox settings of the signed-in user.</span></span>
<span data-ttu-id="8327c-168">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8327c-168">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/mailboxSettings",
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
        "startTime": "08:00:00.0000000",
        "endTime": "17:00:00.0000000",
        "timeZone":{
            "name":"Pacific Standard Time"
        }
    },
    "dateFormat": "MM/dd/yyyy",
    "timeFormat": "hh:mm tt",
    "delegateMeetingMessageDeliveryOptions": "sendToDelegateOnly"
}
```

### <a name="example-2"></a><span data-ttu-id="8327c-169">Exemplo 2</span><span class="sxs-lookup"><span data-stu-id="8327c-169">Example 2</span></span>
#### <a name="request"></a><span data-ttu-id="8327c-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8327c-170">Request</span></span>
<span data-ttu-id="8327c-171">O segundo exemplo obtém especificamente as configurações de respostas automáticas da caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="8327c-171">The second example gets specifically the automatic replies settings of the signed-in user's mailbox.</span></span>

# <a name="http"></a>[<span data-ttu-id="8327c-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="8327c-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailboxSettings/automaticRepliesSetting
```
# <a name="c"></a>[<span data-ttu-id="8327c-173">C#</span><span class="sxs-lookup"><span data-stu-id="8327c-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailboxsettings-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8327c-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8327c-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailboxsettings-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8327c-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8327c-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailboxsettings-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8327c-176">Java</span><span class="sxs-lookup"><span data-stu-id="8327c-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailboxsettings-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="8327c-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="8327c-177">Response</span></span>
<span data-ttu-id="8327c-178">A resposta inclui apenas as configurações de respostas automáticas.</span><span class="sxs-lookup"><span data-stu-id="8327c-178">The response includes only the automatic replies settings.</span></span>
<span data-ttu-id="8327c-179">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8327c-179">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/mailboxSettings/automaticRepliesSetting",
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

### <a name="example-3"></a><span data-ttu-id="8327c-180">Exemplo 3</span><span class="sxs-lookup"><span data-stu-id="8327c-180">Example 3</span></span>
#### <a name="request"></a><span data-ttu-id="8327c-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8327c-181">Request</span></span>
<span data-ttu-id="8327c-182">O terceiro exemplo obtém especificamente as configurações de horário de trabalho da caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="8327c-182">The third example gets specifically the working hour settings of the signed-in user's mailbox.</span></span>

# <a name="http"></a>[<span data-ttu-id="8327c-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="8327c-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/mailboxSettings/workingHours
```
# <a name="c"></a>[<span data-ttu-id="8327c-184">C#</span><span class="sxs-lookup"><span data-stu-id="8327c-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailboxsettings-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8327c-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8327c-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailboxsettings-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8327c-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8327c-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailboxsettings-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8327c-187">Java</span><span class="sxs-lookup"><span data-stu-id="8327c-187">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mailboxsettings-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="8327c-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="8327c-188">Response</span></span>
<span data-ttu-id="8327c-189">A resposta inclui apenas as configurações de horário de trabalho.</span><span class="sxs-lookup"><span data-stu-id="8327c-189">The response includes only the working hours settings.</span></span> <span data-ttu-id="8327c-190">As horas de trabalho do usuário estão em um [fuso horário personalizado](../resources/customtimezone.md).</span><span class="sxs-lookup"><span data-stu-id="8327c-190">Notice that the user's work hours are in a [custom time zone](../resources/customtimezone.md).</span></span>
<span data-ttu-id="8327c-191">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8327c-191">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_mailboxsettings_3",
  "truncated": true,
  "@odata.type": "microsoft.graph.workingHours"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('94447c6e-ea4c-494c-a9ed-d905e366c5cb')/mailboxSettings/workingHours",
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
<!-- {
  "type": "#page.annotation",
  "description": "Get mailbox settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
