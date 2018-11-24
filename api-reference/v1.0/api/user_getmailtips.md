# <a name="user-getmailtips"></a><span data-ttu-id="f7757-101">usuário: getMailTips</span><span class="sxs-lookup"><span data-stu-id="f7757-101">user: getMailTips</span></span>

<span data-ttu-id="f7757-102">Obtenha dicas de email de um ou mais destinatários conforme disponível ao entrou no [usuário](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="f7757-102">Get the MailTips of one or more recipients as available to the signed-in [user](../resources/user.md).</span></span>

<span data-ttu-id="f7757-103">Observe que, tornando uma `POST` chamada para o `getMailTips` ação, você poderá solicitar tipos específicos de dicas de email a ser retornado por mais de um destinatário de uma só vez.</span><span class="sxs-lookup"><span data-stu-id="f7757-103">Note that by making a `POST` call to the `getMailTips` action, you can request specific types of MailTips to be returned for more than one recipient at one time.</span></span> <span data-ttu-id="f7757-104">As dicas de email solicitadas são retornadas em uma coleção de [dicas de email](../resources/mailtips.md) .</span><span class="sxs-lookup"><span data-stu-id="f7757-104">The requested MailTips are returned in a [mailTips](../resources/mailtips.md) collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7757-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="f7757-105">Permissions</span></span>
<span data-ttu-id="f7757-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f7757-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f7757-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7757-108">Permission type</span></span>      | <span data-ttu-id="f7757-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f7757-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7757-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7757-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f7757-111">Mail.Read, Mail.Read.Shared</span><span class="sxs-lookup"><span data-stu-id="f7757-111">Mail.Read, Mail.Read.Shared</span></span>    |
|<span data-ttu-id="f7757-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7757-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7757-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f7757-113">Mail.Read</span></span>    |
|<span data-ttu-id="f7757-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7757-114">Application</span></span> | <span data-ttu-id="f7757-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f7757-115">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7757-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7757-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMailTips
POST /users/{id|userPrincipalName}/getMailTips
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f7757-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f7757-117">Optional query parameters</span></span>
<span data-ttu-id="f7757-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f7757-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f7757-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7757-119">Request headers</span></span>
| <span data-ttu-id="f7757-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f7757-120">Header</span></span>       | <span data-ttu-id="f7757-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f7757-121">Value</span></span>|
|:-----------  |:------|
| <span data-ttu-id="f7757-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7757-122">Authorization</span></span> | <span data-ttu-id="f7757-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7757-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f7757-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f7757-125">Content-Type</span></span>  | <span data-ttu-id="f7757-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f7757-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f7757-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7757-127">Request body</span></span>
<span data-ttu-id="f7757-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7757-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f7757-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f7757-129">Property</span></span>     | <span data-ttu-id="f7757-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7757-130">Type</span></span>   |<span data-ttu-id="f7757-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7757-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7757-132">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="f7757-132">EmailAddresses</span></span>|<span data-ttu-id="f7757-133">String collection</span><span class="sxs-lookup"><span data-stu-id="f7757-133">String collection</span></span>|<span data-ttu-id="f7757-134">Uma coleção de endereços SMTP de destinatários para receber as Dicas de Email.</span><span class="sxs-lookup"><span data-stu-id="f7757-134">A collection of SMTP addresses of recipients to get MailTips for.</span></span>|
|<span data-ttu-id="f7757-135">MailTipsOptions</span><span class="sxs-lookup"><span data-stu-id="f7757-135">MailTipsOptions</span></span>|<span data-ttu-id="f7757-136">String</span><span class="sxs-lookup"><span data-stu-id="f7757-136">String</span></span>|<span data-ttu-id="f7757-137">Enumeração dos sinalizadores que representa as dicas de email solicitadas.</span><span class="sxs-lookup"><span data-stu-id="f7757-137">A enumeration of flags that represents the requested mailtips.</span></span> <span data-ttu-id="f7757-138">Os valores possíveis são: `automaticReplies`, `customMailTip`, `deliveryRestriction`, `externalMemberCount`, `mailboxFullStatus`, `maxMessageSize`, `moderationStatus`, `recipientScope`, `recipientSuggestions`, e `totalMemberCount`.</span><span class="sxs-lookup"><span data-stu-id="f7757-138">Possible values are: `automaticReplies`, `customMailTip`, `deliveryRestriction`, `externalMemberCount`, `mailboxFullStatus`, `maxMessageSize`, `moderationStatus`, `recipientScope`, `recipientSuggestions`, and `totalMemberCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="f7757-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7757-139">Response</span></span>

<span data-ttu-id="f7757-140">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos de [dicas de email](../resources/mailtips.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7757-140">If successful, this method returns a `200 OK` response code and a collection of [mailTips](../resources/mailtips.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f7757-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f7757-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f7757-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7757-142">Request</span></span>
<span data-ttu-id="f7757-143">O exemplo a seguir obtém as dicas de email para os destinatários especificados, para quaisquer configurações de resposta automática e o status completo de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="f7757-143">The following example gets MailTips for the specified recipients, for any automatic reply settings and the mailbox full status.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_getmailtips"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMailTips
Content-Type: application/json

{
    "EmailAddresses": [
        "danas@contoso.onmicrosoft.com", 
        "fannyd@contoso.onmicrosoft.com"
    ],
    "MailTipsOptions": "automaticReplies, mailboxFullStatus"
}
```

##### <a name="response"></a><span data-ttu-id="f7757-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7757-144">Response</span></span>
<span data-ttu-id="f7757-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f7757-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailTips",
  isCollection: true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.mailTips)",
    "value":[
        {
            "emailAddress":{
                "name":"",
                "address":"danas@contoso.onmicrosoft.com"
            },
            "automaticReplies":{
                "message":"<style type=\"text/css\" style=\"\">\r\n<!--\r\np\r\n\t{margin-top:0;\r\n\tmargin-bottom:0}\r\n-->\r\n</style>\r\n<div dir=\"ltr\">\r\n<div id=\"x_divtagdefaultwrapper\" style=\"font-size:12pt; color:#000000; background-color:#FFFFFF; font-family:Calibri,Arial,Helvetica,sans-serif\">\r\n<p>Hi, I am on vacation right now. I'll get back to you after I return.<br>\r\n</p>\r\n</div>\r\n</div>",
                "messageLanguage":{
                    "locale":"en-US",
                    "displayName":"English (United States)"
                },
                "scheduledStartTime": {
                    "dateTime": "2018-08-07T02:00:00.0000000",
                    "timeZone": "UTC"
                },
                "scheduledEndTime": {
                    "dateTime": "2018-08-09T02:00:00.0000000",
                    "timeZone": "UTC"
                }
            },
            "mailboxFull":false
        },
        {
            "emailAddress":{
                "name":"",
                "address":"fannyd@contoso.onmicrosoft.com"
            },
            "automaticReplies":{
                "message":""
            },
            "mailboxFull":false
        }
    ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: getMailTips",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
