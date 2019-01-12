---
title: Obter as configurações da caixa de correio do usuário
description: 'Obtenha mailboxSettings do usuário. Isso inclui configurações para respostas automáticas (notificar as pessoas automaticamente ao '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9623aa2d02b83609088360779c6b40dcc7f98556
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991836"
---
# <a name="get-user-mailbox-settings"></a><span data-ttu-id="a141c-104">Obter as configurações da caixa de correio do usuário</span><span class="sxs-lookup"><span data-stu-id="a141c-104">Get user mailbox settings</span></span>

> <span data-ttu-id="a141c-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a141c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a141c-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a141c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a141c-107">Obtenha do usuário [mailboxSettings](../resources/mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="a141c-107">Get the user's [mailboxSettings](../resources/mailboxsettings.md).</span></span> <span data-ttu-id="a141c-108">Isso inclui configurações para respostas automáticas (notificar as pessoas automaticamente após o recebimento de seus emails), (país/região e idioma) de localidade, fuso horário e horário de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a141c-108">This includes settings for automatic replies (notify people automatically upon receipt of their email), locale (language and country/region), time zone, and working hours.</span></span>

<span data-ttu-id="a141c-109">Você pode exibir todas as configurações de caixa de correio ou obter configurações específicas.</span><span class="sxs-lookup"><span data-stu-id="a141c-109">You can view all mailbox settings, or, get specific settings.</span></span>

<span data-ttu-id="a141c-110">O fuso horário é uma das configurações de preferência que um usuário pode fazer na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="a141c-110">Time zone is one of the preferred settings a user can set up for the user's mailbox.</span></span> <span data-ttu-id="a141c-111">O usuário escolhe-lo de que o [suporte para fusos horários](outlookuser-supportedtimezones.md) que um administrador tiver configurado para o servidor de caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="a141c-111">The user chooses it from the [supported time zones](outlookuser-supportedtimezones.md) that an administrator has set up for the user's mailbox server.</span></span> <span data-ttu-id="a141c-112">O administrador configura fusos horários no formato de fuso horário do Windows ou o [fuso horário de autoridade de números atribuídos da Internet (IANA)](https://www.iana.org/time-zones) (também conhecido como fuso horário Olson).</span><span class="sxs-lookup"><span data-stu-id="a141c-112">The administrator sets up time zones in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="a141c-113">O formato do Windows é o padrão.</span><span class="sxs-lookup"><span data-stu-id="a141c-113">The Windows format is the default.</span></span> 

<span data-ttu-id="a141c-114">Ao obter o fuso horário de preferência de um usuário, ele é retornado no formato em que foi configurado.</span><span class="sxs-lookup"><span data-stu-id="a141c-114">When you get a user's preferred time zone, the time zone is returned in the format that it was set up.</span></span> <span data-ttu-id="a141c-115">Se quiser que o fuso horário esteja em um formato específico (Windows ou IANA), você pode primeiro [atualizar o fuso horário de preferência nesse formato como uma configuração de caixa de correio](user-update-mailboxsettings.md).</span><span class="sxs-lookup"><span data-stu-id="a141c-115">If you want that time zone to be in a specific format (Windows or IANA), you can first [update the preferred time zone in that format as a mailbox setting](user-update-mailboxsettings.md).</span></span> <span data-ttu-id="a141c-116">Posteriormente, você poderá obter o fuso horário nesse formato.</span><span class="sxs-lookup"><span data-stu-id="a141c-116">Subsequently you will be able to get the time zone in that format.</span></span> <span data-ttu-id="a141c-117">Como alternativa, você pode gerenciar a conversão de formato separadamente no seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a141c-117">Alternatively, you can manage the format conversion separately in your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="a141c-118">Permissões</span><span class="sxs-lookup"><span data-stu-id="a141c-118">Permissions</span></span>
<span data-ttu-id="a141c-p106">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a141c-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a141c-121">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a141c-121">Permission type</span></span>      | <span data-ttu-id="a141c-122">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a141c-122">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a141c-123">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a141c-123">Delegated (work or school account)</span></span> | <span data-ttu-id="a141c-124">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a141c-124">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="a141c-125">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a141c-125">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a141c-126">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a141c-126">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="a141c-127">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a141c-127">Application</span></span> | <span data-ttu-id="a141c-128">MailboxSettings.Read, MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a141c-128">MailboxSettings.Read, MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a141c-129">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a141c-129">HTTP request</span></span>
<span data-ttu-id="a141c-130">Para obter todas as definições de caixa de correio de um usuário:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="a141c-130">To get all the mailbox settings for a user: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailboxSettings
GET /users/{id|userPrincipalName}/mailboxSettings
```

<span data-ttu-id="a141c-131">Para obter configurações específicas - apenas as configurações de respostas automáticas, localidade, fuso horário ou horário de trabalho:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="a141c-131">To get specific settings - only the automatic replies settings, locale, time zone, or working hours: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me/mailboxSettings/automaticRepliesSetting
GET /users/{id|userPrincipalName}/mailboxSettings/automaticRepliesSetting

GET /me/mailboxSettings/language
GET /users/{id|userPrincipalName}/mailboxSettings/language

GET /me/mailboxSettings/timeZone
GET /users/{id|userPrincipalName}/mailboxSettings/timeZone

GET /me/mailboxSettings/workingHours
GET /users/{id|userPrincipalName}/mailboxSettings/workingHours
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a141c-132">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a141c-132">Optional query parameters</span></span>
<span data-ttu-id="a141c-133">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a141c-133">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="a141c-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a141c-134">Request headers</span></span>
| <span data-ttu-id="a141c-135">Nome</span><span class="sxs-lookup"><span data-stu-id="a141c-135">Name</span></span>       | <span data-ttu-id="a141c-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="a141c-136">Type</span></span> | <span data-ttu-id="a141c-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="a141c-137">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a141c-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="a141c-138">Authorization</span></span>  | <span data-ttu-id="a141c-139">string</span><span class="sxs-lookup"><span data-stu-id="a141c-139">string</span></span>  | <span data-ttu-id="a141c-p107">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a141c-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a141c-142">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a141c-142">Request body</span></span>
<span data-ttu-id="a141c-143">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a141c-143">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a141c-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="a141c-144">Response</span></span>

<span data-ttu-id="a141c-145">Se for bem-sucedido, este método retornará um código de resposta `200 OK` e um dos seguintes objetos solicitados no corpo da resposta:</span><span class="sxs-lookup"><span data-stu-id="a141c-145">If successful, this method returns a `200 OK` response code and one of the following requested objects in the response body:</span></span>

- <span data-ttu-id="a141c-146">Objeto [mailboxSettings](../resources/mailboxsettings.md)</span><span class="sxs-lookup"><span data-stu-id="a141c-146">[mailboxSettings](../resources/mailboxsettings.md) object</span></span>
- <span data-ttu-id="a141c-147">Objeto [automaticRepliesSetting](../resources/automaticrepliessetting.md)</span><span class="sxs-lookup"><span data-stu-id="a141c-147">[automaticRepliesSetting](../resources/automaticrepliessetting.md) object</span></span>
- <span data-ttu-id="a141c-148">Objeto [localeInfo](../resources/localeinfo.md)</span><span class="sxs-lookup"><span data-stu-id="a141c-148">[localeInfo](../resources/localeinfo.md) object</span></span>
- <span data-ttu-id="a141c-149">cadeia de caracteres (para **timeZone**)</span><span class="sxs-lookup"><span data-stu-id="a141c-149">string (for **timeZone**)</span></span>
- [<span data-ttu-id="a141c-150">workingHours</span><span class="sxs-lookup"><span data-stu-id="a141c-150">workingHours</span></span>](../resources/workinghours.md)

## <a name="example"></a><span data-ttu-id="a141c-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a141c-151">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="a141c-152">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="a141c-152">Request 1</span></span>
<span data-ttu-id="a141c-153">O primeiro exemplo obtém todas as configurações da caixa de correio do usuário conectado, que incluem configurações de fuso horário, respostas automáticas, localidade (idioma e país/região) e horário de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a141c-153">The first example gets all the mailbox settings of the signed-in user's mailbox, which include settings for time zone, automatic replies, locale (language and country/region), and working hours.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_1"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings
```
##### <a name="response-1"></a><span data-ttu-id="a141c-154">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="a141c-154">Response 1</span></span>
<span data-ttu-id="a141c-155">A resposta inclui todas as configurações de caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="a141c-155">The response includes all the mailbox settings of the signed-in user.</span></span> <span data-ttu-id="a141c-156">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="a141c-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a141c-157">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a141c-157">All of the properties will be returned from an actual call.</span></span>
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
    }
}
```

##### <a name="request-2"></a><span data-ttu-id="a141c-158">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="a141c-158">Request 2</span></span>
<span data-ttu-id="a141c-159">O segundo exemplo obtém especificamente as configurações de respostas automáticas da caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="a141c-159">The second example gets specifically the automatic replies settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_2"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings/automaticRepliesSetting
```
##### <a name="response-2"></a><span data-ttu-id="a141c-160">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="a141c-160">Response 2</span></span>
<span data-ttu-id="a141c-p109">A resposta inclui apenas as configurações de respostas automáticas. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a141c-p109">The response includes only the automatic replies settings. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


##### <a name="request-3"></a><span data-ttu-id="a141c-164">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="a141c-164">Request 3</span></span>
<span data-ttu-id="a141c-165">O terceiro exemplo obtém especificamente as configurações de horário de trabalho da caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="a141c-165">The third example gets specifically the working hour settings of the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_mailboxsettings_3"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailboxSettings/workingHours
```
##### <a name="response-3"></a><span data-ttu-id="a141c-166">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="a141c-166">Response 3</span></span>
<span data-ttu-id="a141c-167">A resposta inclui apenas as configurações de horário de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a141c-167">The response includes only the working hours settings.</span></span> <span data-ttu-id="a141c-168">As horas de trabalho do usuário estão em um [fuso horário personalizado](../resources/customtimezone.md).</span><span class="sxs-lookup"><span data-stu-id="a141c-168">Notice that the user's work hours are in a [custom time zone](../resources/customtimezone.md).</span></span> <span data-ttu-id="a141c-169">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="a141c-169">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a141c-170">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a141c-170">All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get mailbox settings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
