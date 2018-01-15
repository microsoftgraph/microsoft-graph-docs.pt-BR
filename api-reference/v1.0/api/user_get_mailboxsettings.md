# <a name="get-user-mailbox-settings"></a><span data-ttu-id="e2df4-101">Obter as configurações da caixa de correio do usuário</span><span class="sxs-lookup"><span data-stu-id="e2df4-101">Get user mailbox settings</span></span>

<span data-ttu-id="e2df4-p101">Obtenha as [mailboxSettings](../resources/mailboxsettings.md) do usuário. Isso inclui configurações para respostas automáticas (notificar as pessoas automaticamente ao receber seus emails), localidade (país/região e idioma) e fuso horário.</span><span class="sxs-lookup"><span data-stu-id="e2df4-p101">Get the user's [mailboxSettings](../resources/mailboxsettings.md). This includes settings for automatic replies (notify people automatically upon receipt of their email), locale (language and country/region), and time zone.</span></span>

<span data-ttu-id="e2df4-104">Você pode exibir todas as configurações de caixa de correio ou obter configurações específicas.</span><span class="sxs-lookup"><span data-stu-id="e2df4-104">You can view all mailbox settings, or, get specific settings.</span></span>

<span data-ttu-id="e2df4-105">O fuso horário é uma das configurações de preferência que um usuário pode fazer na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="e2df4-105">Time zone is one of the preferred settings a user can set up for the user's mailbox.</span></span> <span data-ttu-id="e2df4-106">Entre os formatos de fuso horário válidos estão o do Windows e o da [Autoridade para Atribuição de Números na Internet (IANA)]((http://www.iana.org/time-zones)) (também conhecido como fuso horário de Olson).</span><span class="sxs-lookup"><span data-stu-id="e2df4-106">Valid time zone formats include the Windows time zone format and [Internet Assigned Numbers Authority (IANA) time zone]((http://www.iana.org/time-zones)) (also known as Olson time zone) format.</span></span> <span data-ttu-id="e2df4-107">O formato do Windows é o padrão.</span><span class="sxs-lookup"><span data-stu-id="e2df4-107">The Windows format is the default.</span></span> 

<span data-ttu-id="e2df4-108">Ao obter o fuso horário de preferência de um usuário, ele é retornado no formato em que foi configurado.</span><span class="sxs-lookup"><span data-stu-id="e2df4-108">When you get a user's preferred time zone, the time zone is returned in the format that it was set up.</span></span> <span data-ttu-id="e2df4-109">Se quiser que o fuso horário esteja em um formato específico (Windows ou IANA), você pode primeiro [atualizar o fuso horário de preferência nesse formato como uma configuração de caixa de correio](user_update_mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="e2df4-109">If you want that time zone to be in a specific format (Windows or IANA), you can first [update the preferred time zone in that format as a mailbox setting](user_update_mailboxsettings.md).</span></span> <span data-ttu-id="e2df4-110">Posteriormente, você poderá obter o fuso horário nesse formato.</span><span class="sxs-lookup"><span data-stu-id="e2df4-110">Subsequently you will be able to get the time zone in that format.</span></span> <span data-ttu-id="e2df4-111">Como alternativa, você pode gerenciar a conversão de formato separadamente no seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e2df4-111">Alternatively, you can manage the format conversion separately in your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2df4-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="e2df4-112">Permissions</span></span>
<span data-ttu-id="e2df4-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e2df4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e2df4-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e2df4-115">Permission type</span></span>      | <span data-ttu-id="e2df4-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e2df4-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2df4-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e2df4-117">Delegated (work or school account)</span></span> | <span data-ttu-id="e2df4-118">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e2df4-118">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="e2df4-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e2df4-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2df4-120">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e2df4-120">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="e2df4-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e2df4-121">Application</span></span> | <span data-ttu-id="e2df4-122">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e2df4-122">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2df4-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e2df4-123">HTTP request</span></span>
<span data-ttu-id="e2df4-124">Para acessar todas as configurações de email que incluem configurações de respostas automáticas:</span><span class="sxs-lookup"><span data-stu-id="e2df4-124">To get all mailbox settings which include automatic replies settings:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

<span data-ttu-id="e2df4-125">Para obter configurações específicas, por exemplo, somente as configurações de respostas automáticas, localidade ou fuso horário:</span><span class="sxs-lookup"><span data-stu-id="e2df4-125">To get specific settings - for example, only the automatic replies settings, locale, or time zone:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings/automaticRepliesSetting
GET /users/{id|userPrincipalName}/mailboxSettings/automaticRepliesSetting

GET /me/mailboxSettings/language
GET /users/{id|userPrincipalName}/mailboxSettings/language

GET /me/mailboxSettings/timeZone
GET /users/{id|userPrincipalName}/mailboxSettings/timeZone
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e2df4-126">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e2df4-126">Optional query parameters</span></span>
<span data-ttu-id="e2df4-127">Este método dá suporte a [Parâmetros de consulta OData]((http://developer.microsoft.com/pt-BR/graph/docs/overview/query_parameters)) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e2df4-127">This method supports the [OData Query Parameters]((http://developer.microsoft.com/pt-BR/graph/docs/overview/query_parameters)) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e2df4-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e2df4-128">Request headers</span></span>
| <span data-ttu-id="e2df4-129">Nome</span><span class="sxs-lookup"><span data-stu-id="e2df4-129">Name</span></span>       | <span data-ttu-id="e2df4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2df4-130">Type</span></span> | <span data-ttu-id="e2df4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2df4-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e2df4-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="e2df4-132">Authorization</span></span>  | <span data-ttu-id="e2df4-133">string</span><span class="sxs-lookup"><span data-stu-id="e2df4-133">string</span></span>  | <span data-ttu-id="e2df4-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2df4-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2df4-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e2df4-136">Request body</span></span>
<span data-ttu-id="e2df4-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e2df4-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2df4-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2df4-138">Response</span></span>

<span data-ttu-id="e2df4-139">Se for bem-sucedido, este método retornará um código de resposta `200 OK` e um dos seguintes objetos solicitados no corpo da resposta:</span><span class="sxs-lookup"><span data-stu-id="e2df4-139">If successful, this method returns a `200 OK` response code and one of the following requested objects in the response body:</span></span>

- <span data-ttu-id="e2df4-140">Objeto [mailboxSettings](../resources/mailboxsettings.md)</span><span class="sxs-lookup"><span data-stu-id="e2df4-140">[mailboxSettings](../resources/mailboxsettings.md) object</span></span>
- <span data-ttu-id="e2df4-141">Objeto [automaticRepliesSetting](../resources/automaticRepliesSetting.md)</span><span class="sxs-lookup"><span data-stu-id="e2df4-141">[automaticRepliesSetting](../resources/automaticRepliesSetting.md) object</span></span>
- <span data-ttu-id="e2df4-142">Objeto [localeInfo](../resources/localeinfo.md)</span><span class="sxs-lookup"><span data-stu-id="e2df4-142">[localeInfo](../resources/localeinfo.md) object</span></span>
- <span data-ttu-id="e2df4-143">cadeia de caracteres (para **timeZone**)</span><span class="sxs-lookup"><span data-stu-id="e2df4-143">string (for **timeZone**)</span></span>

## <a name="example"></a><span data-ttu-id="e2df4-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e2df4-144">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="e2df4-145">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="e2df4-145">Request 1</span></span>
<span data-ttu-id="e2df4-146">O primeiro exemplo obtém todas as configurações da caixa de correio do usuário conectado, que incluem configurações de respostas automáticas, fuso horário e configurações de idioma.</span><span class="sxs-lookup"><span data-stu-id="e2df4-146">The first example gets all the mailbox settings of the signed-in user's mailbox, which include automatic replies settings, time zone, and language settings.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings
```
##### <a name="response-1"></a><span data-ttu-id="e2df4-147">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="e2df4-147">Response 1</span></span>
<span data-ttu-id="e2df4-p106">A resposta inclui todas as configurações de caixa de correio. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e2df4-p106">The response includes all the mailbox settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="e2df4-151">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="e2df4-151">Request 2</span></span>
<span data-ttu-id="e2df4-152">O segundo exemplo obtém especificamente as configurações de respostas automáticas da caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="e2df4-152">The second example gets specifically the automatic replies settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings/automaticRepliesSetting
```
##### <a name="response-2"></a><span data-ttu-id="e2df4-153">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="e2df4-153">Response 2</span></span>
<span data-ttu-id="e2df4-p107">A resposta inclui apenas as configurações de respostas automáticas. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e2df4-p107">The response includes only the automatic replies settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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