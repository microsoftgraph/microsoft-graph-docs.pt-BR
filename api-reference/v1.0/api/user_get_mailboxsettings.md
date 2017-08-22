# <a name="get-user-mailbox-settings"></a><span data-ttu-id="97175-101">Obter as configurações da caixa de correio do usuário</span><span class="sxs-lookup"><span data-stu-id="97175-101">Get user mailbox settings</span></span>

<span data-ttu-id="97175-p101">Obtenha as [mailboxSettings](../resources/mailboxsettings.md) do usuário. Isso inclui configurações para respostas automáticas (notificar as pessoas automaticamente ao receber seus emails), localidade (país/região e idioma) e fuso horário.</span><span class="sxs-lookup"><span data-stu-id="97175-p101">Get the user's [mailboxSettings](../resources/mailboxsettings.md). This includes settings for automatic replies (notify people automatically upon receipt of their email), locale (language and country/region), and time zone.</span></span>

<span data-ttu-id="97175-104">Você pode exibir todas as configurações de caixa de correio ou obter configurações específicas.</span><span class="sxs-lookup"><span data-stu-id="97175-104">You can view all mailbox settings, or, get specific settings.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97175-105">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="97175-105">Prerequisites</span></span>
<span data-ttu-id="97175-106">O seguinte **escopo** é obrigatório para executar esta API: *MailboxSettings.Read*</span><span class="sxs-lookup"><span data-stu-id="97175-106">The following **scope** is required to execute this API: *MailboxSettings.Read*</span></span>  

## <a name="http-request"></a><span data-ttu-id="97175-107">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97175-107">HTTP request</span></span>
<span data-ttu-id="97175-108">Para acessar todas as configurações de email que incluem configurações de respostas automáticas:</span><span class="sxs-lookup"><span data-stu-id="97175-108">To get all mailbox settings which include automatic replies settings:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

<span data-ttu-id="97175-109">Para obter configurações específicas, por exemplo, somente as configurações de respostas automáticas, localidade ou fuso horário:</span><span class="sxs-lookup"><span data-stu-id="97175-109">To get specific settings - for example, only the automatic replies settings, locale, or time zone:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailboxSettings/automaticRepliesSetting
GET /users/{id|userPrincipalName}/mailboxSettings/automaticRepliesSetting

GET /me/mailboxSettings/language
GET /users/{id|userPrincipalName}/mailboxSettings/language

GET /me/mailboxSettings/timeZone
GET /users/{id|userPrincipalName}/mailboxSettings/timeZone
```
## <a name="optional-query-parameters"></a><span data-ttu-id="97175-110">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="97175-110">Optional query parameters</span></span>
<span data-ttu-id="97175-111">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="97175-111">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="97175-112">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="97175-112">Request headers</span></span>
| <span data-ttu-id="97175-113">Nome</span><span class="sxs-lookup"><span data-stu-id="97175-113">Name</span></span>       | <span data-ttu-id="97175-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="97175-114">Type</span></span> | <span data-ttu-id="97175-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="97175-115">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="97175-116">Autorização</span><span class="sxs-lookup"><span data-stu-id="97175-116">Authorization</span></span>  | <span data-ttu-id="97175-117">string</span><span class="sxs-lookup"><span data-stu-id="97175-117">string</span></span>  | <span data-ttu-id="97175-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97175-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="97175-120">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97175-120">Request body</span></span>
<span data-ttu-id="97175-121">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="97175-121">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97175-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="97175-122">Response</span></span>

<span data-ttu-id="97175-123">Se for bem-sucedido, este método retornará um código de resposta `200 OK` e um dos seguintes objetos solicitados no corpo da resposta:</span><span class="sxs-lookup"><span data-stu-id="97175-123">If successful, this method returns a `200 OK` response code and one of the following requested objects in the response body:</span></span>

- <span data-ttu-id="97175-124">Objeto [mailboxSettings](../resources/mailboxsettings.md)</span><span class="sxs-lookup"><span data-stu-id="97175-124">[mailboxSettings](../resources/mailboxsettings.md) object</span></span>
- <span data-ttu-id="97175-125">Objeto [automaticRepliesSetting](../resources/automaticRepliesSetting.md)</span><span class="sxs-lookup"><span data-stu-id="97175-125">[automaticRepliesSetting](../resources/automaticRepliesSetting.md) object</span></span>
- <span data-ttu-id="97175-126">Objeto [localeInfo](../resources/localeinfo.md)</span><span class="sxs-lookup"><span data-stu-id="97175-126">[localeInfo](../resources/localeinfo.md) object</span></span>
- <span data-ttu-id="97175-127">cadeia de caracteres (para **timeZone**)</span><span class="sxs-lookup"><span data-stu-id="97175-127">string (for **timeZone**)</span></span>

## <a name="example"></a><span data-ttu-id="97175-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97175-128">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="97175-129">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="97175-129">Request 1</span></span>
<span data-ttu-id="97175-130">O primeiro exemplo obtém todas as configurações da caixa de correio do usuário conectado, que incluem configurações de respostas automáticas, fuso horário e configurações de idioma.</span><span class="sxs-lookup"><span data-stu-id="97175-130">The first example gets all the mailbox settings of the signed-in user's mailbox, which include automatic replies settings, time zone, and language settings.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings
```
##### <a name="response-1"></a><span data-ttu-id="97175-131">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="97175-131">Response 1</span></span>
<span data-ttu-id="97175-p103">A resposta inclui todas as configurações de caixa de correio. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="97175-p103">The response includes all the mailbox settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="97175-135">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="97175-135">Request 2</span></span>
<span data-ttu-id="97175-136">O segundo exemplo obtém especificamente as configurações de respostas automáticas da caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="97175-136">The second example gets specifically the automatic replies settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailboxSettings/automaticRepliesSetting
```
##### <a name="response-2"></a><span data-ttu-id="97175-137">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="97175-137">Response 2</span></span>
<span data-ttu-id="97175-p104">A resposta inclui apenas as configurações de respostas automáticas. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="97175-p104">The response includes only the automatic replies settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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