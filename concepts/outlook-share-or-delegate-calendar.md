---
title: Compartilhar ou delegar um calendário no Outlook
description: No Outlook, um proprietário de calendário pode compartilhá-lo com outro usuário ou delegar outro usuário para gerenciar reuniões no calendário principal do proprietário.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 26319854c20401d96f94a5fa6735777a1645d2a9
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013650"
---
# <a name="share-or-delegate-a-calendar-in-outlook"></a>Compartilhar ou delegar um calendário no Outlook

No Outlook, o proprietário do calendário pode compartilhá-lo com outro usuário. O proprietário pode especificar quais informações em eventos não particulares podem ser visualizadas e pode conceder acesso de gravação para os usuários na mesma organização. 

O proprietário também pode delegar outro usuário a gerenciar reuniões no calendário _principal_ do proprietário. Delegados são sharees que podem visualizar todas as informações e ter acesso de gravação a eventos não privados. Eles também recebem solicitações de reunião e respostas, além de responder a solicitações de reunião em nome do proprietário. Além disso, o proprietário pode conceder permissões explícitas a delegados para exibir os eventos _particulares_ do proprietário no calendário. 

Antes que o compartilhamento ou delegação de calendário entre em vigor, o proprietário envia um sharee ou delega um convite e o sharee ou o delegado aceita o convite ou adiciona explicitamente o calendário compartilhado ou delegado para acesso. O convite e a adição de um calendário compartilhado ou delegado ocorrem em um cliente do Outlook. 

Depois de configurar o compartilhamento ou a delegação no Outlook, os aplicativos poderão usar a API do Microsoft Graph para gerenciar o compartilhamento e a delegação.

O restante deste artigo baseia-se no exemplo a seguir:

- Alex Rodrigues delegou a Sara Melo seu calendário principal e também permitiu Sara para visualizar eventos privados nesse calendário. 
- Alex compartilhou no calendário o evento "festa das crianças" com Adele Vance e Sara Melo, e atribuiu Adele e a Sara permissões `read` para todos os detalhes de eventos não privados no calendário "festas das crianças" e o status de disponibilidade para eventos privados. 

Este artigo descreve programaticamente a execução das seguintes tarefas com um calendário compartilhado ou delegado:

- [Obtenha informações de calendário sobre compartilhamento, delegados e permissões permitidas e atualize permissões individuais](#get-calendar-information-about-sharees-and-delegates-and-update-individual-permissions).
- [Obtenha as propriedades que descrevem o compartilhamento ou a delegação de calendário](#get-properties-of-a-shared-or-delegated-calendar).
- [Obtenha ou defina a configuração de caixa de correio para receber solicitações de reunião e respostas para um calendário delegado](#get-or-set-mailbox-setting-to-receive-meeting-requests-and-responses).
- [Exclua um compartilhamento ou um representante de um calendário](#delete-a-sharee-or-delegate-of-a-calendar).

Os aplicativos também podem fazer o seguinte usando a API que geralmente está disponível:

- [Obter calendário do Outlook compartilhado ou delegado ou seus eventos](outlook-get-shared-events-calendars.md)
- [Criar eventos do Outlook em um calendário compartilhado ou delegado](outlook-create-event-in-shared-delegated-calendar.md)

> [!NOTE]
> As propriedades e API para compartilhamento e delegação de calendário conforme descrito neste tópico estão disponíveis atualmente no ponto de extremidade v1.0, com exceção das propriedades de calendário **isShared** e **isSharedWithMe**. Essas duas propriedades são expostas apenas no ponto de extremidade beta.

## <a name="get-calendar-information-about-sharees-and-delegates-and-update-individual-permissions"></a>Obtenha informações de calendário sobre compartilhamento, delegados e permissões permitidas e atualize permissões individuais.

Nesta seção:

- [Proprietário do calendário: obter informações e permissões de compartilhamento e delegação](#calendar-owner-get-sharing-or-delegation-information-and-permissions)
- [Proprietário do calendário: atualizar permissões para um compartilhamento existente ou delegado em um calendário](#calendar-owner-update-permissions-for-an-existing-sharee-or-delegate-on-a-calendar)

Todos os calendários estão associados a um conjunto de objetos [calendarPermission](/graph/api/resources/calendarpermission), cada um deles descreve um compartilhamento ou delegado e a permissão associada que o proprietário do calendário configurou. A enumeração [calendarRoleType](/graph/api/resources/calendarpermission#calendarroletype-values) define o intervalo de permissões que o Microsoft Graph dá suporte:

- `none` Esse valor se aplica somente a `My Organization` que não tem permissões para o calendário. Isso não se aplica a usuários individuais, pois somente os usuários com permissões estão associados a um objeto **calendarPermission** para o calendário.
- `freeBusyRead` O sharee pode exibir o status de disponibilidade do proprietário, mas não outros detalhes no calendário.
- `limitedRead` O sharee pode exibir o status de disponibilidade do proprietário e os títulos e locais de eventos não privados no calendário.
- `read` O sharee pode visualizar o status de disponibilidade do proprietário em eventos privados e todos os detalhes de eventos não privados no calendário.
- `write` O sharee pode visualizar o status de disponibilidade do proprietário em eventos privados e pode exibir todos os detalhes e editar (criar, atualizar ou excluir) eventos não privados no calendário.
- `delegateWithoutPrivateEventAccess` O _delegado_ pode visualizar o status de disponibilidade do proprietário em eventos privados e tem `write` acesso a eventos não privados no calendário.
- `delegateWithPrivateEventAccess` O _delegado_ pode visualizar o status de disponibilidade do proprietário em eventos privados e tem acesso `write` a eventos não privados no calendário.

O calendário principal de um usuário sempre é compartilhado com a "Minha Organização", que representa os usuários na mesma organização do proprietário. Por padrão, eles podem ler o status de disponibilidade do proprietário no calendário e ter a permissão `freeBusyRead`.


### <a name="calendar-owner-get-sharing-or-delegation-information-and-permissions"></a>Proprietário do calendário: obter informações e permissões de compartilhamento e delegação

Este exemplo mostra com o consentimento de Alex ou administrador, como obter os objetos **calendarPermission** associados ao calendário principal de Alex. A solicitação retorna dois objetos de permissão:

- O primeiro objeto **calendarPermission** é atribuído ao delegado, Sara, e tem os seguintes valores de propriedade:

  - **isRemovable** está definida como true, o que permite a cancelamento de uma delegação.
  - **isInsideOrganization** é verdadeiro, pois somente os usuários na mesma organização podem ser delegados.
  - **a função** de Sara é `delegateWithPrivateEventAccess`, conforme configurado por Alex.
  - **allowedRoles** inclui os tipos de função `delegateWithoutPrivateEventAccess`e`delegateWithPrivateEventAccess` que oferecem suporte à delegação.
  - **emailAddress** especifica Sara.

- O segundo objeto **calendarPermission** é um objeto padrão atribuído a "My Organization" e tem os seguintes valores de propriedade:

  - **isRemovable** está definido como falso, uma vez que o calendário principal é sempre compartilhado com a organização do proprietário.
  - **isInsideOrganization** é verdadeiro.
  - **a função** é`freeBusyRead`, a configuração padrão para "My Organization".
  - **emailAddress** especifica a subpropriedade **name** como "My Organization"; o **endereço** de "My Organization" é nulo.

#### <a name="microsoft-graph-permissions"></a>Permissões do Microsoft Graph
Use a permissão delegada ou de aplicativo com menos privilégios, `Calendars.Read`, conforme apropriado, para esta operação. Para obter mais informações, confira [permissões de calendário](permissions-reference.md#calendars-permissions).

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendarperms"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/calendar/calendarPermissions
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendarperms-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendarperms-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendarperms-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "name": "get_calendarperms",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarPermission",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/calendar/calendarPermissions",
    "value": [
        {
            "id": "L289RXhjaGFuZ2VMYWJTWVnYW5C",
            "isRemovable": true,
            "isInsideOrganization": true,
            "role": "delegateWithPrivateEventAccess",
            "allowedRoles": [
                "freeBusyRead",
                "limitedRead",
                "read",
                "write",
                "delegateWithoutPrivateEventAccess",
                "delegateWithPrivateEventAccess"
            ],
            "emailAddress": {
                "name": "Megan Bowen",
                "address": "MeganB@contoso.OnMicrosoft.com"
            }
        },
        {
            "id": "RGVmYXVsdA==",
            "isRemovable": false,
            "isInsideOrganization": true,
            "role": "freeBusyRead",
            "allowedRoles": [
                "none",
                "freeBusyRead",
                "limitedRead",
                "read",
                "write"
            ],
            "emailAddress": {
                "name": "My Organization"
            }
        }
    ]
}
```


### <a name="calendar-owner-update-permissions-for-an-existing-sharee-or-delegate-on-a-calendar"></a>Proprietário do calendário: atualizar permissões para um sharee existente ou delegado em um calendário

Com o consentimento de Alex ou do administrador, você pode atualizar as permissões atribuídas a um compartilhamento ou delegado existente (especificado pela propriedade **função**), contanto que as novas permissões sejam compatíveis com **allowedRoles** configurado inicialmente para o sharee ou o delegado desse calendário. 

Com exceção da propriedade **função**, você não pode atualizar outras propriedades de um sharee ou delegado existente. Alterar o valor da propriedade **emailAddress** exige a exclusão do compartilhamento ou do representante e a configuração de uma nova instância do **calendarPermission** novamente.

O exemplo nesta seção atualiza a propriedade **função**, alterando a permissão de um sharee existente, Adele, de `read` para `write` para o calendário personalizado "Festas infantis".

#### <a name="microsoft-graph-permissions"></a>Permissões do Microsoft Graph
Use a permissão delegada ou de aplicativo com menos privilégios, `Calendars.ReadWrite`, conforme apropriado, para esta operação. Para obter mais informações, confira [permissões de calendário](permissions-reference.md#calendars-permissions).

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_calendarperm",
  "sampleKeys": ["AlexW@contoso.OnMicrosoft.com", "AAMkADAwAABf02bAAAA=", "L289RXhjaGFuZ2VMYWJQWRlbGVW"]
}-->
```http
PATCH https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/calendars/AAMkADAwAABf02bAAAA=/calendarPermissions/L289RXhjaGFuZ2VMYWJQWRlbGVW
Content-type: application/json

{
  "role": "write"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-calendarperm-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-calendarperm-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-calendarperm-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "name": "update_calendarperm",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarPermission"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/calendars('AAMkADAwAABf02bAAAA%3D')/calendarPermissions/$entity",
    "id": "L289RXhjaGFuZ2VMYWJQWRlbGVW",
    "isRemovable": true,
    "isInsideOrganization": true,
    "role": "write",
    "allowedRoles": [
        "freeBusyRead",
        "limitedRead",
        "read",
        "write"
    ],
    "emailAddress": {
        "name": "Adele Vance",
        "address": "AdeleV@contoso.OnMicrosoft.com"
    }
}
```


## <a name="get-properties-of-a-shared-or-delegated-calendar"></a>Obter propriedades de um calendário compartilhado ou delegado

Nesta seção:

- [Proprietário do calendário: Obter propriedades de um calendário compartilhado ou delegado](#calendar-owner-get-properties-of-a-shared-or-delegated-calendar)
- [Compartilhar ou delegar: obter propriedades de calendário compartilhado ou delegado](#sharee-or-delegate-get-properties-of-shared-or-delegated-calendar)

Lembrando deste exemplo, Alex delegou seu calendário principal e concedeu à delegada, Sara Melo, a permissão para exibir itens de calendário marcados como particulares.
Esta seção mostra as propriedades do calendário delegado, primeiro a partir da perspectiva de e com o consentimento do proprietário, Alex, da perspectiva de e com o consentimento da delegada, Sara. O consentimento do administrador também funciona para todos os casos.

### <a name="calendar-owner-get-properties-of-a-shared-or-delegated-calendar"></a>Proprietário do calendário: Obter propriedades de um calendário compartilhado ou delegado

O exemplo nesta seção obtém as propriedades do calendário principal da perspectiva do proprietário, Alex. 

Observe as seguintes propriedades de Alex:

- **canshare** é verdadeiro, pois Alex é o proprietário.
- **canViewPrivateItems** é verdadeiro, uma vez que Alex é o proprietário.
- **isShared** é definido como verdadeiro, uma vez que o Alex configurou um delegado para este calendário.
- **isSharedWithMe** é sempre falso para o proprietário do calendário.
- **owner** mostra Alex como proprietário.

#### <a name="microsoft-graph-permissions"></a>Permissões do Microsoft Graph
Use a permissão delegada ou de aplicativo com menos privilégios, `Calendars.Read`, conforme apropriado, para esta operação. Para obter mais informações, confira [permissões de calendário](permissions-reference.md#calendars-permissions).

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendar_props_owner",
  "sampleKeys": ["AlexW@contoso.OnMicrosoft.com"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/calendar
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendar-props-owner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendar-props-owner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendar-props-owner-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "name": "get_calendar_props_owner",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/calendar/$entity",
    "id": "AQMkADAw7QAAAJfygAAAA==",
    "name": "Calendar",
    "color": "auto",
    "hexColor": "",
    "changeKey": "NEXywgsVrkeNsFsyVyRrtAAAAAACOg==",
    "canShare": true,
    "canViewPrivateItems": true,
    "isShared": true,
    "isSharedWithMe": false,
    "canEdit": true,
    "allowedOnlineMeetingProviders": [
        "teamsForBusiness"
    ],
    "defaultOnlineMeetingProvider": "teamsForBusiness",
    "isTallyingResponses": true,
    "isRemovable": false,
    "owner": {
        "name": "Alex Wilber",
        "address": "AlexW@contoso.OnMicrosoft.com"
    }
}
```


### <a name="sharee-or-delegate-get-properties-of-shared-or-delegated-calendar"></a>Compartilhar ou delegar: obter propriedades de calendário compartilhado ou delegado

O exemplo nesta seção obtém as propriedades do mesmo calendário da perspectiva da delegada, Sara. 

Observe as seguintes propriedades:

- **nome** do calendário é, por padrão, o nome de exibição do proprietário. Nesse caso, é "Alex Rodrigues", já que o calendário de Alex, foi delegado a Sara. 
- **canShare** é falso, uma vez que Sara não é a proprietária do calendário.
- **canViewPrivateItems** é verdadeiro para a delegada Sara, conforme configurado por Alex. Para um sharee que não seja um delegado essa propriedade será sempre falsa.
- **isShared** é falso. Esta propriedade indica apenas ao _proprietário_ do calendário se o calendário foi compartilhado ou delegado.
- A propriedade **isSharedWithMe** é verdadeira, uma vez que Sara é uma delegada.
- **CanEdit** é verdadeiro, uma vez que os delegados, incluindo Sara, têm acesso de gravação.
- **owner** está definido como Alex.

> [!NOTE] 
> Um compartilhamento ou representante só pode personalizar a propriedade **nome** de um calendário compartilhado/delegado. A atualização é visível apenas para eles mesmos; o proprietário do calendário não vê essas alterações no nome do calendário.

#### <a name="microsoft-graph-permissions"></a>Permissões do Microsoft Graph
Use a permissão delegada com menos privilégios, `Calendars.Read.Shared`, ou permissão de aplicativo, `Calendars.Read`, conforme apropriado, para esta operação. Para obter mais informações, confira [permissões de calendário](permissions-reference.md#calendars-permissions).

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_calendar_props_delegate",
  "sampleKeys": ["meganb@contoso.OnMicrosoft.com", "AAMkADlAABhbftjAAA="]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/meganb@contoso.OnMicrosoft.com/calendars/AAMkADlAABhbftjAAA=
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-calendar-props-delegate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-calendar-props-delegate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-calendar-props-delegate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "name": "get_calendar_props_delegate",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('meganb%40contoso.OnMicrosoft.com')/calendars/$entity",
    "id": "AAMkADlAABhbftjAAA=",
    "name": "Alex Wilber",
    "color": "auto",
    "hexColor": "",
    "changeKey": "E6LznKWmX0KTsAD9qRJjeAAAYWo3EQ==",
    "canShare": false,
    "canViewPrivateItems": true,
    "isShared": false,
    "isSharedWithMe": true,
    "canEdit": true,
    "allowedOnlineMeetingProviders": [
        "teamsForBusiness"
    ],
    "defaultOnlineMeetingProvider": "teamsForBusiness",
    "isTallyingResponses": true,
    "isRemovable": true,
    "owner": {
        "name": "Alex Wilber",
        "address": "AlexW@contoso.OnMicrosoft.com"
    }
}
```


## <a name="get-or-set-mailbox-setting-to-receive-meeting-requests-and-responses"></a>Obtenha ou defina a configuração de caixa de correio para receber solicitações de reunião e respostas

Nesta seção:

- [Obter a configuração de entrega de delegação para a caixa de correio de um usuário](#get-delegation-delivery-setting-for-a-users-mailbox)
- [Definir a configuração de entrega de delegação para a caixa de correio de um usuário](#set-delegation-delivery-setting-for-a-users-mailbox)

Dependendo do nível de delegação que um proprietário de calendário prefere, o proprietário poderá especificar quem deve receber solicitações de reunião e respostas para gerenciar as reuniões no calendário. 

Programaticamente, você pode obter ou definir a propriedade **delegateMeetingMessageDeliveryOptions** do proprietário do calendário [mailboxSettings](/graph/api/resources/mailboxsettings) para especificar para quem o Outlook deve direcionar as instâncias [eventMessageRequest](/graph/api/resources/eventmessagerequest) e [eventMessageResponse](/graph/api/resources/eventmessageresponse):

- `sendToDelegateOnly`

    O Outlook para direcionar as instâncias **eventMessageRequest** e **eventMessageResponse** para delegados. Esta é a configuração padrão. O proprietário pode ver as respostas a uma reunião ou responder a um convite através do **evento** correspondente no calendário delegado.
- `sendToDelegateAndInformationToPrincipal`

    O Outlook direciona as instâncias **eventMessageRequest** e **eventMessageResponse** para delegados e para o proprietário do calendário. Somente os representantes veem a opção de aceitar ou recusar uma solicitação de reunião, e a notificação enviada ao proprietário aparece como uma mensagem de e-mail normal. O proprietário ainda pode responder à reunião, abrindo o **evento** no calendário delegado e respondendo.
- `sendToDelegateAndPrincipal`

    O Outlook direciona as instâncias **eventMessageRequest** e **eventMessageResponse** para delegados e para o proprietário do calendário, ou seja, que podem responder à solicitação de reunião.

Essa é uma configuração para toda a caixa de correio; portanto, a mesma configuração se aplica a todos os delegados do proprietário da caixa de correio.

### <a name="get-delegation-delivery-setting-for-a-users-mailbox"></a>Obter a configuração de entrega de delegação para a caixa de correio de um usuário

O exemplo nesta seção obtém as **mailboxSettings** de um proprietário de calendário que permite que o Outlook direcione solicitações e respostas de reunião apenas para delegados de calendário; ou seja, **delegateMeetingMessageDeliveryOptions** é definido como `sendToDelegateOnly`.

#### <a name="microsoft-graph-permissions"></a>Permissões do Microsoft Graph
Use a permissão delegada ou de aplicativo com menos privilégios, `MailboxSettings.Read`, conforme apropriado, para esta operação. Para obter mais informações sobre permissões de caixa de correio, confira [permissões de email](permissions-reference.md#mail-permissions).

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mailboxsettings_owner",
  "sampleKeys": ["AlexW@contoso.OnMicrosoft.com"]
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/mailboxsettings
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mailboxsettings-owner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mailboxsettings-owner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mailboxsettings-owner-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "name": "get_mailboxsettings_owner",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/mailboxSettings",
    "archiveFolder": "AQMkADAwAGVQAAAKfowAAAA==",
    "timeZone": "Pacific Standard Time",
    "delegateMeetingMessageDeliveryOptions": "sendToDelegateOnly",
    "dateFormat": "M/d/yyyy",
    "timeFormat": "h:mm tt",
    "automaticRepliesSetting": {
        "status": "disabled",
        "externalAudience": "all",
        "internalReplyMessage": "",
        "externalReplyMessage": "",
        "scheduledStartDateTime": {
            "dateTime": "2019-12-24T05:00:00.0000000",
            "timeZone": "UTC"
        },
        "scheduledEndDateTime": {
            "dateTime": "2019-12-25T05:00:00.0000000",
            "timeZone": "UTC"
        }
    },
    "language": {
        "locale": "en-US",
        "displayName": "English (United States)"
    },
    "workingHours": {
        "daysOfWeek": [
            "monday",
            "tuesday",
            "wednesday",
            "thursday",
            "friday"
        ],
        "startTime": "08:00:00.0000000",
        "endTime": "17:00:00.0000000",
        "timeZone": {
            "name": "Pacific Standard Time"
        }
    }
}
```

### <a name="set-delegation-delivery-setting-for-a-users-mailbox"></a>Definir a configuração de entrega de delegação para a caixa de correio de um usuário

O exemplo nesta seção atualiza a propriedade **delegateMeetingMessageDeliveryOptions** para `sendToDelegateAndPrincipal`, para que o Outlook direcione solicitações de reunião e respostas do calendário delegado para todos os delegados e o proprietário.

#### <a name="microsoft-graph-permissions"></a>Permissões do Microsoft Graph
Use a permissão delegada ou de aplicativo com menos privilégios, `MailboxSettings.ReadWrite`, conforme apropriado, para esta operação. Para obter mais informações sobre permissões de caixa de correio, confira [permissões de email](permissions-reference.md#mail-permissions).

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "patch_mailboxsettings_owner",
  "sampleKeys": ["AlexW@contoso.OnMicrosoft.com"]
}-->
```http
PATCH https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/mailboxsettings
Content-type: application/json

{
  "delegateMeetingMessageDeliveryOptions": "sendToDelegateAndPrincipal"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/patch-mailboxsettings-owner-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/patch-mailboxsettings-owner-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/patch-mailboxsettings-owner-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "name": "patch_mailboxsettings_owner",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailboxSettings"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('64339082-ed84-4b0b-b4ab-004ae54f3747')/mailboxSettings",
    "delegateMeetingMessageDeliveryOptions": "sendToDelegateAndPrincipal"
}
```


## <a name="delete-a-sharee-or-delegate-of-a-calendar"></a>Exclua um compartilhamento ou um representante de um calendário.

No exemplo abaixo, Alex exclui Sara como um sharee do calendário "Festas infantis".

#### <a name="microsoft-graph-permissions"></a>Permissões do Microsoft Graph
Use a permissão delegada ou de aplicativo com menos privilégios, `Calendars.ReadWrite`, conforme apropriado, para esta operação. Para obter mais informações, confira [permissões de calendário](permissions-reference.md#calendars-permissions).

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_sharee",
  "sampleKeys": ["AlexW@contoso.OnMicrosoft.com", "AAMkADAwAABf02bAAAA=", "L289RXhjaGFuZ2VMYWJTWVnYW5C"]
}-->
```http
DELETE https://graph.microsoft.com/beta/users/AlexW@contoso.OnMicrosoft.com/calendars/AAMkADAwAABf02bAAAA=/calendarPermissions/L289RXhjaGFuZ2VMYWJTWVnYW5C
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-sharee-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-sharee-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-sharee-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- {
  "blockType": "response",
  "name": "delete_sharee",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```


## <a name="next-steps"></a>Próximas etapas

Saiba mais sobre:

- Como os clientes do Outlook têm suporte para compartilhar e delegar calendários:
  - [Compartilhar um calendário do Outlook com outras pessoas ](https://support.office.com/article/share-an-outlook-calendar-with-other-people-353ed2c1-3ec5-449d-8c73-6931a0adab88
)
  - [Permitir que outra pessoa gerencie o email e o calendário como delegado](https://support.office.com/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926)
  - [Compartilhar seu calendário no Outlook na Web](https://support.office.com/article/share-your-calendar-in-outlook-on-the-web-7ecef8ae-139c-40d9-bae2-a23977ee58d5)
  - [Delegação de calendário no Outlook na Web](https://support.office.com/article/calendar-delegation-in-outlook-on-the-web-532e6410-ee80-42b5-9b1b-a09345ccef1b
)
- [Obter eventos do Outlook em um calendário compartilhado ou delegado](outlook-get-shared-events-calendars.md)
- [Criar eventos do Outlook em um calendário compartilhado ou delegado](outlook-create-event-in-shared-delegated-calendar.md)
- [Por que se integrar com o calendário do Outlook](outlook-calendar-concept-overview.md)
- A [API de calendário](/graph/api/resources/calendar) do Outlook no Microsoft Graph beta.
