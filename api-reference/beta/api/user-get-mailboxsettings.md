---
title: Obter as configurações da caixa de correio do usuário
description: 'Obtenha as configurações de caixa de correio do usuário. Isso inclui configurações para respostas automáticas (notificar pessoas automaticamente quando '
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c9b33037b9dc43f1296fea398e1354d42e43eb09
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458630"
---
# <a name="get-user-mailbox-settings"></a><span data-ttu-id="59e4d-104">Obter as configurações da caixa de correio do usuário</span><span class="sxs-lookup"><span data-stu-id="59e4d-104">Get user mailbox settings</span></span>

<span data-ttu-id="59e4d-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59e4d-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59e4d-106">Obtenha as [mailboxSettings](../resources/mailboxsettings.md) do usuário.</span><span class="sxs-lookup"><span data-stu-id="59e4d-106">Get the user's [mailboxSettings](../resources/mailboxsettings.md).</span></span> <span data-ttu-id="59e4d-107">Você pode exibir todas as configurações de caixa de correio ou obter configurações específicas.</span><span class="sxs-lookup"><span data-stu-id="59e4d-107">You can view all mailbox settings, or get specific settings.</span></span>

<span data-ttu-id="59e4d-108">Os usuários podem definir as configurações a seguir para suas caixas de correio por meio de um cliente do Outlook:</span><span class="sxs-lookup"><span data-stu-id="59e4d-108">Users can set the following settings for their mailboxes through an Outlook client:</span></span>

- <span data-ttu-id="59e4d-109">[respostas automáticas](../resources/automaticrepliessetting.md) (notificar pessoas automaticamente ao receber seus emails)</span><span class="sxs-lookup"><span data-stu-id="59e4d-109">[automatic replies](../resources/automaticrepliessetting.md) (notify people automatically upon receipt of their email)</span></span>
- <span data-ttu-id="59e4d-110">formato de data</span><span class="sxs-lookup"><span data-stu-id="59e4d-110">date format</span></span>
- <span data-ttu-id="59e4d-111">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="59e4d-111">delegateMeetingMessageDeliveryOptions</span></span>
- <span data-ttu-id="59e4d-112">[localidade](../resources/localeinfo.md) (idioma e país/região)</span><span class="sxs-lookup"><span data-stu-id="59e4d-112">[locale](../resources/localeinfo.md) (language and country/region)</span></span>
- <span data-ttu-id="59e4d-113">formato de hora</span><span class="sxs-lookup"><span data-stu-id="59e4d-113">time format</span></span>
- <span data-ttu-id="59e4d-114">fuso horário</span><span class="sxs-lookup"><span data-stu-id="59e4d-114">time zone</span></span>
- [<span data-ttu-id="59e4d-115">horário de trabalho</span><span class="sxs-lookup"><span data-stu-id="59e4d-115">working hours</span></span>](../resources/workinghours.md)
- [<span data-ttu-id="59e4d-116">finalidade do usuário</span><span class="sxs-lookup"><span data-stu-id="59e4d-116">user purpose</span></span>](../resources/userpurpose.md)

<span data-ttu-id="59e4d-117">Os usuários podem definir os formatos de data e hora preferidos usando o Outlook na Web.</span><span class="sxs-lookup"><span data-stu-id="59e4d-117">Users can set their preferred date and time formats using Outlook on the web.</span></span> <span data-ttu-id="59e4d-118">Os usuários podem escolher um dos formatos de [data abreviada](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortDate) ou de [tempo abreviado](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortTime) com suporte.</span><span class="sxs-lookup"><span data-stu-id="59e4d-118">Users can choose one of the supported [short date](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortDate) or [short time](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortTime) formats.</span></span> <span data-ttu-id="59e4d-119">Essa operação `GET` retorna o formato escolhido pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="59e4d-119">This `GET` operation returns the format the user has chosen.</span></span>

<span data-ttu-id="59e4d-120">Os usuários podem definir o fuso horário preferido em qualquer cliente do Outlook, escolhendo entre os [fusos horários com suporte](outlookuser-supportedtimezones.md) que o administrador configurou para o servidor da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="59e4d-120">Users can set the time zone they prefer on any Outlook client, by choosing from the [supported time zones](outlookuser-supportedtimezones.md) that their administrator has set up for their mailbox server.</span></span> <span data-ttu-id="59e4d-121">O administrador pode configurar os fusos horários no formato de fuso horário do Windows ou no formato de [fuso horário de Autoridade para Atribuição de Números na Internet (IANA)](https://www.iana.org/time-zones) (também conhecido como fuso horário de Olson).</span><span class="sxs-lookup"><span data-stu-id="59e4d-121">The administrator can set up time zones in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="59e4d-122">O formato do Windows é o padrão.</span><span class="sxs-lookup"><span data-stu-id="59e4d-122">The Windows format is the default.</span></span> 

<span data-ttu-id="59e4d-123">Essa operação `GET` retorna o fuso horário preferido do usuário no formato configurado pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="59e4d-123">This `GET` operation returns the user's preferred time zone in the format that the administrator has set up.</span></span> <span data-ttu-id="59e4d-124">Se quiser que o fuso horário esteja em um formato específico (Windows ou IANA), você pode primeiro [atualizar o fuso horário de preferência nesse formato como uma configuração de caixa de correio](user-update-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="59e4d-124">If you want that time zone to be in a specific format (Windows or IANA), you can first [update the preferred time zone in that format as a mailbox setting](user-update-mailboxsettings.md).</span></span> <span data-ttu-id="59e4d-125">Posteriormente, você poderá obter o fuso horário nesse formato.</span><span class="sxs-lookup"><span data-stu-id="59e4d-125">Subsequently you will be able to get the time zone in that format.</span></span> <span data-ttu-id="59e4d-126">Como alternativa, você pode gerenciar a conversão de formato separadamente no seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="59e4d-126">Alternatively, you can manage the format conversion separately in your app.</span></span> 

## <a name="permissions"></a><span data-ttu-id="59e4d-127">Permissões</span><span class="sxs-lookup"><span data-stu-id="59e4d-127">Permissions</span></span>
<span data-ttu-id="59e4d-p106">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="59e4d-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59e4d-130">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="59e4d-130">Permission type</span></span>      | <span data-ttu-id="59e4d-131">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="59e4d-131">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59e4d-132">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="59e4d-132">Delegated (work or school account)</span></span> | <span data-ttu-id="59e4d-133">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59e4d-133">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="59e4d-134">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="59e4d-134">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59e4d-135">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59e4d-135">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="59e4d-136">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="59e4d-136">Application</span></span> | <span data-ttu-id="59e4d-137">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="59e4d-137">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="59e4d-138">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="59e4d-138">HTTP request</span></span>
<span data-ttu-id="59e4d-139">Para obter todas as configurações de caixa de correio de um usuário:</span><span class="sxs-lookup"><span data-stu-id="59e4d-139">To get all the mailbox settings for a user:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

<span data-ttu-id="59e4d-140">Para obter configurações específicas, somente as configurações de respostas automáticas, o formato de data, a localidade, o formato de hora, o fuso horário, o horário de trabalho ou a finalidade do usuário:</span><span class="sxs-lookup"><span data-stu-id="59e4d-140">To get specific settings - only the automatic replies settings, date format, locale, time format, time zone, working hours, or user purpose:</span></span>
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

GET /me/mailboxSettings/userPurpose
GET /users/{id|userPrincipalName}/mailboxSettings/userPurpose
```
## <a name="optional-query-parameters"></a><span data-ttu-id="59e4d-141">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="59e4d-141">Optional query parameters</span></span>
<span data-ttu-id="59e4d-142">Este método também dá suporte a alguns [Parâmetros de Consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="59e4d-142">This method supports some of the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="59e4d-143">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="59e4d-143">Request headers</span></span>
| <span data-ttu-id="59e4d-144">Nome</span><span class="sxs-lookup"><span data-stu-id="59e4d-144">Name</span></span>       | <span data-ttu-id="59e4d-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="59e4d-145">Type</span></span> | <span data-ttu-id="59e4d-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="59e4d-146">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="59e4d-147">Autorização</span><span class="sxs-lookup"><span data-stu-id="59e4d-147">Authorization</span></span>  | <span data-ttu-id="59e4d-148">string</span><span class="sxs-lookup"><span data-stu-id="59e4d-148">string</span></span>  | <span data-ttu-id="59e4d-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="59e4d-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="59e4d-151">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="59e4d-151">Request body</span></span>
<span data-ttu-id="59e4d-152">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="59e4d-152">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59e4d-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="59e4d-153">Response</span></span>

<span data-ttu-id="59e4d-154">Se for bem-sucedido, este método retornará um código de resposta `200 OK` e um dos seguintes objetos solicitados no corpo da resposta:</span><span class="sxs-lookup"><span data-stu-id="59e4d-154">If successful, this method returns a `200 OK` response code and one of the following requested objects in the response body:</span></span>

- <span data-ttu-id="59e4d-155">Objeto [mailboxSettings](../resources/mailboxsettings.md)</span><span class="sxs-lookup"><span data-stu-id="59e4d-155">[mailboxSettings](../resources/mailboxsettings.md) object</span></span>
- <span data-ttu-id="59e4d-156">Objeto [automaticRepliesSetting](../resources/automaticrepliessetting.md)</span><span class="sxs-lookup"><span data-stu-id="59e4d-156">[automaticRepliesSetting](../resources/automaticrepliessetting.md) object</span></span>
- <span data-ttu-id="59e4d-157">cadeia de caracteres (para **dateFormat**)</span><span class="sxs-lookup"><span data-stu-id="59e4d-157">string (for **dateFormat**)</span></span>
- <span data-ttu-id="59e4d-158">Cadeia de caracteres (para **delegateMeetingMessageDeliveryOptions**)</span><span class="sxs-lookup"><span data-stu-id="59e4d-158">string (for **delegateMeetingMessageDeliveryOptions**)</span></span>
- <span data-ttu-id="59e4d-159">Objeto [localeInfo](../resources/localeinfo.md)</span><span class="sxs-lookup"><span data-stu-id="59e4d-159">[localeInfo](../resources/localeinfo.md) object</span></span>
- <span data-ttu-id="59e4d-160">cadeia de caracteres (para **timeFormat**)</span><span class="sxs-lookup"><span data-stu-id="59e4d-160">string (for **timeFormat**)</span></span>
- <span data-ttu-id="59e4d-161">cadeia de caracteres (para **timeZone**)</span><span class="sxs-lookup"><span data-stu-id="59e4d-161">string (for **timeZone**)</span></span>
- [<span data-ttu-id="59e4d-162">workingHours</span><span class="sxs-lookup"><span data-stu-id="59e4d-162">workingHours</span></span>](../resources/workinghours.md)
- [<span data-ttu-id="59e4d-163">userpurpose</span><span class="sxs-lookup"><span data-stu-id="59e4d-163">userPurpose</span></span>](../resources/userpurpose.md)

## <a name="examples"></a><span data-ttu-id="59e4d-164">Exemplos</span><span class="sxs-lookup"><span data-stu-id="59e4d-164">Examples</span></span>

### <a name="example-1"></a><span data-ttu-id="59e4d-165">Exemplo 1</span><span class="sxs-lookup"><span data-stu-id="59e4d-165">Example 1</span></span>
#### <a name="request"></a><span data-ttu-id="59e4d-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59e4d-166">Request</span></span> 
<span data-ttu-id="59e4d-167">O primeiro exemplo obtém todas as configurações de caixa de correio da caixa de correio do usuário conectado, que incluem configurações de respostas automáticas, formato de data, localidade (idioma e país/região), formato de hora, fuso horário, horas de trabalho e finalidade do usuário.</span><span class="sxs-lookup"><span data-stu-id="59e4d-167">The first example gets all the mailbox settings of the signed-in user's mailbox, which include settings for automatic replies, date format, locale (language and country/region), time format, time zone, working hours, and user purpose.</span></span>

# <a name="http"></a>[<span data-ttu-id="59e4d-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="59e4d-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailboxSettings
```
# <a name="c"></a>[<span data-ttu-id="59e4d-169">C#</span><span class="sxs-lookup"><span data-stu-id="59e4d-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailboxsettings-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="59e4d-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59e4d-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailboxsettings-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="59e4d-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="59e4d-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailboxsettings-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="59e4d-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="59e4d-172">Response</span></span>
<span data-ttu-id="59e4d-173">A resposta inclui todas as configurações da caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="59e4d-173">The response includes all the mailbox settings of the signed-in user.</span></span> <span data-ttu-id="59e4d-174">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="59e4d-174">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="59e4d-175">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="59e4d-175">All of the properties will be returned from an actual call.</span></span>
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
    "userPurpose": {
        "value": "user"
    },
    "dateFormat": "MM/dd/yyyy",
    "timeFormat": "hh:mm tt",
    "delegateMeetingMessageDeliveryOptions": "sendToDelegateOnly"
}
```

### <a name="example-2"></a><span data-ttu-id="59e4d-176">Exemplo 2</span><span class="sxs-lookup"><span data-stu-id="59e4d-176">Example 2</span></span>
#### <a name="request"></a><span data-ttu-id="59e4d-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59e4d-177">Request</span></span>
<span data-ttu-id="59e4d-178">O segundo exemplo obtém especificamente as configurações de respostas automáticas da caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="59e4d-178">The second example gets specifically the automatic replies settings of the signed-in user's mailbox.</span></span>

# <a name="http"></a>[<span data-ttu-id="59e4d-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="59e4d-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailboxSettings/automaticRepliesSetting
```
# <a name="c"></a>[<span data-ttu-id="59e4d-180">C#</span><span class="sxs-lookup"><span data-stu-id="59e4d-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailboxsettings-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="59e4d-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59e4d-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailboxsettings-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="59e4d-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="59e4d-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailboxsettings-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="59e4d-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="59e4d-183">Response</span></span>
<span data-ttu-id="59e4d-p109">A resposta inclui apenas as configurações de respostas automáticas. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="59e4d-p109">The response includes only the automatic replies settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-3"></a><span data-ttu-id="59e4d-187">Exemplo 3</span><span class="sxs-lookup"><span data-stu-id="59e4d-187">Example 3</span></span>
#### <a name="request"></a><span data-ttu-id="59e4d-188">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59e4d-188">Request</span></span>
<span data-ttu-id="59e4d-189">O terceiro exemplo obtém especificamente as configurações de horário de trabalho da caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="59e4d-189">The third example gets specifically the working hour settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_mailboxsettings_3"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings/workingHours
```
#### <a name="response"></a><span data-ttu-id="59e4d-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="59e4d-190">Response</span></span>
<span data-ttu-id="59e4d-191">A resposta inclui apenas as configurações de horário de trabalho.</span><span class="sxs-lookup"><span data-stu-id="59e4d-191">The response includes only the working hours settings.</span></span> <span data-ttu-id="59e4d-192">As horas de trabalho do usuário estão em um [fuso horário personalizado](../resources/customtimezone.md).</span><span class="sxs-lookup"><span data-stu-id="59e4d-192">Notice that the user's work hours are in a [custom time zone](../resources/customtimezone.md).</span></span> <span data-ttu-id="59e4d-193">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="59e4d-193">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="59e4d-194">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="59e4d-194">All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-4"></a><span data-ttu-id="59e4d-195">Exemplo 4</span><span class="sxs-lookup"><span data-stu-id="59e4d-195">Example 4</span></span>
#### <a name="request"></a><span data-ttu-id="59e4d-196">Solicitação</span><span class="sxs-lookup"><span data-stu-id="59e4d-196">Request</span></span>
<span data-ttu-id="59e4d-197">O quarto exemplo obtém especificamente as configurações de [finalidade do usuário](../resources/userpurpose.md) da caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="59e4d-197">The fourth example gets specifically the [user purpose](../resources/userpurpose.md) settings of the signed-in user's mailbox.</span></span>

# <a name="http"></a>[<span data-ttu-id="59e4d-198">HTTP</span><span class="sxs-lookup"><span data-stu-id="59e4d-198">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_4"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailboxSettings/userPurpose
```
# <a name="c"></a>[<span data-ttu-id="59e4d-199">C#</span><span class="sxs-lookup"><span data-stu-id="59e4d-199">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailboxsettings-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="59e4d-200">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59e4d-200">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailboxsettings-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="59e4d-201">Objective-C</span><span class="sxs-lookup"><span data-stu-id="59e4d-201">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailboxsettings-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="59e4d-202">Resposta</span><span class="sxs-lookup"><span data-stu-id="59e4d-202">Response</span></span>
<span data-ttu-id="59e4d-203">A resposta inclui apenas as configurações de [finalidade do usuário](../resources/userpurpose.md) .</span><span class="sxs-lookup"><span data-stu-id="59e4d-203">The response includes only the [user purpose](../resources/userpurpose.md) settings.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_mailboxsettings_4",
  "truncated": true,
  "@odata.type": "microsoft.graph.userPurpose"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('622eaaff-0683-4862-9de4-f2ec83c2bd98')/mailboxSettings/userPurpose",
    "value": "user"
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
