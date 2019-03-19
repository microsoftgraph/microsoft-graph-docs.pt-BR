---
title: Obtenha a agenda de horários livres/ocupados de usuários e recursos (visualização)
description: Em uma configuração de escola ou trabalho, um cenário comum é ver quando um usuário está livre para um reunião, ou então pesquisar a disponibilidade de uma equipe, sala ou equipamento para um período de tempo.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: b2ed37055beb344c254e6715777b430baeceebf5
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657383"
---
# <a name="get-freebusy-schedule-of-users-and-resources-preview"></a><span data-ttu-id="5b950-103">Obtenha a agenda de horários livres/ocupados de usuários e recursos (visualização)</span><span class="sxs-lookup"><span data-stu-id="5b950-103">Get free/busy schedule of users and resources (preview)</span></span>

<span data-ttu-id="5b950-104">Em uma configuração de escola ou trabalho, um cenário comum é ver quando um usuário está livre para um reunião, ou então pesquisar a disponibilidade de uma equipe, sala ou equipamento para um período de tempo.</span><span class="sxs-lookup"><span data-stu-id="5b950-104">In a work or school setting, a common scenario is to see when a user is free for meeting, or to browse the availability of a team, room, or equipment for a time period.</span></span>

<span data-ttu-id="5b950-105">A ação [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-beta) permite que você obtenha as informações de disponibilidade de uma ou mais entidades (usuários, listas de distribuição ou recursos) para um período específico de tempo.</span><span class="sxs-lookup"><span data-stu-id="5b950-105">The [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-beta) action lets you get the availability information of one or more entities - users, distribution lists, or resources - for a specific period of time.</span></span> 

## <a name="example"></a><span data-ttu-id="5b950-106">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5b950-106">Example</span></span>

<span data-ttu-id="5b950-107">Um exemplo simples é encontrar a agenda de horários livres/ocupados de um colega de trabalho, Alex, em um dia específico, das 9 às 18 horas, Fuso Horário Padrão do Pacífico (PST):</span><span class="sxs-lookup"><span data-stu-id="5b950-107">A simple example is to find the free/busy schedule of a coworker, Alex, on a specific day, from 9am to 6pm, Pacitfic Standard Time:</span></span>

<!-- {
  "blockType": "ignored",
  "name": "calendar_getSchedule_concept"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendar/getschedule 
Prefer: outlook.timezone="Pacific Standard Time"
Content-Type: application/json

{        
    "Schedules": ["AlexW@contoso.OnMicrosoft.com"],
    "StartTime": {
        "dateTime": "2018-08-06T09:00:00",
        "timeZone": "Pacific Standard Time"
    },
    "EndTime": {
        "dateTime": "2018-08-06T18:00:00",
        "timeZone": "Pacific Standard Time"
    },
    "availabilityViewInterval": "15"
}
```

<span data-ttu-id="5b950-108">**getSchedule** retorna dois itens de agenda que correspondem aos eventos existentes no calendário padrão do Alex, mostrando os horários de início e término de cada evento e seu status de disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="5b950-108">**getSchedule** returns two schedule items that match existing events in Alex' default calendar, showing the start and end times of each event and its free/busy status.</span></span> <span data-ttu-id="5b950-109">Você poderá supor que Alex está livre pelo restante do tempo desse intervalo de data/hora.</span><span class="sxs-lookup"><span data-stu-id="5b950-109">You can assume Alex is free for the remaining time in that date/time range.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.scheduleInformation",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.scheduleInformation)",
    "value":[
        {
            "scheduleId":"AlexW@contoso.OnMicrosoft.com",
            "availabilityView":"111111002222222200000000000000000000",
            "scheduleItems":[
                {
                    "isPrivate":false,
                    "status":"Tentative",
                    "start":{
                        "dateTime":"2018-08-06T09:00:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    },
                    "end":{
                        "dateTime":"2018-08-06T10:30:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    }
                },
                {
                    "isPrivate":false,
                    "status":"Busy",
                    "start":{
                        "dateTime":"2018-08-06T11:00:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    },
                    "end":{
                        "dateTime":"2018-08-06T13:00:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    }
                }
            ],
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
                    "@odata.type":"#microsoft.graph.customTimeZone",
                    "bias":480,
                    "name":"Customized Time Zone",
                    "standardOffset":{
                        "time":"02:00:00.0000000",
                        "dayOccurrence":1,
                        "dayOfWeek":"sunday",
                        "month":11,
                        "year":0
                    },
                    "daylightOffset":{
                        "daylightBias":-60,
                        "time":"02:00:00.0000000",
                        "dayOccurrence":2,
                        "dayOfWeek":"sunday",
                        "month":3,
                        "year":0
                    }
                }
            }
        }
    ]
}

```

<span data-ttu-id="5b950-110">Além da disponibilidade da agenda e das horas de trabalho do Alex, **getSchedule** também retorna **availabilityView**, que é uma visualização mesclada da disponibilidade do Alex a cada dia.</span><span class="sxs-lookup"><span data-stu-id="5b950-110">Apart from the free/busy schedule and working hours of Alex, **getSchedule** also returns **availabilityView**, which is a merged view of Alex' availability for that day.</span></span> <span data-ttu-id="5b950-111">O modo de exibição mesclado é uma cadeia de caracteres que consiste em intervalos de tempo abrangendo aquele dia, sendo que cada intervalo de tempo indica a disponibilidade do Alex usando a seguinte convenção:</span><span class="sxs-lookup"><span data-stu-id="5b950-111">The merged view is a string that consists of time slots covering that day, with each time slot indicating Alex' availability using the following convention:</span></span> 

- <span data-ttu-id="5b950-112">`0` = livre</span><span class="sxs-lookup"><span data-stu-id="5b950-112">`0`= free</span></span>
- <span data-ttu-id="5b950-113">`1` = provisório</span><span class="sxs-lookup"><span data-stu-id="5b950-113">`1`= tentative</span></span>
- <span data-ttu-id="5b950-114">`2` = ocupado</span><span class="sxs-lookup"><span data-stu-id="5b950-114">`2`= busy</span></span>
- <span data-ttu-id="5b950-115">`3` = ausência temporária</span><span class="sxs-lookup"><span data-stu-id="5b950-115">`3`= out of office</span></span>
- <span data-ttu-id="5b950-116">`4`= trabalhando em outro lugar.</span><span class="sxs-lookup"><span data-stu-id="5b950-116">`4`= working elsewhere.</span></span> 

<span data-ttu-id="5b950-117">Por padrão, a duração de cada intervalo de tempo é de 30 minutos.</span><span class="sxs-lookup"><span data-stu-id="5b950-117">By default, the length of each time slot is 30 minutes.</span></span> <span data-ttu-id="5b950-118">Este exemplo usa a propriedade **availabilityViewInterval** para personalizar o intervalo de tempo para 15 minutos.</span><span class="sxs-lookup"><span data-stu-id="5b950-118">This example uses the **availabilityViewInterval** property to customize the time slot to be 15 minutes.</span></span>

## <a name="how-is-getschedule-different-from-findmeetingtimes"></a><span data-ttu-id="5b950-119">Como getSchedule difere de findMeetingTimes</span><span class="sxs-lookup"><span data-stu-id="5b950-119">How is getSchedule different from findMeetingTimes</span></span>

<span data-ttu-id="5b950-120">A ação [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-1.0) é semelhante a **getSchedule** pelo fato de que as duas leem o status de disponibilidade e as horas de trabalho de usuários e recursos específicos.</span><span class="sxs-lookup"><span data-stu-id="5b950-120">The [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-1.0) action is similar to **getSchedule** in that both read the free/busy status and working hours of specified users and resources.</span></span> <span data-ttu-id="5b950-121">As duas ações são diferentes de algumas maneiras principais.</span><span class="sxs-lookup"><span data-stu-id="5b950-121">The two actions differ in a few major ways.</span></span>

### <a name="application"></a><span data-ttu-id="5b950-122">Aplicação</span><span class="sxs-lookup"><span data-stu-id="5b950-122">Application</span></span>

<span data-ttu-id="5b950-123">**findMeetingTimes** aplica determinada lógica de negócios para sugerir horários e locais de reunião, como:</span><span class="sxs-lookup"><span data-stu-id="5b950-123">**findMeetingTimes** applies certain business logic to suggest meeting times and locations, such as:</span></span>

- <span data-ttu-id="5b950-124">Participação opcional ou obrigatória de cada entidade</span><span class="sxs-lookup"><span data-stu-id="5b950-124">Optional or mandatory attendance of each entity</span></span>
- <span data-ttu-id="5b950-125">A natureza da atividade solicitada para a hora do dia</span><span class="sxs-lookup"><span data-stu-id="5b950-125">The nature of the requested activity for the time of the day</span></span>
- <span data-ttu-id="5b950-126">A participação mínima necessária para o quórum da reunião</span><span class="sxs-lookup"><span data-stu-id="5b950-126">The minimum attendance required for a quorum for a meeting</span></span>

<span data-ttu-id="5b950-127">É apropriada para cenários que dependem de [simplificação de reservas de compromissos](findmeetingtimes-example.md).</span><span class="sxs-lookup"><span data-stu-id="5b950-127">It is appropriate for scenarios that depend on [streamlining appointment booking](findmeetingtimes-example.md).</span></span>

<span data-ttu-id="5b950-128">**getSchedule** simplesmente retorna o status de disponibilidade dos eventos existentes em cada calendário solicitado para um determinado período de tempo, e supõe que o tempo restante daquele período de tempo seja livre.</span><span class="sxs-lookup"><span data-stu-id="5b950-128">**getSchedule** simply returns the free/busy status of existing events in each of the requested calendars for a given time period, and assumes the remaining time in that time period tp be free.</span></span> <span data-ttu-id="5b950-129">Você deve aplicar mais lógica de negócios para fazer uso desses dados para completar seu cenário.</span><span class="sxs-lookup"><span data-stu-id="5b950-129">You would then apply further business logic to make use of this data to complete your scenario.</span></span>

### <a name="app-only-support"></a><span data-ttu-id="5b950-130">Suporte somente aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b950-130">App-only support</span></span>

<span data-ttu-id="5b950-131">**findmeetingtimes** dá suporte somente a cenários delegados que exigem que o usuário se conecte ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5b950-131">**findmeetingtimes** supports only delegated scenarios which require a user to have signed in to the app.</span></span> <span data-ttu-id="5b950-132">O aplicativo pode ler eventos apenas nos calendários que o usuário conectado pode acessar.</span><span class="sxs-lookup"><span data-stu-id="5b950-132">The app can read events in only the calendars that the signed-in user can access.</span></span> <span data-ttu-id="5b950-133">Isso pode incluir os calendários que outros usuários delegaram ou compartilharam com o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="5b950-133">This can include calendars that other users have delegated or shared with the signed-in user.</span></span>

<span data-ttu-id="5b950-134">**getSchedule** é compatível com o cenários delegados e somente aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5b950-134">**getSchedule** supports both delegated and app-only scenarios.</span></span> <span data-ttu-id="5b950-135">No último, o administrador consente que o aplicativo acesse todos os calendários sem um usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="5b950-135">In the latter, an administrator consents the app to access all calendars without a signed-in user.</span></span>


### <a name="version-support"></a><span data-ttu-id="5b950-136">Suporte para versões</span><span class="sxs-lookup"><span data-stu-id="5b950-136">Version support</span></span>

<span data-ttu-id="5b950-137">**findmeetingtimes** geralmente é disponibilizado para todos os aplicativos.</span><span class="sxs-lookup"><span data-stu-id="5b950-137">**findmeetingtimes** is generally available for all apps.</span></span> 

<span data-ttu-id="5b950-138">**getSchedule** está disponível atualmente [no status de visualização](versioning-and-support.md#beta-version), e portanto não é apropriado para uso em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5b950-138">**getSchedule** is currently available [in preview status](versioning-and-support.md#beta-version), and therefore is not appropriate for use in production apps.</span></span>


## <a name="permissions"></a><span data-ttu-id="5b950-139">Permissions</span><span class="sxs-lookup"><span data-stu-id="5b950-139">Permissions</span></span>
<span data-ttu-id="5b950-140">A permissão menos privilegiada que você necessita para obter informações de disponibilidade é Calendar.Read.</span><span class="sxs-lookup"><span data-stu-id="5b950-140">The least privileged permission you need to get free/busy information is Calendar.Read.</span></span> <span data-ttu-id="5b950-141">Dependendo do cenário do aplicativo, esse consentimento pode vir do usuário conectado ou do administrador.</span><span class="sxs-lookup"><span data-stu-id="5b950-141">Depending on your app scenario, this can be consented by the signed-in user or administrator.</span></span>
<span data-ttu-id="5b950-142">Além do status de disponibilidade e do horário de trabalho das entidades solicitadas, **getSchedule** também pode retornar o assunto e o local de um evento, contanto que:</span><span class="sxs-lookup"><span data-stu-id="5b950-142">Other than the free/busy status and working hours of requested entities, **getSchedule** can also return the subject and location of an event, provided that:</span></span>

- <span data-ttu-id="5b950-143">Se o evento estiver marcado com nível de confidencialidade baixa – `normal` ou `personal` E uma ou mais das seguintes condições serão aplicados:</span><span class="sxs-lookup"><span data-stu-id="5b950-143">If the event is marked with low sensitivity level - `normal` or `personal` AND one or more of the following conditions applies:</span></span>

- <span data-ttu-id="5b950-144">As configurações de calendário do usuário solicitado permitem que todos os usuários da organização visualizem títulos e locais</span><span class="sxs-lookup"><span data-stu-id="5b950-144">The requested user’s calendar settings allow all the users in the organization to view titles and locations</span></span>
- <span data-ttu-id="5b950-145">O calendário do usuário solicitado é compartilhado com o usuário conectado</span><span class="sxs-lookup"><span data-stu-id="5b950-145">The requested user’s calendar is shared with the signed-in user</span></span>
- <span data-ttu-id="5b950-146">O usuário conectado é um administrador da mesma organização que o usuário solicitado.</span><span class="sxs-lookup"><span data-stu-id="5b950-146">The signed-in user is an administrator of the same organization as the requested user.</span></span>

## <a name="time-zone-representation"></a><span data-ttu-id="5b950-147">Representação de fuso horário</span><span class="sxs-lookup"><span data-stu-id="5b950-147">Time zone representation</span></span>
<span data-ttu-id="5b950-148">Por padrão, as horas de início e de término de itens de agenda retornado são representados em UTC.</span><span class="sxs-lookup"><span data-stu-id="5b950-148">By default, the start and end times of the returned schedule items are represented in UTC.</span></span> <span data-ttu-id="5b950-149">Você pode usar um `Prefer` cabeçalho para especificar um fuso horário apropriado para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5b950-149">You can use a `Prefer` header to specify a time zone appropriate for your app.</span></span> <span data-ttu-id="5b950-150">Como exemplo:</span><span class="sxs-lookup"><span data-stu-id="5b950-150">As an example:</span></span> 
```
Prefer: outlook.timezone="Pacific Standard Time"
```

## <a name="limits-and-error-conditions"></a><span data-ttu-id="5b950-151">Limites e condições do erro</span><span class="sxs-lookup"><span data-stu-id="5b950-151">Limits and error conditions</span></span>
<span data-ttu-id="5b950-152">Fique atento para os seguintes limites e condições de erro:</span><span class="sxs-lookup"><span data-stu-id="5b950-152">Be aware of the following limits and error condition:</span></span>

- <span data-ttu-id="5b950-153">**getSchedule** pode dar suporte procurando informações sobre disponibilidade para até 20 entidades ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="5b950-153">**getSchedule** can support looking up free/busy information for up to 20 entities at once.</span></span> <span data-ttu-id="5b950-154">Este limite se aplica ao número de usuários identificados individualmente ou como membros de uma lista de distribuição, e também ao número de recursos.</span><span class="sxs-lookup"><span data-stu-id="5b950-154">This limit applies to the number of users identified individually or as members of a distribution list, and to the number of resources as well.</span></span>
- <span data-ttu-id="5b950-155">O período de tempo para pesquisar deve ser menor que 42 dias.</span><span class="sxs-lookup"><span data-stu-id="5b950-155">The time period to look up must be less than 42 days.</span></span>
- <span data-ttu-id="5b950-156">Se **getSchedule** não puder identificar um usuário ou um recurso especificados, ela retornará um item de agenda único e indicará o erro</span><span class="sxs-lookup"><span data-stu-id="5b950-156">If **getSchedule** cannot identify a specified user or resource, it returns a single schedule item and indicates the error.</span></span> 

## <a name="see-also"></a><span data-ttu-id="5b950-157">Confira também</span><span class="sxs-lookup"><span data-stu-id="5b950-157">See also</span></span>
- [<span data-ttu-id="5b950-158">Referência de permissões</span><span class="sxs-lookup"><span data-stu-id="5b950-158">Permissions reference</span></span>](permissions-reference.md#calendars-permissions)
- [<span data-ttu-id="5b950-159">Encontrar possíveis horários de reunião no calendário do Outlook</span><span class="sxs-lookup"><span data-stu-id="5b950-159">Find possible meeting times on the Outlook calendar</span></span>](findmeetingtimes-example.md)
