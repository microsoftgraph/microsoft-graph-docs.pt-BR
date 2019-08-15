---
title: Atualizar as configurações de caixa de correio do usuário
description: Atualize uma ou mais configurações da caixa de correio do usuário. Isso inclui as configurações para respostas automáticas (notificar as pessoas automaticamente no recebimento de seus emails), localidade (idioma e país/região), fuso horário e horário de trabalho.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fe39d03850c9e3d006827593cb4151c0cdac376b
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421796"
---
# <a name="update-user-mailbox-settings"></a><span data-ttu-id="de526-104">Atualizar as configurações de caixa de correio do usuário</span><span class="sxs-lookup"><span data-stu-id="de526-104">Update user mailbox settings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de526-p102">Atualize uma ou mais configurações da caixa de correio do usuário. Isso inclui configurações de [respostas automáticas](../resources/automaticrepliessetting.md) (notificar pessoas automaticamente ao receber emails), [localidade](../resources/localeinfo.md) (idioma e país/região), fuso horário e [horário de trabalho](../resources/workinghours.md).</span><span class="sxs-lookup"><span data-stu-id="de526-p102">Update one or more settings for the user's mailbox. This includes settings for [automatic replies](../resources/automaticrepliessetting.md) (notify people automatically upon receipt of their email), [locale](../resources/localeinfo.md) (language and country/region), time zone, and [working hours](../resources/workinghours.md).</span></span>

<span data-ttu-id="de526-107">Você pode habilitar, configurar ou desabilitar um ou mais destas configurações como parte de [mailboxSettings](../resources/mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="de526-107">You can enable, configure, or disable one or more of these settings as part of [mailboxSettings](../resources/mailboxsettings.md).</span></span>

<span data-ttu-id="de526-108">**Observação** você não pode criar nem excluir configurações da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="de526-108">**Note** You cannot create or delete any mailbox settings.</span></span>

<span data-ttu-id="de526-109">Ao atualizar o fuso horário preferencial de um usuário, você pode especificá-lo no formato do Windows ou da [Autoridade para Atribuição de Números na Internet (IANA)](https://www.iana.org/time-zones) (também conhecido como fuso horário de Olson).</span><span class="sxs-lookup"><span data-stu-id="de526-109">When you update the preferred time zone for a user, you can specify it in the Windows or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="de526-110">Você também pode personalizar ainda mais o fuso horário, conforme mostrado no [exemplo 2](#request-2) abaixo.</span><span class="sxs-lookup"><span data-stu-id="de526-110">You can also further customize the time zone as shown in [example 2](#request-2) below.</span></span>

## <a name="permissions"></a><span data-ttu-id="de526-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="de526-111">Permissions</span></span>
<span data-ttu-id="de526-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de526-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de526-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de526-114">Permission type</span></span>      | <span data-ttu-id="de526-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="de526-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="de526-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de526-116">Delegated (work or school account)</span></span> | <span data-ttu-id="de526-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de526-117">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="de526-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de526-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de526-119">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de526-119">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="de526-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="de526-120">Application</span></span> | <span data-ttu-id="de526-121">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de526-121">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="de526-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de526-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailboxSettings
PATCH /users/{id|userPrincipalName}/mailboxSettings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="de526-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="de526-123">Optional query parameters</span></span>
<span data-ttu-id="de526-124">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="de526-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="de526-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de526-125">Request headers</span></span>
| <span data-ttu-id="de526-126">Nome</span><span class="sxs-lookup"><span data-stu-id="de526-126">Name</span></span>       | <span data-ttu-id="de526-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="de526-127">Type</span></span> | <span data-ttu-id="de526-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="de526-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="de526-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="de526-129">Authorization</span></span>  | <span data-ttu-id="de526-130">string</span><span class="sxs-lookup"><span data-stu-id="de526-130">string</span></span>  | <span data-ttu-id="de526-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de526-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="de526-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de526-133">Request body</span></span>
<span data-ttu-id="de526-p106">No corpo da solicitação, forneça os valores para as propriedades relevantes que devem ser atualizadas. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade. Para obter o melhor desempenho, não inclua valores existentes que não foram alterados. Estas são as propriedades graváveis/atualizáveis:</span><span class="sxs-lookup"><span data-stu-id="de526-p106">In the request body, supply the values for the relevant properties that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. The following are the writable/updatable properties:</span></span>

| <span data-ttu-id="de526-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="de526-138">Property</span></span>     | <span data-ttu-id="de526-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="de526-139">Type</span></span>   |<span data-ttu-id="de526-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="de526-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de526-141">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="de526-141">automaticRepliesSetting</span></span>|[<span data-ttu-id="de526-142">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="de526-142">automaticRepliesSetting</span></span>](../resources/automaticrepliessetting.md)|<span data-ttu-id="de526-143">Definições de configuração para notificar automaticamente o remetente de um email recebido com uma mensagem do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="de526-143">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span> <span data-ttu-id="de526-144">Você pode definir essas notificações para apenas um intervalo de datas futuras.</span><span class="sxs-lookup"><span data-stu-id="de526-144">You can set such notifications for only a future date range.</span></span>|
|<span data-ttu-id="de526-145">idioma</span><span class="sxs-lookup"><span data-stu-id="de526-145">language</span></span>|[<span data-ttu-id="de526-146">localeInfo</span><span class="sxs-lookup"><span data-stu-id="de526-146">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="de526-147">Informações sobre a localidade do usuário, incluindo o idioma preferencial e o país/região.</span><span class="sxs-lookup"><span data-stu-id="de526-147">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="de526-148">timeZone</span><span class="sxs-lookup"><span data-stu-id="de526-148">timeZone</span></span>|<span data-ttu-id="de526-149">string</span><span class="sxs-lookup"><span data-stu-id="de526-149">string</span></span>|<span data-ttu-id="de526-150">O fuso horário padrão para a caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="de526-150">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="de526-151">workingHours</span><span class="sxs-lookup"><span data-stu-id="de526-151">workingHours</span></span>|[<span data-ttu-id="de526-152">workingHours</span><span class="sxs-lookup"><span data-stu-id="de526-152">workingHours</span></span>](../resources/workinghours.md)|<span data-ttu-id="de526-153">As horas, os dias de uma semana e o fuso horário em que o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="de526-153">The hours, days of a week, and time zone that the user works.</span></span>|

## <a name="response"></a><span data-ttu-id="de526-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="de526-154">Response</span></span>

<span data-ttu-id="de526-155">Se tiver êxito, este método retornará um código de resposta `200 OK` e o objeto [mailboxSettings](../resources/mailboxsettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de526-155">If successful, this method returns a `200 OK` response code and [mailboxSettings](../resources/mailboxsettings.md) object in the response body.</span></span>

## <a name="errors"></a><span data-ttu-id="de526-156">Erros</span><span class="sxs-lookup"><span data-stu-id="de526-156">Errors</span></span>

<span data-ttu-id="de526-157">Definir horas de trabalho com valores inadequados pode retornar os seguintes erros.</span><span class="sxs-lookup"><span data-stu-id="de526-157">Setting working hours with inappropriate values may return the following errors.</span></span>

| <span data-ttu-id="de526-158">Cenário</span><span class="sxs-lookup"><span data-stu-id="de526-158">Scenario</span></span>   | <span data-ttu-id="de526-159">Código de status de HTTP</span><span class="sxs-lookup"><span data-stu-id="de526-159">HTTP status code</span></span> | <span data-ttu-id="de526-160">Código de erro</span><span class="sxs-lookup"><span data-stu-id="de526-160">Error code</span></span> | <span data-ttu-id="de526-161">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="de526-161">Error message</span></span> |
|:-----------|:------|:----------|:----------|
| <span data-ttu-id="de526-162">**startTime** ou **endTime** inválido</span><span class="sxs-lookup"><span data-stu-id="de526-162">Invalid **startTime** or **endTime**</span></span> | <span data-ttu-id="de526-163">400</span><span class="sxs-lookup"><span data-stu-id="de526-163">400</span></span> | <span data-ttu-id="de526-164">RequestBodyRead</span><span class="sxs-lookup"><span data-stu-id="de526-164">RequestBodyRead</span></span> | <span data-ttu-id="de526-165">Não é possível converter o literal '08"para o tipo 'Edm.TimeOfDay' esperado.</span><span class="sxs-lookup"><span data-stu-id="de526-165">Cannot convert the literal '08' to the expected type 'Edm.TimeOfDay'.</span></span>|
| <span data-ttu-id="de526-166">A hora de início é maior do que a hora de término</span><span class="sxs-lookup"><span data-stu-id="de526-166">Start time is greater than end time</span></span> | <span data-ttu-id="de526-167">400</span><span class="sxs-lookup"><span data-stu-id="de526-167">400</span></span> | <span data-ttu-id="de526-168">ErrorInvalidTimeSettings</span><span class="sxs-lookup"><span data-stu-id="de526-168">ErrorInvalidTimeSettings</span></span> | <span data-ttu-id="de526-169">A Hora de Início deve ocorrer antes da Hora de Término.</span><span class="sxs-lookup"><span data-stu-id="de526-169">Start Time should occur before End Time.</span></span> |
| <span data-ttu-id="de526-170">Dia inválido em **daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="de526-170">Invalid day in **daysOfWeek**</span></span> | <span data-ttu-id="de526-171">400</span><span class="sxs-lookup"><span data-stu-id="de526-171">400</span></span> | <span data-ttu-id="de526-172">InvalidArguments</span><span class="sxs-lookup"><span data-stu-id="de526-172">InvalidArguments</span></span> | <span data-ttu-id="de526-173">O valor solicitada "RandomDay" não foi encontrado.</span><span class="sxs-lookup"><span data-stu-id="de526-173">Requested value 'RandomDay' was not found.</span></span>|
| <span data-ttu-id="de526-174">**timeZone** inválido</span><span class="sxs-lookup"><span data-stu-id="de526-174">Invalid **timeZone**</span></span> | <span data-ttu-id="de526-175">400</span><span class="sxs-lookup"><span data-stu-id="de526-175">400</span></span> | <span data-ttu-id="de526-176">InvalidTimeZone</span><span class="sxs-lookup"><span data-stu-id="de526-176">InvalidTimeZone</span></span> | <span data-ttu-id="de526-177">As configurações de Fuso Horário fornecidas são inválidas.</span><span class="sxs-lookup"><span data-stu-id="de526-177">Time Zone settings provided are invalid.</span></span>|


## <a name="example"></a><span data-ttu-id="de526-178">Exemplo</span><span class="sxs-lookup"><span data-stu-id="de526-178">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="de526-179">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="de526-179">Request 1</span></span>
<span data-ttu-id="de526-180">O primeiro exemplo habilita as respostas automáticas de um intervalo de datas, definindo as seguintes propriedades da propriedade **automaticRepliesSetting**: **status**, **scheduledStartDateTime** e **scheduledEndDateTime**.</span><span class="sxs-lookup"><span data-stu-id="de526-180">The first example enables automatic replies for a date range, by setting the following properties of the **automaticRepliesSetting** property: **status**, **scheduledStartDateTime** and **scheduledEndDateTime**.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="de526-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="de526-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_mailboxsettings_1"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailboxSettings
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/mailboxSettings",
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="de526-182">C#</span><span class="sxs-lookup"><span data-stu-id="de526-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-mailboxsettings-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="de526-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="de526-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-mailboxsettings-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="de526-184">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="de526-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-mailboxsettings-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response-1"></a><span data-ttu-id="de526-185">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="de526-185">Response 1</span></span>
<span data-ttu-id="de526-186">A resposta inclui apenas as configurações atualizadas de respostas automáticas.</span><span class="sxs-lookup"><span data-stu-id="de526-186">The response includes the updated settings for automatic replies.</span></span> <span data-ttu-id="de526-187">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="de526-187">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="de526-188">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="de526-188">All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/mailboxSettings",
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


##### <a name="request-2"></a><span data-ttu-id="de526-189">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="de526-189">Request 2</span></span>
<span data-ttu-id="de526-190">O segundo exemplo personaliza o fuso horário das horas de trabalho do usuário conectado definindo a propriedade **timeZone** para um [fuso horário personalizado](../resources/customtimezone.md).</span><span class="sxs-lookup"><span data-stu-id="de526-190">The second example customizes the time zone for the working hours of the signed-in user, by setting the **timeZone** property to a [custom time zone](../resources/customtimezone.md).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "update_mailboxsettings_2"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailboxSettings
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
##### <a name="response-2"></a><span data-ttu-id="de526-191">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="de526-191">Response 2</span></span>
<span data-ttu-id="de526-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="de526-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('94447c6e-ea4c-494c-a9ed-d905e366c5cb')/mailboxSettings",
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
<!--
{
  "type": "#page.annotation",
  "description": "Update mailbox settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
