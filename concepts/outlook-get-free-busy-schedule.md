---
title: Obter agenda de disponibilidade de usuários e recursos do calendário do Outlook
description: Use a ação getSchedule para obter as informações de disponibilidade de um ou mais usuários, listas de distribuição ou recursos por um período específico.
author: tariq-sharif
ms.localizationpriority: high
ms.prod: outlook
ms.openlocfilehash: 263e3b5462b688f0dff98714bd646a247dde9765
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66439029"
---
# <a name="get-freebusy-schedule-of-outlook-calendar-users-and-resources"></a>Obter agenda de disponibilidade de usuários e recursos do calendário do Outlook

Em uma configuração de escola ou trabalho, um cenário comum é ver quando um usuário está livre para um reunião, ou então pesquisar a disponibilidade de uma equipe, sala ou equipamento para um período de tempo.

A [ação getSchedule](/graph/api/calendar-getschedule) permite que você obtenha as informações de disponibilidade de uma ou mais entidades&mdash;usuários, listas de distribuição ou recursos&mdash;por um período específico.

## <a name="example"></a>Exemplo

Um exemplo simples é encontrar a agenda de horários livres/ocupados de um colega de trabalho, Alex, em um dia específico, das 9 às 18 horas, Fuso Horário Padrão do Pacífico (PST):

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

**getSchedule** retorna dois itens de agenda que correspondem aos eventos existentes no calendário padrão do Alex, mostrando os horários de início e término de cada evento e seu status de disponibilidade. Você poderá supor que Alex está livre pelo restante do tempo desse intervalo de data/hora.

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

Além da disponibilidade da agenda e das horas de trabalho do Alex, **getSchedule** também retorna **availabilityView**, que é uma visualização mesclada da disponibilidade do Alex a cada dia. O modo de exibição mesclado é uma cadeia de caracteres que consiste em intervalos de tempo abrangendo aquele dia, sendo que cada intervalo de tempo indica a disponibilidade do Alex usando a seguinte convenção: 

- `0` = livre
- `1` = provisório
- `2` = ocupado
- `3` = ausência temporária
- `4`= trabalhando em outro lugar. 

Por padrão, a duração de cada intervalo de tempo é de 30 minutos. Este exemplo usa a propriedade **availabilityViewInterval** para personalizar o intervalo de tempo para 15 minutos.

## <a name="how-does-getschedule-compare-with-findmeetingtimes"></a>Como o getSchedule se compara ao findMeetingTimes

A ação [findMeetingTimes](/graph/api/user-findmeetingtimes) é semelhante a **getSchedule** pelo fato de que as duas leem o status de disponibilidade e as horas de trabalho de usuários e recursos específicos. As duas ações são diferentes de algumas maneiras principais.

### <a name="application"></a>Aplicação

**findMeetingTimes** aplica determinada lógica de negócios para sugerir horários e locais de reunião, como:

- Participação opcional ou obrigatória de cada entidade
- A natureza da atividade solicitada para a hora do dia
- A participação mínima necessária para o quórum da reunião

É apropriada para cenários que dependem de [simplificação de reservas de compromissos](findmeetingtimes-example.md).

O **getSchedule** simplesmente retorna o status de disponibilidade dos eventos existentes em cada calendário solicitado por um determinado período de tempo e supõe que o tempo restante daquele período de tempo esteja livre. Você deve aplicar mais lógica de negócios para fazer uso desses dados para completar seu cenário.

### <a name="app-only-support"></a>Suporte somente aplicativo

**findmeetingtimes** dá suporte somente a cenários delegados que exigem que o usuário se conecte ao aplicativo. O aplicativo pode ler eventos apenas nos calendários que o usuário conectado pode acessar. Isso pode incluir os calendários que outros usuários delegaram ou compartilharam com o usuário conectado.

**getSchedule** é compatível com o cenários delegados e somente aplicativo. No último, o administrador consente que o aplicativo acesse todos os calendários sem um usuário conectado.

### <a name="permissions"></a>Permissões
A permissão menos privilegiada exigida pelo **findmeetingtimes** é Calendars.Read.Shared.

A permissão menos privilegiada exigida por **getSchedule** é Calendars.Read. 

### <a name="version-support"></a>Suporte para versões

O **findmeetingtimes** e o **getSchedule** estão geralmente disponíveis e adequados para uso em aplicativos de produção.


## <a name="event-data-returned"></a>Dados de evento retornados
A permissão menos privilegiada exigida por **getSchedule** para que um aplicativo obtenha informações de disponibilidade é Calendars.Read. Dependendo do cenário do aplicativo, este consentimento pode vir do usuário conectado ou do administrador.

Embora a permissão consentida permite com que um aplicativo use o **getSchedule** nos calendários dos usuários solicitados pelo Outlook, o usuário solicitado controla quais dados de evento, caso existam, o **getSchedule** retornará. 

Por exemplo, o **getSchedule** pode retornar o status de disponibilidade e as horas de trabalho dos usuários solicitados ou também retornar as propriedades **subject**, **location**, e **isPrivate** de um evento, desde que:

- O evento esteja marcado com um nível de confidencialidade baixo - `normal` ou `personal`- E uma ou mais das seguintes condições se aplicam:

  - As configurações de calendário do usuário solicitado permitem com que o usuário conectado veja as linhas de assunto e localizações
  - O calendário do usuário solicitado é compartilhado com o usuário conectado

Estas condições se aplicam independentemente se o usuário conectado é um administrador na organização. O usuário solicitado tem controle sobre os dados de eventos retornados.

## <a name="time-zone-representation"></a>Representação de fuso horário
Por padrão, as horas de início e de término de itens de agenda retornado são representados em UTC. Você pode usar um `Prefer` cabeçalho para especificar um fuso horário apropriado para o aplicativo. Como exemplo: 
``` http
Prefer: outlook.timezone="Pacific Standard Time"
```

## <a name="limits-and-error-conditions"></a>Limites e condições do erro
Fique atento para os seguintes limites e condições de erro:

- **getSchedule** pode dar suporte procurando informações sobre disponibilidade para até 20 entidades ao mesmo tempo. Este limite se aplica ao número de usuários identificados individualmente ou como membros de uma lista de distribuição, e também ao número de recursos.
- O período de tempo para pesquisar deve ser menor que 42 dias.
- Se **getSchedule** não puder identificar um usuário ou um recurso especificados, ela retornará um item de agenda único e indicará o erro 


## <a name="see-also"></a>Confira também
- [Referência de permissões](permissions-reference.md#calendars-permissions)
- [Encontrar possíveis horários de reunião no calendário do Outlook](findmeetingtimes-example.md)
