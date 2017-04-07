# <a name="user-resource-type"></a>tipo de recurso de usuário

Representa uma conta de usuário do Azure AD. Herda de [directoryObject](directoryobject.md).


## <a name="methods"></a>Métodos
| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter usuário](../api/user_get.md) | [user](user.md) |Ler propriedades e relações do objeto user.|
|[Atualizar usuário](../api/user_update.md) | [user](user.md) |Atualizar o objeto user. |
|[Excluir usuário](../api/user_delete.md) | Nenhum |Excluir o objeto user. |
|[Listar mensagens](../api/user_list_messages.md) |Coleção [Message](message.md)| Obter todas as mensagens na caixa de correio do usuário conectado.|
|[Criar Mensagem](../api/user_post_messages.md) |[Message](message.md)| Criar uma nova Mensagem postando na coleção messages.|
|[Listar mailFolders](../api/user_list_mailfolders.md) |Coleção [MailFolder](mailfolder.md)| Obter a coleção de pastas de email sob a pasta raiz do usuário conectado. |
|[Criar MailFolder](../api/user_post_mailfolders.md) |[MailFolder](mailfolder.md)| Criar uma nova MailFolder postando na coleção mailFolders.|
|[sendMail](../api/user_sendmail.md)|Nenhum|Enviar a mensagem especificada no corpo da solicitação.|
|[Listar eventos](../api/user_list_events.md) |Coleção [Event](event.md)| Obter uma lista de objetos event na caixa de correio do usuário. A lista contém reuniões de instância única e reuniões mestres em série.|
|[Criar evento](../api/user_post_events.md) |[Event](event.md)| Criar um novo Event postando na coleção events.|
|[Listar calendários](../api/user_list_calendars.md) |Coleção [Calendar](calendar.md)| Obter uma coleção de objetos Calendar.|
|[Criar calendário](../api/user_post_calendars.md) |[Calendar](calendar.md)| Criar um novo Calendar postando na coleção calendars.|
|[Listar calendarGroups](../api/user_list_calendargroups.md) |Coleção [CalendarGroup](calendargroup.md)| Obter uma coleção de objetos CalendarGroup.|
|[Criar calendarGroup](../api/user_post_calendargroups.md) |[CalendarGroup](calendargroup.md)| Criar um novo CalendarGroup postando na coleção calendarGroups.|
|[Listar calendarView](../api/user_list_calendarview.md) |Coleção [Event](event.md)| Obter uma coleção de objetos Event.|
|[Listar contatos](../api/user_list_contacts.md) |Coleção [Contact](contact.md)| Obter uma coleção de contatos da pasta Contatos padrão do usuário conectado.|
|[Criar Contato](../api/user_post_contacts.md) |[Contact](contact.md)| Criar um novo Contact postando na coleção contacts.|
|[Listar contactFolders](../api/user_list_contactfolders.md) |Coleção [ContactFolder](contactfolder.md)| Obter a coleção de pastas de contatos na pasta Contatos padrão do usuário conectado.|
|[Criar ContactFolder](../api/user_post_contactfolders.md) |[ContactFolder](contactfolder.md)| Criar uma nova ContactFolder postando na coleção contactFolders.|
|[Listar directReports](../api/user_list_directreports.md) |Coleção [directoryObject](directoryobject.md)| Obter os usuários ou contatos subordinados ao usuário da propriedade de navegação directReports.|
|[Listar gerente](../api/user_list_manager.md) |[directoryObject](directoryobject.md) | Obter o usuário ou contato que é o gerente do usuário da propriedade de navegação manager.|
|[Listar memberOf](../api/user_list_memberof.md) |Coleção [directoryObject](directoryobject.md)| Obter os grupos e as funções de diretório dos quais o usuário é membro direto da propriedade de navegação memberOf.|
|[Listar ownedDevices](../api/user_list_owneddevices.md) |Coleção [directoryObject](directoryobject.md)| Obter os dispositivos que pertencem ao usuário da propriedade de navegação ownedDevices.|
|[Listar ownedObjects](../api/user_list_ownedobjects.md) |Coleção [directoryObject](directoryobject.md)| Obter os objetos directory que pertencem ao usuário da propriedade de navegação ownedObjects.|
|[Listar registeredDevices](../api/user_list_registereddevices.md) |Coleção [directoryObject](directoryobject.md)| Obter os dispositivos que estão registrados para o usuário da propriedade de navegação registeredDevices.|
|[Listar createdObjects](../api/user_list_createdobjects.md) |Coleção [directoryObject](directoryobject.md)| Obter os objetos directory criados pelo usuário da propriedade de navegação createdObjects.|
|[assignLicense](../api/user_assignlicense.md)|[user](user.md)|Adicionar ou remover assinaturas para o usuário. Você também pode habilitar e desabilitar planos específicos associados a uma assinatura.|
|[checkMemberGroups](../api/user_checkmembergroups.md)|Coleção de cadeias de caracteres|Verifique se há uma associação em uma lista de grupos. A verificação é transitiva.|
|[getMemberGroups](../api/user_getmembergroups.md)|Coleção de cadeias de caracteres|Retorne todos os grupos dos quais o usuário é membro. A verificação é transitiva.|
|[getMemberObjects](../api/user_getmemberobjects.md)|Coleção de cadeias de caracteres| Retorna todos os grupos e funções de diretório dos quais o usuário é membro. A verificação é transitiva. |
|[reminderView](../api/user_reminderview.md)|Coleção [Reminder](reminder.md)|Retorna uma lista de lembretes de calendário nas horas de início e término especificadas.|



## <a name="properties"></a>Propriedades
| Propriedade	       | Tipo	    |Descrição|
|:---------------|:--------|:----------|
|aboutMe|String|Um campo de entrada de texto em forma livre para o usuário se descrever.|
|accountEnabled|Booliano| **true** se a conta estiver habilitada; caso contrário, **false**. Essa propriedade é obrigatória quando um usuário é criado. Oferece suporte a $filter.    |
|assignedLicenses|Coleção [assignedLicense](assignedlicense.md)|As licenças que são atribuídas ao usuário. Não anulável.            |
|assignedPlans|Coleção [assignedPlan](assignedplan.md)|Os planos que são atribuídos ao usuário. Somente leitura. Não anulável. |
|birthday|DateTimeOffset|O aniversário do usuário. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|city|String|A cidade em que o usuário está localizado. Oferece suporte a $filter.|
|country|String|País/região em que o usuário está localizado. Por exemplo, "EUA" ou "Reino Unido". Oferece suporte a $filter.|
|department|String|O nome do departamento no qual o usuário trabalha. Oferece suporte a $filter.|
|displayName|String|O nome exibido no catálogo de endereços do usuário. É geralmente a combinação do nome, da inicial do meio e do sobrenome do usuário. Essa propriedade é obrigatória quando um usuário é criado e não pode ser apagado durante atualizações. Oferece suporte a $filter e $orderby.|
|givenName|String|O nome fornecido (nome) do usuário. Oferece suporte a $filter.|
|hireDate|DateTimeOffset|A data de contratação do usuário. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|id|String|O identificador exclusivo do usuário. Herdado de [directoryObject](directoryobject.md). Chave. Não anulável. Somente leitura.|
|interests|Coleção de cadeias de caracteres|Uma lista para o usuário descrever os interesses dele.|
|jobTitle|String|O cargo do usuário. Oferece suporte a $filter.|
|mail|String|O endereço SMTP do usuário, por exemplo, "jeff@contoso.onmicrosoft.com". Somente Leitura. Oferece suporte a $filter.|
|mailboxSettings|[mailboxSettings](mailboxsettings.md)|Configurações da caixa de correio principal do usuário conectado. Você pode [obter](../api/user_get_mailboxsettings.md) ou [atualizar](../api/user_update_mailboxsettings.md) as configurações de localidade, fuso horário ou de envio de respostas automáticas a mensagens de entrada.|
|mailNickname|String|O alias de email do usuário. Essa propriedade deve ser especificada quando um usuário é criado. Oferece suporte a $filter.|
|mobilePhone|String|O número de celular principal do usuário.|
|mySite|String|A URL do site pessoal do usuário.|
|officeLocation|String|A localização do escritório no local de trabalho do usuário.|
|onPremisesImmutableId|String|Essa propriedade é usada para associar uma conta de usuário do Active Directory local com seu objeto de usuário do Azure AD. Essa propriedade deverá ser especificada ao criar uma nova conta de usuário no Graph se você estiver usando um domínio federado para a propriedade **userPrincipalName** (UPN) do usuário. **Importante:** Os caracteres **$** e **_** não podem ser usados ao especificar essa propriedade. Oferece suporte a $filter.                            |
|onPremisesLastSyncDateTime|DateTimeOffset|Indica a última vez em que o objeto foi sincronizado com o diretório local; por exemplo: "2013-02-16T03:04:54Z". O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.|
|onPremisesSecurityIdentifier|String|Contém o identificador de segurança (SID) local do usuário que foi sincronizado do local com a nuvem. Somente leitura.|
|onPremisesSyncEnabled|Booliano| **True** se esse objeto está sincronizado de um diretório local; **false** se esse objeto foi originalmente sincronizado de um diretório local, mas não está mais sincronizado; **null** se esse objeto nunca foi sido sincronizado de um diretório local (padrão). Somente leitura |
|passwordPolicies|String|Especifica as políticas de senha do usuário. Esse valor é uma enumeração cujo um dos valores possíveis é "DisableStrongPassword", o que permite especificar senhas mais fracas do que a política padrão. Também é possível especificar "DisablePasswordExpiration". Ambos podem ser especificados juntos; por exemplo: "DisablePasswordExpiration, DisableStrongPassword".|
|passwordProfile|[PasswordProfile](passwordprofile.md)|Especifica o perfil de senha do usuário. O perfil contém a senha do usuário. Essa propriedade é obrigatória quando um usuário é criado. A senha no perfil deve atender a requisitos mínimos, conforme especificado pela propriedade **passwordPolicies**. Por padrão, é obrigatória uma senha forte.|
|pastProjects|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar seus projetos anteriores.|
|postalCode|String|O código postal do endereço postal do usuário. O código postal é específico para o país/região do usuário. Nos Estados Unidos, esse atributo contém o CEP.|
|preferredLanguage|String|O idioma preferencial do usuário. Deve seguir o código ISO 639-1; por exemplo "en-US".|
|preferredName|String|O nome preferencial do usuário.|
|provisionedPlans|Coleção [ProvisionedPlan](provisionedplan.md)|Os planos que estão provisionados para o usuário. Somente leitura. Não anulável. |
|proxyAddresses|Coleção de cadeias de caracteres|Por exemplo: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` O operador **any** é obrigatório para expressões de filtro em propriedades de vários valores. Somente leitura, não anulável. Oferece suporte a $filter.          |
|responsibilities|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar suas responsabilidades.|
|schools|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar as escolas que ele frequentou.|
|skills|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar suas qualificações.|
|state|String|O estado ou município no endereço do usuário. Oferece suporte a $filter.|
|streetAddress|String|O endereço do local de trabalho do usuário.|
|surname|String|O sobrenome do usuário (nome de família ou sobrenome). Oferece suporte a $filter.|
|usageLocation|String|Um código de duas letras (padrão ISO 3166). Obrigatório para os usuários que receberão licenças devido à exigência legal de verificar a disponibilidade de serviços nos países.  Entre os exemplos temos: "US", "JT" e "GB". Não anulável. Oferece suporte a $filter.|
|userPrincipalName|String|O nome UPN do usuário. O nome UPN é um nome de logon para o usuário ao estilo da Internet com base na RFC 822 padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email do usuário. O formato geral é alias@domain, em que o domínio deve estar presente na coleção de domínios verificados do locatário. Essa propriedade é obrigatória quando um usuário é criado. Os domínios verificados para o locatário podem ser acessados pela propriedade **verifiedDomains** de [organization](organization.md). Oferece suporte a $filter e $orderby.
|userType|String|Um valor de cadeia de caracteres que pode ser usado para classificar tipos de usuários no seu diretório, como “Member” e “Guest”. Oferece suporte a $filter.          |

## <a name="relationships"></a>Relações
| Relação | Tipo	    |Descrição|
|:---------------|:--------|:----------|
|calendar|[Calendar](calendar.md)|O calendário principal do usuário. Somente leitura.|
|calendarGroups|Coleção [CalendarGroup](calendargroup.md)|Os grupos de calendários do usuário. Somente leitura. Anulável.|
|calendarView|Coleção [Event](event.md)|O modo de exibição do calendário. Somente leitura. Anulável.|
|calendars|Coleção [Calendar](calendar.md)|Os calendários do usuário. Somente leitura. Anulável.|
|contactFolders|Coleção [ContactFolder](contactfolder.md)|As pastas de contatos do usuário. Somente leitura. Anulável.|
|contatos|Coleção [Contact](contact.md)|Os contatos do usuário. Somente leitura. Anulável.|
|createdObjects|Coleção [directoryObject](directoryobject.md)|Objetos directory que foram criados pelo usuário. Somente leitura. Anulável.|
|directReports|Coleção [directoryObject](directoryobject.md)|Os usuários e contatos subordinados ao usuário. (Os usuários e contatos cuja propriedade manager está definida como esse usuário.) Somente leitura. Anulável. |
|drive|[drive](drive.md)|O OneDrive do usuário. Somente leitura.|
|events|Coleção [Event](event.md)|Os eventos do usuário. O padrão é mostrar eventos no Calendário Padrão. Somente leitura. Anulável.|
|inferenceClassification | [inferenceClassification](inferenceClassification.md) | Classificação de relevância das mensagens do usuário com base em designações explícitas que substituem a relevância ou importância deduzida. |
|mailFolders|Coleção [MailFolder](mailfolder.md)| As pastas de email do usuário. Somente leitura. Anulável.|
|manager|[directoryObject](directoryobject.md)|O usuário ou contato que é o gerente do usuário. Somente leitura. (Métodos HTTP: GET, PUT, DELETE.)|
|memberOf|Coleção [directoryObject](directoryobject.md)|Os grupos e as funções de diretório dos quais o usuário é membro. Somente leitura. Anulável.|
|mensagens|Coleção [Message](message.md)|As mensagens em uma caixa de correio ou pasta. Somente leitura. Anulável.|
|ownedDevices|Coleção [directoryObject](directoryobject.md)|Dispositivos que pertencem ao usuário. Somente leitura. Anulável.|
|ownedObjects|Coleção [directoryObject](directoryobject.md)|Objetos de diretório que pertencem ao usuário. Somente leitura. Anulável.|
|photo|[profilePhoto](profilephoto.md)| A foto de perfil do usuário. Somente leitura.|
|registeredDevices|Coleção [directoryObject](directoryobject.md)|Dispositivos que estão registrados para o usuário. Somente leitura. Anulável.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "appRoleAssignments",
    "calendar",
    "calendarGroups",
    "calendarView",
    "calendars",
    "contactFolders",
    "contacts",
    "createdObjects",
    "directReports",
    "drive",
    "events",
    "joinedGroups",
    "mailFolders",
    "manager",
    "memberOf",
    "messages",
    "oauth2PermissionGrants",
    "ownedDevices",
    "ownedObjects",
    "photo",
    "registeredDevices"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}-->

```json
{
  "aboutMe": "string",
  "accountEnabled": true,
  "assignedLicenses": [{"@odata.type": "microsoft.graph.assignedLicense"}],
  "assignedPlans": [{"@odata.type": "microsoft.graph.assignedPlan"}],
  "birthday": "String (timestamp)",
  "businessPhones": ["string"],
  "city": "string",
  "companyName": "string",
  "country": "string",
  "department": "string",
  "displayName": "string",
  "givenName": "string",
  "hireDate": "String (timestamp)",
  "id": "string (identifier)",
  "interests": ["string"],
  "jobTitle": "string",
  "mail": "string",
  "mailboxSettings": {"@odata.type": "microsoft.graph.mailboxSettings"},
  "mailNickname": "string",
  "mobilePhone": "string",
  "mySite": "string",
  "officeLocation": "string",
  "onPremisesImmutableId": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
  "passwordPolicies": "string",
  "passwordProfile": {"@odata.type": "microsoft.graph.passwordProfile"},
  "pastProjects": ["string"],
  "postalCode": "string",
  "preferredLanguage": "string",
  "preferredName": "string",
  "provisionedPlans": [{"@odata.type": "microsoft.graph.provisionedPlan"}],
  "proxyAddresses": ["string"],
  "responsibilities": ["string"],
  "schools": ["string"],
  "skills": ["string"],
  "state": "string",
  "streetAddress": "string",
  "surname": "string",
  "usageLocation": "string",
  "userPrincipalName": "string",
  "userType": "string",

  "calendar": { "@odata.type": "microsoft.graph.calendar" },
  "calendarGroups": [{ "@odata.type": "microsoft.graph.calendarGroup" }],
  "calendarView": [{ "@odata.type": "microsoft.graph.event" }],
  "calendars": [ {"@odata.type": "microsoft.graph.calendar"} ],
  "contacts": [ { "@odata.type": "microsoft.graph.contact" } ],
  "contactFolders": [ { "@odata.type": "microsoft.graph.contactFolder" } ],
  "createdObjects": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "directReports": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "events": [ { "@odata.type": "microsoft.graph.event" } ],
  "inferenceClassification": { "@odata.type": "microsoft.graph.inferenceClassification" },
  "mailFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "manager": { "@odata.type": "microsoft.graph.directoryObject" },
  "memberOf": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "ownedDevices": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "photo": { "@odata.type": "microsoft.graph.profilePhoto" },
  "registeredDevices": [ { "@odata.type": "microsoft.graph.directoryObject" } ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
