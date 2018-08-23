# <a name="update-user-mailbox-settings"></a><span data-ttu-id="00801-101">Atualizar as configurações de caixa de correio do usuário</span><span class="sxs-lookup"><span data-stu-id="00801-101">Update user mailbox settings</span></span>

<span data-ttu-id="00801-p101">Atualize uma ou mais configurações da caixa de correio do usuário. Isso inclui configurações de [respostas automáticas](../resources/automaticrepliessetting.md) (notificar pessoas automaticamente ao receber emails), [localidade](../resources/localeinfo.md) (idioma e país/região), fuso horário e [horário de trabalho](../resources/workinghours.md).</span><span class="sxs-lookup"><span data-stu-id="00801-p101">Update one or more settings for the user's mailbox. This includes settings for [automatic replies](../resources/automaticrepliessetting.md) (notify people automatically upon receipt of their email), [locale](../resources/localeinfo.md) (language and country/region), time zone, and [working hours](../resources/workinghours.md).</span></span>

<span data-ttu-id="00801-104">Você pode habilitar, configurar ou desabilitar um ou mais destas configurações como parte de [mailboxSettings](../resources/mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="00801-104">You can enable, configure, or disable one or more of these settings as part of [mailboxSettings](../resources/mailboxsettings.md).</span></span>

<span data-ttu-id="00801-105">**Observação** você não pode criar nem excluir configurações da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="00801-105">**Note** You cannot create or delete any mailbox settings.</span></span>

<span data-ttu-id="00801-106">Ao atualizar o fuso horário preferencial de um usuário, você pode especificá-lo no formato do Windows ou da [Autoridade para Atribuição de Números na Internet (IANA)](http://www.iana.org/time-zones) (também conhecido como fuso horário de Olson).</span><span class="sxs-lookup"><span data-stu-id="00801-106">When you update the preferred time zone for a user, you can specify it in the Windows or  [Internet Assigned Numbers Authority (IANA) time zone](http://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span>

## <a name="permissions"></a><span data-ttu-id="00801-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="00801-107">Permissions</span></span>
<span data-ttu-id="00801-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="00801-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="00801-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="00801-110">Permission type</span></span>      | <span data-ttu-id="00801-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="00801-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00801-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="00801-112">Delegated (work or school account)</span></span> | <span data-ttu-id="00801-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00801-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="00801-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="00801-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00801-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00801-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="00801-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="00801-116">Application</span></span> | <span data-ttu-id="00801-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="00801-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="00801-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="00801-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailboxSettings
PATCH /users/{id|userPrincipalName}/mailboxSettings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="00801-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="00801-119">Optional query parameters</span></span>
<span data-ttu-id="00801-120">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="00801-120">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="00801-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="00801-121">Request headers</span></span>
| <span data-ttu-id="00801-122">Nome</span><span class="sxs-lookup"><span data-stu-id="00801-122">Name</span></span>       | <span data-ttu-id="00801-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="00801-123">Type</span></span> | <span data-ttu-id="00801-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="00801-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="00801-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="00801-125">Authorization</span></span>  | <span data-ttu-id="00801-126">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="00801-126">string</span></span>  | <span data-ttu-id="00801-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="00801-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="00801-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="00801-129">Request body</span></span>
<span data-ttu-id="00801-p104">No corpo da solicitação, forneça os valores para as propriedades relevantes que devem ser atualizadas. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade. Para obter o melhor desempenho, não inclua valores existentes que não foram alterados. Estas são as propriedades graváveis/atualizáveis:</span><span class="sxs-lookup"><span data-stu-id="00801-p104">In the request body, supply the values for the relevant properties that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. The following are the writable/updatable properties:</span></span>

| <span data-ttu-id="00801-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="00801-134">Property</span></span>     | <span data-ttu-id="00801-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="00801-135">Type</span></span>   |<span data-ttu-id="00801-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="00801-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00801-137">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="00801-137">automaticRepliesSetting</span></span>|[<span data-ttu-id="00801-138">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="00801-138">automaticRepliesSetting</span></span>](../resources/automaticrepliessetting.md)|<span data-ttu-id="00801-139">Definições de configuração para notificar automaticamente o remetente de um email recebido com uma mensagem do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="00801-139">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span> <span data-ttu-id="00801-140">Você pode definir essas notificações para apenas um intervalo de data futuro.</span><span class="sxs-lookup"><span data-stu-id="00801-140">You can set such notifications for only a future date range.</span></span>|
|<span data-ttu-id="00801-141">idioma</span><span class="sxs-lookup"><span data-stu-id="00801-141">language</span></span>|[<span data-ttu-id="00801-142">localeInfo</span><span class="sxs-lookup"><span data-stu-id="00801-142">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="00801-143">Informações sobre a localidade do usuário, incluindo o idioma preferencial e o país/região.</span><span class="sxs-lookup"><span data-stu-id="00801-143">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="00801-144">timeZone</span><span class="sxs-lookup"><span data-stu-id="00801-144">timeZone</span></span>|<span data-ttu-id="00801-145">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="00801-145">string</span></span>|<span data-ttu-id="00801-146">O fuso horário padrão para a caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="00801-146">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="00801-147">workingHours</span><span class="sxs-lookup"><span data-stu-id="00801-147">workingHours</span></span>|[<span data-ttu-id="00801-148">workingHours</span><span class="sxs-lookup"><span data-stu-id="00801-148">workingHours</span></span>](../resources/workinghours.md)|<span data-ttu-id="00801-149">As horas, os dias de uma semana e o fuso horário em que o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="00801-149">The hours, days of a week, and time zone that the user works.</span></span>|

## <a name="response"></a><span data-ttu-id="00801-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="00801-150">Response</span></span>

<span data-ttu-id="00801-151">Se tiver êxito, este método retornará um código de resposta `200 OK` e o objeto [mailboxSettings](../resources/mailboxSettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="00801-151">If successful, this method returns a `200 OK` response code and [mailboxSettings](../resources/mailboxSettings.md) object in the response body.</span></span>


## <a name="errors"></a><span data-ttu-id="00801-152">Erros</span><span class="sxs-lookup"><span data-stu-id="00801-152">Errors</span></span>

<span data-ttu-id="00801-153">Definir horas de trabalho com valores inadequados pode retornar os seguintes erros.</span><span class="sxs-lookup"><span data-stu-id="00801-153">Setting working hours with inappropriate values may return the following errors.</span></span>

| <span data-ttu-id="00801-154">Cenário</span><span class="sxs-lookup"><span data-stu-id="00801-154">Scenario</span></span>   | <span data-ttu-id="00801-155">Código de status de HTTP</span><span class="sxs-lookup"><span data-stu-id="00801-155">HTTP status code</span></span> | <span data-ttu-id="00801-156">Código de erro</span><span class="sxs-lookup"><span data-stu-id="00801-156">Error code</span></span> | <span data-ttu-id="00801-157">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="00801-157">Error message</span></span> |
|:-----------|:------|:----------|:----------|
| <span data-ttu-id="00801-158">**startTime** ou **endTime** inválido</span><span class="sxs-lookup"><span data-stu-id="00801-158">Invalid **startTime** or **endTime**</span></span> | <span data-ttu-id="00801-159">400</span><span class="sxs-lookup"><span data-stu-id="00801-159">4.0.0</span></span> | <span data-ttu-id="00801-160">RequestBodyRead</span><span class="sxs-lookup"><span data-stu-id="00801-160">RequestBodyRead</span></span> | <span data-ttu-id="00801-161">Não é possível converter o literal '08"para o tipo 'Edm.TimeOfDay' esperado.</span><span class="sxs-lookup"><span data-stu-id="00801-161">Cannot convert the literal '08' to the expected type 'Edm.TimeOfDay'.</span></span>|
| <span data-ttu-id="00801-162">A hora de início é maior do que a hora de término</span><span class="sxs-lookup"><span data-stu-id="00801-162">Start time is greater than end time</span></span> | <span data-ttu-id="00801-163">400</span><span class="sxs-lookup"><span data-stu-id="00801-163">4.0.0</span></span> | <span data-ttu-id="00801-164">ErrorInvalidTimeSettings</span><span class="sxs-lookup"><span data-stu-id="00801-164">ErrorInvalidTimeSettings</span></span> | <span data-ttu-id="00801-165">A Hora de Início deve ocorrer antes da Hora de Término.</span><span class="sxs-lookup"><span data-stu-id="00801-165">Start Time should occur before End Time.</span></span> |
| <span data-ttu-id="00801-166">Dia inválido em **daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="00801-166">Invalid day in **daysOfWeek**</span></span> | <span data-ttu-id="00801-167">400</span><span class="sxs-lookup"><span data-stu-id="00801-167">4.0.0</span></span> | <span data-ttu-id="00801-168">InvalidArguments</span><span class="sxs-lookup"><span data-stu-id="00801-168">InvalidArguments</span></span> | <span data-ttu-id="00801-169">O valor solicitada "RandomDay" não foi encontrado.</span><span class="sxs-lookup"><span data-stu-id="00801-169">Requested value 'RandomDay' was not found.</span></span>|
| <span data-ttu-id="00801-170">**timeZone** inválido</span><span class="sxs-lookup"><span data-stu-id="00801-170">Invalid **timeZone**</span></span> | <span data-ttu-id="00801-171">400</span><span class="sxs-lookup"><span data-stu-id="00801-171">4.0.0</span></span> | <span data-ttu-id="00801-172">InvalidTimeZone</span><span class="sxs-lookup"><span data-stu-id="00801-172">InvalidTimeZone</span></span> | <span data-ttu-id="00801-173">As configurações de Fuso Horário fornecidas são inválidas.</span><span class="sxs-lookup"><span data-stu-id="00801-173">Time Zone settings provided are invalid.</span></span>|


## <a name="example"></a><span data-ttu-id="00801-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="00801-174">Example</span></span>
##### <a name="request"></a><span data-ttu-id="00801-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="00801-175">Request</span></span>
<span data-ttu-id="00801-176">O primeiro exemplo habilita as respostas automáticas de um intervalo de datas, definindo as seguintes propriedades da propriedade **automaticRepliesSetting**: **status**, **scheduledStartDateTime** e **scheduledEndDateTime**.</span><span class="sxs-lookup"><span data-stu-id="00801-176">The first example enables automatic replies for a date range, by setting the following properties of the **automaticRepliesSetting** property: **status**, **scheduledStartDateTime** and **scheduledEndDateTime**.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_mailboxsettings"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/mailboxSettings
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/mailboxSettings",
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
##### <a name="response"></a><span data-ttu-id="00801-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="00801-177">Response</span></span>
<span data-ttu-id="00801-178">A resposta inclui apenas as configurações atualizadas de respostas automáticas.</span><span class="sxs-lookup"><span data-stu-id="00801-178">The response includes the updated settings for automatic replies.</span></span> <span data-ttu-id="00801-179">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="00801-179">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="00801-180">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="00801-180">All of the properties will be returned from an actual call.</span></span>
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
        "status": "scheduled",
        "externalAudience": "all",
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
    }
}
```


##### <a name="request-2"></a><span data-ttu-id="00801-181">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="00801-181">Request 2</span></span>
<span data-ttu-id="00801-182">O segundo exemplo personaliza o fuso horário das horas de trabalho do usuário conectado definindo a propriedade **timeZone** para um [fuso horário personalizado](../resources/customtimezone.md).</span><span class="sxs-lookup"><span data-stu-id="00801-182">The second example customizes the time zone for the working hours of the signed-in user, by setting the **timeZone** property to a [custom time zone](../resources/customtimezone.md).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "update_mailboxsettings_2"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/mailboxSettings
Content-Type: application/json

{
  "workingHours": {
      "endTime" : "18:30:00.0000000", 
      "daysOfWeek": [ 
          "Monday", 
          "Tuesday", 
          "Wednesday", 
          "Thursday", 
          "Friday", 
          "Saturday" 
      ], 
      "timeZone" : { 
         "@odata.type": "#microsoft.graph.customTimeZone", 
         "bias":-300, 
         "name": "Customized Time Zone",
         "standardOffset":{   
           "time":"02:00:00.0000000", 
           "dayOccurrence":2, 
           "dayOfWeek":"Sunday", 
           "month":10, 
           "year":0 
         }, 
         "daylightOffset":{   
           "daylightBias":100, 
           "time":"02:00:00.0000000", 
           "dayOccurrence":4, 
           "dayOfWeek":"Sunday", 
           "month":5, 
           "year":0 
         } 
      } 
  }
} 
```
##### <a name="response-2"></a><span data-ttu-id="00801-183">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="00801-183">Response 2</span></span>
<span data-ttu-id="00801-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="00801-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "update_mailboxsettings_2",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('94447c6e-ea4c-494c-a9ed-d905e366c5cb')/mailboxSettings",
    "workingHours":{
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