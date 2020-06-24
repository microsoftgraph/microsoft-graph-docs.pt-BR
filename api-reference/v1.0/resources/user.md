---
title: Tipo de recurso de usuário
description: Represents an Azure AD user account. Inherits from directoryObject.
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: f18cc3f56a39f072a6501c94e7f4179746d893f4
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845314"
---
# <a name="user-resource-type"></a>Tipo de recurso de usuário

Namespace: microsoft.graph

Represents an Azure AD user account. Inherits from [directoryObject](directoryobject.md).

Esse recurso permite:

- Adicionar seus próprios dados às propriedades personalizadas como [extensions](/graph/extensibility-overview).
- Assinar as [notificações de alteração](/graph/webhooks).
- Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/user-delta.md).

## <a name="methods"></a>Métodos

| Método                                                                                     | Tipo de retorno                                                                      | Descrição                                                                                                                                                                                                                         |
|:-------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [Listar usuários](../api/user-list.md)                                                          | Coleção [user](user.md)                                                       | Recuperar uma lista de objetos user.                                                                                                                                                                                                         |
| [Criar usuário](../api/user-post-users.md)                                                   | [user](user.md)                                                                  | Criar um novo objeto user.                                                                                                                                                                                                           |
| [Obter usuário](../api/user-get.md)                                                             | [user](user.md)                                                                  | Ler propriedades e relações do objeto user.                                                                                                                                                                                   |
| [Atualizar usuário](../api/user-update.md)                                                       | [user](user.md)                                                                  | Atualizar o objeto user.                                                                                                                                                                                                                 |
| [Excluir usuário](../api/user-delete.md)                                                       | Nenhum                                                                             | Excluir o objeto user.                                                                                                                                                                                                                 |
| [Obter delta](../api/user-delta.md)                                                          | Coleção [usuário](user.md)                                                       | Obter as alterações incrementais para usuários.                                                                                                                                                                                                  |
| **Atribuições de função de aplicativo**                                                                   |                                                                                  |                                                                                                                                                                                                                                     |
| [List appRoleAssignments](../api/user-list-approleassignments.md)                          | [appRoleAssignment](approleassignment.md) collection                             | Obtenha os aplicativos e as funções de aplicativo que esse usuário foi atribuído.                                                                                                                                                                       |
| [Adicionar appRoleAssignment](../api/user-post-approleassignments.md)                            | [appRoleAssignment](approleassignment.md)                                        | Atribuir uma função de aplicativo a este usuário.                                                                                                                                                                                                    |
| [Remover appRoleAssignment](../api/user-delete-approleassignments.md)                       | Nenhum                                                                             | Remova uma atribuição de função de aplicativo deste usuário.                                                                                                                                                                                       |
| **Calendário**                                                                               |                                                                                  |                                                                                                                                                                                                                                     |
| [Criar calendário](../api/user-post-calendars.md)                                           | [Calendar](calendar.md)                                                          | Criar um novo Calendar postando na coleção calendars.                                                                                                                                                                       |
| [Criar calendarGroup](../api/user-post-calendargroups.md)                                 | [CalendarGroup](calendargroup.md)                                                | Criar um novo CalendarGroup postando na coleção calendarGroups.                                                                                                                                                             |
| [Criar evento](../api/user-post-events.md)                                                 | [event](event.md)                                                                | Criar um novo Event postando na coleção de eventos.                                                                                                                                                                             |
| [findMeetingTimes](../api/user-findmeetingtimes.md)                                        | [meetingTimeSuggestionsResult](meetingtimesuggestionsresult.md)                  | Encontrar o tempo e locais para reunião com base na disponibilidade dos participantes, localização ou restrições de tempo.                                                                                                                                      |
| [getSchedule](../api/calendar-getschedule.md)                                              | [scheduleInformation](scheduleinformation.md)                                    | Adquira as informações de disponibilidade para um conjunto de usuários, listas de distribuição ou recursos (salas e equipamentos) para um período de tempo especificado.                                                                           |
| [Listar calendários](../api/user-list-calendars.md)                                            | Coleção [calendar](calendar.md)                                               | Obter uma coleção de objetos Calendar.                                                                                                                                                                                                   |
| [Listar calendarGroups](../api/user-list-calendargroups.md)                                  | Coleção de [CalendarGroup](calendargroup.md)                                     | Obter uma coleção de objetos CalendarGroup.                                                                                                                                                                                              |
| [Listar calendarView](../api/user-list-calendarview.md)                                      | Coleção [event](event.md)                                                     | Obtenha uma coleção do objeto Event.                                                                                                                                                                                                      |
| [Listar eventos](../api/user-list-events.md)                                                  | Coleção [event](event.md)                                                     | Get a list of event objects in the user's mailbox. The list contains single instance meetings and series masters.                                                                                                                   |
| [reminderView](../api/user-reminderview.md)                                                | Coleção [Reminder](reminder.md)                                               | Retorna uma lista de lembretes de calendário nas horas de início e término especificadas.                                                                                                                                                       |
| **Contatos**                                                                               |                                                                                  |                                                                                                                                                                                                                                     |
| [Criar contato](../api/user-post-contacts.md)                                             | [contato](contact.md)                                                            | Criar um novo Contact postando na coleção contacts.                                                                                                                                                                         |
| [Criar contactFolder](../api/user-post-contactfolders.md)                                 | [pastadeContatos](contactfolder.md)                                                | Criar uma nova ContactFolder postando na coleção contactFolders.                                                                                                                                                             |
| [Listar contatos](../api/user-list-contacts.md)                                              | Coleção de[contato](contact.md)                                                 | Obter uma coleção de contatos da pasta Contatos padrão do usuário conectado.                                                                                                                                                    |
| [Listar contactFolders](../api/user-list-contactfolders.md)                                  | Coleção de [pastadeContatos](contactfolder.md)                                     | Obter a coleção de pastas de contatos na pasta Contatos padrão do usuário conectado.                                                                                                                                             |
| **Objetos de diretório**                                                                      |                                                                                  |                                                                                                                                                                                                                                     |
| [assignLicense](../api/user-assignlicense.md)                                              | [user](user.md)                                                                  | Add or remove subscriptions for the user. You can also enable and disable specific plans associated with a subscription.                                                                                                            |
| [checkMemberGroups](../api/user-checkmembergroups.md)                                      | Coleção de cadeias de caracteres                                                                | Check for membership in a list of groups. The check is transitive.                                                                                                                                                                  |
| [checkMemberObjects](../api/user-checkmemberobjects.md)                                    | Coleção de cadeias de caracteres                                                                | Verifique se há associação em uma lista de grupo, função de diretório ou objetos de unidade administrativa. Essa função é transitiva.                                                                                                                |
| [exportPersonalData](../api/user-exportpersonaldata.md)                                    | Nenhum                                                                             | Envia uma solicitação de operação de política de dados, realizada por um administrador da empresa para exportar os dados de um usuário da organização.                                                                                                                   |
| [getByIds](../api/directoryobject-getbyids.md)                                             | Coleção de cadeias de caracteres                                                                | Retorna os objetos de diretório especificados a partir de uma lista de ids.                                                                                                                                                                           |
| [getMemberGroups](../api/user-getmembergroups.md)                                          | Coleção de cadeias de caracteres                                                                | Return all the groups that the user is a member of. The check is transitive.                                                                                                                                                        |
| [getMemberObjects](../api/user-getmemberobjects.md)                                        | String collection                                                                | Return all of the groups and directory roles that the user is a member of. The check is transitive.                                                                                                                                 |
| [Listar createdObjects](../api/user-list-createdobjects.md)                                  | Coleção [directoryObject](directoryobject.md)                                 | Obter os objetos directory criados pelo usuário da propriedade de navegação createdObjects.                                                                                                                                          |
| [Listar licenseDetails](../api/user-list-licensedetails.md)                                  | Coleção [licenseDetails](licensedetails.md)                                   | Obtenha uma coleção de objetos licenseDetails.                                                                                                                                                                                             |
| [Listar ownedDevices](../api/user-list-owneddevices.md)                                      | Coleção [directoryObject](directoryobject.md)                                 | Obter os dispositivos que pertencem ao usuário da propriedade de navegação ownedDevices.                                                                                                                                               |
| [Listar ownedObjects](../api/user-list-ownedobjects.md)                                      | [directoryObject](directoryobject.md) collection                                 | Obter os objetos directory que pertencem ao usuário da propriedade de navegação ownedObjects.                                                                                                                                     |
| [Listar registeredDevices](../api/user-list-registereddevices.md)                            | Coleção [directoryObject](directoryobject.md)                                 | Obter os dispositivos que estão registrados para o usuário da propriedade de navegação registeredDevices.                                                                                                                                    |
| [reprocessLicense](../api/user-reprocesslicenseassignment.md)                              | [user](user.md)                                                                  | Reprocessar as atribuições de assinatura do usuário.                                                                                                                                                                                    |
| [revokeSignInSessions](../api/user-revokesigninsessions.md)                                | Nenhum                                                                             | Revoga todos os tokens de sessão e de atualização do usuário emitidos para aplicativos, redefinindo a propriedade do usuário **signInSessionsValidFromDateTime** para data e a hora atuais. Força o usuário a entrar novamente nesses aplicativos. |
| **Drive**                                                                                  |                                                                                  |                                                                                                                                                                                                                                     |
| [Obter unidade](../api/drive-get.md)                                                           | [unidade](drive.md)                                                                | Recuperar as propriedades e as relações de um recurso Drive.                                                                                                                                                                      |
| [Filhos de lista](../api/driveitem-list-children.md)                                         | [DriveItems](driveitem.md)                                                       | Retornar uma coleção de DriveItems no relacionamento filho de um DriveItem.                                                                                                                                                      |
| **Grupos**                                                                                 |                                                                                  |                                                                                                                                                                                                                                     |
| [Listar joinedTeams](../api/user-list-joinedteams.md)                                        | Coleção [team](team.md)                                                       | Obter as equipes do Microsoft Teams no qual o usuário é membro direto da propriedade de navegação joinedTeams.                                                                                                                         |
| [Listar memberOf](../api/user-list-memberof.md)                                              | [directoryObject](directoryobject.md) collection                                 | Obter os grupos e as funções de diretório dos quais o usuário é membro direto da propriedade de navegação memberOf.                                                                                                                       |
| [Listar memberOf transitivos](../api/user-list-transitivememberof.md)                         | Coleção [directoryObject](directoryobject.md)                                 | Enumera os grupos e as funções de diretório dos quais o usuário é membro. Essa operação é transitiva e inclui os grupos dos quais o usuário é membro aninhado.                                                                         |
| **Email**                                                                                   |                                                                                  |                                                                                                                                                                                                                                     |
| [Create inferenceClassificationOverride](../api/inferenceclassification-post-overrides.md) | Criar uma substituição da Caixa de Entrada Destaques para um remetente identificado por um endereço SMTP.      |                                                                                                                                                                                                                                     |
| [Criar MailFolder](../api/user-post-mailfolders.md)                                       | [mailFolder](mailfolder.md)                                                      | Criar uma nova MailFolder postando na coleção mailFolders.                                                                                                                                                                   |
| [Criar mensagem](../api/user-post-messages.md)                                             | [message](message.md)                                                            | Criar uma nova Mensagem postando na coleção messages.                                                                                                                                                                         |
| [Criar messageRule](../api/mailfolder-post-messagerules.md)                               | [messageRule](messagerule.md)                                                    | Crie um objeto messageRule especificando um conjunto de condições e ações.                                                                                                                                                          |
| [getMailTips](../api/user-getmailtips.md)                                                  | Coleção [mailTips](mailtips.md)                                               | Retornar dicas de email de um ou mais destinatários conforme disponíveis para o usuário conectado.                                                                                                                                                   |
| [Listar mailFolders](../api/user-list-mailfolders.md)                                        | Coleção [mailFolder](mailfolder.md)                                           | Obter o conjunto de pastas de email sob a pasta raiz do usuário conectado.                                                                                                                                                         |
| [Listar mensagens](../api/user-list-messages.md)                                              | Coleção [message](message.md)                                                 | Obter todas as mensagens na caixa de correio do usuário conectado.                                                                                                                                                                               |
| [List overrides](../api/inferenceclassification-list-overrides.md)                         | Coleção [inferenceClassificationOverride](inferenceclassificationoverride.md) | Obtenha as substituições da Caixa de Entrada Destaques que um usuário configurou para sempre classificar as mensagens de determinados remetentes de maneiras específicas.                                                                                                           |
| [Listar regras](../api/mailfolder-list-messagerules.md)                                       | Coleção [messageRule](messagerule.md)                                         | Obtenha todos os objetos messageRule definidos para a caixa de entrada do usuário.                                                                                                                                                                       |
| [Enviar email](../api/user-sendmail.md)                                                       | Nenhum                                                                             | Enviar a mensagem especificada no corpo da solicitação.                                                                                                                                                                                     |
| **Anotações**                                                                                  |                                                                                  |                                                                                                                                                                                                                                     |
| [Criar bloco de anotações](../api/onenote-post-notebooks.md)                                        | [bloco de anotações](notebook.md)                                                          | Crie um novo bloco de anotações do OneNote.                                                                                                                                                                                                      |
| [Listar blocos de anotações](../api/onenote-list-notebooks.md)                                         | Coleção [bloco de anotações](notebook.md)                                               | Recuperar uma lista de objetos do bloco de anotações.                                                                                                                                                                                                |
| **Extensões abertas**                                                                        |                                                                                  |                                                                                                                                                                                                                                     |
| [Criar extensão aberta](../api/opentypeextension-post-opentypeextension.md)                | [openTypeExtension](opentypeextension.md)                                        | Crie uma extensão aberta e adicione propriedades personalizadas a uma instância nova ou existente de um recurso.                                                                                                                                                   |
| [Obter extensão aberta](../api/opentypeextension-get.md)                                      | Coleção [openTypeExtension](opentypeextension.md)                             | Obtenha uma extensão aberta identificada pelo nome da extensão.                                                                                                                                                                             |
| **Hierarquia da organização**                                                                          |                                                                                  |                                                                                                                                                                                                                                     |
| [Atribuir gerente](../api/user-post-manager.md)                                              | [directoryObject](directoryobject.md)                                            | Atribuir um usuário ou um contato organizacional como o gerente do usuário.                                                                                                                                                                  |
| [Obter gerenciador](../api/user-list-manager.md)                                                 | [directoryObject](directoryobject.md)                                            | Obter o usuário ou o contato organizacional que é o gerente do usuário da propriedade de navegação do gerente.                                                                                                                            |
| [Listar directReports](../api/user-list-directreports.md)                                    | Coleção [directoryObject](directoryobject.md)                                 | Obter os usuários ou contatos subordinados ao usuário da propriedade de navegação directReports.                                                                                                                                      |
| **Configurações do Outlook**                                                                       |                                                                                  |                                                                                                                                                                                                                                     |
| [Criar categoria do Outlook](../api/outlookuser-post-mastercategories.md)                     | [outlookCategory](outlookcategory.md)                                            | Cria um objeto outlookCategory na lista mestra de categorias do usuário.                                                                                                                                                           |
| [Obter supportedLanguages](../api/outlookuser-supportedlanguages.md),                         | Coleção [localeInfo](localeinfo.md)                                           | Obtém a lista de locais e idiomas com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.                                                                                                                  |
| [Obter supportedTimeZones](../api/outlookuser-supportedtimezones.md)                         | [timeZoneInformation](timezoneinformation.md collection)                         | Obtém a lista de fusos horários com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.                                                                                                                             |
| [Obtém configurações de caixa de correio do usuário](../api/user-get-mailboxsettings.md)                            | [mailboxSettings](mailboxsettings.md)                                            | Obtém as configurações de caixa de correio do usuário.                                                                                                                                                                                                     |
| [Listar as categorias do Outlook](../api/outlookuser-list-mastercategories.md)                     | Coleção [outlookCategory](outlookcategory.md)                                 | Obtém todas as categorias que foram definidas para o usuário.                                                                                                                                                                         |
| [Converter IDs do Exchange](../api/user-translateexchangeids.md)                              | coleção [convertIdResult](convertidresult.md)                                 | Traduzir os identificadores de recursos relacionados ao Outlook entre formatos.                                                                                                                                                                 |
| [Atualizar configurações da caixa de correio do usuário](../api/user-update-mailboxsettings.md)                      | [mailboxSettings](mailboxsettings.md)                                            | Habilitar, configurar ou desabilitar o mailboxSettings de um ou mais usuários.                                                                                                                                                                   |
| **Foto**                                                                                  |                                                                                  |                                                                                                                                                                                                                                     |
| [Obter foto](../api/profilephoto-get.md)                                                    | [profilePhoto](profilephoto.md)                                                  | Obtém o profilePhoto especificado ou seus metadados (propriedades profilePhoto).                                                                                                                                                           |
| [Atualizar profilephoto](../api/profilephoto-update.md)                                       | Nenhum                                                                             | Atualiza a foto de qualquer usuário no locatário, incluindo o usuário conectado ou o grupo ou contato especificado.                                                                                                                        |
| **Planejador**                                                                                |                                                                                  |                                                                                                                                                                                                                                     |
| [Listar tarefas](../api/planneruser-list-tasks.md)                                             | Coleção [plannerTask](plannertask.md)                                         | Obter o plannerTasks atribuído ao usuário.                                                                                                                                                                                              |
| **Extensões de esquema**                                                                      |                                                                                  |                                                                                                                                                                                                                                     |
| [Adicionar valores de extensões de esquema](/graph/extensibility-schema-groups)                          | Nenhum                                                                             | Cria uma definição para a extensão de esquema e usa-a para adicionar dados digitados personalizados a um recurso.                                                                                                                                        |
| **Configurações do usuário**                                                                          |                                                                                  |                                                                                                                                                                                                                                     |
| [Obter configurações](../api/usersettings-get.md)                                                 | [userSettings](usersettings.md)                                                  | Leia o usuário e o objeto de configurações da organização.                                                                                                                                                                                     |
| [Atualizar configurações](../api/usersettings-update.md)                                           | [userSettings](usersettings.md)                                                  | Atualize as propriedades do objeto de configurações.                                                                                                                                                                                       |

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo    |Descrição|
|:---------------|:--------|:----------|
|aboutMe|String|Um campo de entrada de texto em forma livre para o usuário se descrever.|
|accountEnabled|Boolean| **true** if the account is enabled; otherwise, **false**. This property is required when a user is created. Supports $filter.    |
|ageGroup|String|Define a faixa etária do usuário. Valores permitidos: `null`, `minor`, `notAdult` e `adult`. Confira as [definições de propriedades da faixa etária legal](#legal-age-group-property-definitions) para obter mais informações. |
|assignedLicenses|Coleção [assignedLicense](assignedlicense.md)|The licenses that are assigned to the user. Not nullable.            |
|assignedPlans|Coleção [assignedPlan](assignedplan.md)|The plans that are assigned to the user. Read-only. Not nullable. |
|birthday|DateTimeOffset|The birthday of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|businessPhones|Coleção de cadeias de caracteres|The telephone numbers for the user. NOTE: Although this is a string collection, only one number can be set for this property.|
|city|String|The city in which the user is located. Supports $filter.|
|companyName | String | O nome da empresa em que o usuário está associado. Essa propriedade pode ser útil para descrever a empresa de onde procede um usuário externo. |
|consentProvidedForMinor|String|Define se o consentimento foi obtido para menores. Valores permitidos: `null`, `granted`, `denied` e `notRequired`. Confira as [definições de propriedades da faixa etária legal](#legal-age-group-property-definitions) para obter mais informações.|
|country|Cadeia de caracteres|The country/region in which the user is located; for example, “US” or “UK”. Supports $filter.|
|createdDateTime | DateTimeOffset |Data de criação do objeto do usuário. |
|creationType|String|Indica se a conta de usuário foi criada como uma conta corporativa ou de estudante (`null`), uma conta externa (`Invitation`), uma conta local para um locatário do Azure Active Directory B2C (`LocalAccount`) ou uma inscrição de autoatendimento usando a verificação de email (`EmailVerified`). Somente leitura.|
|deletedDateTime| DateTimeOffset | A data e hora que o usuário foi excluído. <br><br>Retornado apenas em $select. |
|department|String|The name for the department in which the user works. Supports $filter.|
|displayName|String|The name displayed in the address book for the user. This is usually the combination of the user's first name, middle initial and last name. This property is required when a user is created and it cannot be cleared during updates. Supports $filter and $orderby.|
|employeeId|String|O identificador de funcionário atribuído ao usuário pela organização. Com suporte para $filter.|
|externalUserState|String|Para um usuário externo convidado para o locatário usando a [API de convite](../api/invitation-post.md), essa propriedade representa o status do convite do usuário convidado. Para usuários convidados, o estado pode ser `PendingAcceptance` ou `Accepted` ou `null` para todos os outros usuários. <br><br>Retornado apenas `$select` . Oferece suporte `$filter` com os valores com suporte. Por exemplo: `$filter=externalUserState eq 'PendingAcceptance'`.|
|externalUserStateChangeDateTime|DateTimeOffset|Mostra o carimbo de data/hora da última alteração na propriedade **externalUserState** . <br><br>Retornado apenas `$select` .|
|faxNumber|String|O número de fax do usuário.|
|givenName|String|The given name (first name) of the user. Supports $filter.|
|hireDate|DateTimeOffset|The hire date of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`|
|id|String|The unique identifier for the user. Inherited from [directoryObject](directoryobject.md). Key. Not nullable. Read-only.|
|Identidades|Coleção [objectIdentity](objectIdentity.md)| Representa as identidades que podem ser usadas para entrar nesta conta de usuário. Uma identidade pode ser fornecida pela Microsoft (também conhecida como conta local), por organizações ou por provedores de identidade social, como o Facebook, Google e Microsoft, e está vinculada a uma conta de usuário. Pode conter vários itens com o mesmo valor **signInType**. <br>Oferece suporte a $filter.|
|imAddresses|String collection|The instant message voice over IP (VOIP) session initiation protocol (SIP) addresses for the user. Read-only.|
|interests|Coleção de cadeias de caracteres|Uma lista para o usuário descrever os interesses dele.|
|isResourceAccount|Booliano| **Verdadeiro** se o usuário é uma conta de recursos; caso contrário, **falso**. O valor nulo deve ser considerado **falso**.|
|jobTitle|String|The user’s job title. Supports $filter.|
|lastPasswordChangeDateTime| DateTimeOffset | A hora em que o usuário do Azure AD alterou a senha dele pela última vez. As informações de data e hora usam o formato ISO 8601 e estão sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'|
|legalAgeGroupClassification|String| Usado por aplicativos empresariais para determinar a faixa etária legal do usuário. Essa propriedade é somente leitura e calculada com base nas propriedades `ageGroup` e `consentProvidedForMinor`. Valores permitidos: `null`, `minorWithOutParentalConsent`, `minorWithParentalConsent`, `minorNoParentalConsentRequired`, `notAdult` e `adult`. Confira as [definições de propriedades da faixa etária legal](#legal-age-group-property-definitions) para obter mais informações.|
|licenseAssignmentStates|Coleção [licenseAssignmentState](licenseassignmentstate.md)|Estado das atribuições de licenças para esse usuário. Somente leitura.|
|email|String|The SMTP address for the user, for example, "jeff@contoso.onmicrosoft.com". Read-Only. Supports $filter.|
|mailboxSettings|[mailboxSettings](mailboxsettings.md)|Settings for the primary mailbox of the signed-in user. You can [get](../api/user-get-mailboxsettings.md) or [update](../api/user-update-mailboxsettings.md) settings for sending automatic replies to incoming messages, locale and time zone.|
|mailNickname|String|The mail alias for the user. This property must be specified when a user is created. Supports $filter.|
|mobilePhone|String|O número de celular principal do usuário.|
|mySite|String|A URL do site pessoal do usuário.|
|officeLocation|String|A localização do escritório no local de trabalho do usuário.|
|onPremisesDistinguishedName|String| Contém o `distinguished name` do Active Directory no local ou `DN`. A propriedade somente é preenchida para os clientes que estejam sincronizando o seu diretório local ao Azure Active Directory pelo Azure AD Connect. Somente leitura. |
|onPremisesDomainName|String| Contém o `domainFQDN` local, também chamado dnsDomainName sincronizado do diretório local. A propriedade somente é preenchida para os clientes que estejam sincronizando o seu diretório local ao Azure Active Directory pelo Azure AD Connect. Somente leitura. |
|onPremisesExtensionAttributes|[onPremisesExtensionAttributes](onpremisesextensionattributes.md)|Contém extensionAttributes 1-15 para o usuário. Observe que os atributos de extensão individuais não são selecionáveis nem filtráveis. Para um usuário `onPremisesSyncEnabled`, esse conjunto de propriedades é masterizado no local e somente leitura. Para um usuário somente na nuvem (onde `onPremisesSyncEnabled` é falso), essas propriedades podem ser definidas durante a criação ou atualização. |
|onPremisesImmutableId|String|Essa propriedade é usada para associar uma conta de usuário do Active Directory local com seu objeto de usuário do Azure AD. Esta propriedade deverá ser especificada ao criar uma nova conta de usuário no Graph se você estiver usando um domínio federado para a propriedade **userPrincipalName** (UPN) do usuário. **Importante:** Os caracteres **$** e **\_** não podem ser usados ao especificar esta propriedade. Oferece suporte a $filter.                            |
|onPremisesLastSyncDateTime|DateTimeOffset|Indicates the last time at which the object was synced with the on-premises directory; for example: "2013-02-16T03:04:54Z". The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.|
|onPremisesProvisioningErrors|coleção [OnPremisesProvisioningError](onpremisesprovisioningerror.md)| Erros ao usar o produto de sincronização da Microsoft durante o provisionamento. |
|onPremisesSamAccountName|Cadeia de Caracteres| Contém o `samAccountName` local sincronizado no diretório local. A propriedade somente é preenchida para os clientes que estejam sincronizando o seu diretório local ao Azure Active Directory pelo Azure AD Connect. Somente leitura. |
|onPremisesSecurityIdentifier|String|Contains the on-premises security identifier (SID) for the user that was synchronized from on-premises to the cloud. Read-only.|
|onPremisesSyncEnabled|Booliano| **true** if this object is synced from an on-premises directory; **false** if this object was originally synced from an on-premises directory but is no longer synced; **null** if this object has never been synced from an on-premises directory (default). Read-only |
|onPremisesUserPrincipalName|String| Contém o `userPrincipalName` local sincronizado no diretório local. A propriedade somente é preenchida para os clientes que estejam sincronizando o seu diretório local ao Azure Active Directory pelo Azure AD Connect. Somente leitura. |
|otherMails|String| Uma lista de endereços de email adicional para o usuário; Por exemplo: `["bob@contoso.com", "Robert@fabrikam.com"]`. Oferece suporte a $filter.|
|passwordPolicies|String|Specifies password policies for the user. This value is an enumeration with one possible value being “DisableStrongPassword”, which allows weaker passwords than the default policy to be specified. “DisablePasswordExpiration” can also be specified. The two may be specified together; for example: "DisablePasswordExpiration, DisableStrongPassword".|
|passwordProfile|[passwordProfile](passwordprofile.md)|Specifies the password profile for the user. The profile contains the user’s password. This property is required when a user is created. The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property. By default, a strong password is required.|
|pastProjects|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar seus projetos anteriores.|
|postalCode|Cadeia de caracteres|The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code.|
|preferredDataLocation|String|O local de dados preferido para o usuário. Para saber mais, confira [OneDrive Online Multi-Geo](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction).|
|preferredLanguage|String|The preferred language for the user. Should follow ISO 639-1 Code; for example "en-US".|
|preferredName|String|O nome preferencial do usuário.|
|provisionedPlans|coleção [provisionedPlan](provisionedplan.md)|The plans that are provisioned for the user. Read-only. Not nullable. |
|proxyAddresses|Coleção de cadeias de caracteres|For example: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` The **any** operator is required for filter expressions on multi-valued properties. Read-only, Not nullable. Supports $filter.|
|refreshTokensValidFromDateTime|DateTimeOffset|Os tokens de atualização ou de sessão (cookies de sessão) emitidos antes dessa hora são inválidos e os aplicativos recebem um erro ao usar um token de atualização ou de sessão inválido para adquirir um token de acesso delegado (para acessar APIs como o Microsoft Graph).  Se isso acontecer, o aplicativo precisará adquirir um novo token de atualização, fazendo uma solicitação ao ponto de extremidade de autorização. <br><br>Retornado apenas em $select. Apenas leitura. |
|responsibilities|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar suas responsabilidades.|
|schools|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar as escolas que frequentou.|
|showInAddressList|Booliano|**true** se a lista de endereços global do Outlook deve conter o usuário, caso contrário **false**. Se não estiver configurado, isso será tratado como **true**. Para os usuários convidados por meio do Gerenciador de convites, essa propriedade será definida como **false**.|
|skills|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar suas qualificações.|
|signInSessionsValidFromDateTime|DateTimeOffset| Os tokens de atualização ou de sessão (cookies de sessão) emitidos antes dessa hora são inválidos e os aplicativos recebem um erro ao usar um token de atualização ou de sessão inválido para adquirir um token de acesso delegado (para acessar APIs como o Microsoft Graph).  Se isso acontecer, o aplicativo precisará adquirir um novo token de atualização, fazendo uma solicitação ao ponto de extremidade de autorização. Somente leitura. Use [revokeSignInSessions](../api/user-revokesigninsessions.md) para redefinir.|
|state|Cadeia de caracteres|The state or province in the user's address. Supports $filter.|
|streetAddress|String|O endereço do local de trabalho do usuário.|
|surname|String|The user's surname (family name or last name). Supports $filter.|
|usageLocation|String|A two letter country code (ISO standard 3166). Required for users that will be assigned licenses due to legal requirement to check for availability of services in countries.  Examples include: "US", "JP", and "GB". Not nullable. Supports $filter.|
|userPrincipalName|Cadeia de caracteres|The user principal name (UPN) of the user. The UPN is an Internet-style login name for the user based on the Internet standard RFC 822. By convention, this should map to the user's email name. The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains. This property is required when a user is created. The verified domains for the tenant can be accessed from the **verifiedDomains** property of [organization](organization.md). Supports $filter and $orderby.
|userType|String|A string value that can be used to classify user types in your directory, such as “Member” and “Guest”. Supports $filter.          |

### <a name="legal-age-group-property-definitions"></a>Definições de propriedade da faixa etária legal

Esta seção explica como as três propriedades de faixa etária (`legalAgeGroupClassification`, `ageGroup` e `consentProvidedForMinor`) são usadas pelos administradores do Azure AD e desenvolvedores de aplicativos empresariais para atender às normas de idade.

Por exemplo: Cameron é o administrador de um diretório em uma escola de ensino fundamental em Holyport, no Reino Unido. No início do ano letivo ele usa a documentação de admissão para obter o consentimento dos pais dos menores baseado nos regulamentos relacionadas com a idade no Reino Unido. O consentimento obtido do pai permite que a conta do menor seja usado pela escola de Holyport e os aplicativos da Microsoft. Cameron cria todas as contas e define o ageGroup para "menor" e consentProvidedForMinor para "concedido". Os aplicativos usados por seus alunos poderão, então suprimir recursos que não são adequados para menores.

#### <a name="legal-age-group-classification"></a>Classificação da faixa etária legal

Essa propriedade de somente leitura é usada por desenvolvedores de aplicativos empresariais para garantir a manipulação correta do usuário com base em sua faixa etária legal. É calculada com base nas propriedades de `ageGroup` e `consentProvidedForMinor` do usuário.

| Valor    | #  |Descrição|
|:---------------|:--------|:----------|
|null|,0|Valor padrão, nenhum `ageGroup` foi definido para o usuário.|
|minorWithoutParentalConsent |1 |(Reservado para uso futuro)|
|minorWithParentalConsent|2 | O usuário é considerado menor baseado nos regulamentos relacionados com a idade de seu país ou região, e o administrador da conta obteve o consentimento apropriado dos pais ou responsável.|
|adult|3 |O usuário é considerado adulto baseado nos regulamentos relacionadas com a idade do seu país ou região.|
|notAdult|4 |O usuário é de um país ou região com regulamentações adicionais relacionados à idade (por exemplo, Estados Unidos, Reino Unido, União Europeia ou Coreia do Sul) e a idade do usuário está entre menor e adulto (como estipulado com base no país ou região). Em geral, isso significa que adolescentes são considerados como `notAdult` em países regulamentados.|
|minorNoParentalConsentRequired|5 |O usuário é menor de idade, mas é de um país ou região que não tem com regulamentações relacionadas com a idade.|

#### <a name="age-group-and-minor-consent"></a>Faixa etária e consentimento de menor

As propriedades de faixa etária e consentimento de menor são propriedades opcionais usadas por administradores do Azure AD para garantir que o uso da conta é tratado corretamente com base nas regras de regulamentação relacionadas à idade que regem o país ou a região do usuário.

#### <a name="agegroup-property"></a>propriedade ageGroup

| Valor    | #  |Descrição|
|:---------------|:--------|:----------|
|null|,0|Valor padrão, nenhum `ageGroup` foi definido para o usuário.|
|minor|1 |O usuário é considerado um secundário.|
|notAdult|2 |O usuário é de um país que têm regulamentações estatutárias (Estados Unidos, Reino Unido, União Europeia ou Coreia do Sul) e a idade do usuário é maior do que o limite de idade para criança (conforme o país) e menor que o limite inferior de idade para adulto (como estipulado com base no país ou região). Basicamente, adolescentes são considerados como `notAdult` em países regulamentados.|
|adult|3 |O usuário deve ser tratado como um adulto.|

#### <a name="consentprovidedforminor-property"></a>Propriedade consentProvidedForMinor

| Valor    | #  |Descrição|
|:---------------|:--------|:----------|
|null|,0|Valor padrão, nenhum `consentProvidedForMinor` foi definido para o usuário.|
|granted|1 |O consentimento foi obtido para o usuário ter uma conta.|
|denied|2 |O consentimento não foi obtido para o usuário ter uma conta.|
|notRequired|3 |O usuário é de um local que não exige consentimento.|

## <a name="relationships"></a>Relações

| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|activities|Coleção [userActivity](projectrome-activity.md)|Atividades do usuário em vários dispositivos. Somente leitura. Anulável.|
|calendar|[calendar](calendar.md)|The user's primary calendar. Read-only.|
|calendarGroups|Coleção [CalendarGroup](calendargroup.md)|The user's calendar groups. Read-only. Nullable.|
|calendarView|Coleção [event](event.md)|The calendar view for the calendar. Read-only. Nullable.|
|calendars|Coleção [calendar](calendar.md)|The user's calendars. Read-only. Nullable.|
|contactFolders|Coleção [ContactFolder](contactfolder.md)|The user's contacts folders. Read-only. Nullable.|
|contacts|Coleção [Contact](contact.md)|The user's contacts. Read-only. Nullable.|
|createdObjects|Coleção [directoryObject](directoryobject.md)|Directory objects that were created by the user. Read-only. Nullable.|
|directReports|Coleção [directoryObject](directoryobject.md)|The users and contacts that report to the user. (The users and contacts that have their manager property set to this user.) Read-only. Nullable. |
|drive|[unidade](drive.md)|The user's OneDrive. Read-only.|
|unidades|Coleção [drive](drive.md)| A collection of drives available for this user. Read-only. |
|eventos|Coleção [event](event.md)|The user's events. Default is to show Events under the Default Calendar. Read-only. Nullable.|
|extensions|[extension](extension.md) collection|The collection of open extensions defined for the user. Read-only. Nullable.|
|inferenceClassification | [inferenceClassification](inferenceclassification.md) | Classificação de relevância das mensagens do usuário com base em designações explícitas que substituem a relevância ou importância deduzida. |
|insights|[officeGraphInsights](officegraphinsights.md) | Read-only. Nullable.|
|licenseDetails|Coleção de[licenseDetails](licensedetails.md)|Uma coleção de detalhes da licença do usuário. Somente leitura.|
|mailFolders|Coleção [mailFolder](mailfolder.md)| The user's mail folders. Read-only. Nullable.|
|manager|[directoryObject](directoryobject.md)|The user or contact that is this user’s manager. Read-only. (HTTP Methods: GET, PUT, DELETE.)|
|memberOf|Coleção [directoryObject](directoryobject.md)|The groups and directory roles that the user is a member of. Read-only. Nullable.|
|messages|Coleção [message](message.md)|The messages in a mailbox or folder. Read-only. Nullable.|
|onenote|[onenote](onenote.md)| Somente leitura.|
|outlook|[outlookUser](outlookuser.md)| Somente leitura.|
|ownedDevices|Coleção [directoryObject](directoryobject.md)|Devices that are owned by the user. Read-only. Nullable.|
|ownedObjects|[directoryObject](directoryobject.md) collection|Directory objects that are owned by the user. Read-only. Nullable.|
|people|Coleção [person](person.md)| Pessoas que são relevantes para o usuário. Somente leitura. Anulável.
|photo|[profilePhoto](profilephoto.md)| The user's profile photo. Read-only.|
|planner|[plannerUser](planneruser.md)| Ponto de entrada para o recurso Planejador que pode existir para um usuário. Somente leitura.|
|registeredDevices|Coleção [directoryObject](directoryobject.md)|Devices that are registered for the user. Read-only. Nullable.|

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
  "createdDateTime": "String (timestamp)",
  "creationType": "string",
  "department": "string",
  "displayName": "string",
  "employeeId": "string",
  "faxNumber" : "string",
  "givenName": "string",
  "hireDate": "String (timestamp)",
  "id": "string (identifier)",
  "identities": [{"@odata.type": "microsoft.graph.objectIdentity"}],
  "imAddresses": ["string"],
  "interests": ["string"],
  "isResourceAccount": false,
  "jobTitle": "string",
  "legalAgeGroupClassification": "string",
  "licenseAssignmentStates": [{"@odata.type": "microsoft.graph.licenseAssignmentState"}],
  "lastPasswordChangeDateTime": "String (timestamp)",
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
  "responsibilities": ["string"],
  "schools": ["string"],
  "showInAddressList": true,
  "signInSessionsValidFromDateTime": "String (timestamp)",
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

- [Adicionar dados personalizados a recursos usando extensões](/graph/extensibility-overview)
- [Adicionar dados personalizados aos usuários usando extensões abertas](/graph/extensibility-open-users)
- [Adicionar dados personalizados a grupos usando as extensões do esquema](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user resource",
  "keywords": "",
  "suppressions" : [
     "Warning: /api-reference/v1.0/resources/user.md/microsoft.graph.user:
      Property 'createdDateTime' found in markdown table but not in resource definition."
  ],
  "section": "documentation",
  "tocPath": ""
}-->
