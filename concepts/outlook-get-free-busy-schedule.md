---
title: Obter agenda de disponibilidade de usuários e recursos
description: Em uma configuração de escola ou trabalho, um cenário comum é ver quando um usuário está livre para um reunião, ou então pesquisar a disponibilidade de uma equipe, sala ou equipamento para um período de tempo.
author: tariq-sharif
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: d3d8379f05d6e19505bdf3c45cca0863a685423d
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317128"
---
# <a name="get-freebusy-schedule-of-users-and-resources"></a><span data-ttu-id="5ebe2-103">Obter agenda de disponibilidade de usuários e recursos</span><span class="sxs-lookup"><span data-stu-id="5ebe2-103">Get free/busy schedule of users and resources</span></span>

<span data-ttu-id="5ebe2-104">Em uma configuração de escola ou trabalho, um cenário comum é ver quando um usuário está livre para um reunião, ou então pesquisar a disponibilidade de uma equipe, sala ou equipamento para um período de tempo.</span><span class="sxs-lookup"><span data-stu-id="5ebe2-104">In a work or school setting, a common scenario is to see when a user is free for meeting, or to browse the availability of a team, room, or equipment for a time period.</span></span>

<span data-ttu-id="5ebe2-105">A ação [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-1.0) permite que você obtenha as informações de disponibilidade de uma ou mais entidades (usuários, listas de distribuição ou recursos) para um período específico de tempo.</span><span class="sxs-lookup"><span data-stu-id="5ebe2-105">The [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-1.0) action lets you get the availability information of one or more entities - users, distribution lists, or resources - for a specific period of time.</span></span> 

## <a name="example"></a><span data-ttu-id="5ebe2-106">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ebe2-106">Example</span></span>

<span data-ttu-id="5ebe2-107">Um exemplo simples é encontrar a agenda de horários livres/ocupados de um colega de trabalho, Alex, em um dia específico, das 9 às 18 horas, Fuso Horário Padrão do Pacífico (PST):</span><span class="sxs-lookup"><span data-stu-id="5ebe2-107">A simple example is to find the free/busy schedule of a coworker, Alex, on a specific day, from 9am to 6pm, Pacific Standard Time:</span></span>

<!-- {
  "blockType": "ignored",
  "name": "calendar_getSchedule_concept"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/calendar/getschedule 
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

<span data-ttu-id="5ebe2-108">**getSchedule** retorna dois itens de agenda que correspondem aos eventos existentes no calendário padrão do Alex, mostrando os horários de início e término de cada evento e seu status de disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="5ebe2-108">**getSchedule** returns two schedule items that match existing events in Alex' default calendar, showing the start and end times of each event and its free/busy status.</span></span> <span data-ttu-id="5ebe2-109">Você poderá supor que Alex está livre pelo restante do tempo desse intervalo de data/hora.</span><span class="sxs-lookup"><span data-stu-id="5ebe2-109">You can assume Alex is free for the remaining time in that date/time range.</span></span>

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
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.scheduleInformation)",
    "value":[
        {
            "scheduleId":"AlexW@contoso.OnMicrosoft.com",
            "availabilityView":"111111002222222200000000000000000000",
            "scheduleItems":[
                {
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

<span data-ttu-id="5ebe2-110">Além da disponibilidade da agenda e das horas de trabalho do Alex, **getSchedule** também retorna **availabilityView**, que é uma visualização mesclada da disponibilidade do Alex a cada dia.</span><span class="sxs-lookup"><span data-stu-id="5ebe2-110">Apart from the free/busy schedule and working hours of Alex, **getSchedule** also returns **availabilityView**, which is a merged view of Alex' availability for that day.</span></span> <span data-ttu-id="5ebe2-111">O modo de exibição mesclado é uma cadeia de caracteres que consiste em intervalos de tempo abrangendo aquele dia, sendo que cada intervalo de tempo indica a disponibilidade do Alex usando a seguinte convenção:</span><span class="sxs-lookup"><span data-stu-id="5ebe2-111">The merged view is a string that consists of time slots covering that day, with each time slot indicating Alex' availability using the following convention:</span></span> 

- <span data-ttu-id="5ebe2-112">`0` = livre</span><span class="sxs-lookup"><span data-stu-id="5ebe2-112">`0`= free</span></span>
- <span data-ttu-id="5ebe2-113">`1` = provisório</span><span class="sxs-lookup"><span data-stu-id="5ebe2-113">`1`= tentative</span></span>
- <span data-ttu-id="5ebe2-114">`2` = ocupado</span><span class="sxs-lookup"><span data-stu-id="5ebe2-114">`2`= busy</span></span>
- <span data-ttu-id="5ebe2-115">`3` = ausência temporária</span><span class="sxs-lookup"><span data-stu-id="5ebe2-115">`3`= out of office</span></span>
- <span data-ttu-id="5ebe2-116">`4`= trabalhando em outro lugar.</span><span class="sxs-lookup"><span data-stu-id="5ebe2-116">`4`= working elsewhere.</span></span> 

<span data-ttu-id="5ebe2-117">Por padrão, a duração de cada intervalo de tempo é de 30 minutos.</span><span class="sxs-lookup"><span data-stu-id="5ebe2-117">By default, the length of each time slot is 30 minutes.</span></span> <span data-ttu-id="5ebe2-118">Este exemplo usa a propriedade **availabilityViewInterval** para personalizar o intervalo de tempo para 15 minutos.</span><span class="sxs-lookup"><span data-stu-id="5ebe2-118">This example uses the **availabilityViewInterval** property to customize the time slot to be 15 minutes.</span></span>

## <a name="how-does-getschedule-compare-with-findmeetingtimes"></a><span data-ttu-id="5ebe2-119">Como o getSchedule se compara ao findMeetingTimes</span><span class="sxs-lookup"><span data-stu-id="5ebe2-119">How does getSchedule compare with findMeetingTimes</span></span>

<span data-ttu-id="5ebe2-120">A ação [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-1.0) é semelhante a **getSchedule** pelo fato de que as duas leem o status de disponibilidade e as horas de trabalho de usuários e recursos específicos.</span><span class="sxs-lookup"><span data-stu-id="5ebe2-120">The [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-1.0) action is similar to **getSchedule** in that both read the free/busy status and working hours of specified users and resources.</span></span> <span data-ttu-id="5ebe2-121">As duas ações são diferentes de algumas maneiras principais.</span><span class="sxs-lookup"><span data-stu-id="5ebe2-121">The two actions differ in a few major ways.</span></span>

### <a name="application"></a><span data-ttu-id="5ebe2-122">Aplicação</span><span class="sxs-lookup"><span data-stu-id="5ebe2-122">Application</span></span>

<span data-ttu-id="5ebe2-123">**findMeetingTimes** aplica determinada lógica de negócios para sugerir horários e locais de reunião, como:</span><span class="sxs-lookup"><span data-stu-id="5ebe2-123">**findMeetingTimes** applies certain business logic to suggest meeting times and locations, such as:</span></span>

- <span data-ttu-id="5ebe2-124">Participação opcional ou obrigatória de cada entidade</span><span class="sxs-lookup"><span data-stu-id="5ebe2-124">Optional or mandatory attendance of each entity</span></span>
- <span data-ttu-id="5ebe2-125">A natureza da atividade solicitada para a hora do dia</span><span class="sxs-lookup"><span data-stu-id="5ebe2-125">The nature of the requested activity for the time of the day</span></span>
- <span data-ttu-id="5ebe2-126">A participação mínima necessária para o quórum da reunião</span><span class="sxs-lookup"><span data-stu-id="5ebe2-126">The minimum attendance required for a quorum for a meeting</span></span>

<span data-ttu-id="5ebe2-127">É apropriada para cenários que dependem de [simplificação de reservas de compromissos](findmeetingtimes-example.md).</span><span class="sxs-lookup"><span data-stu-id="5ebe2-127">It is appropriate for scenarios that depend on [streamlining appointment booking](findmeetingtimes-example.md).</span></span>

<span data-ttu-id="5ebe2-128">O **getSchedule** simplesmente retorna o status de disponibilidade dos eventos existentes em cada calendário solicitado por um determinado período de tempo e supõe que o tempo restante daquele período de tempo esteja livre.</span><span class="sxs-lookup"><span data-stu-id="5ebe2-128">**getSchedule** simply returns the free/busy status of existing events in each of the requested calendars for a given time period, and assumes the remaining time in that time period to be free.</span></span> <span data-ttu-id="5ebe2-129">Você deve aplicar mais lógica de negócios para fazer uso desses dados para completar seu cenário.</span><span class="sxs-lookup"><span data-stu-id="5ebe2-129">You would then apply further business logic to make use of this data to complete your scenario.</span></span>

### <a name="app-only-support"></a><span data-ttu-id="5ebe2-130">Suporte somente aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ebe2-130">App-only support</span></span>

<span data-ttu-id="5ebe2-131">**findmeetingtimes** dá suporte somente a cenários delegados que exigem que o usuário se conecte ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5ebe2-131">**findmeetingtimes** supports only delegated scenarios which require a user to have signed in to the app.</span></span> <span data-ttu-id="5ebe2-132">O aplicativo pode ler eventos apenas nos calendários que o usuário conectado pode acessar.</span><span class="sxs-lookup"><span data-stu-id="5ebe2-132">The app can read events in only the calendars that the signed-in user can access.</span></span> <span data-ttu-id="5ebe2-133">Isso pode incluir os calendários que outros usuários delegaram ou compartilharam com o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="5ebe2-133">This can include calendars that other users have delegated or shared with the signed-in user.</span></span>

<span data-ttu-id="5ebe2-134">**getSchedule** é compatível com o cenários delegados e somente aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5ebe2-134">**getSchedule** supports both delegated and app-only scenarios.</span></span> <span data-ttu-id="5ebe2-135">No último, o administrador consente que o aplicativo acesse todos os calendários sem um usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="5ebe2-135">In the latter, an administrator consents the app to access all calendars without a signed-in user.</span></span>

### <a name="permissions"></a><span data-ttu-id="5ebe2-136">Permissões</span><span class="sxs-lookup"><span data-stu-id="5ebe2-136">Permissions</span></span>
<span data-ttu-id="5ebe2-137">A permissão menos privilegiada exigida pelo **findmeetingtimes** é Calendars.Read.Shared.</span><span class="sxs-lookup"><span data-stu-id="5ebe2-137">The least privileged permissions required by **findmeetingtimes** is Calendars.Read.Shared.</span></span>

<span data-ttu-id="5ebe2-138">A permissão menos privilegiada exigida por **getSchedule** é Calendars.Read.</span><span class="sxs-lookup"><span data-stu-id="5ebe2-138">The least privileged permission required by **getSchedule** is Calendars.Read.</span></span> 

### <a name="version-support"></a><span data-ttu-id="5ebe2-139">Suporte para versões</span><span class="sxs-lookup"><span data-stu-id="5ebe2-139">Version support</span></span>

<span data-ttu-id="5ebe2-140">O **findmeetingtimes** e o **getSchedule** estão geralmente disponíveis e adequados para uso em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5ebe2-140">**findmeetingtimes** and **getSchedule** are both generally available and appropriate for use in production apps.</span></span>


## <a name="event-data-returned"></a><span data-ttu-id="5ebe2-141">Dados de evento retornados</span><span class="sxs-lookup"><span data-stu-id="5ebe2-141">Event data returned</span></span>
<span data-ttu-id="5ebe2-142">A permissão menos privilegiada exigida por **getSchedule** para que um aplicativo obtenha informações de disponibilidade é Calendars.Read.</span><span class="sxs-lookup"><span data-stu-id="5ebe2-142">The least privileged permission required by **getSchedule** for an app to get free/busy information is Calendars.Read.</span></span> <span data-ttu-id="5ebe2-143">Dependendo do cenário do aplicativo, este consentimento pode vir do usuário conectado ou do administrador.</span><span class="sxs-lookup"><span data-stu-id="5ebe2-143">Depending on your app scenario, this can be consented by the signed-in user or administrator.</span></span>

<span data-ttu-id="5ebe2-144">Embora a permissão consentida permite com que um aplicativo use o **getSchedule** nos calendários dos usuários solicitados pelo Outlook, o usuário solicitado controla quais dados de evento, caso existam, o **getSchedule** retornará.</span><span class="sxs-lookup"><span data-stu-id="5ebe2-144">While the consented permission lets an app use **getSchedule** on the requested users' calendars, through Outlook, the requested user controls which event data, if any, that **getSchedule** returns.</span></span> 

<span data-ttu-id="5ebe2-145">Por exemplo, o **getSchedule** pode retornar o status de disponibilidade e as horas de trabalho dos usuários solicitados ou também retornar as propriedades **subject**, **location**, e **isPrivate** de um evento, desde que:</span><span class="sxs-lookup"><span data-stu-id="5ebe2-145">For example, **getSchedule** can return the free/busy status and working hours of the requested users, or it can also return the **subject**, **location**, and **isPrivate** properties of an event, provided that:</span></span>

- <span data-ttu-id="5ebe2-146">O evento esteja marcado com um nível de confidencialidade baixo - `normal` ou `personal`- E uma ou mais das seguintes condições se aplicam:</span><span class="sxs-lookup"><span data-stu-id="5ebe2-146">The event is marked with low sensitivity level - `normal` or `personal` - AND one or more of the following conditions apply:</span></span>

  - <span data-ttu-id="5ebe2-147">As configurações de calendário do usuário solicitado permitem com que o usuário conectado veja as linhas de assunto e localizações</span><span class="sxs-lookup"><span data-stu-id="5ebe2-147">The requested user’s calendar settings allow the signed-in user to view subject lines and locations</span></span>
  - <span data-ttu-id="5ebe2-148">O calendário do usuário solicitado é compartilhado com o usuário conectado</span><span class="sxs-lookup"><span data-stu-id="5ebe2-148">The requested user’s calendar is shared with the signed-in user</span></span>

<span data-ttu-id="5ebe2-149">Estas condições se aplicam independentemente se o usuário conectado é um administrador na organização.</span><span class="sxs-lookup"><span data-stu-id="5ebe2-149">These conditions apply regardless of whether the signed-in user is an administrator in the organization.</span></span> <span data-ttu-id="5ebe2-150">O usuário solicitado tem controle sobre os dados de eventos retornados.</span><span class="sxs-lookup"><span data-stu-id="5ebe2-150">The requested user has control over the event data returned.</span></span>

## <a name="time-zone-representation"></a><span data-ttu-id="5ebe2-151">Representação de fuso horário</span><span class="sxs-lookup"><span data-stu-id="5ebe2-151">Time zone representation</span></span>
<span data-ttu-id="5ebe2-152">Por padrão, as horas de início e de término de itens de agenda retornado são representados em UTC.</span><span class="sxs-lookup"><span data-stu-id="5ebe2-152">By default, the start and end times of the returned schedule items are represented in UTC.</span></span> <span data-ttu-id="5ebe2-153">Você pode usar um `Prefer` cabeçalho para especificar um fuso horário apropriado para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5ebe2-153">You can use a `Prefer` header to specify a time zone appropriate for your app.</span></span> <span data-ttu-id="5ebe2-154">Como exemplo:</span><span class="sxs-lookup"><span data-stu-id="5ebe2-154">As an example:</span></span> 
``` http
Prefer: outlook.timezone="Pacific Standard Time"
```

## <a name="limits-and-error-conditions"></a><span data-ttu-id="5ebe2-155">Limites e condições do erro</span><span class="sxs-lookup"><span data-stu-id="5ebe2-155">Limits and error conditions</span></span>
<span data-ttu-id="5ebe2-156">Fique atento para os seguintes limites e condições de erro:</span><span class="sxs-lookup"><span data-stu-id="5ebe2-156">Be aware of the following limits and error condition:</span></span>

- <span data-ttu-id="5ebe2-157">**getSchedule** pode dar suporte procurando informações sobre disponibilidade para até 20 entidades ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="5ebe2-157">**getSchedule** can support looking up free/busy information for up to 20 entities at once.</span></span> <span data-ttu-id="5ebe2-158">Este limite se aplica ao número de usuários identificados individualmente ou como membros de uma lista de distribuição, e também ao número de recursos.</span><span class="sxs-lookup"><span data-stu-id="5ebe2-158">This limit applies to the number of users identified individually or as members of a distribution list, and to the number of resources as well.</span></span>
- <span data-ttu-id="5ebe2-159">O período de tempo para pesquisar deve ser menor que 42 dias.</span><span class="sxs-lookup"><span data-stu-id="5ebe2-159">The time period to look up must be less than 42 days.</span></span>
- <span data-ttu-id="5ebe2-160">Se **getSchedule** não puder identificar um usuário ou um recurso especificados, ela retornará um item de agenda único e indicará o erro</span><span class="sxs-lookup"><span data-stu-id="5ebe2-160">If **getSchedule** cannot identify a specified user or resource, it returns a single schedule item and indicates the error.</span></span> 


## <a name="see-also"></a><span data-ttu-id="5ebe2-161">Confira também</span><span class="sxs-lookup"><span data-stu-id="5ebe2-161">See also</span></span>
- [<span data-ttu-id="5ebe2-162">Referência de permissões</span><span class="sxs-lookup"><span data-stu-id="5ebe2-162">Permissions reference</span></span>](permissions-reference.md#calendars-permissions)
- [<span data-ttu-id="5ebe2-163">Encontrar possíveis horários de reunião no calendário do Outlook</span><span class="sxs-lookup"><span data-stu-id="5ebe2-163">Find possible meeting times on the Outlook calendar</span></span>](findmeetingtimes-example.md)
