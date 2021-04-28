---
title: Atualizar as configurações de caixa de correio do usuário
description: Atualize uma ou mais configurações da caixa de correio do usuário. Isso inclui configurações de respostas automáticas (notificar pessoas automaticamente ao receber emails), localidade (idioma e país/região), fuso horário e horário de trabalho.
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f703560c561360379df793cc36582b3f141e48d8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050203"
---
# <a name="update-user-mailbox-settings"></a><span data-ttu-id="80420-104">Atualizar as configurações de caixa de correio do usuário</span><span class="sxs-lookup"><span data-stu-id="80420-104">Update user mailbox settings</span></span>

<span data-ttu-id="80420-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80420-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="80420-106">Habilitar, configurar ou desabilitar uma ou mais das seguintes configurações como parte das caixas de correio de um [usuárioConfigurações](../resources/mailboxsettings.md):</span><span class="sxs-lookup"><span data-stu-id="80420-106">Enable, configure, or disable one or more of the following settings as part of a user's [mailboxSettings](../resources/mailboxsettings.md):</span></span>

- <span data-ttu-id="80420-107">[respostas automáticas](../resources/automaticrepliessetting.md) (notificar pessoas automaticamente ao receber seus emails)</span><span class="sxs-lookup"><span data-stu-id="80420-107">[automatic replies](../resources/automaticrepliessetting.md) (notify people automatically upon receipt of their email)</span></span>
- <span data-ttu-id="80420-108">dateFormat</span><span class="sxs-lookup"><span data-stu-id="80420-108">dateFormat</span></span>
- <span data-ttu-id="80420-109">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="80420-109">delegateMeetingMessageDeliveryOptions</span></span>
- <span data-ttu-id="80420-110">[localidade](../resources/localeinfo.md) (idioma e país/região)</span><span class="sxs-lookup"><span data-stu-id="80420-110">[locale](../resources/localeinfo.md) (language and country/region)</span></span>
- <span data-ttu-id="80420-111">timeFormat</span><span class="sxs-lookup"><span data-stu-id="80420-111">timeFormat</span></span>
- <span data-ttu-id="80420-112">fuso horário</span><span class="sxs-lookup"><span data-stu-id="80420-112">time zone</span></span>
- [<span data-ttu-id="80420-113">horário de trabalho</span><span class="sxs-lookup"><span data-stu-id="80420-113">working hours</span></span>](../resources/workinghours.md)

<span data-ttu-id="80420-114">Ao atualizar o formato de data ou hora preferencial para um usuário, especifique-o, respectivamente, no formato de [data curta](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortDate) ou [de curto](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortTime) período.</span><span class="sxs-lookup"><span data-stu-id="80420-114">When updating the preferred date or time format for a user, specify it in respectively, the [short date](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortDate) or [short time](/dotnet/standard/base-types/standard-date-and-time-format-strings#ShortTime) format.</span></span>

<span data-ttu-id="80420-115">Ao atualizar o fuso horário preferencial para um usuário, especifique-o no formato de fuso horário Windows internet [ou IANA (também](https://www.iana.org/time-zones) conhecido como fuso horário Olson).</span><span class="sxs-lookup"><span data-stu-id="80420-115">When updating the preferred time zone for a user, specify it in the Windows or [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="80420-116">Você também pode personalizar ainda mais o fuso horário, conforme mostrado no [exemplo 2](#example-2) abaixo.</span><span class="sxs-lookup"><span data-stu-id="80420-116">You can also further customize the time zone as shown in [example 2](#example-2) below.</span></span>

> [!TIP]
> <span data-ttu-id="80420-117">Não é possível criar ou excluir configurações de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="80420-117">You cannot create or delete any mailbox settings.</span></span>

## <a name="permissions"></a><span data-ttu-id="80420-118">Permissões</span><span class="sxs-lookup"><span data-stu-id="80420-118">Permissions</span></span>
<span data-ttu-id="80420-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80420-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80420-121">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="80420-121">Permission type</span></span>      | <span data-ttu-id="80420-122">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="80420-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80420-123">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="80420-123">Delegated (work or school account)</span></span> | <span data-ttu-id="80420-124">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="80420-124">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="80420-125">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="80420-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80420-126">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="80420-126">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="80420-127">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="80420-127">Application</span></span> | <span data-ttu-id="80420-128">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="80420-128">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="80420-129">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="80420-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailboxSettings
PATCH /users/{id|userPrincipalName}/mailboxSettings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="80420-130">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="80420-130">Optional query parameters</span></span>
<span data-ttu-id="80420-131">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="80420-131">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="80420-132">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="80420-132">Request headers</span></span>
| <span data-ttu-id="80420-133">Nome</span><span class="sxs-lookup"><span data-stu-id="80420-133">Name</span></span>       | <span data-ttu-id="80420-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="80420-134">Type</span></span> | <span data-ttu-id="80420-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="80420-135">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="80420-136">Autorização</span><span class="sxs-lookup"><span data-stu-id="80420-136">Authorization</span></span>  | <span data-ttu-id="80420-137">string</span><span class="sxs-lookup"><span data-stu-id="80420-137">string</span></span>  | <span data-ttu-id="80420-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="80420-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="80420-140">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="80420-140">Request body</span></span>
<span data-ttu-id="80420-p105">No corpo da solicitação, forneça os valores para as propriedades relevantes que devem ser atualizadas. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações em outros valores de propriedade. Para obter o melhor desempenho, não inclua valores existentes que não foram alterados. Estas são as propriedades graváveis/atualizáveis:</span><span class="sxs-lookup"><span data-stu-id="80420-p105">In the request body, supply the values for the relevant properties that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed. The following are the writable/updatable properties:</span></span>

| <span data-ttu-id="80420-145">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80420-145">Property</span></span>     | <span data-ttu-id="80420-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="80420-146">Type</span></span>   |<span data-ttu-id="80420-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="80420-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="80420-148">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="80420-148">automaticRepliesSetting</span></span>|[<span data-ttu-id="80420-149">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="80420-149">automaticRepliesSetting</span></span>](../resources/automaticrepliessetting.md)|<span data-ttu-id="80420-150">Definições de configuração para notificar automaticamente o remetente de um email recebido com uma mensagem do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="80420-150">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span> <span data-ttu-id="80420-151">Você pode definir essas notificações apenas para um intervalo de datas futuro.</span><span class="sxs-lookup"><span data-stu-id="80420-151">You can set such notifications for only a future date range.</span></span>|
|<span data-ttu-id="80420-152">dateFormat</span><span class="sxs-lookup"><span data-stu-id="80420-152">dateFormat</span></span>|<span data-ttu-id="80420-153">string</span><span class="sxs-lookup"><span data-stu-id="80420-153">string</span></span>|<span data-ttu-id="80420-154">O formato de data para a caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="80420-154">The date format for the user's mailbox.</span></span>|
|<span data-ttu-id="80420-155">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="80420-155">delegateMeetingMessageDeliveryOptions</span></span>|<span data-ttu-id="80420-156">delegateMeetingMessageDeliveryOptions</span><span class="sxs-lookup"><span data-stu-id="80420-156">delegateMeetingMessageDeliveryOptions</span></span>| <span data-ttu-id="80420-157">Se o usuário tiver um representante de calendário, isso especifica se o representante, o proprietário da caixa de correio ou ambos recebem mensagens de reunião e respostas de reunião.</span><span class="sxs-lookup"><span data-stu-id="80420-157">If the user has a calendar delegate, this specifies whether the delegate, mailbox owner, or both receive meeting messages and meeting responses.</span></span> <span data-ttu-id="80420-158">Os valores possíveis são: `sendToDelegateAndInformationToPrincipal`, `sendToDelegateAndPrincipal`, `sendToDelegateOnly`.</span><span class="sxs-lookup"><span data-stu-id="80420-158">Possible values are: `sendToDelegateAndInformationToPrincipal`, `sendToDelegateAndPrincipal`, `sendToDelegateOnly`.</span></span>|
|<span data-ttu-id="80420-159">idioma</span><span class="sxs-lookup"><span data-stu-id="80420-159">language</span></span>|[<span data-ttu-id="80420-160">localeInfo</span><span class="sxs-lookup"><span data-stu-id="80420-160">localeInfo</span></span>](../resources/localeinfo.md)|<span data-ttu-id="80420-161">Informações sobre a localidade do usuário, incluindo o idioma preferencial e o país/região.</span><span class="sxs-lookup"><span data-stu-id="80420-161">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="80420-162">timeFormat</span><span class="sxs-lookup"><span data-stu-id="80420-162">timeFormat</span></span>|<span data-ttu-id="80420-163">string</span><span class="sxs-lookup"><span data-stu-id="80420-163">string</span></span>|<span data-ttu-id="80420-164">O formato de hora da caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="80420-164">The time format for the user's mailbox.</span></span>|
|<span data-ttu-id="80420-165">timeZone</span><span class="sxs-lookup"><span data-stu-id="80420-165">timeZone</span></span>|<span data-ttu-id="80420-166">string</span><span class="sxs-lookup"><span data-stu-id="80420-166">string</span></span>|<span data-ttu-id="80420-167">O fuso horário padrão para a caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="80420-167">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="80420-168">workingHours</span><span class="sxs-lookup"><span data-stu-id="80420-168">workingHours</span></span>|[<span data-ttu-id="80420-169">workingHours</span><span class="sxs-lookup"><span data-stu-id="80420-169">workingHours</span></span>](../resources/workinghours.md)|<span data-ttu-id="80420-170">As horas, os dias de uma semana e o fuso horário em que o usuário trabalha.</span><span class="sxs-lookup"><span data-stu-id="80420-170">The hours, days of a week, and time zone that the user works.</span></span>|

## <a name="response"></a><span data-ttu-id="80420-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="80420-171">Response</span></span>

<span data-ttu-id="80420-172">Se tiver êxito, este método retornará um código de resposta e as propriedades `200 OK` atualizadas de um [objeto mailboxSettings](../resources/mailboxsettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="80420-172">If successful, this method returns a `200 OK` response code and the updated properties of a [mailboxSettings](../resources/mailboxsettings.md) object in the response body.</span></span>

## <a name="errors"></a><span data-ttu-id="80420-173">Erros</span><span class="sxs-lookup"><span data-stu-id="80420-173">Errors</span></span>

<span data-ttu-id="80420-174">Definir horas de trabalho com valores inadequados pode retornar os seguintes erros.</span><span class="sxs-lookup"><span data-stu-id="80420-174">Setting working hours with inappropriate values may return the following errors.</span></span>

| <span data-ttu-id="80420-175">Cenário</span><span class="sxs-lookup"><span data-stu-id="80420-175">Scenario</span></span>   | <span data-ttu-id="80420-176">Código de status de HTTP</span><span class="sxs-lookup"><span data-stu-id="80420-176">HTTP status code</span></span> | <span data-ttu-id="80420-177">Código de erro</span><span class="sxs-lookup"><span data-stu-id="80420-177">Error code</span></span> | <span data-ttu-id="80420-178">Mensagem de erro</span><span class="sxs-lookup"><span data-stu-id="80420-178">Error message</span></span> |
|:-----------|:------|:----------|:----------|
| <span data-ttu-id="80420-179">**startTime** ou **endTime** inválido</span><span class="sxs-lookup"><span data-stu-id="80420-179">Invalid **startTime** or **endTime**</span></span> | <span data-ttu-id="80420-180">400</span><span class="sxs-lookup"><span data-stu-id="80420-180">400</span></span> | <span data-ttu-id="80420-181">RequestBodyRead</span><span class="sxs-lookup"><span data-stu-id="80420-181">RequestBodyRead</span></span> | <span data-ttu-id="80420-182">Não é possível converter o literal '08"para o tipo 'Edm.TimeOfDay' esperado.</span><span class="sxs-lookup"><span data-stu-id="80420-182">Cannot convert the literal '08' to the expected type 'Edm.TimeOfDay'.</span></span>|
| <span data-ttu-id="80420-183">A hora de início é maior do que a hora de término</span><span class="sxs-lookup"><span data-stu-id="80420-183">Start time is greater than end time</span></span> | <span data-ttu-id="80420-184">400</span><span class="sxs-lookup"><span data-stu-id="80420-184">400</span></span> | <span data-ttu-id="80420-185">ErrorInvalidTimeSettings</span><span class="sxs-lookup"><span data-stu-id="80420-185">ErrorInvalidTimeSettings</span></span> | <span data-ttu-id="80420-186">A Hora de Início deve ocorrer antes da Hora de Término.</span><span class="sxs-lookup"><span data-stu-id="80420-186">Start Time should occur before End Time.</span></span> |
| <span data-ttu-id="80420-187">Dia inválido em **daysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="80420-187">Invalid day in **daysOfWeek**</span></span> | <span data-ttu-id="80420-188">400</span><span class="sxs-lookup"><span data-stu-id="80420-188">400</span></span> | <span data-ttu-id="80420-189">InvalidArguments</span><span class="sxs-lookup"><span data-stu-id="80420-189">InvalidArguments</span></span> | <span data-ttu-id="80420-190">O valor solicitada "RandomDay" não foi encontrado.</span><span class="sxs-lookup"><span data-stu-id="80420-190">Requested value 'RandomDay' was not found.</span></span>|
| <span data-ttu-id="80420-191">**timeZone** inválido</span><span class="sxs-lookup"><span data-stu-id="80420-191">Invalid **timeZone**</span></span> | <span data-ttu-id="80420-192">400</span><span class="sxs-lookup"><span data-stu-id="80420-192">400</span></span> | <span data-ttu-id="80420-193">InvalidTimeZone</span><span class="sxs-lookup"><span data-stu-id="80420-193">InvalidTimeZone</span></span> | <span data-ttu-id="80420-194">As configurações de Fuso Horário fornecidas são inválidas.</span><span class="sxs-lookup"><span data-stu-id="80420-194">Time Zone settings provided are invalid.</span></span>|


## <a name="examples"></a><span data-ttu-id="80420-195">Exemplos</span><span class="sxs-lookup"><span data-stu-id="80420-195">Examples</span></span>
### <a name="example-1"></a><span data-ttu-id="80420-196">Exemplo 1</span><span class="sxs-lookup"><span data-stu-id="80420-196">Example 1</span></span>
#### <a name="request"></a><span data-ttu-id="80420-197">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80420-197">Request</span></span>
<span data-ttu-id="80420-198">O primeiro exemplo habilita as respostas automáticas de um intervalo de datas, definindo as seguintes propriedades da propriedade **automaticRepliesSetting**: **status**, **scheduledStartDateTime** e **scheduledEndDateTime**.</span><span class="sxs-lookup"><span data-stu-id="80420-198">The first example enables automatic replies for a date range, by setting the following properties of the **automaticRepliesSetting** property: **status**, **scheduledStartDateTime** and **scheduledEndDateTime**.</span></span>


# <a name="http"></a>[<span data-ttu-id="80420-199">HTTP</span><span class="sxs-lookup"><span data-stu-id="80420-199">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="80420-200">C#</span><span class="sxs-lookup"><span data-stu-id="80420-200">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-mailboxsettings-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="80420-201">JavaScript</span><span class="sxs-lookup"><span data-stu-id="80420-201">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-mailboxsettings-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="80420-202">Objective-C</span><span class="sxs-lookup"><span data-stu-id="80420-202">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-mailboxsettings-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="80420-203">Java</span><span class="sxs-lookup"><span data-stu-id="80420-203">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-mailboxsettings-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="80420-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="80420-204">Response</span></span>
<span data-ttu-id="80420-205">A resposta inclui apenas as configurações atualizadas de respostas automáticas.</span><span class="sxs-lookup"><span data-stu-id="80420-205">The response includes the updated settings for automatic replies.</span></span> <span data-ttu-id="80420-206">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="80420-206">Note: The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2"></a><span data-ttu-id="80420-207">Exemplo 2</span><span class="sxs-lookup"><span data-stu-id="80420-207">Example 2</span></span>
#### <a name="request"></a><span data-ttu-id="80420-208">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80420-208">Request</span></span>
<span data-ttu-id="80420-209">O segundo exemplo personaliza o fuso horário das horas de trabalho do usuário conectado definindo a propriedade **timeZone** para um [fuso horário personalizado](../resources/customtimezone.md).</span><span class="sxs-lookup"><span data-stu-id="80420-209">The second example customizes the time zone for the working hours of the signed-in user, by setting the **timeZone** property to a [custom time zone](../resources/customtimezone.md).</span></span>


# <a name="http"></a>[<span data-ttu-id="80420-210">HTTP</span><span class="sxs-lookup"><span data-stu-id="80420-210">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
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
# <a name="c"></a>[<span data-ttu-id="80420-211">C#</span><span class="sxs-lookup"><span data-stu-id="80420-211">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-mailboxsettings-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="80420-212">JavaScript</span><span class="sxs-lookup"><span data-stu-id="80420-212">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-mailboxsettings-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="80420-213">Objective-C</span><span class="sxs-lookup"><span data-stu-id="80420-213">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-mailboxsettings-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="80420-214">Java</span><span class="sxs-lookup"><span data-stu-id="80420-214">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-mailboxsettings-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="80420-215">Resposta</span><span class="sxs-lookup"><span data-stu-id="80420-215">Response</span></span>
<span data-ttu-id="80420-216">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="80420-216">Here is an example of the response.</span></span> <span data-ttu-id="80420-217">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="80420-217">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
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
