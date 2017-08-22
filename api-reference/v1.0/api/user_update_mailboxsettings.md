# <a name="update-user-mailbox-settings"></a><span data-ttu-id="e3542-101">Atualizar as configurações de caixa de correio do usuário</span><span class="sxs-lookup"><span data-stu-id="e3542-101">Update user mailbox settings</span></span>

<span data-ttu-id="e3542-p101">Atualize uma ou mais configurações da caixa de correio do usuário. Isso inclui configurações de fuso horário, localidade ou respostas automáticas (notificar as pessoas automaticamente ao receber seus emails).</span><span class="sxs-lookup"><span data-stu-id="e3542-p101">Update one or more settings for the user's mailbox. This includes settings for automatic replies (notify people automatically upon receipt of their email), locale, or time zone.</span></span>

<span data-ttu-id="e3542-104">Você pode habilitar, configurar ou desabilitar um ou mais destas configurações como parte de [mailboxSettings](../resources/mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="e3542-104">You can enable, configure, or disable one or more of these settings as part of [mailboxSettings](../resources/mailboxsettings.md).</span></span>

<span data-ttu-id="e3542-105">**Observação** você não pode criar nem excluir configurações da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="e3542-105">**Note** You cannot create or delete any mailbox settings.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e3542-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e3542-106">Prerequisites</span></span>
<span data-ttu-id="e3542-107">O seguinte **escopo** é obrigatório para executar esta API: *MailboxSettings.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="e3542-107">The following **scope** is required to execute this API: *MailboxSettings.ReadWrite*</span></span>  
## <a name="http-request"></a><span data-ttu-id="e3542-108">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3542-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailboxSettings
PATCH /users/{id|userPrincipalName}/mailboxSettings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e3542-109">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e3542-109">Optional query parameters</span></span>
<span data-ttu-id="e3542-110">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e3542-110">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e3542-111">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3542-111">Request headers</span></span>
| <span data-ttu-id="e3542-112">Nome</span><span class="sxs-lookup"><span data-stu-id="e3542-112">Name</span></span>       | <span data-ttu-id="e3542-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3542-113">Type</span></span> | <span data-ttu-id="e3542-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3542-114">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e3542-115">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3542-115">Authorization</span></span>  | <span data-ttu-id="e3542-116">string</span><span class="sxs-lookup"><span data-stu-id="e3542-116">string</span></span>  | <span data-ttu-id="e3542-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3542-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e3542-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3542-119">Request body</span></span>
<span data-ttu-id="e3542-p103">No corpo da solicitação, forneça os valores para as propriedades relevantes que devem ser atualizadas. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade. Para obter o melhor desempenho, não inclua valores existentes que não foram alterados. Estas são as propriedades graváveis/atualizáveis:</span><span class="sxs-lookup"><span data-stu-id="e3542-p103">In the request body, supply the values for the relevant properties that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. The following are the writable/updatable properties:</span></span>

| <span data-ttu-id="e3542-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3542-124">Property</span></span>     | <span data-ttu-id="e3542-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3542-125">Type</span></span>   |<span data-ttu-id="e3542-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3542-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3542-127">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="e3542-127">automaticRepliesSetting</span></span>|[<span data-ttu-id="e3542-128">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="e3542-128">automaticRepliesSetting</span></span>](../resources/automaticrepliessetting.md)|<span data-ttu-id="e3542-129">Definições de configuração para notificar automaticamente o remetente de um email recebido com uma mensagem do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="e3542-129">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="e3542-130">idioma</span><span class="sxs-lookup"><span data-stu-id="e3542-130">language</span></span>|[<span data-ttu-id="e3542-131">localeInfo</span><span class="sxs-lookup"><span data-stu-id="e3542-131">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="e3542-132">Informações sobre a localidade do usuário, incluindo o idioma preferencial e o país/região.</span><span class="sxs-lookup"><span data-stu-id="e3542-132">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="e3542-133">timeZone</span><span class="sxs-lookup"><span data-stu-id="e3542-133">timeZone</span></span>|<span data-ttu-id="e3542-134">string</span><span class="sxs-lookup"><span data-stu-id="e3542-134">string</span></span>|<span data-ttu-id="e3542-135">O fuso horário padrão para a caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="e3542-135">The default time zone for the user's mailbox.</span></span>|

## <a name="response"></a><span data-ttu-id="e3542-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3542-136">Response</span></span>

<span data-ttu-id="e3542-137">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [mailboxSettings](../resources/mailboxSettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3542-137">If successful, this method returns a `200 OK` response code and [mailboxSettings](../resources/mailboxSettings.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e3542-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e3542-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e3542-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3542-139">Request</span></span>
<span data-ttu-id="e3542-140">O exemplo a seguir habilita as respostas automáticas para um intervalo de datas, definindo as seguintes propriedades da propriedade **automaticRepliesSetting**: **status**, **scheduledStartDateTime** e **scheduledEndDateTime**.</span><span class="sxs-lookup"><span data-stu-id="e3542-140">The following example enables automatic replies for a date range, by setting the following properties of the **automaticRepliesSetting** property: **status**, **scheduledStartDateTime** and **scheduledEndDateTime**.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_mailboxsettings"
}-->
```http
PATCH https://graph.microsoft.com/api/v1.0/me/mailboxSettings
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/api/v1.0/$metadata#Me/mailboxSettings",
    "automaticRepliesSetting": {
        "status": "Scheduled",
        "scheduledStartDateTime": {
          "dateTime": "2016-03-20T18:00:00.0000000",
          "timeZone": "UTC"
        },
        "scheduledEndDateTime": {
          "dateTime": "2016-03-28T18:00:00.0000000",
          "timeZone": "UTC"
        }
    }
}
```
##### <a name="response"></a><span data-ttu-id="e3542-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3542-141">Response</span></span>
<span data-ttu-id="e3542-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e3542-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/api/v1.0/$metadata#Me/mailboxSettings",
    "automaticRepliesSetting": {
        "status": "scheduled",
        "externalAudience": "none",
        "scheduledStartDateTime": {
            "dateTime": "2016-03-20T02:00:00.0000000",
            "timeZone": "UTC"
        },
        "scheduledEndDateTime": {
            "dateTime": "2016-03-28T02:00:00.0000000",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update mailbox settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->