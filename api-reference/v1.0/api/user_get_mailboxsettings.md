# <a name="get-user-mailbox-settings"></a><span data-ttu-id="e9639-101">Obter as configurações da caixa de correio do usuário</span><span class="sxs-lookup"><span data-stu-id="e9639-101">Get user mailbox settings</span></span>

<span data-ttu-id="e9639-p101">Obtenha as [mailboxSettings](../resources/mailboxsettings.md) do usuário. Isso inclui configurações para respostas automáticas (notificar as pessoas automaticamente ao receber seus emails), localidade (país/região e idioma) e fuso horário.</span><span class="sxs-lookup"><span data-stu-id="e9639-p101">Get the user's [mailboxSettings](../resources/mailboxsettings.md). This includes settings for automatic replies (notify people automatically upon receipt of their email), locale (language and country/region), and time zone.</span></span>

<span data-ttu-id="e9639-104">Você pode exibir todas as configurações de caixa de correio ou obter configurações específicas.</span><span class="sxs-lookup"><span data-stu-id="e9639-104">You can view all mailbox settings, or, get specific settings.</span></span>

## <a name="permissions"></a><span data-ttu-id="e9639-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e9639-105">Permissions</span></span>
<span data-ttu-id="e9639-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e9639-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e9639-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e9639-108">Permission type</span></span>      | <span data-ttu-id="e9639-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e9639-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9639-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e9639-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e9639-111">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9639-111">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="e9639-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e9639-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9639-113">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9639-113">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="e9639-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e9639-114">Application</span></span> | <span data-ttu-id="e9639-115">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e9639-115">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9639-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e9639-116">HTTP request</span></span>
<span data-ttu-id="e9639-117">Para acessar todas as configurações de email que incluem configurações de respostas automáticas:</span><span class="sxs-lookup"><span data-stu-id="e9639-117">To get all mailbox settings which include automatic replies settings:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

<span data-ttu-id="e9639-118">Para obter configurações específicas, por exemplo, somente as configurações de respostas automáticas, localidade ou fuso horário:</span><span class="sxs-lookup"><span data-stu-id="e9639-118">To get specific settings - for example, only the automatic replies settings, locale, or time zone:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings/automaticRepliesSetting
GET /users/{id|userPrincipalName}/mailboxSettings/automaticRepliesSetting

GET /me/mailboxSettings/language
GET /users/{id|userPrincipalName}/mailboxSettings/language

GET /me/mailboxSettings/timeZone
GET /users/{id|userPrincipalName}/mailboxSettings/timeZone
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e9639-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e9639-119">Optional query parameters</span></span>
<span data-ttu-id="e9639-120">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e9639-120">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e9639-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e9639-121">Request headers</span></span>
| <span data-ttu-id="e9639-122">Nome</span><span class="sxs-lookup"><span data-stu-id="e9639-122">Name</span></span>       | <span data-ttu-id="e9639-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="e9639-123">Type</span></span> | <span data-ttu-id="e9639-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9639-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e9639-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e9639-125">Authorization</span></span>  | <span data-ttu-id="e9639-126">string</span><span class="sxs-lookup"><span data-stu-id="e9639-126">string</span></span>  | <span data-ttu-id="e9639-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e9639-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e9639-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e9639-129">Request body</span></span>
<span data-ttu-id="e9639-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e9639-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e9639-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e9639-131">Response</span></span>

<span data-ttu-id="e9639-132">Se for bem-sucedido, este método retornará um código de resposta `200 OK` e um dos seguintes objetos solicitados no corpo da resposta:</span><span class="sxs-lookup"><span data-stu-id="e9639-132">If successful, this method returns a `200 OK` response code and one of the following requested objects in the response body:</span></span>

- <span data-ttu-id="e9639-133">Objeto [mailboxSettings](../resources/mailboxsettings.md)</span><span class="sxs-lookup"><span data-stu-id="e9639-133">[mailboxSettings](../resources/mailboxsettings.md) object</span></span>
- <span data-ttu-id="e9639-134">Objeto [automaticRepliesSetting](../resources/automaticRepliesSetting.md)</span><span class="sxs-lookup"><span data-stu-id="e9639-134">[automaticRepliesSetting](../resources/automaticRepliesSetting.md) object</span></span>
- <span data-ttu-id="e9639-135">Objeto [localeInfo](../resources/localeinfo.md)</span><span class="sxs-lookup"><span data-stu-id="e9639-135">[localeInfo](../resources/localeinfo.md) object</span></span>
- <span data-ttu-id="e9639-136">cadeia de caracteres (para **timeZone**)</span><span class="sxs-lookup"><span data-stu-id="e9639-136">string (for **timeZone**)</span></span>

## <a name="example"></a><span data-ttu-id="e9639-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e9639-137">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="e9639-138">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="e9639-138">Request 1</span></span>
<span data-ttu-id="e9639-139">O primeiro exemplo obtém todas as configurações da caixa de correio do usuário conectado, que incluem configurações de respostas automáticas, fuso horário e configurações de idioma.</span><span class="sxs-lookup"><span data-stu-id="e9639-139">The first example gets all the mailbox settings of the signed-in user's mailbox, which include automatic replies settings, time zone, and language settings.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings
```
##### <a name="response-1"></a><span data-ttu-id="e9639-140">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="e9639-140">Response 1</span></span>
<span data-ttu-id="e9639-p104">A resposta inclui todas as configurações de caixa de correio. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e9639-p104">The response includes all the mailbox settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    }
}
```

##### <a name="request-2"></a><span data-ttu-id="e9639-144">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="e9639-144">Request 2</span></span>
<span data-ttu-id="e9639-145">O segundo exemplo obtém especificamente as configurações de respostas automáticas da caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="e9639-145">The second example gets specifically the automatic replies settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings/automaticRepliesSetting
```
##### <a name="response-2"></a><span data-ttu-id="e9639-146">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="e9639-146">Response 2</span></span>
<span data-ttu-id="e9639-p105">A resposta inclui apenas as configurações de respostas automáticas. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e9639-p105">The response includes only the automatic replies settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.automaticRepliesSetting"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/api/v1.0/$metadata#Me/mailboxSettings/automaticRepliesSetting",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get mailbox settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->