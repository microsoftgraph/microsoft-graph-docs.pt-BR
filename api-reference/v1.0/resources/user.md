# <a name="user-resource-type"></a>tipo de recurso de usuário

Representa uma conta de usuário do Azure AD. Herda de [directoryObject](directoryobject.md).

Esse recurso permite:

- Adicionar seus próprios dados às propriedades personalizadas usando [extensions](../../../concepts/extensibility_overview.md).
- Inscrever-se para receber [notificações de alteração](../../../concepts/webhooks.md).
- Usar a [consulta delta](../../../concepts/delta_query_overview.md) para controlar adições, exclusões e atualizações incrementais por meio de uma função [delta](../api/user_delta.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar usuários](../api/user_list.md) |Coleção [user](user.md)| Recuperar uma lista de objetos user.|
|[Criar usuário](../api/user_post_users.md) |[user](user.md)| Criar um novo objeto user.|
|[Obter usuário](../api/user_get.md) | [user](user.md) |Ler propriedades e relações do objeto user.|
|[Atualizar usuário](../api/user_update.md) | [user](user.md) |Atualizar o objeto user. |
|[Excluir usuário](../api/user_delete.md) | Nenhum |Excluir o objeto user. |
|[Listar mensagens](../api/user_list_messages.md) |Coleção [Message](message.md)| Obter todas as mensagens na caixa de correio do usuário conectado.|
|[Criar Mensagem](../api/user_post_messages.md) |[Menssagem](message.md)| Criar uma nova Mensagem postando na coleção messages.|
|[Listar mailFolders](../api/user_list_mailfolders.md) |Coleção [MailFolder](mailfolder.md)| Obter a coleção de pastas de email sob a pasta raiz do usuário conectado. |
|[Criar MailFolder](../api/user_post_mailfolders.md) |[MailFolder](mailfolder.md)| Criar uma nova MailFolder postando na coleção mailFolders.|
|[sendMail](../api/user_sendmail.md)|Nenhum|Enviar a mensagem especificada no corpo da solicitação.|
|[Listar eventos](../api/user_list_events.md) |Coleção [Event](event.md)| Obter uma lista de objetos event na caixa de correio do usuário. A lista contém reuniões de instância única e reuniões mestres em série.|
|[Criar evento](../api/user_post_events.md) |[Evento](event.md)| Criar um novo Event postando na coleção events.|
|[Listar calendários](../api/user_list_calendars.md) |Coleção [Calendar](calendar.md)| Obter uma coleção de objetos Calendar.|
|[Criar calendário](../api/user_post_calendars.md) |[Calendário](calendar.md)| Criar um novo Calendar postando na coleção calendars.|
|[Listar calendarGroups](../api/user_list_calendargroups.md) |Coleção [CalendarGroup](calendargroup.md)| Obter uma coleção de objetos CalendarGroup.|
|[Criar calendarGroup](../api/user_post_calendargroups.md) |[CalendarGroup](calendargroup.md)| Criar um novo CalendarGroup postando na coleção calendarGroups.|
|[Listar calendarView](../api/user_list_calendarview.md) |Coleção [Event](event.md)| Obter uma coleção de objetos Event.|
|[Listar contatos](../api/user_list_contacts.md) |Coleção [Contact](contact.md)| Obter uma coleção de contatos da pasta Contatos padrão do usuário conectado.|
|[Criar Contato](../api/user_post_contacts.md) |[Contato](contact.md)| Criar um novo Contact postando na coleção contacts.|
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
|[Listar licenseDetails](../api/user_list_licensedetails.md) |Coleção [licenseDetails](licensedetails.md)| Obtenha uma coleção de objetos licenseDetails.|
|[checkMemberGroups](../api/user_checkmembergroups.md)|Coleção de cadeias de caracteres|Verifique se há uma associação em uma lista de grupos. A verificação é transitiva.|
|[getMemberGroups](../api/user_getmembergroups.md)|Coleção de cadeias de caracteres|Retorne todos os grupos dos quais o usuário é membro. A verificação é transitiva.|
|[getMemberObjects](../api/user_getmemberobjects.md)|Coleção de cadeias de caracteres| Retorna todos os grupos e funções de diretório dos quais o usuário é membro. A verificação é transitiva. |
|[reminderView](../api/user_reminderview.md)|Coleção [Reminder](reminder.md)|Retorna uma lista de lembretes de calendário nas horas de início e término especificadas.|
|[delta](../api/user_delta.md)|coleção de usuários| Obtenha as alterações incrementais para usuários. |
|**Extensões abertas**| | |
|[Criar extensão aberta](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Crie uma extensão aberta e adicione propriedades personalizadas a uma instância nova ou existente de um recurso.|
|[Obter extensão aberta](../api/opentypeextension_get.md) |Coleção [openTypeExtension](opentypeextension.md)| Obtenha uma extensão aberta identificada pelo nome da extensão.|
|**Extensões de esquema**| | |
|[Adicionar valores de extensões de esquema](../../../concepts/extensibility_schema_groups.md) || Criar uma definição para a extensão de esquema e usá-la para adicionar dados digitados personalizados a um recurso.|

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo    |Descrição|
|:---------------|:--------|:----------|
|aboutMe|Sequência de caracteres|Um campo de entrada de texto em forma livre para o usuário se descrever.|
|accountEnabled|Booleano| **true** se a conta estiver habilitada; caso contrário, **false**. Essa propriedade é obrigatória quando um usuário é criado. Oferece suporte a $filter.    |
|ageGroup|Cadeia de caracteres|Define a faixa etário do usuário. Valores permitidos: `null`, `minor`, `notAdult` e `adult`. Para obter mais informações, confira as [definições da propriedade de faixa etária legal](#legal-age-group-property-definitions). |
|assignedLicenses|Coleção [assignedLicense](assignedlicense.md)|As licenças que são atribuídas ao usuário. Não anulável.            |
|assignedPlans|Coleção [assignedPlan](assignedplan.md)|Os planos que são atribuídos ao usuário. Somente leitura. Não anulável. |
|birthday|DateTimeOffset|O aniversário do usuário. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|businessPhones|Coleção de sequência de caracteres|Números de telefone para o usuário. OBSERVAÇÃO: Embora isso seja uma coleção de cadeias de caracteres, somente um número pode ser definido para essa propriedade.|
|city|Sequência de caracteres|A cidade em que o usuário está localizado. Oferece suporte a $filter.|
|companyName| Sequência de caracteres | O nome da empresa em que o usuário está associado. Somente leitura.
|consentProvidedForMinor|Cadeia de caracteres|Define se o consentimento foi obtido para menores. Valores permitidos: `null`, `granted`, `denied` e `notRequired`. Para obter mais informações, confira as [definições da propriedade de faixa etária legal](#legal-age-group-property-definitions).|
|country|Sequência de caracteres|País/região em que o usuário está localizado. Por exemplo, "EUA" ou "Reino Unido". Oferece suporte a $filter.|
|department|Sequência de caracteres|O nome do departamento no qual o usuário trabalha. Oferece suporte a $filter.|
|displayName|Sequência de caracteres|O nome exibido no catálogo de endereços do usuário. É geralmente a combinação do nome, da inicial do meio e do sobrenome do usuário. Essa propriedade é obrigatória quando um usuário é criado e não pode ser apagado durante atualizações. Oferece suporte a $filter e $orderby.|
|givenName|Sequência de caracteres|O nome fornecido (nome) do usuário. Oferece suporte a $filter.|
|hireDate|DateTimeOffset|A data de contratação do usuário. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|id|Sequência de caracteres|O identificador exclusivo do usuário. Herdado de [directoryObject](directoryobject.md). Chave. Não anulável. Somente leitura.|
|imAddresses|Coleção de sequência de caracteres|Os endereços do Protocolo de Início de Sessão (SIP) de VoIP (Voice over IP) da mensagem instantânea para o usuário. Somente leitura.|
|interests|Coleção de cadeias de caracteres|Uma lista para o usuário descrever os interesses dele.|
|jobTitle|Sequência de caracteres|O cargo do usuário. Oferece suporte a $filter.|
|legalAgeGroupClassification|Cadeia de caracteres| Usado por aplicativos empresariais para determinar a faixa etária legal do usuário. Essa propriedade é somente leitura e calculada com base nas propriedades `ageGroup` e `consentProvidedForMinor`. Valores permitidos: `null`, `minorWithOutParentalConsent`, `minorWithParentalConsent`, `minorNoParentalConsentRequired`, `notAdult` and `adult`. Para obter mais informações, confira as [definições da propriedade de faixa etária legal](#legal-age-group-property-definitions).)|
|Email|Sequência de caracteres|O endereço SMTP do usuário, por exemplo, "jeff@contoso.onmicrosoft.com". Somente Leitura. Oferece suporte a $filter.|
|mailboxSettings|[mailboxSettings](mailboxsettings.md)|Configurações da caixa de correio principal do usuário conectado. Você pode [obter](../api/user_get_mailboxsettings.md) ou [atualizar](../api/user_update_mailboxsettings.md) as configurações de localidade, fuso horário ou de envio de respostas automáticas a mensagens de entrada.|
|mailNickname|Sequência de caracteres|O alias de email do usuário. Essa propriedade deve ser especificada quando um usuário é criado. Oferece suporte a $filter.|
|mobilePhone|Sequência de caracteres|O número de celular principal do usuário.|
|mySite|Sequência de caracteres|A URL do site pessoal do usuário.|
|officeLocation|Sequência de caracteres|A localização do escritório no local de trabalho do usuário.|
|onPremisesDomainName|Sequência de caracteres| Contém o local `domainFQDN`, também chamado de dnsDomainName sincronizado para o diretório local. A propriedade é preenchida apenas para os clientes que estão sincronizando seu diretório local no Active Directory do Azure por meio do Azure AD Connect. Somente leitura. |
|onPremisesExtensionAttributes|[OnPremisesExtensionAttributes](onpremisesextensionattributes.md)|Contém extensionAttributes 1-15 para o usuário. Observe que os atributos de extensão individuais não podem ser selecionados nem filtrados. Para um usuário `onPremisesSyncEnabled`, esse conjunto de propriedades é masterizado localmente e é somente leitura. Para um usuário somente na nuvem (onde `onPremisesSyncEnabled`  é false), essas propriedades podem ser definidas durante a criação ou atualização. |
|onPremisesImmutableId|Sequência de caracteres|Essa propriedade é usada para associar uma conta de usuário do Active Directory local com seu objeto de usuário do Azure AD. Essa propriedade deverá ser especificada ao criar uma nova conta de usuário no Graph se você estiver usando um domínio federado para a propriedade **userPrincipalName** (UPN) do usuário. **Importante:** Os caracteres **$** e **_** não podem ser usados ao especificar essa propriedade. Oferece suporte a $filter.                            |
|onPremisesLastSyncDateTime|DateTimeOffset|Indica a última vez em que o objeto foi sincronizado com o diretório local; por exemplo: "2013-02-16T03:04:54Z". O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.|
|onPremisesProvisioningErrors|coleção [onPremisesProvisioningError](onpremisesprovisioningerror.md)| Erros ao usar o produto de sincronização da Microsoft durante a configuração. |
|onPremisesSamAccountName|Cadeia de caracteres| Contém o `samAccountName` local sincronizado com o diretório local. A propriedade é preenchida apenas para os clientes que estão sincronizando seu diretório local no Active Directory do Azure por meio do Azure AD Connect. Somente leitura. |
|onPremisesSecurityIdentifier|Sequência de caracteres|Contém o identificador de segurança (SID) local do usuário que foi sincronizado do local com a nuvem. Somente leitura.|
|onPremisesSyncEnabled|Booleano| **True** se esse objeto está sincronizado de um diretório local; **false** se esse objeto foi originalmente sincronizado de um diretório local, mas não está mais sincronizado; **null** se esse objeto nunca foi sido sincronizado de um diretório local (padrão). Somente leitura |
|onPremisesUserPrincipalName|Cadeia de caracteres| Contém o `userPrincipalName` local sincronizado com o diretório local. A propriedade é preenchida apenas para os clientes que estão sincronizando seu diretório local no Active Directory do Azure por meio do Azure AD Connect. Somente leitura. |
|passwordPolicies|Sequência de caracteres|Especifica as políticas de senha do usuário. Esse valor é uma enumeração cujo um dos valores possíveis é "DisableStrongPassword", o que permite especificar senhas mais fracas do que a política padrão. Também é possível especificar "DisablePasswordExpiration". Ambos podem ser especificados juntos; por exemplo: "DisablePasswordExpiration, DisableStrongPassword".|
|passwordProfile|[PasswordProfile](passwordprofile.md)|Especifica o perfil de senha do usuário. O perfil contém a senha do usuário. Essa propriedade é obrigatória quando um usuário é criado. A senha no perfil deve atender a requisitos mínimos, conforme especificado pela propriedade **passwordPolicies**. Por padrão, é obrigatória uma senha forte.|
|pastProjects|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar seus projetos anteriores.|
|postalCode|Sequência de caracteres|O código postal do endereço postal do usuário. O código postal é específico para o país/região do usuário. Nos Estados Unidos, esse atributo contém o CEP.|
|preferredLanguage|Sequência de caracteres|O idioma preferencial do usuário. Deve seguir o código ISO 639-1; por exemplo "en-US".|
|preferredName|Sequência de caracteres|O nome preferencial do usuário.|
|provisionedPlans|Coleção [ProvisionedPlan](provisionedplan.md)|Os planos que estão provisionados para o usuário. Somente leitura. Não anulável. |
|proxyAddresses|Coleção de cadeias de caracteres|Por exemplo: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` O operador **any** é obrigatório para expressões de filtro em propriedades de vários valores. Somente leitura, não anulável. Oferece suporte a $filter.          |
|responsibilities|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar suas responsabilidades.|
|schools|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar as escolas que ele frequentou.|
|skills|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar suas qualificações.|
|state|Sequência de caracteres|O estado ou município no endereço do usuário. Oferece suporte a $filter.|
|streetAddress|Sequência de caracteres|O endereço do local de trabalho do usuário.|
|surname|Sequência de caracteres|O sobrenome do usuário (nome de família ou sobrenome). Oferece suporte a $filter.|
|usageLocation|Sequência de caracteres|Um código de duas letras (padrão ISO 3166). Obrigatório para os usuários que receberão licenças devido à exigência legal de verificar a disponibilidade de serviços nos países. Entre os exemplos temos: "US", "JP" e "GB". Não anulável. Oferece suporte a $filter.|
|userPrincipalName|Sequência de caracteres|O nome UPN do usuário. O nome UPN é um nome de logon para o usuário ao estilo da Internet com base na RFC 822 padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email do usuário. O formato geral é alias@domain, em que o domínio deve estar presente na coleção de domínios verificados do locatário. Essa propriedade é obrigatória quando um usuário é criado. Os domínios verificados para o locatário podem ser acessados pela propriedade **verifiedDomains** de [organization](organization.md). Oferece suporte a $filter e $orderby.
|userType|Sequência de caracteres|Um valor de cadeia de caracteres que pode ser usado para classificar tipos de usuários no seu diretório, como “Member” e “Guest”. Oferece suporte a $filter.          |

### <a name="legal-age-group-property-definitions"></a>Definições da propriedade de faixa etária legal

Esta seção explica como as três propriedades de faixa etária (`legalAgeGroupClassification`, `ageGroup` e `consentProvidedForMinor`) são usadas pelos administradores do Azure AD e pelos desenvolvedores de aplicativos empresariais para cumprir as normas relacionadas à idade.

Por exemplo: Cameron é o administrador de um diretório de uma escola em Holyport no Reino Unido. No início do ano letivo, ele usa os documentos de admissão para obter o consentimento dos pais dos menores com base nas normas relacionadas à idade do Reino Unido. O consentimento obtido dos pais permite que a conta do menor seja usada pelos aplicativos da escola de Holyport e da Microsoft. Cameron cria todas as contas e define ageGroup como "minor" e consentProvidedForMinor como "granted". Os aplicativos usados pelos alunos podem suprimir recursos que não são adequados para menores.

#### <a name="legal-age-group-classification"></a>Classificação de faixa etária legal

Essa propriedade somente leitura é usada por desenvolvedores de aplicativos empresariais para garantir o tratamento correto de um usuário com base em sua faixa etária legal. Ela é calculada com base nas propriedades `ageGroup` e `consentProvidedForMinor` do usuário.

| Valor    | #  |Descrição|
|:---------------|:--------|:----------|
|nulo|0|Valor padrão, nenhum `ageGroup` foi definido para o usuário.|
|minorWithoutParentalConsent |1|(Reservado para uso futuro)|
|minorWithParentalConsent|2| O usuário será considerado um menor com base nas normas relacionadas à idade de seu país ou região e o administrador da conta deve obter o consentimento apropriado de um pai ou responsável.|
|adult|3|O usuário é considerado um adulto com base nas normas relacionadas à idade de seu país ou região.|
|notAdult|4|O usuário vem de um país ou região que tem normas relacionadas à idade adicionais (por exemplo, Estados Unidos, Reino Unido, União Europeia ou Coreia do Sul) e sua idade está entre as classificações de menor e adulto (conforme estipulado pelo país ou região). Geralmente, isso significa que os adolescentes são considerados `notAdult` em países regulamentados.|
|minorNoParentalConsentRequired|5|O usuário é menor, mas vem de um país ou região que não tem nenhuma regulamentação relacionada à idade.|

#### <a name="age-group-and-minor-consent"></a>Faixa etária e consentimento para menores

As propriedades de faixa etária e consentimento para menores são propriedades opcionais usadas pelos administradores do Azure AD para ajudar a garantir que o uso de uma conta seja tratado corretamente de acordo com as regras normativas relacionadas à idade em vigor no país ou na região do usuário.

#### <a name="agegroup-property"></a>Propriedade ageGroup

| Valor    | #  |Descrição|
|:---------------|:--------|:----------|
|nulo|0|Valor padrão, nenhum `ageGroup` foi definido para o usuário.|
|minor|1|O usuário é considerado um menor.|
|notAdult|2|O usuário vem de um país que tem regulamentações legais (Estados Unidos, Reino Unido, União Europeia ou Coreia do Sul) e sua idade é maior que o limite superior da classificação infantil (de acordo com o país) e menor que o limite inferior da classificação de adulto (conforme estipulado pelo país ou região). Basicamente, adolescentes são considerados `notAdult` em países regulamentados.|
|adult|3|O usuário deve ser tratado como um adulto.|

#### <a name="consentprovidedforminor-property"></a>Propriedade consentProvidedForMinor

| Valor    | #  |Descrição|
|:---------------|:--------|:----------|
|nulo|0|Valor padrão, nenhum `consentProvidedForMinor` foi definido para o usuário.|
|granted|1|O consentimento foi obtido para o usuário ter uma conta.|
|negado|2|O consentimento não foi obtido para o usuário ter uma conta.|
|notRequired|3|O usuário vem de um local que não exige consentimento.|
 
## <a name="relationships"></a>Relações

| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|activities|Coleção [userActivity](projectrome_activity.md)|As atividades do usuário em vários dispositivos. Somente leitura. Anulável.|
|calendar|[Calendário](calendar.md)|O calendário principal do usuário. Somente leitura.|
|calendarGroups|Coleção [CalendarGroup](calendargroup.md)|Os grupos de calendários do usuário. Somente leitura. Anulável.|
|calendarView|Coleção [Event](event.md)|O modo de exibição do calendário. Somente leitura. Anulável.|
|calendars|Coleção [Calendar](calendar.md)|Os calendários do usuário. Somente leitura. Anulável.|
|contactFolders|Coleção [ContactFolder](contactfolder.md)|As pastas de contatos do usuário. Somente leitura. Anulável.|
|contatos|Coleção [Contact](contact.md)|Os contatos do usuário. Somente leitura. Anulável.|
|createdObjects|Coleção [directoryObject](directoryobject.md)|Objetos directory que foram criados pelo usuário. Somente leitura. Anulável.|
|directReports|Coleção [directoryObject](directoryobject.md)|Os usuários e contatos subordinados ao usuário. (Os usuários e contatos cuja propriedade manager está definida como esse usuário.) Somente leitura. Anulável. |
|drive|[drive](drive.md)|O OneDrive do usuário. Somente leitura.|
|drives|Coleção [drive](drive.md)| Uma coleção de unidades disponíveis para esse usuário. Somente leitura. |
|events|Coleção [Event](event.md)|Os eventos do usuário. O padrão é mostrar eventos no Calendário Padrão. Somente leitura. Anulável.|
|extensions|Coleção [extension](extension.md)|A coleção de extensões abertas definidas para o usuário. Somente leitura. Anulável.|
|inferenceClassification | [inferenceClassification](inferenceClassification.md) | Classificação de relevância das mensagens do usuário com base em designações explícitas que substituem a relevância ou importância deduzida. |
|licenseDetails|Coleção [LicenseDetails](licensedetails.md)|Uma coleção de detalhes da licença do usuário. Anulável.|
|mailFolders|Coleção [MailFolder](mailfolder.md)| As pastas de email do usuário. Somente leitura. Anulável.|
|manager|[directoryObject](directoryobject.md)|O usuário ou contato que é o gerente do usuário. Somente leitura. (Métodos HTTP: GET, PUT, DELETE.)|
|memberOf|Coleção [directoryObject](directoryobject.md)|Os grupos e as funções de diretório dos quais o usuário é membro. Somente leitura. Anulável.|
|mensagens|Coleção [Message](message.md)|As mensagens em uma caixa de correio ou pasta. Somente leitura. Anulável.|
|onenote|[Onenote](onenote.md)| Somente leitura.|
|outlook|[OutlookUser](outlookuser.md)| Somente leitura.|
|ownedDevices|Coleção [directoryObject](directoryobject.md)|Dispositivos que pertencem ao usuário. Somente leitura. Anulável.|
|ownedObjects|Coleção [directoryObject](directoryobject.md)|Objetos de diretório que pertencem ao usuário. Somente leitura. Anulável.|
|people|Coleção [person](person.md)| Pessoas que são relevantes para o usuário. Somente leitura. Anulável.
|Foto|[profilePhoto](profilephoto.md)| A foto de perfil do usuário. Somente leitura.|
|planejador|[plannerUser](planneruser.md)| Ponto de entrada para o recurso Planner que pode existir para um usuário. Somente leitura.|
|registeredDevices|Coleção [directoryObject](directoryobject.md)|Dispositivos que estão registrados para o usuário. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true,
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
    "extensions",
    "joinedGroups",
    "mailFolders",
    "manager",
    "memberOf",
    "messages",
    "oauth2PermissionGrants",
    "onenote",
    "ownedDevices",
    "ownedObjects",
    "photo",
    "registeredDevices"
  ],
  "@odata.type": "microsoft.graph.user",
  "@odata.annotations": [
    {
      "capabilities": {
        "changeTracking": true
      }
    },
    {
      "property": "calendar",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "calendarGroups",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "calendars",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "calendarView",
      "capabilities": {
        "changeTracking": true,
        "deletable": false,
        "expandable": true,
        "insertable": false,
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "contactFolders",
      "capabilities": {
        "changeTracking": true,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "contacts",
      "capabilities": {
        "changeTracking": true,
        "expandable": false
      }
    },
    {
      "property": "events",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "inferenceClassification",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false
      }
    },
    {
      "property": "mailFolders",
      "capabilities": {
        "changeTracking": true,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "messages",
      "capabilities": {
        "changeTracking": false,
        "expandable": false
      }
    },
    {
      "property": "people",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "updatable": false
      }
    },
    {
      "property": "photo",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false
      }
    },
    {
      "property": "photos",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "aboutMe": "string",
  "accountEnabled": true,
  "ageGroup": "string",
  "assignedLicenses": [{"@odata.type": "microsoft.graph.assignedLicense"}],
  "assignedPlans": [{"@odata.type": "microsoft.graph.assignedPlan"}],
  "birthday": "String (timestamp)",
  "businessPhones": ["string"],
  "city": "string",
  "companyName": "string",
  "consentProvidedForMinor": "string",
  "country": "string",
  "department": "string",
  "displayName": "string",
  "givenName": "string",
  "hireDate": "String (timestamp)",
  "id": "string (identifier)",
  "imAddresses": ["string"],
  "interests": ["string"],
  "jobTitle": "string",
  "legalAgeGroupClassification": "string",
  "mail": "string",
  "mailboxSettings": {"@odata.type": "microsoft.graph.mailboxSettings"},
  "mailNickname": "string",
  "mobilePhone": "string",
  "mySite": "string",
  "officeLocation": "string",
  "onPremisesDomainName": "string",
  "onPremisesExtensionAttributes": {"@odata.type": "microsoft.graph.onPremisesExtensionAttributes"},
  "onPremisesImmutableId": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSamAccountName": "string",
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
  "onPremisesUserPrincipalName": "string",
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
  "drives": [ { "@odata.type": "microsoft.graph.drive" } ],
  "events": [ { "@odata.type": "microsoft.graph.event" } ],
  "inferenceClassification": { "@odata.type": "microsoft.graph.inferenceClassification" },
  "mailFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "manager": { "@odata.type": "microsoft.graph.directoryObject" },
  "memberOf": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "outlook": { "@odata.type": "microsoft.graph.outlookUser" },
  "ownedDevices": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "ownedObjects": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "photo": { "@odata.type": "microsoft.graph.profilePhoto" },
  "registeredDevices": [ { "@odata.type": "microsoft.graph.directoryObject" } ]
}

```

## <a name="see-also"></a>Confira também

- [Adicionar dados personalizados a recursos usando extensões](../../../concepts/extensibility_overview.md)
- [Adicionar dados personalizados aos usuários usando extensões abertas](../../../concepts/extensibility_open_users.md)
- [Adicionar dados personalizados a grupos usando as extensões do esquema](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
