# <a name="get-outlook-events-in-a-shared-or-delegated-calendar"></a>Obter eventos do Outlook em um calendário compartilhado ou delegado

No Outlook, os clientes podem compartilhar um calendário com outros usuários e permitir que visualizem ou modifiquem os eventos nele. Os clientes também podem nomear um representante para agir em nome deles, para receber ou responder a solicitações de reunião, ou criar e alterar itens do calendário.

Via programação, o Microsoft Graph oferece suporte para obter eventos em calendários compartilhados por outros usuários, bem como para obter o próprio calendário compartilhado. O suporte também se aplica a calendários que foram delegados.

Por exemplo, Garth compartilhou com John seu calendário padrão com acesso de leitura. Se o John entrar no seu aplicativo e apresentar permissões delegadas (Calendars.Read.Shared ou Calendars.ReadWrite.Shared), o seu aplicativo será capaz de acessar o calendário padrão do Garth e os eventos contidos nele, conforme descrito abaixo.

## <a name="get-an-event-in-the-shared-calendar"></a>Obter um evento no calendário compartilhado

Você pode obter um evento específico no calendário padrão compartilhado por Garth:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events/{id}
```

Após a conclusão bem-sucedida, você obterá HTTP 200 OK e a instância [event](../api-reference/v1.0/resources/event.md) identificada por `{id}` do calendário padrão do Garth.

## <a name="get-all-the-events-in-the-shared-calendar"></a>Obter todos os eventos no calendário compartilhado

Obtenha todos os eventos no calendário padrão que Garth compartilhou com John:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events
```

Após a conclusão bem-sucedida, você obterá HTTP 200 OK e um conjunto de instâncias [event](../api-reference/v1.0/resources/event.md) no calendário padrão do Garth.

## <a name="get-the-shared-calendar"></a>Obter o calendário compartilhado

Obtenha o calendário padrão que Garth compartilhou com John.

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar
```

Após a conclusão bem-sucedida, você obterá HTTP 200 OK e uma instância [calendar](../api-reference/v1.0/resources/calendar.md) que representa a pasta padrão do Garth.

Os mesmos recursos de GET se aplicam se Garth delegar a John mais acesso ao seu calendário padrão ou se delegar toda a caixa de correio.

Se Garth não tiver compartilhado seu calendário padrão com John, nem delegado sua caixa de correio, especificando a identificação de usuário do John ou o nome UPN, essas operações GET retornarão um erro. 


## <a name="next-steps"></a>Próximas etapas

Saiba mais sobre:

- [Por que integrar-se com o calendário do Outlook](outlook-calendar-concept-overview.md)
- A [API de calendário](../api-reference/v1.0/resources/calendar.md) no Microsoft Graph v1.0.