# <a name="get-freebusy-schedule-of-users-and-resources-preview"></a><span data-ttu-id="d439a-101">Obtenha a agenda de disponibilidade livre/ocupado de usuários e recursos (versão prévia)</span><span class="sxs-lookup"><span data-stu-id="d439a-101">Get free/busy schedule for users and resources (preview)</span></span>

<span data-ttu-id="d439a-102">Em um ambiente de trabalho ou escola, um cenário comum é ver quando um usuário está livre para reuniões ou procurar a disponibilidade de uma equipe, sala ou equipamento para um período de tempo.</span><span class="sxs-lookup"><span data-stu-id="d439a-102">In a work or school setting, a common scenario is to see when a user is free for meeting, or to browse the availability of a team, room, or equipment for a time period.</span></span>

<span data-ttu-id="d439a-103">A ação [getSchedule](../api-reference/beta/api/calendar_getschedule.md) permite que você obtenha as informações de disponibilidade de uma ou mais entidades - usuários, listas de distribuição ou recursos - para um período de tempo específico.</span><span class="sxs-lookup"><span data-stu-id="d439a-103">The [getSchedule](../api-reference/beta/api/calendar_getschedule.md) action lets you get the availability information of one or more entities - users, distribution lists, or resources - for a specific period of time.</span></span> 

## <a name="example"></a><span data-ttu-id="d439a-104">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d439a-104">Example</span></span>

<span data-ttu-id="d439a-105">Um exemplo simples é encontrar a agenda de disponibilidade de um colega de trabalho, Alex, em um dia específico, das 9h às 18h, horário padrão do Pacífico:</span><span class="sxs-lookup"><span data-stu-id="d439a-105">A simple example is to find the free/busy schedule of a coworker, Alex, on a specific day, from 9am to 6pm, Pacitfic Standard Time:</span></span>

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

<span data-ttu-id="d439a-106">**getSchedule** retorna dois itens de agenda que correspondem aos eventos existentes no calendário padrão do Alex, mostrando os horários de início e término de cada evento e seu status de disponibilidade livre/ocupado.</span><span class="sxs-lookup"><span data-stu-id="d439a-106">**getSchedule** returns two schedule items that match existing events in Alex' default calendar, showing the start and end times of each event and its free/busy status.</span></span> <span data-ttu-id="d439a-107">Você pode assumir que Alex está livre pelo tempo restante nesse intervalo de data/hora.</span><span class="sxs-lookup"><span data-stu-id="d439a-107">You can assume Alex is free for the remaining time in that date/time range.</span></span>

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

<span data-ttu-id="d439a-108">Além da agenda de livre/ocupado e o horário de trabalho de Alex, **getSchedule** também retornará **availabilityView**, que é uma exibição mesclada da disponibilidade de Alex naquele dia.</span><span class="sxs-lookup"><span data-stu-id="d439a-108">Apart from the free/busy schedule and working hours of Alex, **getSchedule** also returns **availabilityView**, which is a merged view of Alex' availability for that day.</span></span> <span data-ttu-id="d439a-109">A visualização mesclada é uma sequência de caracteres que consiste em intervalos de tempo que cobrem esse dia, e cada intervalo de tempo indica a disponibilidade de Alex usando a seguinte convenção:</span><span class="sxs-lookup"><span data-stu-id="d439a-109">The merged view is a string that consists of time slots covering that day, with each time slot indicating Alex' availability using the following convention:</span></span> 

- <span data-ttu-id="d439a-110">`0`= disponível</span><span class="sxs-lookup"><span data-stu-id="d439a-110">`0`= free</span></span>
- <span data-ttu-id="d439a-111">`1`= provisório</span><span class="sxs-lookup"><span data-stu-id="d439a-111">`1`= tentative</span></span>
- <span data-ttu-id="d439a-112">`2`= ocupado</span><span class="sxs-lookup"><span data-stu-id="d439a-112">`2`= busy</span></span>
- <span data-ttu-id="d439a-113">`3`= ausência temporária</span><span class="sxs-lookup"><span data-stu-id="d439a-113">`3`= out of office</span></span>
- <span data-ttu-id="d439a-114">`4`= trabalhando em outros lugares.</span><span class="sxs-lookup"><span data-stu-id="d439a-114">`4`= working elsewhere.</span></span> 

<span data-ttu-id="d439a-115">Por padrão, a duração de cada intervalo de tempo é de 30 minutos.</span><span class="sxs-lookup"><span data-stu-id="d439a-115">Specifies the length of each time slot in minutes. Default is 30 minutes.</span></span> <span data-ttu-id="d439a-116">Este exemplo usa a propriedade **availabilityViewInterval** para personalizar o intervalo de tempo para 15 minutos.</span><span class="sxs-lookup"><span data-stu-id="d439a-116">This example uses the **availabilityViewInterval** property to customize the time slot to be 15 minutes.</span></span>

## <a name="how-is-getschedule-different-from-findmeetingtimes"></a><span data-ttu-id="d439a-117">Como getSchedule é diferente do findMeetingTimes</span><span class="sxs-lookup"><span data-stu-id="d439a-117">How is getSchedule different from findMeetingTimes</span></span>

<span data-ttu-id="d439a-118">A ação [findMeetingTimes](../api-reference/v1.0/api/user_findmeetingtimes.md) é semelhante ao **getSchedule** em que ambos leem o status de disponibilidade livre/ocupado e o horário de trabalho de usuários e de recursos especificados.</span><span class="sxs-lookup"><span data-stu-id="d439a-118">The [findMeetingTimes](../api-reference/v1.0/api/user_findmeetingtimes.md) action is similar to **getSchedule** in that both read the free/busy status and working hours of specified users and resources.</span></span> <span data-ttu-id="d439a-119">As duas ações diferem de algumas maneiras principais.</span><span class="sxs-lookup"><span data-stu-id="d439a-119">The two actions differ in a few major ways.</span></span>

### <a name="application"></a><span data-ttu-id="d439a-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d439a-120">Application</span></span>

<span data-ttu-id="d439a-121">**findMeetingTimes** aplica determinada lógica de negócios para sugerir horários e locais de reunião, como:</span><span class="sxs-lookup"><span data-stu-id="d439a-121">**findMeetingTimes** applies certain business logic to suggest meeting times and locations, such as:</span></span>

- <span data-ttu-id="d439a-122">Participação opcional ou obrigatória de cada entidade</span><span class="sxs-lookup"><span data-stu-id="d439a-122">Optional or mandatory attendance of each entity</span></span>
- <span data-ttu-id="d439a-123">A natureza da atividade solicitada para a hora do dia</span><span class="sxs-lookup"><span data-stu-id="d439a-123">The nature of the requested activity for the time of the day</span></span>
- <span data-ttu-id="d439a-124">A presença mínima necessária para um quorum para uma reunião</span><span class="sxs-lookup"><span data-stu-id="d439a-124">The minimum attendance required for a quorum for a meeting</span></span>

<span data-ttu-id="d439a-125">Ele é adequado para cenários que dependem [da simplificação da reserva de compromissos](findmeetingtimes_example.md).</span><span class="sxs-lookup"><span data-stu-id="d439a-125">It is appropriate for scenarios that depend on [streamlining appointment booking](findmeetingtimes_example.md).</span></span>

<span data-ttu-id="d439a-126">**getSchedule** simplesmente retorna o status livre/ocupado dos eventos existentes em cada um dos calendários solicitados para um determinado período e supõe que o tempo restante nesse período de tempo está livre.</span><span class="sxs-lookup"><span data-stu-id="d439a-126">**getSchedule** simply returns the free/busy status of existing events in each of the requested calendars for a given time period, and assumes the remaining time in that time period tp be free.</span></span> <span data-ttu-id="d439a-127">Em seguida, você aplicaria mais lógica de negócios para usar esses dados para concluir seu cenário.</span><span class="sxs-lookup"><span data-stu-id="d439a-127">You would then apply further business logic to make use of this data to complete your scenario.</span></span>

### <a name="app-only-support"></a><span data-ttu-id="d439a-128">Suporte apenas a aplicativos</span><span class="sxs-lookup"><span data-stu-id="d439a-128">App-only support</span></span>

<span data-ttu-id="d439a-129">**findmeetingtimes** suporta apenas cenários delegados que exigem que um usuário entre no aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d439a-129">**findmeetingtimes** supports only delegated scenarios which require a user to have signed in to the app.</span></span> <span data-ttu-id="d439a-130">O aplicativo pode ler eventos apenas nos calendários que o usuário conectado pode acessar.</span><span class="sxs-lookup"><span data-stu-id="d439a-130">The app can read events in only the calendars that the signed-in user can access.</span></span> <span data-ttu-id="d439a-131">Isso pode incluir calendários que outros usuários delegaram ou compartilharam com o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="d439a-131">This can include calendars that other users have delegated or shared with the signed-in user.</span></span>

<span data-ttu-id="d439a-132">**getSchedule** suporta cenários delegados e somente aplicativos.</span><span class="sxs-lookup"><span data-stu-id="d439a-132">**getSchedule** supports both delegated and app-only scenarios.</span></span> <span data-ttu-id="d439a-133">Neste último, um administrador consente que o aplicativo acesse todos os calendários sem um usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="d439a-133">In the latter, an administrator consents the app to access all calendars without a signed-in user.</span></span>


### <a name="version-support"></a><span data-ttu-id="d439a-134">Suporte à versão</span><span class="sxs-lookup"><span data-stu-id="d439a-134">Version support</span></span>

<span data-ttu-id="d439a-135">**findmeetingtimes** geralmente está disponível para todos os aplicativos.</span><span class="sxs-lookup"><span data-stu-id="d439a-135">**findmeetingtimes** is generally available for all apps.</span></span> 

<span data-ttu-id="d439a-136">**getSchedule** está disponível atualmente [no status de visualização](versioning_and_support.md#beta-version)e, portanto, não é apropriado para uso em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d439a-136">**getSchedule** is currently available [in preview status](versioning_and_support.md#beta-version), and therefore is not appropriate for use in production apps.</span></span>


## <a name="permissions"></a><span data-ttu-id="d439a-137">Permissões</span><span class="sxs-lookup"><span data-stu-id="d439a-137">Permissions</span></span>
<span data-ttu-id="d439a-138">A permissão com menos privilégios que você precisa para obter informações de livre/ocupado é Calendar.Read.</span><span class="sxs-lookup"><span data-stu-id="d439a-138">The least privileged permission you need to get free/busy information is Calendar.Read.</span></span> <span data-ttu-id="d439a-139">Dependendo do cenário do aplicativo, isso pode ser permitido pelo usuário ou administrador conectado.</span><span class="sxs-lookup"><span data-stu-id="d439a-139">Depending on your app scenario, this can be consented by the signed-in user or administrator.</span></span>
<span data-ttu-id="d439a-140">Além do status livre/ocupado e do horário de trabalho das entidades solicitadas, **getSchedule** também pode retornar o assunto e o local de um evento, desde que:</span><span class="sxs-lookup"><span data-stu-id="d439a-140">Other than the free/busy status and working hours of requested entities, **getSchedule** can also return the subject and location of an event, provided that:</span></span>

- <span data-ttu-id="d439a-141">Se o evento é marcado com o nível de confidencialidade baixo - `normal` ou `personal` e uma ou mais das seguintes condições se aplicam:</span><span class="sxs-lookup"><span data-stu-id="d439a-141">If the event is marked with low sensitivity level - `normal` or `personal` AND one or more of the following conditions applies:</span></span>

- <span data-ttu-id="d439a-142">As configurações de calendário do usuário solicitado permitem que todos os usuários da organização visualizem títulos e locais</span><span class="sxs-lookup"><span data-stu-id="d439a-142">The requested user’s calendar settings allow all the users in the organization to view titles and locations</span></span>
- <span data-ttu-id="d439a-143">O calendário do usuário solicitado é compartilhado com o usuário conectado</span><span class="sxs-lookup"><span data-stu-id="d439a-143">The requested user’s calendar is shared with the signed-in user</span></span>
- <span data-ttu-id="d439a-144">O usuário conectado é um administrador da mesma organização que o usuário solicitado.</span><span class="sxs-lookup"><span data-stu-id="d439a-144">The signed-in user is an administrator of the same organization as the requested user.</span></span>

## <a name="time-zone-representation"></a><span data-ttu-id="d439a-145">Representação de fuso horário</span><span class="sxs-lookup"><span data-stu-id="d439a-145">Time zone representation</span></span>
<span data-ttu-id="d439a-146">Por padrão, os horários de início e término dos itens de agendamento retornados são representados em UTC.</span><span class="sxs-lookup"><span data-stu-id="d439a-146">By default, the start and end times of the returned schedule items are represented in UTC.</span></span> <span data-ttu-id="d439a-147">Você pode usar um `Prefer` cabeçalho para especificar um fuso horário apropriado para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d439a-147">You can use a `Prefer` header to specify a time zone appropriate for your app.</span></span> <span data-ttu-id="d439a-148">Como exemplo:</span><span class="sxs-lookup"><span data-stu-id="d439a-148">As an example:</span></span> 
```
Prefer: outlook.timezone="Pacific Standard Time"
```

## <a name="limits-and-error-conditions"></a><span data-ttu-id="d439a-149">Limites e condições de erro</span><span class="sxs-lookup"><span data-stu-id="d439a-149">Limits and error conditions</span></span>
<span data-ttu-id="d439a-150">Esteja ciente dos seguintes limites e condições de erro:</span><span class="sxs-lookup"><span data-stu-id="d439a-150">Be aware of the following limits and error condition:</span></span>

- <span data-ttu-id="d439a-151">**getSchedule** pode suportar a procura de informações de disponibilidade de livre/ocupado para até 20 entidades ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="d439a-151">**getSchedule** can support looking up free/busy information for up to 20 entities at once.</span></span> <span data-ttu-id="d439a-152">Esse limite se aplica ao número de usuários identificados individualmente ou como membros de uma lista de distribuição e também ao número de recursos.</span><span class="sxs-lookup"><span data-stu-id="d439a-152">This limit applies to the number of users identified individually or as members of a distribution list, and to the number of resources as well.</span></span>
- <span data-ttu-id="d439a-153">O período de tempo para procurar deve ser inferior a 42 dias.</span><span class="sxs-lookup"><span data-stu-id="d439a-153">The time period to look up must be less than 42 days.</span></span>
- <span data-ttu-id="d439a-154">Se **getSchedule** não é possível identificar um usuário ou recurso especificado, ele retorna um único item de agenda e indica o erro.</span><span class="sxs-lookup"><span data-stu-id="d439a-154">If **getSchedule** cannot identify a specified user or resource, it returns a single schedule item and indicates the error.</span></span> 

## <a name="see-also"></a><span data-ttu-id="d439a-155">Veja também</span><span class="sxs-lookup"><span data-stu-id="d439a-155">See also</span></span>
- [<span data-ttu-id="d439a-156">Referência de permissões</span><span class="sxs-lookup"><span data-stu-id="d439a-156">Permissions reference</span></span>](permissions_reference.md#calendars-permissions)
- [<span data-ttu-id="d439a-157">Encontrar possíveis horários de reunião no calendário do Outlook</span><span class="sxs-lookup"><span data-stu-id="d439a-157">Find possible meeting times on the Outlook calendar</span></span>](findmeetingtimes_example.md)
