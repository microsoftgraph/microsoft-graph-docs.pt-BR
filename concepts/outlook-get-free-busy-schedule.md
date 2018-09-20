# <a name="get-freebusy-schedule-of-users-and-resources-preview"></a>Obtenha a agenda de disponibilidade livre/ocupado de usuários e recursos (versão prévia)

Em um ambiente de trabalho ou escola, um cenário comum é ver quando um usuário está livre para reuniões ou procurar a disponibilidade de uma equipe, sala ou equipamento para um período de tempo.

A ação [getSchedule](../api-reference/beta/api/calendar_getschedule.md) permite que você obtenha as informações de disponibilidade de uma ou mais entidades - usuários, listas de distribuição ou recursos - para um período de tempo específico. 

## <a name="example"></a>Exemplo

Um exemplo simples é encontrar a agenda de disponibilidade de um colega de trabalho, Alex, em um dia específico, das 9h às 18h, horário padrão do Pacífico:

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

**getSchedule** retorna dois itens de agenda que correspondem aos eventos existentes no calendário padrão do Alex, mostrando os horários de início e término de cada evento e seu status de disponibilidade livre/ocupado. Você pode assumir que Alex está livre pelo tempo restante nesse intervalo de data/hora.

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

Além da agenda de livre/ocupado e o horário de trabalho de Alex, **getSchedule** também retornará **availabilityView**, que é uma exibição mesclada da disponibilidade de Alex naquele dia. A visualização mesclada é uma sequência de caracteres que consiste em intervalos de tempo que cobrem esse dia, e cada intervalo de tempo indica a disponibilidade de Alex usando a seguinte convenção: 

- `0`= disponível
- `1`= provisório
- `2`= ocupado
- `3`= ausência temporária
- `4`= trabalhando em outros lugares. 

Por padrão, a duração de cada intervalo de tempo é de 30 minutos. Este exemplo usa a propriedade **availabilityViewInterval** para personalizar o intervalo de tempo para 15 minutos.

## <a name="how-is-getschedule-different-from-findmeetingtimes"></a>Como getSchedule é diferente do findMeetingTimes

A ação [findMeetingTimes](../api-reference/v1.0/api/user_findmeetingtimes.md) é semelhante ao **getSchedule** em que ambos leem o status de disponibilidade livre/ocupado e o horário de trabalho de usuários e de recursos especificados. As duas ações diferem de algumas maneiras principais.

### <a name="application"></a>Aplicativo

**findMeetingTimes** aplica determinada lógica de negócios para sugerir horários e locais de reunião, como:

- Participação opcional ou obrigatória de cada entidade
- A natureza da atividade solicitada para a hora do dia
- A presença mínima necessária para um quorum para uma reunião

Ele é adequado para cenários que dependem [da simplificação da reserva de compromissos](findmeetingtimes_example.md).

**getSchedule** simplesmente retorna o status livre/ocupado dos eventos existentes em cada um dos calendários solicitados para um determinado período e supõe que o tempo restante nesse período de tempo está livre. Em seguida, você aplicaria mais lógica de negócios para usar esses dados para concluir seu cenário.

### <a name="app-only-support"></a>Suporte apenas a aplicativos

**findmeetingtimes** suporta apenas cenários delegados que exigem que um usuário entre no aplicativo. O aplicativo pode ler eventos apenas nos calendários que o usuário conectado pode acessar. Isso pode incluir calendários que outros usuários delegaram ou compartilharam com o usuário conectado.

**getSchedule** suporta cenários delegados e somente aplicativos. Neste último, um administrador consente que o aplicativo acesse todos os calendários sem um usuário conectado.


### <a name="version-support"></a>Suporte à versão

**findmeetingtimes** geralmente está disponível para todos os aplicativos. 

**getSchedule** está disponível atualmente [no status de visualização](versioning_and_support.md#beta-version)e, portanto, não é apropriado para uso em aplicativos de produção.


## <a name="permissions"></a>Permissões
A permissão com menos privilégios que você precisa para obter informações de livre/ocupado é Calendar.Read. Dependendo do cenário do aplicativo, isso pode ser permitido pelo usuário ou administrador conectado.
Além do status livre/ocupado e do horário de trabalho das entidades solicitadas, **getSchedule** também pode retornar o assunto e o local de um evento, desde que:

- Se o evento é marcado com o nível de confidencialidade baixo - `normal` ou `personal` e uma ou mais das seguintes condições se aplicam:

- As configurações de calendário do usuário solicitado permitem que todos os usuários da organização visualizem títulos e locais
- O calendário do usuário solicitado é compartilhado com o usuário conectado
- O usuário conectado é um administrador da mesma organização que o usuário solicitado.

## <a name="time-zone-representation"></a>Representação de fuso horário
Por padrão, os horários de início e término dos itens de agendamento retornados são representados em UTC. Você pode usar um `Prefer` cabeçalho para especificar um fuso horário apropriado para seu aplicativo. Como exemplo: 
```
Prefer: outlook.timezone="Pacific Standard Time"
```

## <a name="limits-and-error-conditions"></a>Limites e condições de erro
Esteja ciente dos seguintes limites e condições de erro:

- **getSchedule** pode suportar a procura de informações de disponibilidade de livre/ocupado para até 20 entidades ao mesmo tempo. Esse limite se aplica ao número de usuários identificados individualmente ou como membros de uma lista de distribuição e também ao número de recursos.
- O período de tempo para procurar deve ser inferior a 42 dias.
- Se **getSchedule** não é possível identificar um usuário ou recurso especificado, ele retorna um único item de agenda e indica o erro. 

## <a name="see-also"></a>Veja também
- [Referência de permissões](permissions_reference.md#calendars-permissions)
- [Encontrar possíveis horários de reunião no calendário do Outlook](findmeetingtimes_example.md)
