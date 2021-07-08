---
title: Encontrar possíveis horários de reunião no calendário do Outlook
description: 'Em um local de trabalho ou escola, procurar um horário e um local em comum para atender geralmente gera sobrecarga. Os aplicativos do Microsoft Graph podem usar '
localization_priority: Priority
ms.openlocfilehash: 972a22ed302b824c3b4d147338badcfb72c30c6a
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317025"
---
# <a name="find-possible-meeting-times-on-the-outlook-calendar"></a><span data-ttu-id="5aadc-104">Encontrar possíveis horários de reunião no calendário do Outlook</span><span class="sxs-lookup"><span data-stu-id="5aadc-104">Find possible meeting times on the Outlook calendar</span></span>

<span data-ttu-id="5aadc-p102">Seja no trabalho ou em uma instituição de ensino, procurar um horário e local em comum para uma reunião geralmente significa uma sobrecarga. Os aplicativos do Microsoft Graph podem usar a ação [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-1.0) para identificar quaisquer possíveis horários de reunião que atendam aos requisitos de horário, local e outras restrições.</span><span class="sxs-lookup"><span data-stu-id="5aadc-p102">In a workplace or school, looking for a common time and place to meet often incurs overhead. Microsoft Graph applications can use [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-1.0) to identify any possible meeting times that satisfy time, location, and other constraints.</span></span>   

<span data-ttu-id="5aadc-p103">A ação **findMeetingTimes** permite especificar condições, como o intervalo de horário/data, a duração, os participantes opcionais ou obrigatórios, e a natureza da atividade (**activityDomain**). A ação leva em consideração a agenda de trabalho e o status de disponibilidade dos participantes e dos organizadores, e sugere horários apropriados para os participantes e o tipo de atividade. Por exemplo, as sugestões para uma atividade relacionada ao trabalho sempre ocorrem durante o horário de trabalho do organizador e dos participantes, e as sugestões em que os participantes obrigatórios estão disponíveis são classificadas mais acima na lista de sugestões.</span><span class="sxs-lookup"><span data-stu-id="5aadc-p103">The **findMeetingTimes** action lets you specify conditions such as the meeting date/time range, duration, optional or required attendees, and nature of the activity (**activityDomain**). The action takes into account the attendees' and organizer's normal work schedules and free/busy status, and suggests times that are appropriate for the participants and type of activity. For instance, suggestions for a work-related activity always occur during the work hours of the organizer and attendees, and suggestions where required attendees are available are ordered higher up in the suggested list.</span></span>

<span data-ttu-id="5aadc-p104">No Microsoft 365, as horas de trabalho e os fusos horários são configuráveis por caixa de correio. A ação **findMeetingTimes** lida com variações de fuso horário entre o organizador e os participantes. Por padrão, a ação **findMeetingTimes** retorna sugestões em UTC. Você pode usar o seguinte cabeçalho de solicitação para que a ação **findMeetingTimes** retorne sugestões expressas em um fuso horário específico.</span><span class="sxs-lookup"><span data-stu-id="5aadc-p104">In Microsoft 365, work hours and time zones are configurable per mailbox. The **findMeetingTimes** action handles time zone variations among the organizer and attendees. By default, **findMeetingTimes** returns suggestions in UTC. You can use the following request header to have **findMeetingTimes** return suggestions expressed in a specific time zone.</span></span>
``` http
Prefer: outlook.timezone="{time-zone-string}}"
```

<span data-ttu-id="5aadc-114">Especialmente útil para reuniões maiores, você pode especificar um percentual (**minimumAttendeePercentage**) de quorum e fazer com que **findMeetingTimes** retorne sugestões somente se essa disponibilidade mínima de participantes for atingida.</span><span class="sxs-lookup"><span data-stu-id="5aadc-114">Especially useful for larger meetings, you can specify a percentage (**minimumAttendeePercentage**) for a quorum and have **findMeetingTimes** return suggestions only if that minimum attendee availability is met.</span></span>

<span data-ttu-id="5aadc-p105">Se **findMeetingTimes** não puder sugerir nenhum horário de reunião, ele indicará um motivo específico (**emptySuggestionsReason**), como o organizador ou um participante obrigatório que não esteja disponível. Com base nesse valor, é possível ajustar melhor os parâmetros e a chamada **findMeetingTimes** novamente.</span><span class="sxs-lookup"><span data-stu-id="5aadc-p105">If **findMeetingTimes** cannot suggest any meeting times, it indicates a specific reason (**emptySuggestionsReason**), such as the organizer or a required attendee not available. Based on this value, you can better adjust the parameters and call **findMeetingTimes** again.</span></span>

><span data-ttu-id="5aadc-117">**Observação** A ação **findMeetingTimes** está atualmente disponível para caixas de correio de trabalho ou escolares da Microsoft 365, mas não para caixas de correio pessoais do outlook.com.</span><span class="sxs-lookup"><span data-stu-id="5aadc-117">**Note** The **findMeetingTimes** action is currently available to Microsoft 365 work or school mailboxes, but not personal, outlook.com mailboxes.</span></span>

## <a name="example"></a><span data-ttu-id="5aadc-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5aadc-118">Example</span></span>

<span data-ttu-id="5aadc-p106">O exemplo a seguir mostra como usar a ação **findMeetingTimes** para retornar horários para que 2 usuários se reúnam por algumas horas, levando em conta a agenda de trabalho e a disponibilidade dos usuários, e que o participante estará indisponível por parte do tempo. Como há apenas 2 usuários para esta reunião, as sugestões exigem 100% de participação. A seguir está a agenda de disponibilidade dos usuários.</span><span class="sxs-lookup"><span data-stu-id="5aadc-p106">The following example shows how to use **findMeetingTimes** to return possible times for 2 users to meet for a couple of hours, taking into account the users' free/busy and work schedules, and the attendee being away for part of the time. Because there are only 2 users for this meeting, suggestions require 100% attendance. The following shows the users' free/busy schedule.</span></span>

### <a name="organizers-calendar"></a><span data-ttu-id="5aadc-122">Calendário do organizador</span><span class="sxs-lookup"><span data-stu-id="5aadc-122">Organizer's calendar</span></span>

<span data-ttu-id="5aadc-123">![O calendário de trabalho do organizador para os dias 17 a 21 de abril, mostrando os horários disponíveis](./images/findmeetingtimes_organizer_free_busy.jpg "O calendário de trabalho do organizador para os dias 17 a 21 de abril, mostrando os horários livres")</span><span class="sxs-lookup"><span data-stu-id="5aadc-123">![The organizer's work calendar for April 17-21 showing free-busy times](./images/findmeetingtimes_organizer_free_busy.jpg "The organizer's work calendar for April 17-21 showing free-busy times")</span></span>

### <a name="attendees-calendar"></a><span data-ttu-id="5aadc-124">Calendário do participante</span><span class="sxs-lookup"><span data-stu-id="5aadc-124">Attendee's calendar</span></span>

<span data-ttu-id="5aadc-125">![O calendário de trabalho do participante para os dias 17 a 21 de abril, mostrando os horários disponíveis](./images/findmeetingtimes_attendee_free_busy.jpg "O calendário de trabalho do participante para os dias 17 a 21 de abril, mostrando os horários disponíveis")</span><span class="sxs-lookup"><span data-stu-id="5aadc-125">![The attendee's work calendar for April 17-21 showing free-busy times](./images/findmeetingtimes_attendee_free_busy.jpg "The attendee's work calendar for April 17-21 showing free-busy times")</span></span>

<span data-ttu-id="5aadc-126">O exemplo faz 2 chamadas para **findMeetingTimes**:</span><span class="sxs-lookup"><span data-stu-id="5aadc-126">The example makes 2 calls to **findMeetingTimes**:</span></span>

1. <span data-ttu-id="5aadc-p107">A primeira chamada analisa no intervalo de datas de 18 a 20 de abril. Como o participante estará ausente de 18 a 19 de abril e não há nenhum horário comum disponível em 20 de abril, a primeira chamada não retornará nenhuma sugestão, com o motivo (**emptySuggestionsReason**) que os participantes não estão disponíveis.</span><span class="sxs-lookup"><span data-stu-id="5aadc-p107">The first call looks in the date range of April 18-20. As the attendee is out-of-office on April 18-19, and there is no commonly available time on April 20, the first call returns no suggestions with the reason (**emptySuggestionsReason**) that attendees are not available.</span></span>
2. <span data-ttu-id="5aadc-129">A segunda chamada analisa a disponibilidade em 21 de abril e retorna uma sugestão das 14h às 16h.</span><span class="sxs-lookup"><span data-stu-id="5aadc-129">The second call looks for availability on April 21 and returns a suggestion of 2-4pm.</span></span>

<span data-ttu-id="5aadc-p108">As duas chamadas para **findMeetingTimes** incluem os seguintes parâmetros. Todos os [parâmetros](/graph/api/user-findmeetingtimes?view=graph-rest-1.0#request-body) para **findMeetingTimes** são opcionais.</span><span class="sxs-lookup"><span data-stu-id="5aadc-p108">The two calls to **findMeetingTimes** include the following parameters. All [parameters](/graph/api/user-findmeetingtimes?view=graph-rest-1.0#request-body) for **findMeetingTimes** are optional.</span></span>

- <span data-ttu-id="5aadc-132">**attendees**: um participante, Sara Melo, definido como `required` para a propriedade **type**</span><span class="sxs-lookup"><span data-stu-id="5aadc-132">**attendees**: one attendee, Samantha Booth, set as `required` for the **type** property</span></span>
- <span data-ttu-id="5aadc-133">**locationConstraint**: não requer nenhuma sugestão de localização</span><span class="sxs-lookup"><span data-stu-id="5aadc-133">**locationConstraint**: does not require any location suggestion</span></span>
- <span data-ttu-id="5aadc-134">**timeConstraint**: a primeira chamada analisa o intervalo de datas/horário de 18 de abril, às 9h, a 20 de abril, às 17h; depois que a primeira chamada não conseguir sugerir nenhum horário, a segunda chamada analisará 21 de abril, das 9h às 17h</span><span class="sxs-lookup"><span data-stu-id="5aadc-134">**timeConstraint**: the first call looks in the date/time range of April 18, 9am to April 20, 5pm; after the first call fails to suggest any times, the second call looks at April 21, 9am to 5pm</span></span>
- <span data-ttu-id="5aadc-135">**meetingDuration**: duas horas</span><span class="sxs-lookup"><span data-stu-id="5aadc-135">**meetingDuration**: two hours</span></span>
- <span data-ttu-id="5aadc-136">**returnSuggestionReasons**: este exemplo requer um motivo para cada sugestão</span><span class="sxs-lookup"><span data-stu-id="5aadc-136">**returnSuggestionReasons**: this example requires a reason for each suggestion</span></span>
- <span data-ttu-id="5aadc-137">**minimumAttendeePercentage**: 100%, uma vez que o participante deve ser capaz de participar de qualquer horário sugerido</span><span class="sxs-lookup"><span data-stu-id="5aadc-137">**minimumAttendeePercentage**: 100%, as the attendee must be able to attend for any suggested time</span></span>

### <a name="first-request"></a><span data-ttu-id="5aadc-138">Primeira solicitação</span><span class="sxs-lookup"><span data-stu-id="5aadc-138">First request</span></span>

<span data-ttu-id="5aadc-139">Procure por um intervalo de tempo disponível de 2 horas para ambos os usuários de 18 a 20 abril.</span><span class="sxs-lookup"><span data-stu-id="5aadc-139">Look for a 2-hour free time slot for both users over April 18-20.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "findmeetingtimes_example_first"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/findMeetingTimes
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json

{ 
  "attendees": [ 
    { 
      "type": "required",  
      "emailAddress": { 
        "name": "Samantha Booth",
        "address": "samanthab@contoso.onmicrosoft.com" 
      } 
    }
  ],  
  "locationConstraint": { 
    "isRequired": false,  
    "suggestLocation": false,  
    "locations": [ 
      { 
        "resolveAvailability": false,
        "displayName": "Conf room Hood" 
      } 
    ] 
  },  
  "timeConstraint": {
    "activityDomain":"work", 
    "timeslots": [ 
      { 
        "start": { 
          "dateTime": "2017-04-18T09:00:00",  
          "timeZone": "Pacific Standard Time" 
        },  
        "end": { 
          "dateTime": "2017-04-20T17:00:00",  
          "timeZone": "Pacific Standard Time" 
        } 
      } 
    ] 
  },  
  "meetingDuration": "PT2H",
  "returnSuggestionReasons": true,
  "minimumAttendeePercentage": 100
}
```

### <a name="first-response"></a><span data-ttu-id="5aadc-140">Primeira resposta</span><span class="sxs-lookup"><span data-stu-id="5aadc-140">First response</span></span>
<span data-ttu-id="5aadc-141">Não há nenhum intervalo de 2 horas durante o horário de trabalho de 18 a 20 de abril em que ambos os usuários estejam disponíveis.</span><span class="sxs-lookup"><span data-stu-id="5aadc-141">There is no 2-hour time slot during the work hours of April 18-20 when both users are available.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.meetingTimeSuggestionsResult",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.timezone="Pacific Standard Time"
Content-Length: 184

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.meetingTimeSuggestionsResult",
    "emptySuggestionsReason":"AttendeesUnavailable",
    "meetingTimeSuggestions":[

    ]
}
```

### <a name="second-request"></a><span data-ttu-id="5aadc-142">Segunda solicitação</span><span class="sxs-lookup"><span data-stu-id="5aadc-142">Second request</span></span>
<span data-ttu-id="5aadc-143">Procure um intervalo de tempo de 2 horas em 21 de abril.</span><span class="sxs-lookup"><span data-stu-id="5aadc-143">Look for a 2-hour time slot on April 21.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "findmeetingtimes_example_second"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/findMeetingTimes
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json

{ 
  "attendees": [ 
    { 
      "type": "required",  
      "emailAddress": { 
        "name": "Samantha Booth",
        "address": "samanthab@contoso.onmicrosoft.com" 
      } 
    }
  ],  
  "locationConstraint": { 
    "isRequired": false,  
    "suggestLocation": false,  
    "locations": [ 
      { 
        "resolveAvailability": false,
        "displayName": "Conf room Hood" 
      } 
    ] 
  },  
  "timeConstraint": {
    "activityDomain":"work", 
    "timeslots": [ 
      { 
        "start": { 
          "dateTime": "2017-04-21T09:00:00",  
          "timeZone": "Pacific Standard Time" 
        },  
        "end": { 
          "dateTime": "2017-04-21T17:00:00",  
          "timeZone": "Pacific Standard Time" 
        } 
      } 
    ] 
  },  
  "meetingDuration": "PT2H",
  "returnSuggestionReasons": true,
  "minimumAttendeePercentage": 100
}
```

### <a name="second-response"></a><span data-ttu-id="5aadc-144">Segunda resposta</span><span class="sxs-lookup"><span data-stu-id="5aadc-144">Second response</span></span>
<span data-ttu-id="5aadc-145">A segunda solicitação **findMeetingTimes** sugere de 21 de abril, das 14h às 16h, para que os dois usuários se reúnam.</span><span class="sxs-lookup"><span data-stu-id="5aadc-145">The second **findMeetingTimes** request suggests April 21, 2-4pm for both users to meet.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.meetingTimeSuggestionsResult",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.timezone="Pacific Standard Time"
Content-Length: 714

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.meetingTimeSuggestionsResult",
    "emptySuggestionsReason":"",
    "meetingTimeSuggestions":[
        {
            "confidence":100.0,
            "organizerAvailability":"free",
            "suggestionReason":"Suggested because it is one of the nearest times when all attendees are available.",
            "meetingTimeSlot":{
                "start":{
                    "dateTime":"2017-04-21T14:00:00.0000000",
                    "timeZone":"Pacific Standard Time"
                },
                "end":{
                    "dateTime":"2017-04-21T16:00:00.0000000",
                    "timeZone":"Pacific Standard Time"
                }
            },
            "attendeeAvailability":[
                {
                    "availability":"free",
                    "attendee":{
                        "type":"required",
                        "emailAddress":{
                            "address":"samanthab@contoso.onmicrosoft.com"
                        }
                    }
                }
            ],
            "locations":[
                {
                    "displayName":"Conf room Hood"
                }
            ]
        }
    ]
}
```



## <a name="next-steps"></a><span data-ttu-id="5aadc-146">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="5aadc-146">Next steps</span></span>

<span data-ttu-id="5aadc-p109">Há momentos em que nem todos os participantes podem participar de uma reunião. Você pode fazer com que a ação **findMeetingTimes** sugira um horário se a _confiança_ para a presença atingir um certo percentual, especificando o parâmetro opcional **minimumAttendeePercentage**. Saiba mais sobre a [confiança de uma sugestão de reunião](/graph/api/user-findmeetingtimes?view=graph-rest-1.0#the-confidence-of-a-meeting-suggestion) e outros [parâmetros](/graph/api/user-findmeetingtimes?view=graph-rest-1.0#request-body), e aplique-os conforme apropriado para reuniões maiores.</span><span class="sxs-lookup"><span data-stu-id="5aadc-p109">There are times when not all attendees can attend a meeting. You can have **findMeetingTimes** suggest a time if the _confidence_ for attendance reaches a certain percentage, by specifying the **minimumAttendeePercentage** optional parameter. Learn more about the [confidence of a meeting suggestion](/graph/api/user-findmeetingtimes?view=graph-rest-1.0#the-confidence-of-a-meeting-suggestion) and other [parameters](/graph/api/user-findmeetingtimes?view=graph-rest-1.0#request-body), and apply them as appropriate for meetings of larger sizes.</span></span>

<span data-ttu-id="5aadc-150">Depois de receber sugestões de horário de reunião, você talvez queira:</span><span class="sxs-lookup"><span data-stu-id="5aadc-150">After getting meeting time suggestions, you may want to:</span></span>

1. <span data-ttu-id="5aadc-151">[Criar um evento e enviá-lo como uma solicitação de reunião](/graph/api/user-post-events?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="5aadc-151">[Create an event and send it as a meeting request](/graph/api/user-post-events?view=graph-rest-1.0).</span></span>
2. <span data-ttu-id="5aadc-152">[Adicionar um anexo](/graph/api/event-post-attachments?view=graph-rest-1.0) a um evento.</span><span class="sxs-lookup"><span data-stu-id="5aadc-152">[Add an attachment](/graph/api/event-post-attachments?view=graph-rest-1.0) to the event.</span></span>

<span data-ttu-id="5aadc-153">Veja mais detalhes em [integração com o calendário do Outlook](outlook-calendar-concept-overview.md).</span><span class="sxs-lookup"><span data-stu-id="5aadc-153">Find out more about [integrating with Outlook calendar](outlook-calendar-concept-overview.md).</span></span>
