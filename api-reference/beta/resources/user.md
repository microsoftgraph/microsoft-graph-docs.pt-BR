---
title: Tipo de recurso de usuário
description: Representa uma conta de usuário do Azure AD. Herda de directoryObject.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e96d55115338073b7a60ce3e47de004de64d0cf6
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/21/2019
ms.locfileid: "37539278"
---
# <a name="user-resource-type"></a>Tipo de recurso de usuário

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma conta de usuário do Azure AD. Herda de [directoryObject](directoryobject.md).

Esse recurso permite:

- Adicionar seus próprios dados às propriedades personalizadas como [extensions](/graph/extensibility-overview).
- Assinar as [notificações de alteração](/graph/webhooks).
- Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/user-delta.md).

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:-------|:------------|:------------|
|[Listar usuários](../api/user-list.md) |Coleção [user](user.md)| Recuperar uma lista de objetos user.|
|[Criar usuário](../api/user-post-users.md) |[user](user.md)| Criar um novo objeto user.|
|[Obter usuário](../api/user-get.md) | [user](user.md) |Ler propriedades e relações do objeto user.|
|[Atualizar usuário](../api/user-update.md) | [user](user.md) |Atualizar o objeto user. |
|[Excluir usuário](../api/user-delete.md) | Nenhum |Excluir o objeto user. |
|[Listar mensagens](../api/user-list-messages.md) |Coleção [message](message.md)| Obter todas as mensagens na caixa de correio do usuário conectado.|
|[Criar mensagem](../api/user-post-messages.md) |[message](message.md)| Crie uma mensagem postando na coleção de mensagens.|
|[Listar mailFolders](../api/user-list-mailfolders.md) |Coleção [mailFolder](mailfolder.md)| Obter o conjunto de pastas de email sob a pasta raiz do usuário conectado. |
|[Criar MailFolder](../api/user-post-mailfolders.md) |[mailFolder](mailfolder.md)| Crie um novo mailFolder postando na coleção mailFolders.|
|[sendMail](../api/user-sendmail.md)|Nenhum|Enviar a mensagem especificada no corpo da solicitação.|
|[Listar eventos](../api/user-list-events.md) |Coleção [event](event.md)| Obter uma lista de objetos event na caixa de correio do usuário. A lista contém reuniões de instância única e reuniões mestres em série.|
|[Criar evento](../api/user-post-events.md) |[event](event.md)| Criar um novo Event postando na coleção de eventos.|
|[Listar calendários](../api/user-list-calendars.md) |Coleção [Calendar](calendar.md)| Obter uma coleção de objetos Calendar.|
|[Criar calendário](../api/user-post-calendars.md) |[Calendar](calendar.md)| Criar um novo Calendar postando na coleção calendars.|
|[Listar calendarGroups](../api/user-list-calendargroups.md) |Coleção [CalendarGroup](calendargroup.md)| Obter uma coleção de objetos CalendarGroup.|
|[Criar calendarGroup](../api/user-post-calendargroups.md) |[CalendarGroup](calendargroup.md)| Criar um novo CalendarGroup postando na coleção calendarGroups.|
|[Listar calendarView](../api/user-list-calendarview.md) |Coleção [event](event.md)| Obter uma coleção de objetos de evento.|
|[Listar contatos](../api/user-list-contacts.md) |Coleção [Contact](contact.md)| Obter uma coleção de contatos da pasta padrão de contatos do usuário conectado.|
|[Criar contato](../api/user-post-contacts.md) |[contato](contact.md)| Crie um novo contato postando na coleção de contatos.|
|[Listar contactFolders](../api/user-list-contactfolders.md) |Coleção [ContactFolder](contactfolder.md)| Obtenha a coleção de pastas de contatos na pasta de contatos padrão do usuário conectado.|
|[Criar contactFolder](../api/user-post-contactfolders.md) |[contactFolder](contactfolder.md)| Crie um novo contactFolder postando na coleção contactFolders.|
|[Listar directReports](../api/user-list-directreports.md) |Coleção [directoryObject](directoryobject.md)| Obter os usuários ou contatos subordinados ao usuário da propriedade de navegação directReports.|
|[Listar gerente](../api/user-list-manager.md) |[directoryObject](directoryobject.md) | Obter o usuário ou contato que é o gerente do usuário da propriedade de navegação manager.|
|[Listar memberOf](../api/user-list-memberof.md) |Coleção [directoryObject](directoryobject.md)| Obter os grupos, funções de diretório e as unidades administrativas dos quais esse usuário é membro direto, da propriedade de navegação memberOf.|
|[Listar memberOf transitivos](../api/user-list-transitivememberof.md) |Coleção [directoryObject](directoryobject.md)| Lista os grupos e funções de diretório e unidades administrativas dos quais o usuário é membro. Essa operação é transitiva e inclui os grupos dos quais o usuário é membro aninhado. |
|[Listar joinedTeams](../api/user-list-joinedteams.md) |Coleção [team](team.md)| Obter as equipes do Microsoft Teams no qual o usuário é membro direto da propriedade de navegação joinedTeams.|
|[Listar ownedDevices](../api/user-list-owneddevices.md) |Coleção [directoryObject](directoryobject.md)| Obter os dispositivos que pertencem ao usuário da propriedade de navegação ownedDevices.|
|[Listar ownedObjects](../api/user-list-ownedobjects.md) |Coleção [directoryObject](directoryobject.md)| Obter os objetos directory que pertencem ao usuário da propriedade de navegação ownedObjects.|
|[Listar plannerTasks](../api/planneruser-list-tasks.md) |Coleção [plannerTask](plannertask.md)| Obter o plannerTasks atribuído ao usuário.|
|[Listar registeredDevices](../api/user-list-registereddevices.md) |Coleção [directoryObject](directoryobject.md)| Obter os dispositivos que estão registrados para o usuário da propriedade de navegação registeredDevices.|
|[Listar associações de função com escopo](../api/user-list-scopedrolememberof.md) |Coleção [scopedRoleMembership](scopedrolemembership.md)| Obter as associações de unidades administrativas de função com escopo deste usuário.|
|[Listar createdObjects](../api/user-list-createdobjects.md) |Coleção [directoryObject](directoryobject.md)| Obter os objetos directory criados pelo usuário da propriedade de navegação createdObjects.|
|[Listar agreementAcceptances](../api/user-list-agreementacceptances.md) | Coleção [agreementAcceptance](agreementacceptance.md) | Obter uma lista de termos de status de aceitação de uso do usuário.|
|[assignLicense](../api/user-assignlicense.md)|[user](user.md)|Adicionar ou remover assinaturas para o usuário. Você também pode habilitar e desabilitar planos específicos associados a uma assinatura.|
|[reprocessLicense](../api/user-reprocesslicenseassignment.md) |[user](user.md)| Reprocessar as atribuições de assinatura do usuário.|
|[Listar licenseDetails](../api/user-list-licensedetails.md) |Coleção [licenseDetails](licensedetails.md)| Obtenha uma coleção de objetos licenseDetails.|
|[checkMemberGroups](../api/user-checkmembergroups.md)|Coleção de cadeias de caracteres|Verifique se há uma associação em uma lista de grupos. A verificação é transitiva.|
|[checkMemberObjects](../api/user-checkmemberobjects.md)|Coleção de cadeias de caracteres|Verifique a associação em uma lista de grupo, função de diretório ou objetos de unidade administrativa. A verificação é transitiva.|
|[delta](../api/user-delta.md)|coleção de usuários| Obter as alterações incrementais para usuários. |
|[findMeetingTimes](../api/user-findmeetingtimes.md)|[meetingTimeSuggestionsResult](meetingtimesuggestionsresult.md)|Encontrar o tempo e locais para reunião com base na disponibilidade dos participantes, localização ou restrições de tempo.|
|[findRoomLists](../api/user-findroomlists.md)|Coleção [emailaddress.md](emailaddress.md) | Obter as listas de salas definidas em um locatário.|
|[findRooms](../api/user-findrooms.md)|Coleção [emailaddress.md](emailaddress.md) | Obter todas as salas de reunião no locatário do usuário ou em uma lista de salas específica. |
|[getMailTips](../api/user-getmailtips.md)|Coleção [mailTips](mailtips.md)|Retornar dicas de email de um ou mais destinatários conforme disponíveis para o usuário conectado. |
|[getMemberGroups](../api/user-getmembergroups.md)|Coleção de cadeias de caracteres|Retorne todos os grupos dos quais o usuário é membro. A verificação é transitiva.|
|[getMemberObjects](../api/user-getmemberobjects.md)|Coleção String| Retornar todos os grupos, funções de diretório e unidades administrativas dos quais o usuário é membro. A verificação é transitiva. |
|[invalidateAllRefreshTokens](../api/user-invalidateallrefreshtokens.md)| Nenhum |Invalidar todos os tokens de sessão e de atualização do usuário emitidos para aplicativos, redefinindo a propriedade do usuário **refreshTokensValidFromDateTime** para a data e a hora atuais. Força o usuário a entrar novamente nesses aplicativos. Este método é substituído por **revokeSignInSessions**.|
|[reminderView](../api/user-reminderview.md)|Coleção [Reminder](reminder.md)|Retorna uma lista de lembretes de calendário nas horas de início e término especificadas.|
|[revokeSignInSessions](../api/user-revokesigninsessions.md)| Nenhum |Revoga todos os tokens de sessão e de atualização do usuário emitidos para aplicativos, redefinindo a propriedade do usuário **signInSessionsValidFromDateTime** para data e a hora atuais. Força o usuário a entrar novamente nesses aplicativos. Este método substitui **invalidateAllRefreshTokens**.|
|[translateExchangeIds](../api/user-translateexchangeids.md) |coleção [convertIdResult](convertidresult.md)| Traduzir os identificadores de recursos relacionados ao Outlook entre formatos.|
|**Extensões abertas**| | |
|[Criar extensão aberta](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Crie uma extensão aberta e adicione propriedades personalizadas a uma instância nova ou existente de um recurso.|
|[Obter extensão aberta](../api/opentypeextension-get.md) |Coleção [openTypeExtension](opentypeextension.md)| Obtenha uma extensão aberta identificada pelo nome da extensão.|
|**Extensões de esquema**| | |
|[Adicionar valores de extensões de esquema](/graph/extensibility-schema-groups) || Criar uma definição para a extensão de esquema e usá-la para adicionar dados digitados personalizados a um recurso.|

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo    | Descrição |
|:---------------|:--------|:------------|
|aboutMe|String|Um campo de entrada de texto em forma livre para o usuário se descrever.|
|accountEnabled|Booliano| `true` se a conta estiver habilitada; caso contrário, `false`. Essa propriedade é obrigatória quando um usuário é criado. Oferece suporte a $filter.    |
|ageGroup|String|Define a faixa etária do usuário. Valores permitidos: `null`, `minor`, `notAdult` e `adult`. Confira as [definições de propriedades da faixa etária legal](#legal-age-group-property-definitions) para obter mais informações. |
|assignedLicenses|Coleção [assignedLicense](assignedlicense.md)|As licenças que são atribuídas ao usuário. Não anulável.            |
|assignedPlans|Coleção [assignedPlan](assignedplan.md)|Os planos que são atribuídos ao usuário. Somente leitura. Não anulável. |
|birthday|DateTimeOffset|O aniversário do usuário. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|businessPhones|String collection|Números de telefone para o usuário. OBSERVAÇÃO: Embora isso seja uma coleção de cadeias de caracteres, somente um número pode ser definido para essa propriedade.|
|city|String|A cidade em que o usuário está localizado. Oferece suporte a $filter.|
|companyName| String | O nome da empresa em que o usuário está associado. Essa propriedade pode ser útil para descrever a empresa de onde procede um usuário externo. |
|consentProvidedForMinor|String|Define se o consentimento foi obtido para menores. Valores permitidos: `null`, `granted`, `denied` e `notRequired`. Confira as [definições de propriedades da faixa etária legal](#legal-age-group-property-definitions) para obter mais informações.|
|country|String|O país/região em que o usuário está localizado. Por exemplo, "EUA" ou "Reino Unido". Oferece suporte a $filter.|
|createdDateTime|DateTimeOffset|A data e hora que o usuário foi criado. Não é possível modificar o valor e ele é preenchido automaticamente quando a entidade é criada. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. A propriedade é anulável. Um valor nulo indica que uma hora de criação exata não pode ser determinada pelo usuário. Somente leitura. Oferece suporte a $filter.|
|deletedDateTime|DateTimeOffset| A data e hora que o usuário foi excluído. |
|department|String|O nome do departamento no qual o usuário trabalha. Oferece suporte a $filter.|
|displayName|String|O nome exibido para o usuário no catálogo de endereços. Geralmente o valor é a combinação do nome, da inicial do nome do meio e do sobrenome do usuário. Essa propriedade é obrigatória quando um usuário é criado e não pode ser apagado durante atualizações. Oferece suporte a $filter e $orderby.|
|employeeId|String|O identificador de funcionário atribuído ao usuário pela organização. Oferece suporte a $filter.|
|externalUserState|String|Para um usuário externo convidado para o locatário usando a [API de convite](../api/invitation-post.md), essa propriedade representa o status do convite do usuário convidado. Para usuários convidados, o estado pode ser `PendingAcceptance` ou `Accepted` ou `null` para todos os outros usuários. Suporta o $filter com os valores compatíveis. Por exemplo: `$filter=externalUserState eq 'PendingAcceptance'`.|
|externalUserStateChangeDateTime|String|Mostra o carimbo de hora da alteração mais recente da propriedade externalUserState.|
|FaxNumber|String|O número de fax do usuário.|
|givenName|String|O nome fornecido (nome) do usuário. Oferece suporte a $filter.|
|hireDate|DateTimeOffset|A data de contratação do usuário. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|id|String|O identificador exclusivo do usuário. Herdado de [directoryObject](directoryobject.md). Chave. Não anulável. Somente leitura.|
|Identidades|Coleção [objectIdentity](objectIdentity.md)| Representa as identidades que podem ser usadas para entrar nesta conta de usuário. Uma identidade pode ser fornecida pela Microsoft, por organizações ou por provedores de identidade social, como o Facebook, Google e Microsoft, e está vinculada a uma conta de usuário. Pode conter vários itens com o mesmo valor **signInType**. <br>Oferece suporte a $filter.|
|interests|Coleção de cadeias de caracteres|Uma lista para o usuário descrever os interesses dele.|
|isResourceAccount|Booliano| `true`Se o usuário for uma conta de recurso, caso contrário`false` O valor nulo deve ser considerado `false`.|
|jobTitle|String|O cargo do usuário. Oferece suporte a $filter.|
|lastPasswordChangeDateTime|DateTimeOffset| A hora em que o usuário do Azure AD alterou a senha dele pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|legalAgeGroupClassification|String| Usado por aplicativos empresariais para determinar a faixa etária legal do usuário. Essa propriedade é somente leitura e calculada com base nas propriedades **ageGroup ** e **consentProvidedForMinor **. Valores permitidos: `null`, `minorWithOutParentalConsent`, `minorWithParentalConsent`, `minorNoParentalConsentRequired`, `notAdult` e `adult`. Confira as [definições de propriedades da faixa etária legal](#legal-age-group-property-definitions) para obter mais informações.|
|licenseAssignmentStates|Coleção [licenseAssignmentState](licenseassignmentstate.md)|Estado das atribuições de licenças para esse usuário. Somente leitura.|
|email|String|O endereço SMTP do usuário, por exemplo, "jeff@contoso.onmicrosoft.com". Somente Leitura. Oferece suporte a $filter.|
|mailboxSettings|[mailboxSettings](mailboxsettings.md)|Configurações para a caixa de correio principal do usuário conectado. Você pode [obter](../api/user-get-mailboxsettings.md) ou [atualizar](../api/user-update-mailboxsettings.md) as configurações de localidade, fuso horário ou de envio de respostas automáticas a mensagens de entrada.|
|mailNickname|String|O alias de email do usuário. Essa propriedade deve ser especificada quando um usuário é criado. Oferece suporte a $filter.|
|mobilePhone|String|O número de celular principal do usuário.|
|mySite|String|A URL do site pessoal do usuário.|
|officeLocation|String|A localização do escritório no local de trabalho do usuário.|
|onPremisesDistinguishedName|String| Contém o `distinguished name` do Active Directory no local ou `DN`. A propriedade somente é preenchida para os clientes que estejam sincronizando o seu diretório local ao Azure Active Directory pelo Azure AD Connect. Somente leitura. |
|onPremisesDomainName|String| Contém o `domainFQDN` local, também chamado dnsDomainName sincronizado do diretório local. A propriedade somente é preenchida para os clientes que estejam sincronizando o seu diretório local ao Azure Active Directory pelo Azure AD Connect. Somente leitura. |
|onPremisesExtensionAttributes|[onPremisesExtensionAttributes](onpremisesextensionattributes.md)|Contém extensionAttributes 1-15 para o usuário. Observe que os atributos de extensão individuais não são selecionáveis nem filtráveis. Para um usuário `onPremisesSyncEnabled`, esse conjunto de propriedades é masterizado no local e somente leitura. Para um usuário somente na nuvem (onde `onPremisesSyncEnabled` é falso), essas propriedades podem ser definidas durante a criação ou atualização. |
|onPremisesImmutableId|String|Essa propriedade é usada para associar uma conta de usuário do Active Directory local com seu objeto de usuário do Azure AD. Essa propriedade é usada para associar uma conta de usuário do Active Directory local com seu objeto de usuário do Azure AD. Essa propriedade deverá ser especificada ao criar uma nova conta de usuário no Graph se você estiver usando um domínio federado para a propriedade `userPrincipalName` (UPN) do usuário. Importante: Os caracteres  e _ não podem ser usados ao especificar essa propriedade. Oferece suporte a $filter. **Importante:** Os caracteres **$** e **_** e não podem ser usados ao especificar essa propriedade. Oferece suporte a $filter. |
|onPremisesLastSyncDateTime|DateTimeOffset|Indica a última vez em que o objeto foi sincronizado com o diretório local; por exemplo: "2013-02-16T03:04:54Z". O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.|
|onPremisesProvisioningErrors|coleção [OnPremisesProvisioningError](onpremisesprovisioningerror.md)| Erros ao usar o produto de sincronização da Microsoft durante o provisionamento. |
|onPremisesSamAccountName|String| Contém o `sAMAccountName` local sincronizado no diretório local. A propriedade somente é preenchida para os clientes que estejam sincronizando o seu diretório local ao Azure Active Directory pelo Azure AD Connect. Somente leitura. |
|onPremisesSecurityIdentifier|String|Contém o identificador de segurança (SID) local do usuário que foi sincronizado do local com a nuvem. Somente leitura.|
|onPremisesSyncEnabled|Booliano| `true` se esse objeto está sincronizado de um diretório local; `false` se esse objeto foi originalmente sincronizado de um diretório local, mas não está mais sincronizado; `null` se esse objeto nunca foi sido sincronizado de um diretório local (padrão).  Somente leitura |
|onPremisesUserPrincipalName|String| Contém o `userPrincipalName` local sincronizado no diretório local. A propriedade somente é preenchida para os clientes que estejam sincronizando o seu diretório local ao Azure Active Directory pelo Azure AD Connect. Somente leitura. |
|otherMails|String| Uma lista de endereços de email adicional para o usuário; Por exemplo: `["bob@contoso.com", "Robert@fabrikam.com"]`. Oferece suporte a $filter.|
|passwordPolicies|String|Especifica as políticas de senha do usuário. Esse valor é uma enumeração cujo um dos valores possíveis é "DisableStrongPassword", o que permite especificar senhas mais fracas do que a política padrão. Também é possível especificar "DisablePasswordExpiration". Ambos podem ser especificados juntos; por exemplo: "DisablePasswordExpiration, DisableStrongPassword".|
|passwordProfile|[passwordProfile](passwordprofile.md)|Especifica o perfil de senha do usuário. O perfil contém a senha do usuário. Essa propriedade é obrigatória quando um usuário é criado. A senha no perfil deve atender a requisitos mínimos, conforme especificado pela propriedade **passwordPolicies**. Por padrão, é obrigatória uma senha forte.|
|pastProjects|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar seus projetos anteriores.|
|postalCode|String|O código postal do endereço postal do usuário. O código postal é específico para o país/região do usuário. Nos Estados Unidos, esse atributo contém o CEP.|
|preferredDataLocation|String|O local de dados preferido para o usuário. Para saber mais, confira [OneDrive Online Multi-Geo](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction).|
|preferredLanguage|String|O idioma preferencial do usuário. Deve seguir o código ISO 639-1; por exemplo "en-US".|
|preferredName|String|O nome preferencial do usuário.|
|provisionedPlans|coleção [provisionedPlan](provisionedplan.md)|Os planos que estão provisionados para o usuário. Somente leitura. Não anulável. |
|proxyAddresses|Coleção de cadeias de caracteres|Por exemplo: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` O operador **any** é obrigatório para expressões de filtro em propriedades de vários valores. Somente leitura, não anulável. Oferece suporte a $filter.          |
|refreshTokensValidFromDateTime|DateTimeOffset| Os tokens de atualização ou de sessão (cookies de sessão) emitidos antes dessa hora são inválidos e os aplicativos recebem um erro ao usar um token de atualização ou de sessão inválido para adquirir um token de acesso delegado (para acessar APIs como o Microsoft Graph).  Se isso acontecer, o aplicativo precisará adquirir um novo token de atualização, fazendo uma solicitação ao ponto de extremidade de autorização. Somente leitura. Use [invalidateAllRefreshTokens](../api/user-invalidateallrefreshtokens.md) para redefinir.|
|responsibilities|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar suas responsabilidades.|
|schools|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar as escolas que frequentou.|
|showInAddressList|Booliano|`true` se a lista de endereços global do Outlook deve conter o usuário, caso contrário `false`. Se não estiver configurado, isso será tratado como `true`. Para os usuários convidados por meio do Gerenciador de convites, essa propriedade será definida como `false`.|
|signInSessionsValidFromDateTime|DateTimeOffset| Os tokens de atualização ou de sessão (cookies de sessão) emitidos antes dessa hora são inválidos e os aplicativos recebem um erro ao usar um token de atualização ou de sessão inválido para adquirir um token de acesso delegado (para acessar APIs como o Microsoft Graph).  Se isso acontecer, o aplicativo precisará adquirir um novo token de atualização, fazendo uma solicitação ao ponto de extremidade de autorização. Somente leitura. Use [revokeSignInSessions](../api/user-revokesigninsessions.md) para redefinir.|
|skills|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar suas qualificações.|
|state|String|O estado ou município no endereço do usuário. Oferece suporte a $filter.|
|streetAddress|String|O endereço do local de trabalho do usuário.|
|surname|String|O sobrenome do usuário (nome de família ou sobrenome). Oferece suporte a $filter.|
|usageLocation|String|Um código de duas letras (padrão ISO 3166). Obrigatório para os usuários que receberão licenças devido à exigência legal de verificar a disponibilidade de serviços nos países. Entre os exemplos temos: "US", "JP" e "GB". Não anulável. Oferece suporte a $filter.|
|userPrincipalName|String|O nome UPN do usuário. O nome UPN é um nome de logon para o usuário ao estilo da Internet com base na RFC 822 padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email do usuário. O formato geral é alias@domain, em que o domínio deve estar presente na coleção de domínios verificados do locatário. Essa propriedade é obrigatória quando um usuário é criado. Os domínios verificados para o locatário podem ser acessados pela propriedade **verifiedDomains** de [organization](organization.md). Oferece suporte a $filter e $orderby.
|userType|String|Um valor de cadeia de caracteres que pode ser usado para classificar tipos de usuários no seu diretório, como "Member" e "Guest". Oferece suporte a $filter.          |

### <a name="legal-age-group-property-definitions"></a>Definições de propriedade da faixa etária legal

Esta seção explica como as três propriedades de faixa etária (`legalAgeGroupClassification`, `ageGroup` e `consentProvidedForMinor`) são usadas pelos administradores do Azure AD e desenvolvedores de aplicativos empresariais para atender às normas de idade.

Por exemplo: Cameron é o administrador de um diretório em uma escola de ensino fundamental em Holyport, no Reino Unido. No início do ano letivo ele usa a documentação de admissão para obter o consentimento dos pais dos menores baseado nos regulamentos relacionadas com a idade no Reino Unido. O consentimento obtido do pai permite que a conta do menor seja usado pela escola de Holyport e os aplicativos da Microsoft. Cameron cria todas as contas e define o ageGroup para "menor" e consentProvidedForMinor para "concedido". Os aplicativos usados por seus alunos poderão, então suprimir recursos que não são adequados para menores.

#### <a name="legal-age-group-classification"></a>Classificação da faixa etária legal

Essa propriedade de somente leitura é usada por desenvolvedores de aplicativos empresariais para garantir a manipulação correta do usuário com base em sua faixa etária legal. É calculada com base nas propriedades de `ageGroup` e `consentProvidedForMinor` do usuário.

| Valor   | # |Descrição|
|:---------------|:--------|:----------|
|null|0|Valor padrão, nenhum `ageGroup` foi definido para o usuário.|
|minorWithoutParentalConsent |1|(Reservado para uso futuro)|
|minorWithParentalConsent|2| O usuário é considerado menor baseado nos regulamentos relacionados com a idade de seu país ou região, e o administrador da conta obteve o consentimento apropriado dos pais ou responsável.|
|adult|3|O usuário é considerado adulto baseado nos regulamentos relacionadas com a idade do seu país ou região.|
|notAdult|4|O usuário é de um país ou região com regulamentações adicionais relacionados à idade (por exemplo, Estados Unidos, Reino Unido, União Europeia ou Coreia do Sul) e a idade do usuário está entre menor e adulto (como estipulado com base no país ou região). Em geral, isso significa que adolescentes são considerados como `notAdult` em países regulamentados.|
|minorNoParentalConsentRequired|5|O usuário é menor de idade, mas é de um país ou região que não tem com regulamentações relacionadas com a idade.|

#### <a name="age-group-and-minor-consent"></a>Faixa etária e consentimento de menor

As propriedades de faixa etária e consentimento de menor são propriedades opcionais usadas por administradores do Azure AD para garantir que o uso da conta é tratado corretamente com base nas regras de regulamentação relacionadas à idade que regem o país ou a região do usuário.

#### <a name="agegroup-property"></a>propriedade ageGroup

| Valor    | # |Descrição|
|:---------------|:--------|:----------|
|null|0|Valor padrão, nenhum `ageGroup` foi definido para o usuário.|
|minor|1|O usuário é considerado menor de idade.|
|notAdult|2|O usuário é de um país que têm regulamentações estatutárias (Estados Unidos, Reino Unido, União Europeia ou Coreia do Sul) e a idade do usuário é maior do que o limite de idade para criança (conforme o país) e menor que o limite inferior de idade para adulto (como estipulado com base no país ou região). Basicamente, adolescentes são considerados como `notAdult` em países regulamentados.|
|adult|3|O usuário deve ser tratado como um adulto.|

#### <a name="consentprovidedforminor-property"></a>Propriedade consentProvidedForMinor

| Valor    | # |Descrição|
|:---------------|:--------|:----------|
|null|0|Valor padrão, nenhum `consentProvidedForMinor` foi definido para o usuário.|
|granted|1|O consentimento foi obtido para o usuário ter uma conta.|
|denied|2|O consentimento não foi obtido para o usuário ter uma conta.|
|notRequired|3|O usuário é de um local que não exige consentimento.|

## <a name="relationships"></a>Relações

| Relação | Tipo |Descrição|
|:---------------|:--------|:----------|
|agreementAcceptances|Coleção [agreementAcceptance](agreementacceptance.md)| Os termos de usuário do status de aceitação de uso. Somente leitura. Anulável.|
|calendar|[calendar](calendar.md)|O calendário principal do usuário. Somente leitura.|
|calendarGroups|Coleção [CalendarGroup](calendargroup.md)|Os grupos de calendários do usuário. Somente leitura. Anulável.|
|calendarView|Coleção [event](event.md)|O modo de exibição do calendário. Somente leitura. Anulável.|
|calendars|Coleção [calendar](calendar.md)|Os calendários do usuário. Somente leitura. Anulável.|
|contactFolders|Coleção [ContactFolder](contactfolder.md)|As pastas de contatos do usuário. Somente leitura. Anulável.|
|contacts|Coleção [Contact](contact.md)|Os contatos do usuário. Somente leitura. Anulável.|
|createdObjects|Coleção [directoryObject](directoryobject.md)|Objetos directory que foram criados pelo usuário. Somente leitura. Anulável.|
|directReports|Coleção [directoryObject](directoryobject.md)|Os usuários e contatos subordinados ao usuário. (Os usuários e contatos cuja propriedade manager está definida como esse usuário.) Somente leitura. Anulável. |
|drive|[drive](drive.md)|O OneDrive do usuário. Somente leitura.|
|unidades|Coleção [drive](drive.md)| Uma coleção de unidades disponíveis para este usuário. Somente leitura. |
|eventos|Coleção [event](event.md)|Os eventos do usuário. O padrão é mostrar eventos no Calendário Padrão. Somente leitura. Anulável.|
|extensions|Coleção [extension](extension.md)|A coleção de extensões abertas definidas para o usuário. Anulável.|
|inferenceClassification|[inferenceClassification](inferenceclassification.md)| Classificação de relevância das mensagens do usuário com base em designações explícitas que substituem a relevância ou importância deduzida. |
|insights|[officeGraphInsights](officegraphinsights.md) | Somente leitura. Anulável.|
|joinedGroups|Coleção [group](group.md)| Somente leitura. Anulável.|
|mailFolders|Coleção [mailFolder](mailfolder.md)| As pastas de email do usuário. Somente leitura. Anulável.|
|manager|[directoryObject](directoryobject.md)|O usuário ou contato que é o gerente do usuário. Somente leitura. (Métodos HTTP: GET, PUT, DELETE.)|
|memberOf|Coleção [directoryObject](directoryobject.md)|Os grupos e funções de diretório e unidades administrativas dos quais o usuário é membro. Somente leitura. Anulável.|
|joinedTeams|Coleção [team](team.md)|As equipes do Microsoft Teams do qual o usuário é membro. Somente leitura. Anulável.|
|trabalho em equipe|[userTeamwork](userteamwork.md)| Um contêiner dos recursos do Microsoft Teams disponíveis para o usuário. Somente leitura. Anulável.|
|messages|Coleção [message](message.md)|As mensagens em uma caixa de correio ou pasta. Somente leitura. Anulável.|
|onenote|[onenote](onenote.md)| Somente leitura.|
|outlook|[outlookUser](outlookuser.md)| Os serviços seletivos do Outlook disponíveis para o usuário. Somente leitura. Anulável.|
|ownedDevices|Coleção [directoryObject](directoryobject.md)|Dispositivos que pertencem ao usuário. Somente leitura. Anulável.|
|ownedObjects|Coleção [directoryObject](directoryobject.md)|Objetos de diretório que pertencem ao usuário. Somente leitura. Anulável.|
|people|Coleção [person](person.md)| Somente leitura. As pessoas mais relevantes para o usuário. A coleção é ordenada por relevância para o usuário, que é determinado pela comunicação e colaboração e pelas relações comerciais do usuário. Uma pessoa é uma agregação de informações provenientes de emails, contatos e redes sociais.|
|photo|[profilePhoto](profilephoto.md)| A foto de perfil do usuário. Somente leitura.|
|photos|coleção de [fotos](photo.md)| Somente leitura. Anulável.|
|planner|[plannerUser](planneruser.md)| Serviços de planejador seletivo disponíveis para o usuário. Somente leitura. Anulável. |
|scopedRoleMemberOf|Coleção [scopedRoleMembership](scopedrolemembership.md)| As associações de unidade administrativa de função com escopo deste usuário. Somente leitura. Anulável.|
|settings|[userSettings](user-settings.md) | Somente leitura. Anulável.|
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
    "drives",
    "events",
    "extensions",
    "joinedGroups",
    "mailFolders",
    "manager",
    "memberOf",
    "joinedTeams",
    "teamwork",
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
  "createdDateTime": "2019-02-07T21:53:13.067Z",
  "deletedDateTime": "String (timestamp)",
  "department": "string",
  "displayName": "string",
  "employeeId": "string",
  "externalUserState": "PendingAcceptance",
  "externalUserStateChangeDateTime": "2018-11-12T01:13:13Z",
  "faxNumber": "string",
  "givenName": "string",
  "hireDate": "String (timestamp)",
  "id": "string (identifier)",
  "identities": [{"@odata.type": "microsoft.graph.objectIdentity"}],
  "interests": ["string"],
  "isResourceAccount": false,
  "jobTitle": "string",
  "legalAgeGroupClassification": "string",
  "licenseAssignmentStates": [{"@odata.type": "microsoft.graph.licenseAssignmentState"}],
  "mail": "string",
  "mailboxSettings": {"@odata.type": "microsoft.graph.mailboxSettings"},
  "mailNickname": "string",
  "mobilePhone": "string",
  "mySite": "string",
  "officeLocation": "string",
  "onPremisesDistinguishedName": "string",
  "onPremisesDomainName": "string",
  "onPremisesExtensionAttributes": {"@odata.type": "microsoft.graph.onPremisesExtensionAttributes"},
  "onPremisesImmutableId": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSamAccountName": "string",
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
  "onPremisesUserPrincipalName": "string",
  "otherMails": "string",
  "passwordPolicies": "string",
  "passwordProfile": {"@odata.type": "microsoft.graph.passwordProfile"},
  "pastProjects": ["string"],
  "postalCode": "string",
  "preferredDataLocation": "string",
  "preferredLanguage": "string",
  "preferredName": "string",
  "provisionedPlans": [{"@odata.type": "microsoft.graph.provisionedPlan"}],
  "proxyAddresses": ["string"],
  "refreshTokensValidFromDateTime": "2019-02-07T21:53:13.084Z",
  "responsibilities": ["string"],
  "schools": ["string"],
  "showInAddressList": true,
  "signInSessionsValidFromDateTime": "2019-02-07T21:53:13.084Z",
  "skills": ["string"],
  "state": "string",
  "streetAddress": "string",
  "surname": "string",
  "usageLocation": "string",
  "userPrincipalName": "string",
  "userType": "string",
  "calendar": {"@odata.type": "microsoft.graph.calendar"},
  "calendarGroups": [{"@odata.type": "microsoft.graph.calendarGroup"}],
  "calendarView": [{"@odata.type": "microsoft.graph.event"}],
  "calendars": [{"@odata.type": "microsoft.graph.calendar"}],
  "contacts": [{"@odata.type": "microsoft.graph.contact"}],
  "contactFolders": [{"@odata.type": "microsoft.graph.contactFolder"}],
  "createdObjects": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "directReports": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "drive": {"@odata.type": "microsoft.graph.drive"},
  "drives": [{"@odata.type": "microsoft.graph.drive"}],
  "insights": {"@odata.type": "microsoft.graph.officeGraphInsights"},
  "settings": {"@odata.type": "microsoft.graph.userSettings"},
  "events": [{"@odata.type": "microsoft.graph.event"}],
  "extensions": [{"@odata.type": "microsoft.graph.extension"}],
  "inferenceClassification": {"@odata.type": "microsoft.graph.inferenceClassification"},
  "mailFolders": [{"@odata.type": "microsoft.graph.mailFolder"}],
  "manager": {"@odata.type": "microsoft.graph.directoryObject"},
  "memberOf": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "joinedTeams": [{"@odata.type": "microsoft.graph.group"}],
  "teamwork": {"@odata.type": "microsoft.graph.teamwork"},
  "messages": [{ "@odata.type": "microsoft.graph.message"}],
  "outlook": {"@odata.type": "microsoft.graph.outlookUser"},
  "ownedDevices": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "photo": {"@odata.type": "microsoft.graph.profilePhoto"},
  "registeredDevices": [{"@odata.type": "microsoft.graph.directoryObject"}]
}
```

## <a name="see-also"></a>Confira também

- [Adicionar dados personalizados a recursos usando extensões](/graph/extensibility-overview)
- [Adicionar dados personalizados aos usuários usando extensões abertas](/graph/extensibility-open-users)
- [Adicionar dados personalizados a grupos usando as extensões do esquema](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
