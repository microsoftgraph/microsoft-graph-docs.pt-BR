---
title: tipo de recurso de usuário
description: Representa uma conta de usuário do Azure AD. Herda de directoryObject.
author: dkershaw10
localization_priority: Priority
ms.openlocfilehash: 1bec385ef452316e3c7c9eb79989fc10e534de26
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833303"
---
# <a name="user-resource-type"></a>Tipo de recurso de usuário

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa uma conta de usuário do Azure AD. Herda de [directoryObject](directoryobject.md).

Esse recurso permite:

- Adicionar seus próprios dados às propriedades personalizadas como [extensões](/graph/extensibility-overview).
- Assinatura de [notificações de alteração](/graph/webhooks).
- Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/user-delta.md).

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:-------|:------------|:------------|
|[Listar usuários](../api/user-list.md) |Coleção [user](user.md)| Recuperar uma lista de objetos user.|
|[Criar usuário](../api/user-post-users.md) |[user](user.md)| Criar um novo objeto user.|
|[Obter usuário](../api/user-get.md) | [user](user.md) |Ler propriedades e relações do objeto user.|
|[Atualizar usuário](../api/user-update.md) | [user](user.md) |Atualizar o objeto user. |
|[Excluir usuário](../api/user-delete.md) | Nenhum |Excluir o objeto user. |
|[Listar mensagens](../api/user-list-messages.md) |Coleção [Message](message.md)| Obter todas as mensagens na caixa de correio do usuário conectado.|
|[Criar Mensagem](../api/user-post-messages.md) |[Message](message.md)| Crie uma mensagem, postagem à coleção de mensagens.|
|[Listar mailFolders](../api/user-list-mailfolders.md) |Coleção [MailFolder](mailfolder.md)| Obter a coleção de pastas de email sob a pasta raiz do usuário conectado. |
|[Criar MailFolder](../api/user-post-mailfolders.md) |[MailFolder](mailfolder.md)| Criar uma nova MailFolder postando na coleção mailFolders.|
|[sendMail](../api/user-sendmail.md)|Nenhum|Enviar a mensagem especificada no corpo da solicitação.|
|[Listar eventos](../api/user-list-events.md) |Coleção [Event](event.md)| Obter uma lista de objetos event na caixa de correio do usuário. A lista contém reuniões de instância única e reuniões mestres em série.|
|[Criar evento](../api/user-post-events.md) |[Event](event.md)| Criar um novo Event postando na coleção events.|
|[Listar calendários](../api/user-list-calendars.md) |Coleção [Calendar](calendar.md)| Obter uma coleção de objetos Calendar.|
|[Criar calendário](../api/user-post-calendars.md) |[Calendar](calendar.md)| Criar um novo Calendar postando na coleção calendars.|
|[Listar calendarGroups](../api/user-list-calendargroups.md) |Coleção [CalendarGroup](calendargroup.md)| Obter uma coleção de objetos CalendarGroup.|
|[Criar calendarGroup](../api/user-post-calendargroups.md) |[CalendarGroup](calendargroup.md)| Criar um novo CalendarGroup postando na coleção calendarGroups.|
|[Listar calendarView](../api/user-list-calendarview.md) |Coleção [Event](event.md)| Obtenha uma coleção de objetos de evento.|
|[Listar contatos](../api/user-list-contacts.md) |Coleção [Contact](contact.md)| Obter uma coleção de contatos da pasta Contatos padrão do usuário conectado.|
|[Criar Contato](../api/user-post-contacts.md) |[Contact](contact.md)| Criar um novo Contact postando na coleção contacts.|
|[Listar contactFolders](../api/user-list-contactfolders.md) |Coleção [ContactFolder](contactfolder.md)| Obter a coleção de pastas de contatos na pasta Contatos padrão do usuário conectado.|
|[Criar ContactFolder](../api/user-post-contactfolders.md) |[ContactFolder](contactfolder.md)| Criar uma nova ContactFolder postando na coleção contactFolders.|
|[Listar directReports](../api/user-list-directreports.md) |Coleção [directoryObject](directoryobject.md)| Obter os usuários ou contatos subordinados ao usuário da propriedade de navegação directReports.|
|[Listar gerente](../api/user-list-manager.md) |[directoryObject](directoryobject.md) | Obter o usuário ou contato que é o gerente do usuário da propriedade de navegação manager.|
|[Listar memberOf](../api/user-list-memberof.md) |Coleção [directoryObject](directoryobject.md)| Obtenha os grupos, funções de diretório e unidades administrativas que o usuário é um membro direto da propriedade membro navegação.|
|[Membro de lista transitivo](../api/user-list-transitivememberof.md) |Coleção [directoryObject](directoryobject.md)| Liste os grupos, funções de diretório e unidades administrativas que o usuário é membro do. Essa operação é transitiva e inclui os grupos que o usuário é membro de aninhados. |
|[Listar joinedTeams](../api/user-list-joinedteams.md) |coleção [Groups](group.md)| Obtenha Teams Microsoft que o usuário é um membro direto da propriedade joinedTeams navegação.|
|[Listar ownedDevices](../api/user-list-owneddevices.md) |Coleção [directoryObject](directoryobject.md)| Obter os dispositivos que pertencem ao usuário da propriedade de navegação ownedDevices.|
|[Listar ownedObjects](../api/user-list-ownedobjects.md) |Coleção [directoryObject](directoryobject.md)| Obter os objetos directory que pertencem ao usuário da propriedade de navegação ownedObjects.|
|[Listar plannerTasks](../api/planneruser-list-tasks.md) |Coleção [plannerTask](plannertask.md)| Obtenha plannerTasks atribuída ao usuário.|
|[Listar registeredDevices](../api/user-list-registereddevices.md) |Coleção [directoryObject](directoryobject.md)| Obtenha os dispositivos que são registrados para o usuário a partir da propriedade de navegação registeredDevices.|
|[Associações de função com escopo de lista](../api/user-list-scopedrolememberof.md) |coleção [scopedRoleMembership](scopedrolemembership.md)| Associações de unidades administrativas Get a função com escopo para este usuário.|
|[Listar createdObjects](../api/user-list-createdobjects.md) |Coleção [directoryObject](directoryobject.md)| Obter os objetos directory criados pelo usuário da propriedade de navegação createdObjects.|
|[Lista agreementAcceptances](../api/user-list-agreementacceptances.md) | coleção [agreementAcceptance](agreementacceptance.md) | Obtenha uma lista de termos de uso do status de aceitação do usuário.|
|[assignLicense](../api/user-assignlicense.md)|[user](user.md)|Adicionar ou remover assinaturas para o usuário. Você também pode habilitar e desabilitar planos específicos associados a uma assinatura.|
|[Listar licenseDetails](../api/user-list-licensedetails.md) |Coleção [licenseDetails](licensedetails.md)| Obtenha uma coleção de objetos licenseDetails.|
|[checkMemberGroups](../api/user-checkmembergroups.md)|Coleção de cadeias de caracteres|Verifique se há uma associação em uma lista de grupos. A verificação é transitiva.|
|[findmeetingtimes](../api/user-findmeetingtimes.md)|[meetingTimeCandidate](meetingtimecandidate.md)|Encontre o tempo e locais para cumprir com base na disponibilidade do participante, local ou restrições de tempo.|
|[findRoomLists](../api/user-findroomlists.md)|coleção [EmailAddress.MD](emailaddress.md) | Obtenha as listas de salas definidas em um locatário.|
|[findRooms](../api/user-findrooms.md)|coleção [EmailAddress.MD](emailaddress.md) | Obtenha todas as salas de reunião no locatário do usuário ou em uma lista de salas específico. |
|[getMailTips](../api/user-getmailtips.md)|conjunto de [dicas de email](mailtips.md)|Retorne as dicas de email de um ou mais destinatários conforme disponível para o usuário conectado. |
|[getMemberGroups](../api/user-getmembergroups.md)|Coleção de cadeias de caracteres|Retorne todos os grupos dos quais o usuário é membro. A verificação é transitiva.|
|[getMemberObjects](../api/user-getmemberobjects.md)|Coleção de cadeias de caracteres| Retorne todos os grupos, funções de diretório e unidades administrativas que o usuário é membro do. A seleção é transitiva. |
|[invalidateAllRefreshTokens](../api/user-invalidateallrefreshtokens.md)| Nenhum |Invalida tokens de sessão e de atualização do todos os usuários emitidos aos aplicativos, redefinindo a propriedade **refreshTokensValidFromDateTime** do usuário para a data-hora atual. Isso força o usuário entrar para tais aplicativos novamente.|
|[reminderView](../api/user-reminderview.md)|Coleção [Reminder](reminder.md)|Retorna uma lista de lembretes de calendário nas horas de início e término especificadas.|
|[delta](../api/user-delta.md)|coleção de usuários| Obtenha as alterações incrementais para usuários. |
|[Traduzir identificadores do Outlook](../api/user-translateexchangeids.md) |conjunto de [tipo de recurso de convertIdResult](convertidresult.md)| Traduza os identificadores de recursos relacionados ao Outlook entre formatos.|
|**Extensões abertas**| | |
|[Criar extensão aberta](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Crie uma extensão aberta e adicione propriedades personalizadas a uma instância nova ou existente de um recurso.|
|[Obter extensão aberta](../api/opentypeextension-get.md) |Coleção [openTypeExtension](opentypeextension.md)| Obtenha uma extensão aberta identificada pelo nome da extensão.|
|**Extensões de esquema**| | |
|[Adicionar valores de extensões de esquema](/graph/extensibility-schema-groups) || Criar uma definição para a extensão de esquema e usá-la para adicionar dados digitados personalizados a um recurso.|

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo    | Descrição |
|:---------------|:--------|:------------|
|aboutMe|String|Um campo de entrada de texto em forma livre para o usuário se descrever.|
|accountEnabled|Booliano| **true** se a conta estiver habilitada; caso contrário, **false**. Essa propriedade é obrigatória quando um usuário é criado. Oferece suporte a $filter.    |
|ageGroup|Cadeia de caracteres|Define o grupo de idade do usuário. Valores permitidos: `null`, `minor`, `notAdult` e `adult`. Consulte as [definições de propriedade do grupo de idade do departamento jurídico](#legal-age-group-property-definitions) para obter mais informações. |
|assignedLicenses|Coleção [assignedLicense](assignedlicense.md)|As licenças que são atribuídas ao usuário. Não anulável.            |
|assignedPlans|Coleção [assignedPlan](assignedplan.md)|Os planos que são atribuídos ao usuário. Somente leitura. Não anulável. |
|birthday|DateTimeOffset|O aniversário do usuário. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|city|String|A cidade em que o usuário está localizado. Oferece suporte a $filter.|
|companyName| String | O nome da empresa em que o usuário está associado. Somente leitura.
|consentProvidedForMinor|Cadeia de caracteres|Define se o consentimento tiver sido obtido aos menores. Valores permitidos: `null`, `granted`, `denied` e `notRequired`. Consulte as [definições de propriedade do grupo de idade do departamento jurídico](#legal-age-group-property-definitions) para obter mais informações.|
|country|String|O país/região na qual o usuário está localizado; Por exemplo, "EUA" ou "UK". Oferece suporte a $filter.|
|deletedDateTime|DateTimeOffset| A data e hora que o usuário foi excluído. |
|departamento|String|O nome do departamento no qual o usuário trabalha. Oferece suporte a $filter.|
|displayName|String|O nome exibido para o usuário no catálogo de endereços. Geralmente, esse valor é a combinação entre o nome do usuário, intermediário nome inicial e o sobrenome. Essa propriedade é obrigatória quando um usuário é criado e não pode ser apagado durante atualizações. Oferece suporte a $filter e $orderby.|
|employeeId|Cadeia de caracteres|O identificador de funcionário atribuído ao usuário pela organização. Oferece suporte a $filter.|
|externalUserState|Cadeia de caracteres|Para um usuário externo convidado para o inquilino usando a [API do convite](../api/invitation-post.md), essa propriedade representa o status do convite do usuário convidado. Para usuários convidados, o estado pode ser 'PendingAcceptance' ou 'Aceito', ou `null` todos os outros usuários. Suporta $filter com valores suportados. Por exemplo: `$filter=externalUserState eq 'PendingAcceptance'`.|
|externalUserStateChangeDateTime|Cadeia de caracteres|Mostra o carimbo de hora para que a alteração mais recente à propriedade externalUserState.|
|Fax|Cadeia de caracteres|O número de fax do usuário.|
|givenName|String|O nome fornecido (nome) do usuário. Oferece suporte a $filter.|
|hireDate|DateTimeOffset|A data de contratação do usuário. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|id|String|O identificador exclusivo do usuário. Herdado de [directoryObject](directoryobject.md). Chave. Não anulável. Somente leitura.|
|interests|Coleção de cadeias de caracteres|Uma lista para o usuário descrever os interesses dele.|
|jobTitle|String|O cargo do usuário. Oferece suporte a $filter.|
|legalAgeGroupClassification|Cadeia de caracteres| Usado por aplicativos corporativos para determinar o grupo de idade legal do usuário. Essa propriedade é somente leitura e calculados com base em `ageGroup` e `consentProvidedForMinor` propriedades. Valores permitidos: `null`, `minorWithOutParentalConsent`, `minorWithParentalConsent`, `minorNoParentalConsentRequired`, `notAdult` e `adult`. Consulte as [definições de propriedade do grupo de idade do departamento jurídico](#legal-age-group-property-definitions) para obter mais informações.)|
|licenseAssignmentStates|coleção [licenseAssignmentState](licenseassignmentstate.md)|Estado de atribuições de licença para este usuário. Somente leitura.|
|Email|String|O endereço SMTP do usuário, por exemplo, "jeff@contoso.onmicrosoft.com". Somente Leitura. Oferece suporte a $filter.|
|mailboxSettings|[mailboxSettings](mailboxsettings.md)|Configurações para a caixa de correio principal do usuário conectado. Você pode [obter](../api/user-get-mailboxsettings.md) ou [Atualizar](../api/user-update-mailboxsettings.md) configurações para enviar respostas automáticas para mensagens recebidas, localidade e fuso horário.|
|mailNickname|String|O alias de email do usuário. Essa propriedade deve ser especificada quando um usuário é criado. Oferece suporte a $filter.|
|mobilePhone|String|O número de celular principal do usuário.|
|mySite|String|A URL do site pessoal do usuário.|
|officeLocation|String|A localização do escritório no local de trabalho do usuário.|
|onPremisesDistinguishedName|Cadeia de caracteres| Contém o Active Directory no local `distinguished name` ou `DN`. A propriedade é preenchida apenas para os clientes que estão sincronizando seu diretório local no Windows Azure Active Directory por meio do Connect do Azure AD. Somente leitura. |
|onPremisesDomainName|Cadeia de caracteres| Contém o local `domainFQDN`, também chamada Nome_de_domínio_dns sincronizados do diretório local. A propriedade é preenchida apenas para os clientes que estão sincronizando seu diretório local no Windows Azure Active Directory por meio do Connect do Azure AD. Somente leitura. |
|onPremisesExtensionAttributes|[OnPremisesExtensionAttributes](onpremisesextensionattributes.md)|Contém extensionAttributes 1-15 para o usuário. Observe que os atributos de extensão individuais são não selecionável nem filtráveis. Para uma `onPremisesSyncEnabled` usuário, esse conjunto de propriedades mastered local e é somente leitura. Para um usuário somente na nuvem (onde `onPremisesSyncEnabled` é false), essas propriedades podem ser definida durante a criação ou atualização. |
|onPremisesImmutableId|String|Essa propriedade é usada para associar uma conta de usuário do Active Directory local para seus objetos de usuário do Windows Azure AD. Esta propriedade deve ser especificada ao criar uma nova conta de usuário no gráfico, se você estiver usando um domínio federado para o usuário `userPrincipalName` propriedade (UPN). **Importante:** O **$** e **_** caracteres não podem ser usados ao especificar essa propriedade. Oferece suporte a $filter. |
|onPremisesLastSyncDateTime|DateTimeOffset|Indica a última vez em que o objeto foi sincronizado com o diretório local; por exemplo: "2013-02-16T03:04:54Z". O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.|
|onPremisesProvisioningErrors|coleção [onPremisesProvisioningError](onpremisesprovisioningerror.md)| Erros ao usar o produto de sincronização da Microsoft durante o provisionamento. |
|onPremisesSamAccountName|Cadeia de caracteres| Contém o local `sAMAccountName` sincronizados do diretório local. A propriedade é preenchida apenas para os clientes que estão sincronizando seu diretório local no Windows Azure Active Directory por meio do Connect do Azure AD. Somente leitura. |
|onPremisesSecurityIdentifier|String|Contém o identificador de segurança (SID) local do usuário que foi sincronizado do local com a nuvem. Somente leitura.|
|onPremisesSyncEnabled|Booliano| **True** se esse objeto está sincronizado de um diretório local; **false** se esse objeto foi originalmente sincronizado de um diretório local, mas não está mais sincronizado; **null** se esse objeto nunca foi sido sincronizado de um diretório local (padrão). Somente leitura |
|onPremisesUserPrincipalName|Cadeia de caracteres| Contém o local `userPrincipalName` sincronizados do diretório local. A propriedade é preenchida apenas para os clientes que estão sincronizando seu diretório local no Windows Azure Active Directory por meio do Connect do Azure AD. Somente leitura. |
|otherMails|Cadeia de caracteres| Uma lista de endereços de email adicionais para o usuário; Por exemplo: `["bob@contoso.com", "Robert@fabrikam.com"]`. Oferece suporte a $filter.|
|passwordPolicies|String|Especifica as políticas de senha do usuário. Esse valor é uma enumeração cujo um dos valores possíveis é "DisableStrongPassword", o que permite especificar senhas mais fracas do que a política padrão. Também é possível especificar "DisablePasswordExpiration". Ambos podem ser especificados juntos; por exemplo: "DisablePasswordExpiration, DisableStrongPassword".|
|passwordProfile|[PasswordProfile](passwordprofile.md)|Especifica o perfil de senha do usuário. O perfil contém a senha do usuário. Essa propriedade é obrigatória quando um usuário é criado. A senha no perfil deve atender a requisitos mínimos, conforme especificado pela propriedade **passwordPolicies**. Por padrão, é obrigatória uma senha forte.|
|pastProjects|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar seus projetos anteriores.|
|postalCode|String|O código postal do endereço postal do usuário. O código postal é específico para o país/região do usuário. Nos Estados Unidos, esse atributo contém o CEP.|
|preferredDataLocation|Cadeia de caracteres|A localização de dados preferida para o usuário. Para obter mais informações, consulte [Multi-Geo OneDrive Online](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction).|
|preferredLanguage|String|O idioma preferencial do usuário. Deve seguir o código ISO 639-1; por exemplo "en-US".|
|preferredName|String|O nome preferencial do usuário.|
|provisionedPlans|Coleção [ProvisionedPlan](provisionedplan.md)|Os planos que estão provisionados para o usuário. Somente leitura. Não anulável. |
|proxyAddresses|Coleção de cadeias de caracteres|Por exemplo: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` O operador **any** é obrigatório para expressões de filtro em propriedades de vários valores. Somente leitura, não anulável. Oferece suporte a $filter.          |
|refreshTokensValidFromDateTime|DateTimeOffset| Qualquer atualização tokens ou tokens de sessões (cookies de sessão) emitidos antes desta vez são inválidos e aplicativos receberá um erro ao usar uma atualização inválida ou um token de sessões para adquirir um acesso delegado token (para acesso a APIs, como o Microsoft Graph).  Se isso acontecer, o aplicativo será necessário adquirir um novo token refresh fazendo uma solicitação ao ponto de extremidade autorizar. Somente leitura. Use [invalidateAllRefreshTokens](../api/user-invalidateallrefreshtokens.md) para redefinir.|
|responsibilities|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar suas responsabilidades.|
|schools|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar as escolas que ele frequentou.|
|showInAddressList|Booliano|**true** se a lista de endereços global do Outlook deve conter este usuário, caso contrário **false**. Se não definido, isso será tratado como **true**. Para usuários convidados por meio do Gerenciador de convite, definirá esta propriedade como **false**.|
|skills|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar suas qualificações.|
|state|String|O estado ou município no endereço do usuário. Oferece suporte a $filter.|
|streetAddress|String|O endereço do local de trabalho do usuário.|
|surname|String|O sobrenome do usuário (nome de família ou sobrenome). Oferece suporte a $filter.|
|usageLocation|String|Um código de duas letras (padrão ISO 3166). Obrigatório para os usuários que receberão licenças devido à exigência legal de verificar a disponibilidade de serviços nos países. Entre os exemplos temos: "US", "JP" e "GB". Não anulável. Oferece suporte a $filter.|
|userPrincipalName|String|O nome UPN do usuário. O nome UPN é um nome de logon para o usuário ao estilo da Internet com base na RFC 822 padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email do usuário. O formato geral é alias@domain, em que o domínio deve estar presente na coleção de domínios verificados do locatário. Essa propriedade é obrigatória quando um usuário é criado. Os domínios verificados para o locatário podem ser acessados pela propriedade **verifiedDomains** de [organization](organization.md). Oferece suporte a $filter e $orderby.
|userType|String|Um valor de cadeia de caracteres que pode ser usado para classificar os tipos de usuário no seu diretório, como "Membro" e "Convidado". Oferece suporte a $filter.          |

### <a name="legal-age-group-property-definitions"></a>Definições de propriedade do grupo de idade do departamento jurídico

Esta seção explica como os três age propriedades do grupo (`legalAgeGroupClassification`, `ageGroup` e `consentProvidedForMinor`) usadas pelos administradores do Windows Azure AD e os desenvolvedores de aplicativos do enterprise para cumprir as normas relacionadas a idade.

Por exemplo: Cameron é administrador de um diretório para uma escola em Holyport no Reino Unido. No início do ano escola ele usa os trabalhos de papel admissão para obter o consentimento de pais do secundárias com base nas normas relacionadas a idade do Reino Unido. O consentimento obtido do pai permite que a conta do secundárias a ser usado pelo Holyport school e aplicativos do Microsoft. Cameron cria todas as contas e define ageGroup para "secundária" e consentProvidedForMinor "concedida". Aplicativos usados pelo seus alunos são capazes de suprimir recursos que não são adequados para menores.

#### <a name="legal-age-group-classification"></a>Classificação de grupo de idade do departamento jurídico

Essa propriedade somente leitura é usada por desenvolvedores de aplicativos corporativos para garantir o tratamento correto de um usuário com base em seu grupo de idade do departamento jurídico. Ele é calculado com base em que o usuário `ageGroup` e `consentProvidedForMinor` propriedades.

| Valor   | # |Descrição|
|:---------------|:--------|:----------|
|nulo|0|Valor padrão, não `ageGroup` tiver sido definida para o usuário.|
|minorWithoutParentalConsent |1|(Reservado para uso futuro)|
|minorWithParentalConsent|2| O usuário será considerado uma secundárias com base nas normas relacionadas a idade do seu país ou região e o administrador da conta obteve consentimento apropriado de um pai ou responsável.|
|adulto|3|O usuário considerado um adulto com base nas normas relacionadas a idade do seu país ou região.|
|notAdult|4|O usuário é de um país ou região que tenha as normas relacionadas a idade adicionais (por exemplo, os Estados Unidos, Reino Unido, União Europeia ou Coreia do Sul) e a duração do usuário é entre uma secundárias e uma idade adultos (como estipulados com base no país). Geralmente, isso significa que os adolescentes são considerados como `notAdult` em regulamentado países.|
|minorNoParentalConsentRequired|5|O usuário é uma secundárias, mas é de um país ou região que não tenha nenhuma regulamentos relacionados a idade.|

#### <a name="age-group-and-minor-consent"></a>Grupo de idade e consentimento secundário

As propriedades de consentimento secundária e o grupo de idade são propriedades opcionais usadas pelos administradores do Windows Azure AD para ajudar a garantir que o uso de uma conta será tratado corretamente baseado nas relacionados a idade normativas regras que regem o país ou a região do usuário.

#### <a name="agegroup-property"></a>propriedade ageGroup

| Valor    | # |Descrição|
|:---------------|:--------|:----------|
|nulo|0|Valor padrão, não `ageGroup` tiver sido definida para o usuário.|
|secundária|1|O usuário, considere uma secundárias.|
|notAdult|2|O usuário é de um país que tenha legais regulamentos dos Estados Unidos, Reino Unido, União Europeia ou Coreia do Sul) e duração do usuário é maior do que o limite superior da idade filho (conforme o país/região) e limite inferior menor do que a idade adultos (como estipulados com base no país) . Basicamente, adolescentes são considerados como `notAdult` em regulamentado países.|
|adulto|3|O usuário deve ser tratadas como um adulto.|

#### <a name="consentprovidedforminor-property"></a>propriedade consentProvidedForMinor

| Valor    | # |Descrição|
|:---------------|:--------|:----------|
|nulo|0|Valor padrão, não `consentProvidedForMinor` tiver sido definida para o usuário.|
|concedido|1|Tiver sido obtido consentimento para o usuário tenha uma conta.|
|negado|2|Não tiver sido obtido consentimento para o usuário tenha uma conta.|
|notRequired|3|O usuário é de um local que não exigem o consentimento.|

## <a name="relationships"></a>Relações

| Relação | Tipo |Descrição|
|:---------------|:--------|:----------|
|agreementAcceptances|coleção [agreementAcceptance](agreementacceptance.md)| Condições do usuário dos status de aceitação de uso. Somente leitura. Anulável.|
|calendário|[calendar](calendar.md)|O calendário principal do usuário. Somente leitura.|
|calendarGroups|coleção [calendarGroup](calendargroup.md)|Os grupos de calendários do usuário. Somente leitura. Anulável.|
|calendarView|Coleção [event](event.md)|O modo de exibição do calendário. Somente leitura. Anulável.|
|calendars|Coleção [calendar](calendar.md)|Os calendários do usuário. Somente leitura. Anulável.|
|contactFolders|coleção [contactFolder](contactfolder.md)|As pastas de contatos do usuário. Somente leitura. Anulável.|
|contatos|Coleção [Contact](contact.md)|Os contatos do usuário. Somente leitura. Anulável.|
|createdObjects|Coleção [directoryObject](directoryobject.md)|Objetos directory que foram criados pelo usuário. Somente leitura. Anulável.|
|directReports|Coleção [directoryObject](directoryobject.md)|Os usuários e contatos subordinados ao usuário. (Os usuários e contatos cuja propriedade manager está definida como esse usuário.) Somente leitura. Anulável. |
|drive|[drive](drive.md)|O OneDrive do usuário. Somente leitura.|
|events|Coleção [event](event.md)|Os eventos do usuário. O padrão é mostrar eventos no Calendário Padrão. Somente leitura. Anulável.|
|extensions|Coleção [extension](extension.md)|A coleção de extensões open definidas para o usuário. Anulável.|
|inferenceClassification|[inferenceClassification](inferenceclassification.md)| Classificação de relevância das mensagens do usuário com base em designações explícitas que substituem a relevância ou importância deduzida. |
|ideias|coleção [Insights](insights.md)| Somente leitura. Anulável.|
|joinedGroups|Coleção [group](group.md)| Somente leitura. Anulável.|
|mailFolders|Coleção [mailFolder](mailfolder.md)| As pastas de email do usuário. Somente leitura. Anulável.|
|manager|[directoryObject](directoryobject.md)|O usuário ou contato que é o gerente do usuário. Somente leitura. (Métodos HTTP: GET, PUT, DELETE.)|
|memberOf|Coleção [directoryObject](directoryobject.md)|Os grupos, funções de diretório e unidades administrativas que o usuário é membro do. Somente leitura. Anulável.|
|joinedTeams|Coleção [group](group.md)|A Microsoft Teams que o usuário é membro do. Somente leitura. Anulável.|
|mensagens|Coleção [message](message.md)|As mensagens em uma caixa de correio ou pasta. Somente leitura. Anulável.|
|onenote|[OneNote](onenote.md)| Somente leitura.|
|Outlook|[outlookUser](outlookuser.md)| Serviços seletivos Outlook disponíveis para o usuário. Somente leitura. Anulável.|
|ownedDevices|Coleção [directoryObject](directoryobject.md)|Dispositivos que pertencem ao usuário. Somente leitura. Anulável.|
|ownedObjects|Coleção [directoryObject](directoryobject.md)|Objetos de diretório que pertencem ao usuário. Somente leitura. Anulável.|
|pessoas|coleção de [pessoa](person.md)| Somente leitura. As pessoas mais relevantes para o usuário. A coleção é ordenada pela sua relevância para o usuário, que é determinado pela comunicação do usuário, colaboração e relacionamentos de negócios. Uma pessoa é uma agregação de informações em email, contatos e redes sociais.|
|Foto|[profilePhoto](profilephoto.md)| A foto de perfil do usuário. Somente leitura.|
|fotos|Coleção de [foto](photo.md)| Somente leitura. Anulável.|
|planejador|[plannerUser](planneruser.md)| Serviços Planejador seletivos disponíveis para o usuário. Somente leitura. Anulável. |
|SharePoint|[SharePoint](sharepoint.md)| Acesso ao site do SharePoint do usuário. Somente leitura. |
|scopedRoleMemberOf|coleção [scopedRoleMembership](scopedrolemembership.md)| As associações de função com escopo de unidade administrativa para este usuário. Somente leitura. Anulável.|
|configurações|coleção de [definições](user-settings.md)| Somente leitura. Anulável.|
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
    "extensions",
    "joinedGroups",
    "mailFolders",
    "manager",
    "memberOf",
    "joinedTeams",
    "messages",
    "onenote",
    "oauth2PermissionGrants",
    "outlook",
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
  "ageGroup": "string",
  "assignedLicenses": [{"@odata.type": "microsoft.graph.assignedLicense"}],
  "assignedPlans": [{"@odata.type": "microsoft.graph.assignedPlan"}],
  "birthday": "String (timestamp)",
  "businessPhones": ["string"],
  "city": "string",
  "companyName": "string",
  "consentProvidedForMinor": "string",
  "country": "string",
  "deletedDateTime": "String (timestamp)",
  "department": "string",
  "displayName": "string",
  "externalUserState": "PendingAcceptance",
  "externalUserStateChangeDateTime": "2018-11-12T01:13:13Z",
  "givenName": "string",
  "hireDate": "String (timestamp)",
  "id": "string (identifier)",
  "interests": ["string"],
  "jobTitle": "string",
  "legalAgeGroupClassification": "string",
  "licenseAssignmentStates": [{"@odata.type": "microsoft.graph.licenseAssignmentState"}],
  "mail": "string",
  "mailboxSettings": {"@odata.type": "microsoft.graph.mailboxSettings"},
  "mailNickname": "string",
  "mobilePhone": "string",
  "mySite": "string",
  "officeLocation": "string",
  "onPremisesExtensionAttributes": {"@odata.type": "microsoft.graph.onPremisesExtensionAttributes"},
  "onPremisesImmutableId": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
  "passwordPolicies": "string",
  "passwordProfile": {"@odata.type": "microsoft.graph.passwordProfile"},
  "pastProjects": ["string"],
  "postalCode": "string",
  "preferredDataLocation": "string",
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
  "insights": { "@odata.type": "microsoft.graph.officeGraphInsights" },
  "settings": { "@odata.type": "microsoft.graph.userSettings" },
  "events": [ { "@odata.type": "microsoft.graph.event" } ],
  "extensions": [ { "@odata.type": "microsoft.graph.extension" } ],
  "inferenceClassification": { "@odata.type": "microsoft.graph.inferenceClassification" },
  "mailFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "manager": { "@odata.type": "microsoft.graph.directoryObject" },
  "memberOf": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "joinedTeams": [ { "@odata.type": "microsoft.graph.group" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "outlook": { "@odata.type": "microsoft.graph.outlookUser" },
  "ownedDevices": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "photo": { "@odata.type": "microsoft.graph.profilePhoto" },
  "registeredDevices": [ { "@odata.type": "microsoft.graph.directoryObject" } ]
}
```

## <a name="see-also"></a>Confira também

- [Adicionar dados personalizados a recursos usando extensões](/graph/extensibility-overview)
- [Adicionar dados personalizados aos usuários usando extensões abertas](/graph/extensibility-open-users)
- [Adicionar dados personalizados a grupos usando as extensões do esquema](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
