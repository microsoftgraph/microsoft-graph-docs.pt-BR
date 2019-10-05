---
title: Atualizar as configurações de caixa de correio do usuário
description: Atualize uma ou mais configurações da caixa de correio do usuário. Isso inclui as configurações para respostas automáticas (notificar as pessoas automaticamente no recebimento de seus emails), localidade (idioma e país/região), fuso horário e horário de trabalho.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0a224df7acdc0396d13743433d2cb407eb500d06
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402827"
---
# <a name="update-user-mailbox-settings"></a><span data-ttu-id="456a0-104">Atualizar as configurações de caixa de correio do usuário</span><span class="sxs-lookup"><span data-stu-id="456a0-104">Update user mailbox settings</span></span>

<span data-ttu-id="456a0-105">Habilitar, configurar ou desabilitar uma ou mais das seguintes configurações como parte do [mailboxSettings](../resources/mailboxsettings.md)de um usuário:</span><span class="sxs-lookup"><span data-stu-id="456a0-105">Enable, configure, or disable one or more of the following settings as part of a user's [mailboxSettings](../resources/mailboxsettings.md):</span></span>

- <span data-ttu-id="456a0-106">[respostas automáticas](../resources/automaticrepliessetting.md) (notificar pessoas automaticamente após o recebimento de seus emails)</span><span class="sxs-lookup"><span data-stu-id="456a0-106">[automatic replies](../resources/automaticrepliessetting.md) (notify people automatically upon receipt of their email)</span></span>
- <span data-ttu-id="456a0-107">dateFormat</span><span class="sxs-lookup"><span data-stu-id="456a0-107">dateFormat</span></span>
- <span data-ttu-id="456a0-108">[localidade](../resources/localeinfo.md) (idioma e país/região)</span><span class="sxs-lookup"><span data-stu-id="456a0-108">[locale](../resources/localeinfo.md) (language and country/region)</span></span>
- <span data-ttu-id="456a0-109">Formato de TimeFormat</span><span class="sxs-lookup"><span data-stu-id="456a0-109">timeFormat</span></span>
- <span data-ttu-id="456a0-110">fuso horário</span><span class="sxs-lookup"><span data-stu-id="456a0-110">time zone</span></span>
- [<span data-ttu-id="456a0-111">horário comercial</span><span class="sxs-lookup"><span data-stu-id="456a0-111">working hours</span></span>](../resources/workinghours.md)

<span data-ttu-id="456a0-112">Ao atualizar o formato de data ou hora preferencial para um usuário, especifique-o, respectivamente, o formato de [data abreviada](https://docs.microsoft.com/en-us/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortDate) ou de [hora curta](https://docs.microsoft.com/en-us/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortTime) .</span><span class="sxs-lookup"><span data-stu-id="456a0-112">When updating the preferred date or time format for a user, specify it in respectively, the [short date](https://docs.microsoft.com/en-us/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortDate) or [short time](https://docs.microsoft.com/en-us/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortTime) format.</span></span> 

<span data-ttu-id="456a0-113">Ao atualizar o fuso horário preferencial para um usuário, especifique-o no formato de fuso horário do Windows ou da [autoridade de números atribuídos à Internet (IANA)](https://www.iana.org/time-zones) (também conhecido como fuso horário do Olson).</span><span class="sxs-lookup"><span data-stu-id="456a0-113">When updating the preferred time zone for a user, specify it in the Windows or [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="456a0-114">Você também pode personalizar ainda mais o fuso horário, conforme mostrado no [exemplo 2](#example-2) abaixo.</span><span class="sxs-lookup"><span data-stu-id="456a0-114">You can also further customize the time zone as shown in [example 2](#example-2) below.</span></span>

> [!TIP] 
> <span data-ttu-id="456a0-115">Você não pode criar nem excluir nenhuma configuração de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="456a0-115">You cannot create or delete any mailbox settings.</span></span>

## <a name="permissions"></a><span data-ttu-id="456a0-116">Permissões</span><span class="sxs-lookup"><span data-stu-id="456a0-116">Permissions</span></span>
<span data-ttu-id="456a0-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="456a0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="456a0-119">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="456a0-119">Permission type</span></span>      | <span data-ttu-id="456a0-120">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="456a0-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="456a0-121">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="456a0-121">Delegated (work or school account)</span></span> | <span data-ttu-id="456a0-122">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="456a0-122">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="456a0-123">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="456a0-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="456a0-124">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="456a0-124">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="456a0-125">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="456a0-125">Application</span></span> | <span data-ttu-id="456a0-126">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="456a0-126">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="456a0-127">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="456a0-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailboxSettings
PATCH /users/{id|userPrincipalName}/mailboxSettings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="456a0-128">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="456a0-128">Optional query parameters</span></span>
<span data-ttu-id="456a0-129">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="456a0-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="456a0-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="456a0-130">Request headers</span></span>
| <span data-ttu-id="456a0-131">Nome</span><span class="sxs-lookup"><span data-stu-id="456a0-131">Name</span></span>       | <span data-ttu-id="456a0-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="456a0-132">Type</span></span> | <span data-ttu-id="456a0-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="456a0-133">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="456a0-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="456a0-134">Authorization</span></span>  | <span data-ttu-id="456a0-135">string</span><span class="sxs-lookup"><span data-stu-id="456a0-135">string</span></span>  | <span data-ttu-id="456a0-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="456a0-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="456a0-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="456a0-138">Request body</span></span>
<span data-ttu-id="456a0-p105">No corpo da solicitação, forneça os valores para as propriedades relevantes que devem ser atualizadas. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade. Para obter o melhor desempenho, não inclua valores existentes que não foram alterados. Estas são as propriedades graváveis/atualizáveis:</span><span class="sxs-lookup"><span data-stu-id="456a0-p105">In the request body, supply the values for the relevant properties that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. The following are the writable/updatable properties:</span></span>

| <span data-ttu-id="456a0-143">Propriedade</span><span class="sxs-lookup"><span data-stu-id="456a0-143">Property</span></span>     | <span data-ttu-id="456a0-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="456a0-144">Type</span></span>   |<span data-ttu-id="456a0-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="456a0-145">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="456a0-146">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="456a0-146">automaticRepliesSetting</span></span>|[<span data-ttu-id="456a0-147">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="456a0-147">automaticRepliesSetting</span></span>](../resources/automaticrepliessetting.md)|<span data-ttu-id="456a0-148">Definições de configuração para notificar automaticamente o remetente de um email recebido com uma mensagem do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="456a0-148">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span> <span data-ttu-id="456a0-149">Você pode definir essas notificações para apenas um intervalo de datas futuras.</span><span class="sxs-lookup"><span data-stu-id="456a0-149">You can set such notifications for only a future date range.</span></span>|
|<span data-ttu-id="456a0-150">dateFormat</span><span class="sxs-lookup"><span data-stu-id="456a0-150">dateFormat</span></span>|<span data-ttu-id="456a0-151">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="456a0-151">string</span></span>|<span data-ttu-id="456a0-152">O formato de data da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="456a0-152">The date format for the user's mailbox.</span></span>|
|<span data-ttu-id="456a0-153">idioma</span><span class="sxs-lookup"><span data-stu-id="456a0-153">language</span></span>|[<span data-ttu-id="456a0-154">localeInfo</span><span class="sxs-lookup"><span data-stu-id="456a0-154">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="456a0-155">Informações sobre a localidade do usuário, incluindo o idioma preferencial e o país/região.</span><span class="sxs-lookup"><span data-stu-id="456a0-155">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="456a0-156">Formato de TimeFormat</span><span class="sxs-lookup"><span data-stu-id="456a0-156">timeFormat</span></span>|<span data-ttu-id="456a0-157">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="456a0-157">string</span></span>|<span data-ttu-id="456a0-158">O formato de hora da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="456a0-158">The time format for the user's mailbox.</span></span>|
|<span data-ttu-id="456a0-159">timeZone</span><span class="sxs-lookup"><span data-stu-id="456a0-159">timeZone</span></span>|<span data-ttu-id="456a0-160">string</span><span class="sxs-lookup"><span data-stu-id="456a0-160">string</span></span>|<span data-ttu-id="456a0-161">O fuso horário padrão para a caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="456a0-161">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="456a0-162">workingHours</span><span class="sxs-lookup"><span data-stu-id="456a0-162">workingHours</span></span>|[<span data-ttu-id="456a0-163">workingHours</span><span class="sxs-lookup"><span data-stu-id="456a0-163">workingHours</span></span>](../resources/workinghours.md)|<span data-ttu-id="456a0-164">As horas, os dias de uma semana e o fuso horário em que o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="456a0-164">The hours, days of a week, and time zone that the user works.</span></span>|

## <a name="response"></a><span data-ttu-id="456a0-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="456a0-165">Response</span></span>

<span data-ttu-id="456a0-166">Se tiver êxito, este método retornará `200 OK` um código de resposta e as propriedades atualizadas de um objeto [mailboxSettings](../resources/mailboxsettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="456a0-166">If successful, this method returns a `200 OK` response code and the updated properties of a [mailboxSettings](../resources/mailboxsettings.md) object in the response body.</span></span>

## <a name="errors"></a><span data-ttu-id="456a0-167">Erros</span><span class="sxs-lookup"><span data-stu-id="456a0-167">Errors</span></span>

<span data-ttu-id="456a0-168">Definir horas de trabalho com valores inadequados pode retornar os seguintes erros.</span><span class="sxs-lookup"><span data-stu-id="456a0-168">Setting working hours with inappropriate values may return the following errors.</span></span>

| <span data-ttu-id="456a0-169">Cenário</span><span class="sxs-lookup"><span data-stu-id="456a0-169">Scenario</span></span>   | <span data-ttu-id="456a0-170">Código de status de HTTP</span><span class="sxs-lookup"><span data-stu-id="456a0-170">HTTP status code</span></span> | <span data-ttu-id="456a0-171">Código de erro</span><span class="sxs-lookup"><span data-stu-id="456a0-171">Error code</span></span> | <span data-ttu-id="456a0-172">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="456a0-172">Error message</span></span> |
|:-----------|:------|:----------|:----------|
| <span data-ttu-id="456a0-173">**startTime** ou **endTime** inválido</span><span class="sxs-lookup"><span data-stu-id="456a0-173">Invalid **startTime** or **endTime**</span></span> | <span data-ttu-id="456a0-174">400</span><span class="sxs-lookup"><span data-stu-id="456a0-174">400</span></span> | <span data-ttu-id="456a0-175">RequestBodyRead</span><span class="sxs-lookup"><span data-stu-id="456a0-175">RequestBodyRead</span></span> | <span data-ttu-id="456a0-176">Não é possível converter o literal '08"para o tipo 'Edm.TimeOfDay' esperado.</span><span class="sxs-lookup"><span data-stu-id="456a0-176">Cannot convert the literal '08' to the expected type 'Edm.TimeOfDay'.</span></span>|
| <span data-ttu-id="456a0-177">A hora de início é maior do que a hora de término</span><span class="sxs-lookup"><span data-stu-id="456a0-177">Start time is greater than end time</span></span> | <span data-ttu-id="456a0-178">400</span><span class="sxs-lookup"><span data-stu-id="456a0-178">400</span></span> | <span data-ttu-id="456a0-179">ErrorInvalidTimeSettings</span><span class="sxs-lookup"><span data-stu-id="456a0-179">ErrorInvalidTimeSettings</span></span> | <span data-ttu-id="456a0-180">A Hora de Início deve ocorrer antes da Hora de Término.</span><span class="sxs-lookup"><span data-stu-id="456a0-180">Start Time should occur before End Time.</span></span> |
| <span data-ttu-id="456a0-181">Dia inválido em **daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="456a0-181">Invalid day in **daysOfWeek**</span></span> | <span data-ttu-id="456a0-182">400</span><span class="sxs-lookup"><span data-stu-id="456a0-182">400</span></span> | <span data-ttu-id="456a0-183">InvalidArguments</span><span class="sxs-lookup"><span data-stu-id="456a0-183">InvalidArguments</span></span> | <span data-ttu-id="456a0-184">O valor solicitada "RandomDay" não foi encontrado.</span><span class="sxs-lookup"><span data-stu-id="456a0-184">Requested value 'RandomDay' was not found.</span></span>|
| <span data-ttu-id="456a0-185">**timeZone** inválido</span><span class="sxs-lookup"><span data-stu-id="456a0-185">Invalid **timeZone**</span></span> | <span data-ttu-id="456a0-186">400</span><span class="sxs-lookup"><span data-stu-id="456a0-186">400</span></span> | <span data-ttu-id="456a0-187">InvalidTimeZone</span><span class="sxs-lookup"><span data-stu-id="456a0-187">InvalidTimeZone</span></span> | <span data-ttu-id="456a0-188">As configurações de Fuso Horário fornecidas são inválidas.</span><span class="sxs-lookup"><span data-stu-id="456a0-188">Time Zone settings provided are invalid.</span></span>|


## <a name="examples"></a><span data-ttu-id="456a0-189">Exemplos</span><span class="sxs-lookup"><span data-stu-id="456a0-189">Examples</span></span>
### <a name="example-1"></a><span data-ttu-id="456a0-190">Exemplo 1</span><span class="sxs-lookup"><span data-stu-id="456a0-190">Example 1</span></span>
#### <a name="request"></a><span data-ttu-id="456a0-191">Solicitação</span><span class="sxs-lookup"><span data-stu-id="456a0-191">Request</span></span> 
<span data-ttu-id="456a0-192">O primeiro exemplo habilita as respostas automáticas de um intervalo de datas, definindo as seguintes propriedades da propriedade **automaticRepliesSetting**: **status**, **scheduledStartDateTime** e **scheduledEndDateTime**.</span><span class="sxs-lookup"><span data-stu-id="456a0-192">The first example enables automatic replies for a date range, by setting the following properties of the **automaticRepliesSetting** property: **status**, **scheduledStartDateTime** and **scheduledEndDateTime**.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="456a0-193">HTTP</span><span class="sxs-lookup"><span data-stu-id="456a0-193">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_mailboxsettings_1"
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

#### <a name="response"></a><span data-ttu-id="456a0-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="456a0-194">Response</span></span>
<span data-ttu-id="456a0-195">A resposta inclui apenas as configurações atualizadas de respostas automáticas.</span><span class="sxs-lookup"><span data-stu-id="456a0-195">The response includes the updated settings for automatic replies.</span></span> <span data-ttu-id="456a0-196">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="456a0-196">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="456a0-197">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="456a0-197">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "update_mailboxsettings_1",
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

### <a name="example-2"></a><span data-ttu-id="456a0-198">Exemplo 2</span><span class="sxs-lookup"><span data-stu-id="456a0-198">Example 2</span></span>
#### <a name="request"></a><span data-ttu-id="456a0-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="456a0-199">Request</span></span>
<span data-ttu-id="456a0-200">O segundo exemplo personaliza o fuso horário das horas de trabalho do usuário conectado definindo a propriedade **timeZone** para um [fuso horário personalizado](../resources/customtimezone.md).</span><span class="sxs-lookup"><span data-stu-id="456a0-200">The second example customizes the time zone for the working hours of the signed-in user, by setting the **timeZone** property to a [custom time zone](../resources/customtimezone.md).</span></span>

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
#### <a name="response"></a><span data-ttu-id="456a0-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="456a0-201">Response</span></span>
<span data-ttu-id="456a0-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="456a0-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
