---
title: 'user: findMeetingTimes'
description: Localize as sugestões de hora da reunião com base no organizador e na disponibilidade dos participantes, assim como nas restrições de horário ou local especificadas como parâmetros.
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 64149cc41235a1eafa2ac763b1ee676787f7d28b
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292305"
---
# <a name="user-findmeetingtimes"></a>user: findMeetingTimes

Namespace: microsoft.graph

Localize as sugestões de hora da reunião com base no organizador e na disponibilidade dos participantes, assim como nas restrições de horário ou local especificadas como parâmetros.

Se **findMeetingTimes** não retorna nenhuma sugestão de reunião, a resposta seria indicar um motivo na propriedade **emptySuggestionsReason**. Com base nesse valor, é possível ajustar melhor os parâmetros e a chamada **findMeetingTimes** novamente.

O algoritmo usado para ilustrar horários de reunião e locais passa por ajuste fino de tempos em tempos. Cenários como ambientes de teste onde permanecem estáticos parâmetros de entrada e dados de calendário, espere que os resultados sugeridos sejam diferentes ao longo do tempo.


## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Calendars.Read.Shared, Calendars.ReadWrite.Shared    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /me/findMeetingTimes
POST /users/{id|userPrincipalName}/findMeetingTimes
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Valor|
|:---------------|:----------|
| Autorização  | {token} de portador. Obrigatório. |
| Prefira: outlook.timezone | Uma cadeia de caracteres que representa um fuso horário específico para a resposta; por exemplo, "Hora Oficial do Pacífico". Opcional. UTC será usado se esse cabeçalho não for especificado.|

## <a name="request-body"></a>Corpo da solicitação
Todos os parâmetros suportados estão listados abaixo. Dependendo do cenário, especifique um objeto JSON para cada um dos parâmetros necessários no corpo da solicitação. 


| Parâmetro    | Tipo   |Descrição|
|:---------------|:--------|:----------|
|attendees|Coleção [attendeeBase](../resources/attendeebase.md)|Uma coleção de participantes ou recursos da reunião. Como findMeetingTimes pressupõe que qualquer participante que seja uma pessoa será sempre obrigatório, especifique `required` para uma pessoa e `resource` para um recurso na propriedade **type** correspondente. Uma coleção vazia faz com que **findMeetingTimes** procure gratuitamente alocações de tempo somente para o organizador. Opcional.|
|isOrganizerOptional|Edm.Boolean|Especifique `True` se o organizador não tiver necessariamente que participar. O padrão é `false`. Opcional.|
|locationConstraint|[locationConstraint](../resources/locationconstraint.md)|Os requisitos do organizador sobre o local da reunião, tal como se é necessário sugerir de um local de encontro, ou há locais específicos apenas onde a reunião pode ocorrer. Opcional.|
|maxCandidates|Edm.Int32|O número máximo de sugestões de horários de reunião a ser retornados. Opcional.|
|meetingDuration|Edm.Duration|A duração da reunião, indicada no formato [ISO8601](https://www.iso.org/iso/iso8601). Por exemplo, 1 hora é indicada como "PT1H", onde "P" é o designador de duração, "T" é o designador de horário e "H" é o designador de hora. Use M para indicar os minutos da duração; por exemplo, 2 horas e 30 minutos seria “PT2H30M”. Se a duração da reunião não for especificada, **findMeetingTimes** usará o padrão de 30 minutos. Opcional.|
|minimumAttendeePercentage|Edm.Double| O mínimo necessário de [confiança](#the-confidence-of-a-meeting-suggestion) para um intervalo de tempo a ser retornado na resposta. É um valor de % variando de 0 a 100. Opcional.|
|returnSuggestionReasons|Edm.Boolean|Especifique `True` para retornar um motivo para cada sugestão de reunião na propriedade **suggestionReason**. O padrão é `false` para não retornar essa propriedade. Opcional.|
|timeConstraint|[timeConstraint](../resources/timeconstraint.md)|Qualquer restrição de tempo para uma reunião, o que pode incluir a natureza da reunião (propriedade **activityDomain**) e possíveis intervalos de tempo da reunião (propriedade **timeSlots**). **findMeetingTimes** pressupõe **activityDomain** como `work` se você não especificar este parâmetro. Opcional.|

A tabela a seguir descreve as restrições **activityDomain** que você pode especificar ainda mais no parâmetro **timeConstraint**.

|Valor activityDomain|Sugestões de horário para reuniões|
|:-----|:-----|
|trabalho| As sugestões são nas horas de trabalho do usuário que são definidas na configuração do calendário do usuário e podem ser personalizadas pelo usuário ou administrador. As horas de trabalho padrão são de segunda a sexta, das 8h às 17h, no fuso horário definido para a caixa de correio. Este é o valor padrão se nenhum **activityDomain** for especificado. |
|pessoal| As sugestões são dentro das horas de trabalho do usuário, e sábado e domingo. O padrão é de segunda a sexta, das 8h às 17h, na configuração de fuso horário da caixa de correio.|
|irrestrito | As sugestões podem ser todas as horas do dia, todos os dias da semana.|
|desconhecido | Não use esse valor, uma vez que ele será substituído no futuro. Atualmente, se comporta da mesma forma que o `work`. Altere qualquer código existente para usar o `work`, `personal` ou `unrestricted` conforme apropriado.


Com base nos parâmetros especificados,**findMeetingTimes** verifica o status disponível/ocupado nos calendários principais do organizador e dos participantes. A ação calcula os melhores possíveis horários de reuniões e retorna as sugestões de reunião.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna o código de resposta `200 OK` e o recurso [meetingTimeSuggestionsResult](../resources/meetingtimesuggestionsresult.md) no corpo da resposta. 

Um **meetingTimeSuggestionsResult** inclui uma coleção de sugestões de reunião e uma propriedade **emptySuggestionsReason**. Cada sugestão é definida como uma [meetingTimeSuggestion](../resources/meetingtimesuggestion.md), e participantes com um nível de confiança de 50% na média para participar ou uma % específica que definida no parâmetro **minimumAttendeePercentage**. 

Por padrão, cada sugestão de horário de reunião é retornado em UTC. 

Se **findMeetingTimes** não retorna nenhuma sugestão de reunião, a resposta seria indicar um motivo na propriedade **emptySuggestionsReason**. Com base nesse valor, é possível ajustar melhor os parâmetros e a chamada **findMeetingTimes** novamente.

### <a name="the-confidence-of-a-meeting-suggestion"></a>A confiança de uma sugestão de reunião

A propriedade **confidence** de uma **meetingTimeSuggestion** varia de 0% a 100% e representa a chance de que todos os participantes compareçam à reunião, com base em seu status disponível/ocupado:

- Para cada participante, um status livre para um período de tempo de reunião especificado corresponde à chance de 100% de presença, status desconhecido 49% e status ocupado 0%.
- A confiança na sugestão de um horário de reunião é calculada pela média da chance de presença de todos os participantes especificados para essa reunião.
- Você pode usar o parâmetro opcional **minimumAttendeePercentage** **findMeetingTimes** para especificar que apenas as sugestões de horário da reunião com pelo menos determinado nível de confiança retornem. Por exemplo, você pode especificar uma **minimumAttendeePercentage** de 80% se você quiser apenas sugestões que tenham uma chance de 80% ou mais de que todos os participantes comparecerão. Se você não especificar **minimumAttendeePercentage**, **findMeetingTimes** pressupõe um valor de 50%.
- Se houver diversas sugestões de horário de reunião, a ação **findMeetingTimes** primeiramente classifica as sugestões por seu valor de confiança computado que vai de alto para baixo. Se houver sugestões com a mesma confiança, a ação ordena essas sugestões em ordem cronológica.

Por exemplo, se uma sugestão de horário de reunião envolve três participantes com o seguinte status livre/ocupado:

|**Participante**|**Status disponível/ocupado**|**% de chance de comparecer**|
|:-----|:-----|:-----|
|Sara | Disponível | 100% |
|Davi | Desconhecido | 49% |
|Sara | Ocupado | 0% |

Então a confiança na sugestão do horário da reunião, que corresponde à chance média de presença, é (100% + 49% + 0%) /3 = 49.66%.

Se você especificar um **minimumAttendeePercentage** de 80% em uma operação **findMeetingTimes**, pois 49,66%< 80%, a operação não sugerirá esse horário na resposta.

## <a name="example"></a>Exemplo

O exemplo a seguir mostra como encontrar um horário para reunir-se em um local predeterminado e solicitar um motivo para cada sugestão, especificando os seguintes parâmetros no corpo da solicitação:

- **attendees**
- **locationConstraint**
- **timeConstraint**
- **isOrganizerOptional**
- **meetingDuration**
- **returnSuggestionReasons**
- **minimumAttendeePercentage**

Definindo o parâmetro **returnSuggestionReasons**, você também obtém uma explicação na propriedade **suggestionReason** para cada sugestão, se **findMeetingTimes** retornar qualquer sugestão.

Observe que a solicitação especifica o tempo no fuso horário PST. Por padrão, a resposta retorna horário em sugestões UTC. Você pode usar o cabeçalho `Prefer: outlook.timezone` para especificar os valores de horário para o Horário Padrão do Pacífico na resposta.

##### <a name="request"></a>Solicitação
Aqui está a solicitação de exemplo.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_findmeetingtimes"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/findMeetingTimes
Prefer: outlook.timezone="Pacific Standard Time"
Content-Type: application/json

{ 
  "attendees": [ 
    { 
      "type": "required",  
      "emailAddress": { 
        "name": "Alex Wilbur",
        "address": "alexw@contoso.onmicrosoft.com" 
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
    "timeSlots": [ 
      { 
        "start": { 
          "dateTime": "2019-04-16T09:00:00",  
          "timeZone": "Pacific Standard Time" 
        },  
        "end": { 
          "dateTime": "2019-04-18T17:00:00",  
          "timeZone": "Pacific Standard Time" 
        } 
      } 
    ] 
  },  
  "isOrganizerOptional": "false",
  "meetingDuration": "PT1H",
  "returnSuggestionReasons": "true",
  "minimumAttendeePercentage": "100"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-findmeetingtimes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-findmeetingtimes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-findmeetingtimes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-findmeetingtimes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Resposta
Aqui está uma resposta de exemplo. Observação: O objeto da resposta mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.meetingTimeSuggestionsResult",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.timezone="Pacific Standard Time"

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.meetingTimeSuggestionsResult",
    "emptySuggestionsReason": "",
    "meetingTimeSuggestions": [
        {
            "confidence": 100,
            "order": 1,
            "organizerAvailability": "free",
            "suggestionReason": "Suggested because it is one of the nearest times when all attendees are available.",
            "attendeeAvailability": [
                {
                    "availability": "free",
                    "attendee": {
                        "emailAddress": {
                            "address": "alexw@contoso.onmicrosoft.com"
                        }
                    }
                }
            ],
            "locations": [
                {
                    "displayName": "Conf room Hood"
                }
            ],
            "meetingTimeSlot": {
                "start": {
                    "dateTime": "2019-04-18T16:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                },
                "end": {
                    "dateTime": "2019-04-18T17:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                }
            }
        },
        {
            "confidence": 100,
            "order": 2,
            "organizerAvailability": "free",
            "suggestionReason": "Suggested because it is one of the nearest times when all attendees are available.",
            "attendeeAvailability": [
                {
                    "availability": "free",
                    "attendee": {
                        "emailAddress": {
                            "address": "alexw@contoso.onmicrosoft.com"
                        }
                    }
                }
            ],
            "locations": [
                {
                    "displayName": "Conf room Hood"
                }
            ],
            "meetingTimeSlot": {
                "start": {
                    "dateTime": "2019-04-18T08:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                },
                "end": {
                    "dateTime": "2019-04-18T09:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                }
            }
        },
        {
            "confidence": 100,
            "order": 3,
            "organizerAvailability": "tentative",
            "suggestionReason": "Suggested because it is one of the nearest times when all attendees are available.",
            "attendeeAvailability": [
                {
                    "availability": "free",
                    "attendee": {
                        "emailAddress": {
                            "address": "alexw@contoso.onmicrosoft.com"
                        }
                    }
                }
            ],
            "locations": [
                {
                    "displayName": "Conf room Hood"
                }
            ],
            "meetingTimeSlot": {
                "start": {
                    "dateTime": "2019-04-18T15:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                },
                "end": {
                    "dateTime": "2019-04-18T16:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                }
            }
        },
        {
            "confidence": 100,
            "order": 4,
            "organizerAvailability": "tentative",
            "suggestionReason": "Suggested because it is one of the nearest times when all attendees are available.",
            "attendeeAvailability": [
                {
                    "availability": "free",
                    "attendee": {
                        "emailAddress": {
                            "address": "alexw@contoso.onmicrosoft.com"
                        }
                    }
                }
            ],
            "locations": [
                {
                    "displayName": "Conf room Hood"
                }
            ],
            "meetingTimeSlot": {
                "start": {
                    "dateTime": "2019-04-18T09:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                },
                "end": {
                    "dateTime": "2019-04-18T10:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                }
            }
        },
        {
            "confidence": 100,
            "order": 5,
            "organizerAvailability": "tentative",
            "suggestionReason": "Suggested because it is one of the nearest times when all attendees are available.",
            "attendeeAvailability": [
                {
                    "availability": "free",
                    "attendee": {
                        "emailAddress": {
                            "address": "alexw@contoso.onmicrosoft.com"
                        }
                    }
                }
            ],
            "locations": [
                {
                    "displayName": "Conf room Hood"
                }
            ],
            "meetingTimeSlot": {
                "start": {
                    "dateTime": "2019-04-18T12:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                },
                "end": {
                    "dateTime": "2019-04-18T13:00:00.0000000",
                    "timeZone": "Pacific Standard Time"
                }
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: findMeetingTimes",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
      "Error: user_findmeetingtimes/meetingTimeSuggestions/member/confidence:\r\n
      Expected type Double but actual was Int64. Property: confidence, actual value: '100'"
  ],
  "tocPath": ""
}-->

