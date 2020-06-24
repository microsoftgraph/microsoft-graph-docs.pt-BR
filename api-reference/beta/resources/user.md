---
title: Tipo de recurso de usuário
description: Represents an Azure AD user account. Inherits from directoryObject.
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 3905e7165503c235b4b015ba09bec8af4c4ee6aa
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44864081"
---
# <a name="user-resource-type"></a>Tipo de recurso de usuário

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents an Azure AD user account. Inherits from [directoryObject](directoryobject.md).

O recurso **usuário** permite que os aplicativos especifiquem preferências de usuário para idiomas e formatos de data/hora para as caixas de correio principais do Exchange do usuário e para o perfil do Azure AD do usuário. Para obter mais detalhes, consulte [preferências do usuário para idiomas e formatos regionais](#user-preferences-for-languages-and-regional-formats).

Por motivos de desempenho, as operações [create](../api/user-post-users.md), [get](../api/user-get.md) e [list](../api/user-list.md) retornam por padrão apenas um subconjunto das propriedades usadas com mais frequência. Essas propriedades padrão estão listadas na seção [Propriedades](#properties). Para obter as propriedades não retornadas por padrão, especifique-as em uma opção de consulta `$select` do OData.

Esse recurso permite:

- Adicionar seus próprios dados às propriedades personalizadas como [extensions](/graph/extensibility-overview).
- Assinar as [notificações de alteração](/graph/webhooks).
- Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/user-delta.md).

## <a name="methods"></a>Métodos

| Método                                                                                     | Tipo de retorno                                                                      | Descrição                                                                                                                                                                       |
|:-------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [Listar usuários](../api/user-list.md)                                                          | Coleção [user](user.md)                                                       | Recuperar uma lista de objetos user.                                                                                                                                                       |
| [Criar usuário](../api/user-post-users.md)                                                   | [user](user.md)                                                                  | Criar um novo objeto user.                                                                                                                                                         |
| [Obter usuário](../api/user-get.md)                                                             | [user](user.md)                                                                  | Ler propriedades e relações do objeto user.                                                                                                                                 |
| [Atualizar usuário](../api/user-update.md)                                                       | [user](user.md)                                                                  | Atualizar o objeto user.                                                                                                                                                               |
| [Excluir usuário](../api/user-delete.md)                                                       | Nenhum                                                                             | Excluir o objeto user.                                                                                                                                                               |
| [Obter delta](../api/user-delta.md)                                                          | coleção de usuários                                                                  | Obter as alterações incrementais para usuários.                                                                                                                                                |
| **Atribuições de função de aplicativo**                                                                   |                                                                                  |                                                                                                                                                                                   |
| [List appRoleAssignments](../api/user-list-approleassignments.md)                          | [appRoleAssignment](approleassignment.md) collection                             | Obtenha os aplicativos e as funções de aplicativo que esse usuário foi atribuído.                                                                                                                     |
| [Adicionar appRoleAssignment](../api/user-post-approleassignments.md)                            | [appRoleAssignment](approleassignment.md)                                        | Atribuir uma função de aplicativo a este usuário.                                                                                                                                                  |
| [Remover appRoleAssignment](../api/user-delete-approleassignments.md)                       | Nenhum                                                                             | Remova uma atribuição de função de aplicativo deste usuário.                                                                                                                                     |
| **Calendário**                                                                               |                                                                                  |                                                                                                                                                                                   |
| [Criar calendário](../api/user-post-calendars.md)                                           | [Calendar](calendar.md)                                                          | Criar um novo Calendar postando na coleção calendars.                                                                                                                     |
| [Criar calendarGroup](../api/user-post-calendargroups.md)                                 | [CalendarGroup](calendargroup.md)                                                | Criar um novo CalendarGroup postando na coleção calendarGroups.                                                                                                           |
| [Criar evento](../api/user-post-events.md)                                                 | [event](event.md)                                                                | Criar um novo Event postando na coleção de eventos.                                                                                                                           |
| [findMeetingTimes](../api/user-findmeetingtimes.md)                                        | [meetingTimeSuggestionsResult](meetingtimesuggestionsresult.md)                  | Encontrar o tempo e locais para reunião com base na disponibilidade dos participantes, localização ou restrições de tempo.                                                                                    |
| [findRooms](../api/user-findrooms.md)                                                      | Coleção [emailaddress.md](emailaddress.md)                                    | Obter todas as salas de reunião no locatário do usuário ou em uma lista de salas específica.                                                                                                        |
| [findRoomLists](../api/user-findroomlists.md)                                              | Coleção [emailaddress.md](emailaddress.md)                                    | Obter as listas de salas definidas em um locatário.                                                                                                                                           |
| [getSchedule](../api/calendar-getschedule.md)                                              | [scheduleInformation](scheduleinformation.md)                                    | Adquira as informações de disponibilidade para um conjunto de usuários, listas de distribuição ou recursos (salas e equipamentos) para um período de tempo especificado.                         |
| [Listar calendários](../api/user-list-calendars.md)                                            | Coleção [Calendar](calendar.md)                                               | Obter uma coleção de objetos Calendar.                                                                                                                                                 |
| [Listar calendarGroups](../api/user-list-calendargroups.md)                                  | Coleção [CalendarGroup](calendargroup.md)                                     | Obter uma coleção de objetos CalendarGroup.                                                                                                                                            |
| [Listar calendarView](../api/user-list-calendarview.md)                                      | Coleção [event](event.md)                                                     | Obter uma coleção de objetos de evento.                                                                                                                                                   |
| [Listar eventos](../api/user-list-events.md)                                                  | Coleção [event](event.md)                                                     | Get a list of event objects in the user's mailbox. The list contains single instance meetings and series masters.                                                                 |
| [reminderView](../api/user-reminderview.md)                                                | Coleção [Reminder](reminder.md)                                               | Retorna uma lista de lembretes de calendário nas horas de início e término especificadas.                                                                                                     |
| **Contatos**                                                                               |                                                                                  |                                                                                                                                                                                   |
| [Criar contato](../api/user-post-contacts.md)                                             | [contato](contact.md)                                                            | Crie um novo contato postando na coleção de contatos.                                                                                                                       |
| [Criar contactFolder](../api/user-post-contactfolders.md)                                 | [contactFolder](contactfolder.md)                                                | Crie um novo contactFolder postando na coleção contactFolders.                                                                                                           |
| [Listar contatos](../api/user-list-contacts.md)                                              | Coleção [Contact](contact.md)                                                 | Obter uma coleção de contatos da pasta padrão de contatos do usuário conectado.                                                                                                  |
| [Listar contactFolders](../api/user-list-contactfolders.md)                                  | Coleção [ContactFolder](contactfolder.md)                                     | Obtenha a coleção de pastas de contatos na pasta de contatos padrão do usuário conectado.                                                                                           |
| **Objetos de diretório**                                                                      |                                                                                  |                                                                                                                                                                                   |
| [assignLicense](../api/user-assignlicense.md)                                              | [user](user.md)                                                                  | Add or remove subscriptions for the user. You can also enable and disable specific plans associated with a subscription.                                                          |
| [checkMemberGroups](../api/user-checkmembergroups.md)                                      | String collection                                                                | Check for membership in a list of groups. The check is transitive.                                                                                                                |
| [checkMemberObjects](../api/user-checkmemberobjects.md)                                    | Coleção de cadeias de caracteres                                                                | Verifique a associação em uma lista de grupo, função de diretório ou objetos de unidade administrativa. A verificação é transitiva.                                                                 |
| [exportPersonalData](../api/user-exportpersonaldata.md)                                    | Nenhum                                                                             | Envia uma solicitação de operação de política de dados, realizada por um administrador da empresa para exportar os dados de um usuário da organização.                                                                 |
| [getByIds](../api/directoryobject-getbyids.md)                                             | Coleção de cadeias de caracteres                                                                | Retorna os objetos de diretório especificados a partir de uma lista de ids.                                                                                                                         |
| [getMemberGroups](../api/user-getmembergroups.md)                                          | Coleção de cadeias de caracteres                                                                | Return all the groups that the user is a member of. The check is transitive.                                                                                                      |
| [getMemberObjects](../api/user-getmemberobjects.md)                                        | Coleção String                                                                | Retornar todos os grupos, funções de diretório e unidades administrativas dos quais o usuário é membro. A verificação é transitiva.                                                           |
| [Listar createdObjects](../api/user-list-createdobjects.md)                                  | Coleção [directoryObject](directoryobject.md)                                 | Obter os objetos directory criados pelo usuário da propriedade de navegação createdObjects.                                                                                        |
| [Listar licenseDetails](../api/user-list-licensedetails.md)                                  | Coleção [licenseDetails](licensedetails.md)                                   | Obtenha uma coleção de objetos licenseDetails.                                                                                                                                           |
| [Listar ownedDevices](../api/user-list-owneddevices.md)                                      | Coleção [directoryObject](directoryobject.md)                                 | Obter os dispositivos que pertencem ao usuário da propriedade de navegação ownedDevices.                                                                                             |
| [Listar ownedObjects](../api/user-list-ownedobjects.md)                                      | [directoryObject](directoryobject.md) collection                                 | Obter os objetos directory que pertencem ao usuário da propriedade de navegação ownedObjects.                                                                                   |
| [Listar registeredDevices](../api/user-list-registereddevices.md)                            | Coleção [directoryObject](directoryobject.md)                                 | Obter os dispositivos que estão registrados para o usuário da propriedade de navegação registeredDevices.                                                                                  |
| [Listar associações de função com escopo](../api/user-list-scopedrolememberof.md)                     | Coleção [scopedRoleMembership](scopedrolemembership.md)                       | Obter as associações de unidades administrativas de função com escopo deste usuário.                                                                                                               |
| [reprocessLicense](../api/user-reprocesslicenseassignment.md)                              | [user](user.md)                                                                  | Reprocessar as atribuições de assinatura do usuário.                                                                                                                                  |
| [revokeSignInSessions](../api/user-revokesigninsessions.md)                                | Nenhum                                                                             | Revoga todos os tokens de sessão e de atualização do usuário emitidos para aplicativos, redefinindo a propriedade do usuário **signInSessionsValidFromDateTime** para data e a hora atuais. Força o usuário a entrar novamente nesses aplicativos. Este método substitui **invalidateAllRefreshTokens**. |
| **Unidade**                                                                                  |                                                                                  |                                                                                                                                                                                   |
| [Obter unidade](../api/drive-get.md)                                                           | [unidade](drive.md)                                                                | Recuperar as propriedades e as relações de um recurso Drive.                                                                                                                    |
| [Filhos de lista](../api/driveitem-list-children.md)                                         | [DriveItems](driveitem.md)                                                       | Retornar uma coleção de DriveItems no relacionamento filho de um DriveItem.                                                                                                    |
| **Grupos**                                                                                 |                                                                                  |                                                                                                                                                                                   |
| [Listar joinedTeams](../api/user-list-joinedteams.md)                                        | Coleção [team](team.md)                                                       | Obter as equipes do Microsoft Teams no qual o usuário é membro direto da propriedade de navegação joinedTeams.                                                                       |
| [Listar memberOf](../api/user-list-memberof.md)                                              | Coleção [directoryObject](directoryobject.md)                                 | Obter os grupos, funções de diretório e as unidades administrativas dos quais esse usuário é membro direto, da propriedade de navegação memberOf.                                              |
| [Listar memberOf transitivos](../api/user-list-transitivememberof.md)                         | Coleção [directoryObject](directoryobject.md)                                 | Lista os grupos e funções de diretório e unidades administrativas dos quais o usuário é membro. Essa operação é transitiva e inclui os grupos dos quais o usuário é membro aninhado. |
| **Percepções**                                                                               |                                                                                  |                                                                                                                                                                                   |
| [Listar compartilhado](../api/insights-list-shared.md)                                              | coleção [sharedInsight](insights-shared.md)                                   | Visão calculada que retorna a lista de arquivos compartilhados com um usuário.                                                                                                             |
| [Listar tendências](../api/insights-list-trending.md)                                          | coleção [tendências](insights-trending.md)                                       | Insights calculados que retornam a lista de itens de tendências do usuário.                                                                                                       |
| [Listar usados](../api/insights-list-used.md)                                                  | coleção [usedInsight](insights-used.md)                                       | Visão calculada que retorna a lista de arquivos usados com um usuário.                                                                                                               |
| **Email**                                                                                   |                                                                                  |                                                                                                                                                                                   |
| [Create inferenceClassificationOverride](../api/inferenceclassification-post-overrides.md) | Criar uma substituição da Caixa de Entrada Destaques para um remetente identificado por um endereço SMTP.      |                                                                                                                                                                                   |
| [Criar MailFolder](../api/user-post-mailfolders.md)                                       | [mailFolder](mailfolder.md)                                                      | Crie um novo mailFolder postando na coleção mailFolders.                                                                                                                 |
| [Criar mensagem](../api/user-post-messages.md)                                             | [message](message.md)                                                            | Crie uma mensagem postando na coleção de mensagens.                                                                                                                           |
| [Criar messageRule](../api/mailfolder-post-messagerules.md)                               | [messageRule](messagerule.md)                                                    | Crie um objeto messageRule especificando um conjunto de condições e ações.                                                                                                        |
| [getMailTips](../api/user-getmailtips.md)                                                  | Coleção [mailTips](mailtips.md)                                               | Retornar dicas de email de um ou mais destinatários conforme disponíveis para o usuário conectado.                                                                                                 |
| [Listar mailFolders](../api/user-list-mailfolders.md)                                        | Coleção [mailFolder](mailfolder.md)                                           | Obter o conjunto de pastas de email sob a pasta raiz do usuário conectado.                                                                                                       |
| [Listar mensagens](../api/user-list-messages.md)                                              | Coleção [message](message.md)                                                 | Obter todas as mensagens na caixa de correio do usuário conectado.                                                                                                                             |
| [List overrides](../api/inferenceclassification-list-overrides.md)                         | Coleção [inferenceClassificationOverride](inferenceclassificationoverride.md) | Obtenha as substituições da Caixa de Entrada Destaques que um usuário configurou para sempre classificar as mensagens de determinados remetentes de maneiras específicas.                                                         |
| [Listar regras](../api/mailfolder-list-messagerules.md)                                       | Coleção [messageRule](messagerule.md)                                         | Obtenha todos os objetos messageRule definidos para a caixa de entrada do usuário.                                                                                                                     |
| [Enviar email](../api/user-sendmail.md)                                                       | Nenhum                                                                             | Enviar a mensagem especificada no corpo da solicitação.                                                                                                                                   |
| **Anotações**                                                                                  |                                                                                  |                                                                                                                                                                                   |
| [Criar bloco de anotações](../api/onenote-post-notebooks.md)                                        | [bloco de anotações](notebook.md)                                                          | Crie um novo bloco de anotações do OneNote.                                                                                                                                                    |
| [Listar blocos de anotações](../api/onenote-list-notebooks.md)                                         | Coleção [bloco de anotações](notebook.md)                                               | Recuperar uma lista de objetos do bloco de anotações.                                                                                                                                              |
| **Extensões abertas**                                                                        |                                                                                  |                                                                                                                                                                                   |
| [Criar extensão aberta](../api/opentypeextension-post-opentypeextension.md)                | [openTypeExtension](opentypeextension.md)                                        | Crie uma extensão aberta e adicione propriedades personalizadas a uma instância nova ou existente de um recurso.                                                                                                 |
| [Obter extensão aberta](../api/opentypeextension-get.md)                                      | Coleção [openTypeExtension](opentypeextension.md)                             | Obtenha uma extensão aberta identificada pelo nome da extensão.                                                                                                                           |
| **Hierarquia da organização**                                                                          |                                                                                  |                                                                                                                                                                                   |
| [Atribuir gerenciador](../api/user-post-manager.md)                                              | Nenhum                                                                             | Atribuir um gerenciador de usuário.                                                                                                                                                          |
| [Obter gerenciador](../api/user-list-manager.md)                                                 | [directoryObject](directoryobject.md)                                            | Obter o usuário ou contato que é o gerente do usuário da propriedade de navegação manager.                                                                                         |
| [Listar directReports](../api/user-list-directreports.md)                                    | Coleção [directoryObject](directoryobject.md)                                 | Obter os usuários ou contatos subordinados ao usuário da propriedade de navegação directReports.                                                                                    |
| **Configurações do Outlook**                                                                       |                                                                                  |                                                                                                                                                                                   |
| [Criar categoria do Outlook](../api/outlookuser-post-mastercategories.md)                     | [outlookCategory](outlookcategory.md)                                            | Cria um objeto outlookCategory na lista mestra de categorias do usuário.                                                                                                         |
| [Obter supportedLanguages](../api/outlookuser-supportedlanguages.md),                         | Coleção [localeInfo](localeinfo.md)                                           | Obtém a lista de locais e idiomas com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.                                                                |
| [Obter supportedTimeZones](../api/outlookuser-supportedtimezones.md)                         | [timeZoneInformation](timezoneinformation.md collection)                         | Obtém a lista de fusos horários com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário.                                                                           |
| [Obtém configurações de caixa de correio do usuário](../api/user-get-mailboxsettings.md)                            | [mailboxSettings](mailboxsettings.md)                                            | Obtém as configurações de caixa de correio do usuário.                                                                                                                                                   |
| [Listar as categorias do Outlook](../api/outlookuser-list-mastercategories.md)                     | Coleção [outlookCategory](outlookcategory.md)                                 | Obtém todas as categorias que foram definidas para o usuário.                                                                                                                       |
| [Converter IDs do Exchange](../api/user-translateexchangeids.md)                              | coleção [convertIdResult](convertidresult.md)                                 | Traduzir os identificadores de recursos relacionados ao Outlook entre formatos.                                                                                                               |
| [Atualizar configurações da caixa de correio do usuário](../api/user-update-mailboxsettings.md)                      | [mailboxSettings](mailboxsettings.md)                                            | Habilitar, configurar ou desabilitar o mailboxSettings de um ou mais usuários.                                                                                                                 |
| **Tarefas do Outlook**                                                                          |                                                                                  |                                                                                                                                                                                   |
| [Criar outlookTask](../api/outlookuser-post-tasks.md)                                     | [outlookTask](outlooktask.md)                                                    | Criar uma tarefa do Outlook no grupo de tarefas padrão (Minhas Tarefas) e pasta de tarefas padrão (Tarefas) na caixa de correio do usuário.                                                                |
| [Listar tarefas](../api/outlookuser-list-tasks.md)                                             | coleção [outlookTask](outlooktask.md)                                         | Obtenha todas as tarefas do Outlook na caixa de correio do usuário.                                                                                                                                  |
| **Pessoas**                                                                                 |                                                                                  |                                                                                                                                                                                   |
| [Listar pessoas](../api/user-list-people.md)                                                  | [person](person.md)                                                              | Recupere uma lista de objetos person ordenados por relevância para o usuário, o que é determinado pelos padrões de comunicação e colaboração e pelas relações comerciais do usuário. |
| **Foto**                                                                                  |                                                                                  |                                                                                                                                                                                   |
| [Obter foto](../api/profilephoto-get.md)                                                    | [profilePhoto](profilephoto.md)                                                  | Obtém o profilePhoto especificado ou seus metadados (propriedades profilePhoto).                                                                                                         |
| [Atualizar profilephoto](../api/profilephoto-update.md)                                       | Nenhum                                                                             | Atualiza a foto de qualquer usuário no locatário, incluindo o usuário conectado ou o grupo ou contato especificado.                                                                      |
| **Planner**                                                                                |                                                                                  |                                                                                                                                                                                   |
| [Obter plannerUser](../api/planneruser-get.md)                                               | [plannerUser](planneruser.md)                                                    | Recupere as propriedades e relações de um objeto plannerUser.                                                                                                                |
| [Listar favoritePlans](../api/planneruser-list-favoriteplans.md)                             | Coleção [plannerPlan](plannerplan.md)                                         | Recupere uma lista de plannerPlans marcados como favoritos por um usuário.                                                                                                            |
| [Listar recentPlans](../api/planneruser-list-recentplans.md)                                 | coleção [plannerPlan](plannerplan.md)                                         | Recupere uma lista de plannerPlans recentemente exibida por um usuário.                                                                                                                        |
| [Listar tarefas](../api/planneruser-list-tasks.md)                                             | Coleção [plannerTask](plannertask.md)                                         | Obter o plannerTasks atribuído ao usuário.                                                                                                                                            |
| [Atualizar plannerUser](../api/planneruser-update.md)                                         | Nenhum                                                                             | Atualize as propriedades de um objeto plannerUser.                                                                                                                                    |
| **Perfil**                                                                                |                                                                                  |                                                                                                                                                                                   |
| [Obter perfil](../api/profile-get.md)                                                       | [perfil](profile.md)                                                            | Recupere as propriedades e relações de um objeto de perfil para um determinado usuário.                                                                                                   |
| [Excluir perfil](../api/profile-delete.md)                                                 | Nenhum                                                                             | Exclua o objeto de perfil de uma conta de usuário.                                                                                                                                      |
| **Extensões de esquema**                                                                      |                                                                                  |                                                                                                                                                                                   |
| [Adicionar valores de extensões de esquema](/graph/extensibility-schema-groups)                          | Nenhum                                                                             | Cria uma definição para a extensão de esquema e a usa para adicionar dados digitados personalizados a um recurso.                                                                                      |
| **Teamwork**                                                                               |                                                                                  |                                                                                                                                                                                   |
| [Instalar o aplicativo para o usuário](../api/user-add-teamsappinstallation.md)                            | Nenhum                                                                             | Instale um aplicativo no escopo pessoal do usuário especificado.                                                                                                                       |
| [Listar aplicativos instalados para o usuário](../api/user-list-teamsappinstallation.md)                   | [teamsAppInstallation](teamsappinstallation.md)                                  | Recupere a lista de aplicativos instalados no escopo pessoal do usuário especificado.                                                                                                  |
| [Atualizar aplicativo](../api/user-upgrade-teamsappinstallation.md)                                 | Nenhum                                                                             | Atualize uma instalação de aplicativo no escopo pessoal do usuário especificado para a versão mais recente do aplicativo.                                                                         |
| [Desinstalar aplicativo para o usuário](../api/user-delete-teamsappinstallation.md)                       | Nenhum                                                                             | Desinstale um aplicativo do escopo pessoal do usuário especificado.                                                                                                                   |
| **Configurações do usuário**                                                                          |                                                                                  |                                                                                                                                                                                   |
| [Obter configurações](../api/usersettings-get.md)                                                 | [userSettings](usersettings.md)                                                  | Leia o usuário e o objeto de configurações da organização.                                                                                                                                   |
| [Atualizar configurações](../api/usersettings-update.md)                                           | [userSettings](usersettings.md)                                                  | Atualize as propriedades do objeto de configurações.                                                                                                                                     |

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo    | Descrição |
|:---------------|:--------|:------------|
| aboutMe | String | Um campo de entrada de texto em forma livre para o usuário se descrever. <br><br>Retornado apenas em $select. |
| accountEnabled | Booliano | `true` se a conta estiver habilitada; caso contrário, `false`. Essa propriedade é obrigatória quando um usuário é criado. <br><br>Retornado apenas em $select. Oferece suporte a $filter. |
| ageGroup | String | Define a faixa etária do usuário. Valores permitidos: `null`, `minor`, `notAdult` e `adult`. Confira as [definições de propriedades da faixa etária legal](#legal-age-group-property-definitions) para obter mais informações. <br><br>Retornado apenas em $select. |
| assignedLicenses | Coleção [assignedLicense](assignedlicense.md) | As licenças que são atribuídas ao usuário. <br><br>Retornado apenas em $select. Não anulável. |
| assignedPlans | Coleção [assignedPlan](assignedplan.md) | Os planos que são atribuídos ao usuário. <br><br>Retornado apenas em $select. Somente leitura. Não anulável. |
| birthday | DateTimeOffset | The birthday of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'` <br><br>Retornado apenas em $select. |
| businessPhones | Coleção de cadeias de caracteres | Números de telefone para o usuário. Somente um número pode ser definido para essa propriedade. <br><br>Retornado por padrão. |
| city | String | A cidade em que o usuário está localizado. <br><br>Retornado apenas em $select. Oferece suporte a $filter. |
| companyName | String | O nome da empresa em que o usuário está associado. Essa propriedade pode ser útil para descrever a empresa de onde procede um usuário externo. <br><br>Retornado apenas em $select. |
| consentProvidedForMinor | String| Define se o consentimento foi obtido para menores. Valores permitidos: `null`, `granted`, `denied` e `notRequired`. Confira as [definições de propriedades da faixa etária legal](#legal-age-group-property-definitions) para obter mais informações. <br><br>Retornado apenas em $select. |
| country | Cadeia de caracteres | País/região em que o usuário está localizado. Por exemplo, "EUA" ou "Reino Unido". <br><br>Retornado apenas em $select. Oferece suporte a $filter. |
| createdDateTime | DateTimeOffset | A data e hora que o usuário foi criado. Não é possível modificar o valor e ele é preenchido automaticamente quando a entidade é criada. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. A propriedade é anulável. Um valor nulo indica que uma hora de criação exata não pode ser determinada pelo usuário. <br><br>Retornado apenas em $select. Somente leitura. Oferece suporte a $filter. |
| creationType | String | Indica se a conta de usuário foi criada como uma conta corporativa ou de estudante (`null`), uma conta externa (`Invitation`), uma conta local para um locatário do Azure Active Directory B2C (`LocalAccount`) ou uma inscrição de autoatendimento usando a verificação de email (`EmailVerified`). <br><br>Retornado apenas em $select. Somente leitura. |
| deletedDateTime | DateTimeOffset | A data e hora que o usuário foi excluído. <br><br>Retornado apenas em $select. |
| department | String | O nome do departamento no qual o usuário trabalha. <br><br>Retornado apenas em $select. Oferece suporte a $filter. |
| displayName | String | O nome exibido para o usuário no catálogo de endereços. Geralmente o valor é a combinação do nome, da inicial do nome do meio e do sobrenome do usuário. Essa propriedade é obrigatória quando um usuário é criado e não pode ser apagado durante atualizações. <br><br>Retornado por padrão. Oferece suporte a $filter e $orderby.|
| employeeId | String | O identificador de funcionário atribuído ao usuário pela organização. <br><br>Retornado apenas em $select. Oferece suporte a $filter.|
| externalUserState | String | Para um usuário externo convidado para o locatário usando a [API de convite](../api/invitation-post.md), essa propriedade representa o status do convite do usuário convidado. Para usuários convidados, o estado pode ser `PendingAcceptance` ou `Accepted` ou `null` para todos os outros usuários. <br><br>Retornado apenas em $select. Suporta o $filter com os valores compatíveis. Por exemplo: `$filter=externalUserState eq 'PendingAcceptance'`. |
| externalUserStateChangeDateTime | String | Mostra o carimbo de hora da alteração mais recente da propriedade externalUserState. <br><br>Retornado apenas em $select. |
| FaxNumber | String | O número de fax do usuário. <br><br>Retornado apenas em $select. |
| givenName | String | O nome fornecido (nome) do usuário. <br><br>Retornado por padrão. Oferece suporte a $filter.|
| hireDate | DateTimeOffset | The hire date of the user. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'` <br><br>Retornado apenas em $select. |
| id | Cadeia de caracteres | O identificador exclusivo do usuário. Herdado de [directoryObject](directoryobject.md). <br><br>Retornado por padrão. Não anulável. Somente leitura.|
| Identidades | Coleção [objectIdentity](objectIdentity.md) | Representa as identidades que podem ser usadas para entrar nesta conta de usuário. Uma identidade pode ser fornecida pela Microsoft (também conhecida como conta local), por organizações ou por provedores de identidade social, como o Facebook, Google e Microsoft, e está vinculada a uma conta de usuário. Pode conter vários itens com o mesmo valor **signInType**. <br><br>Retornado apenas em $select. Oferece suporte a $filter. |
| imAddresses | String collection | The instant message voice over IP (VOIP) session initiation protocol (SIP) addresses for the user. Read-only.|
| interests | Coleção de cadeias de caracteres | Uma lista para o usuário descrever os interesses dele. <br><br>Retornado apenas em $select. |
| isResourceAccount | Booliano | Não use – reservado para uso futuro. |
| jobTitle | String | O cargo do usuário. <br><br>Retornado por padrão. Oferece suporte a $filter.|
| lastPasswordChangeDateTime | DateTimeOffset | A hora em que o usuário do Azure AD alterou a senha dele pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'` <br><br>Retornado apenas em $select. |
| legalAgeGroupClassification | String | Usado por aplicativos empresariais para determinar a faixa etária legal do usuário. Essa propriedade é somente leitura e calculada com base nas propriedades **ageGroup ** e **consentProvidedForMinor **. Valores permitidos: `null`, `minorWithOutParentalConsent`, `minorWithParentalConsent`, `minorNoParentalConsentRequired`, `notAdult` e `adult`. Confira as [definições de propriedades da faixa etária legal](#legal-age-group-property-definitions) para obter mais informações. <br><br>Retornado apenas em $select. |
| licenseAssignmentStates | Coleção [licenseAssignmentState](licenseassignmentstate.md) | Estado das atribuições de licenças para esse usuário. <br><br>Retornado apenas em $select. Somente leitura. |
| email | String | O endereço SMTP do usuário, por exemplo, "jeff@contoso.onmicrosoft.com". <br><br>Retornado por padrão. Somente Leitura. Oferece suporte a $filter. |
| mailboxSettings | [mailboxSettings](mailboxsettings.md) | Configurações para a caixa de correio principal do usuário conectado. Você pode [obter](../api/user-get-mailboxsettings.md) ou [atualizar](../api/user-update-mailboxsettings.md) as configurações de localidade, fuso horário ou de envio de respostas automáticas a mensagens de entrada. <br><br>Retornado apenas em $select. |
| mailNickname | String | O alias de email do usuário. Essa propriedade deve ser especificada quando um usuário é criado. <br><br>Retornado apenas em $select. Oferece suporte a $filter. |
| mobilePhone | Cadeia de caracteres | O número de celular principal do usuário. <br><br>Retornado por padrão. |
| mySite | String | A URL do site pessoal do usuário. <br><br>Retornado apenas em $select. |
| officeLocation | String | A localização do escritório no local de trabalho do usuário. <br><br>Retornado por padrão. |
| onPremisesDistinguishedName | String | Contém o `distinguished name` do Active Directory no local ou `DN`. A propriedade somente é preenchida para os clientes que estejam sincronizando o seu diretório local com o Azure Active Directory pelo Azure AD Connect. <br><br>Retornado apenas em $select. Somente leitura. |
| onPremisesDomainName | String | Contém o `domainFQDN` local, também chamado dnsDomainName sincronizado do diretório local. A propriedade somente é preenchida para os clientes que estejam sincronizando o seu diretório local com o Azure Active Directory pelo Azure AD Connect. <br><br>Retornado apenas em $select. Somente leitura. |
| onPremisesExtensionAttributes | [onPremisesExtensionAttributes](onpremisesextensionattributes.md) | Contém extensionAttributes 1-15 para o usuário. Observe que os atributos de extensão individuais não são selecionáveis nem filtráveis. Para um `onPremisesSyncEnabled` usuário, a fonte de autoridade para esse conjunto de propriedades é o local e é somente leitura e é somente leitura. Para um usuário somente na nuvem (onde `onPremisesSyncEnabled` é falso), essas propriedades podem ser definidas durante a criação ou atualização. Esses atributos de extensão também são conhecidos como atributos personalizados do Exchange 1-15. <br><br>Retornado apenas em $select. |
| onPremisesImmutableId | String | Essa propriedade é usada para associar uma conta de usuário do Active Directory local com seu objeto de usuário do Azure AD. Essa propriedade é usada para associar uma conta de usuário do Active Directory local com seu objeto de usuário do Azure AD. Essa propriedade deverá ser especificada ao criar uma nova conta de usuário no Graph se você estiver usando um domínio federado para a propriedade `userPrincipalName` (UPN) do usuário. Importante: Os caracteres  e _ não podem ser usados ao especificar essa propriedade. Oferece suporte a $filter. **Importante:** Os caracteres **$** e **\_** não podem ser usados ao especificar esta propriedade. <br><br>Retornado apenas em $select. Oferece suporte a $filter. |
| onPremisesLastSyncDateTime | DateTimeOffset | Indica a última vez em que o objeto foi sincronizado com o diretório local; por exemplo: "2013-02-16T03:04:54Z". O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. <br><br>Retornado apenas em $select. Somente leitura. |
| onPremisesProvisioningErrors | coleção [OnPremisesProvisioningError](onpremisesprovisioningerror.md) | Erros ao usar o produto de sincronização da Microsoft durante a configuração. <br><br>Retornado apenas em $select. |
| onPremisesSamAccountName | Cadeia de Caracteres | Contém o `sAMAccountName` local sincronizado no diretório local. A propriedade somente é preenchida para os clientes que estejam sincronizando o seu diretório local com o Azure Active Directory pelo Azure AD Connect. <br><br>Retornado apenas em $select. Somente leitura. |
| onPremisesSecurityIdentifier | String | Contém o identificador de segurança (SID) local do usuário que foi sincronizado do local com a nuvem. <br><br>Retornado apenas em $select. Somente leitura. |
| onPremisesSyncEnabled | Booliano | `true` se esse objeto está sincronizado de um diretório local; `false` se esse objeto foi originalmente sincronizado de um diretório local, mas não está mais sincronizado; `null` se esse objeto nunca foi sido sincronizado de um diretório local (padrão).  <br><br>Retornado apenas em $select. Somente leitura. |
| onPremisesUserPrincipalName | String | Contém o `userPrincipalName` local sincronizado no diretório local. A propriedade somente é preenchida para os clientes que estejam sincronizando o seu diretório local com o Azure Active Directory pelo Azure AD Connect. <br><br>Retornado apenas em $select. Somente leitura. |
| otherMails | Coleção String | Uma lista de endereços de email adicional para o usuário; Por exemplo: `["bob@contoso.com", "Robert@fabrikam.com"]`.<br><br>Retornado apenas em $select.  Oferece suporte a $filter. |
| passwordPolicies | String | Specifies password policies for the user. This value is an enumeration with one possible value being “DisableStrongPassword”, which allows weaker passwords than the default policy to be specified. “DisablePasswordExpiration” can also be specified. The two may be specified together; for example: "DisablePasswordExpiration, DisableStrongPassword".<br><br>Retornado apenas em $select. |
| passwordProfile | [passwordProfile](passwordprofile.md) | Specifies the password profile for the user. The profile contains the user’s password. This property is required when a user is created. The password in the profile must satisfy minimum requirements as specified by the **passwordPolicies** property. By default, a strong password is required. <br><br>Retornado apenas em $select. |
| pastProjects | Coleção de cadeias de caracteres | Uma lista para o usuário enumerar seus projetos anteriores. <br><br>Retornado apenas em $select. |
| postalCode | Cadeia de caracteres | The postal code for the user's postal address. The postal code is specific to the user's country/region. In the United States of America, this attribute contains the ZIP code. <br><br>Retornado apenas em $select. |
| preferredDataLocation | String | O local de dados preferido para o usuário. Para saber mais, confira [OneDrive Online Multi-Geo](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction). <br><br>Retornado apenas em $select. |
| preferredLanguage | String | The preferred language for the user. Should follow ISO 639-1 Code; for example "en-US". <br><br>Retornado por padrão. |
| preferredName | String | O nome preferencial do usuário. <br><br>Retornado apenas em $select. |
| provisionedPlans | coleção [provisionedPlan](provisionedplan.md) | Os planos que estão provisionados para o usuário. <br><br>Retornado apenas em $select. Somente leitura. Não anulável. |
| proxyAddresses | Coleção de cadeias de caracteres | Por exemplo: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` O operador **any** é obrigatório para expressões de filtro em propriedades de vários valores. <br><br>Retornado apenas em $select. Somente leitura, não anulável. Oferece suporte a $filter. |
| refreshTokensValidFromDateTime | DateTimeOffset | Os tokens de atualização ou de sessão (cookies de sessão) emitidos antes dessa hora são inválidos e os aplicativos recebem um erro ao usar um token de atualização ou de sessão inválido para adquirir um token de acesso delegado (para acessar APIs como o Microsoft Graph).  Se isso acontecer, o aplicativo precisará adquirir um novo token de atualização, fazendo uma solicitação ao ponto de extremidade de autorização. <br><br>Retornado apenas em $select. Somente leitura. Use [invalidateAllRefreshTokens](../api/user-invalidateallrefreshtokens.md) para redefinir. |
| responsibilities | Coleção de cadeias de caracteres | Uma lista para o usuário enumerar suas responsabilidades. <br><br>Retornado apenas em $select. |
| schools | Coleção de cadeias de caracteres | Uma lista para o usuário enumerar as escolas que frequentou. <br><br>Retornado apenas em $select. |
| showInAddressList | Booliano | `true` se a lista de endereços global do Outlook deve conter o usuário, caso contrário `false`. Se não estiver configurado, isso será tratado como `true`. Para os usuários convidados por meio do Gerenciador de convites, essa propriedade será definida como `false`. <br><br>Retornado apenas em $select.|
| signInSessionsValidFromDateTime | DateTimeOffset | Os tokens de atualização ou de sessão (cookies de sessão) emitidos antes dessa hora são inválidos e os aplicativos recebem um erro ao usar um token de atualização ou de sessão inválido para adquirir um token de acesso delegado (para acessar APIs como o Microsoft Graph).  Se isso acontecer, o aplicativo precisará adquirir um novo token de atualização, fazendo uma solicitação ao ponto de extremidade de autorização. <br><br>Retornado apenas em $select. Somente leitura. Use [revokeSignInSessions](../api/user-revokesigninsessions.md) para redefinir.|
| skills | Coleção de cadeias de caracteres | Uma lista para o usuário enumerar suas qualificações. <br><br>Retornado apenas em $select. |
| signInActivity | [signInActivity](signinactivity.md) | Obtenha a última data de entrada e solicite a ID de entrada de um usuário específico.<br><br>Suporta $filter, mas não com nenhuma outra propriedade filtrável. <br><br>Retornado apenas em $select. Somente leitura. |
| state | Cadeia de caracteres | O estado ou município no endereço do usuário. <br><br>Retornado apenas em $select. Oferece suporte a $filter. |
| streetAddress | String | O endereço do local de trabalho do usuário. <br><br>Retornado apenas em $select.|
| surname | String | O sobrenome do usuário (nome de família ou sobrenome). <br><br>Retornado por padrão. Oferece suporte a $filter. |
| usageLocation | String | Um código de duas letras (padrão ISO 3166). Obrigatório para os usuários que receberão licenças devido à exigência legal de verificar a disponibilidade de serviços nos países.  Os exemplos incluem: "US", "JP" e "GB". Não anulável. <br><br>Retornado apenas em $select. Oferece suporte a $filter.|
| userPrincipalName | Cadeia de caracteres | O nome UPN do usuário. O nome UPN é um nome de logon para o usuário ao estilo da Internet com base na RFC 822 padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email do usuário. O formato geral é alias@domain, em que o domínio deve estar presente na coleção de domínios verificados do locatário. Essa propriedade é obrigatória quando um usuário é criado. Os domínios verificados para o locatário podem ser acessados pela propriedade **verifiedDomains** de [organization](organization.md). <br><br>Retornado por padrão. Oferece suporte a $filter e $orderby.
| userType | String | Um valor de cadeia de caracteres que pode ser usado para classificar tipos de usuários no seu diretório, como “Membro” e “Convidado”. <br><br>Retornado apenas em $select. Oferece suporte a $filter. |

### <a name="legal-age-group-property-definitions"></a>Definições de propriedade da faixa etária legal

Esta seção explica como as três propriedades de faixa etária (`legalAgeGroupClassification`, `ageGroup` e `consentProvidedForMinor`) são usadas pelos administradores do Azure AD e desenvolvedores de aplicativos empresariais para atender às normas de idade.

Por exemplo: Cameron é o administrador de um diretório em uma escola de ensino fundamental em Holyport, no Reino Unido. No início do ano letivo ele usa a documentação de admissão para obter o consentimento dos pais dos menores baseado nos regulamentos relacionadas com a idade no Reino Unido. O consentimento obtido do pai permite que a conta do menor seja usado pela escola de Holyport e os aplicativos da Microsoft. Cameron cria todas as contas e define o ageGroup para "menor" e consentProvidedForMinor para "concedido". Os aplicativos usados por seus alunos poderão, então suprimir recursos que não são adequados para menores.

#### <a name="legal-age-group-classification"></a>Classificação da faixa etária legal

Essa propriedade de somente leitura é usada por desenvolvedores de aplicativos empresariais para garantir a manipulação correta do usuário com base em sua faixa etária legal. É calculada com base nas propriedades de `ageGroup` e `consentProvidedForMinor` do usuário.

| Valor   | # |Descrição|
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

| Valor    | # |Descrição|
|:---------------|:--------|:----------|
|null|,0|Valor padrão, nenhum `ageGroup` foi definido para o usuário.|
|minor|1 |O usuário é considerado menor de idade.|
|notAdult|2 |O usuário é de um país que têm regulamentações estatutárias (Estados Unidos, Reino Unido, União Europeia ou Coreia do Sul) e a idade do usuário é maior do que o limite de idade para criança (conforme o país) e menor que o limite inferior de idade para adulto (como estipulado com base no país ou região). Basicamente, adolescentes são considerados como `notAdult` em países regulamentados.|
|adult|3 |O usuário deve ser tratado como um adulto.|

#### <a name="consentprovidedforminor-property"></a>Propriedade consentProvidedForMinor

| Valor    | # |Descrição|
|:---------------|:--------|:----------|
|null|,0|Valor padrão, nenhum `consentProvidedForMinor` foi definido para o usuário.|
|granted|1 |O consentimento foi obtido para o usuário ter uma conta.|
|denied|2 |O consentimento não foi obtido para o usuário ter uma conta.|
|notRequired|3 |O usuário é de um local que não exige consentimento.|

## <a name="relationships"></a>Relações

| Relação | Tipo |Descrição|
|:---------------|:--------|:----------|
|agreementAcceptances|Coleção [agreementAcceptance](agreementacceptance.md)| Os termos de usuário do status de aceitação de uso. Somente leitura. Anulável.|
|calendar|[calendar](calendar.md)|The user's primary calendar. Read-only.|
|calendarGroups|Coleção [CalendarGroup](calendargroup.md)|The user's calendar groups. Read-only. Nullable.|
|calendarView|Coleção [event](event.md)|The calendar view for the calendar. Read-only. Nullable.|
|calendars|Coleção [calendar](calendar.md)|The user's calendars. Read-only. Nullable.|
|contactFolders|Coleção [ContactFolder](contactfolder.md)|The user's contacts folders. Read-only. Nullable.|
|contacts|Coleção [Contact](contact.md)|The user's contacts. Read-only. Nullable.|
|createdObjects|[directoryObject](directoryobject.md) collection|Directory objects that were created by the user. Read-only. Nullable.|
|directReports|Coleção [directoryObject](directoryobject.md)|The users and contacts that report to the user. (The users and contacts that have their manager property set to this user.) Read-only. Nullable. |
|drive|[unidade](drive.md)|The user's OneDrive. Read-only.|
|unidades|Coleção [drive](drive.md)| A collection of drives available for this user. Read-only. |
|eventos|Coleção [event](event.md)|Os eventos do usuário. O padrão é mostrar eventos no Calendário Padrão. Somente leitura. Anulável.|
|extensions|Coleção [extension](extension.md)|A coleção de extensões abertas definidas para o usuário. Anulável.|
|inferenceClassification|[inferenceClassification](inferenceclassification.md)| Classificação de relevância das mensagens do usuário com base em designações explícitas que substituem a relevância ou importância deduzida. |
|insights|[officeGraphInsights](officegraphinsights.md) | Read-only. Nullable.|
|joinedGroups|Coleção [group](group.md)| Read-only. Nullable.|
|mailFolders|Coleção [mailFolder](mailfolder.md)| The user's mail folders. Read-only. Nullable.|
|manager|[directoryObject](directoryobject.md)|The user or contact that is this user’s manager. Read-only. (HTTP Methods: GET, PUT, DELETE.)|
|memberOf|Coleção [directoryObject](directoryobject.md)|Os grupos e funções de diretório e unidades administrativas dos quais o usuário é membro. Somente leitura. Anulável.|
|joinedTeams|Coleção [team](team.md)|As equipes do Microsoft Teams do qual o usuário é membro. Somente leitura. Anulável.|
|trabalho em equipe|[userTeamwork](userteamwork.md)| Um contêiner dos recursos do Microsoft Teams disponíveis para o usuário. Somente leitura. Anulável.|
|messages|Coleção [message](message.md)|The messages in a mailbox or folder. Read-only. Nullable.|
|onenote|[onenote](onenote.md)| Somente leitura.|
|outlook|[outlookUser](outlookuser.md)| Os serviços seletivos do Outlook disponíveis para o usuário. Somente leitura. Anulável.|
|ownedDevices|Coleção [directoryObject](directoryobject.md)|Devices that are owned by the user. Read-only. Nullable.|
|ownedObjects|[directoryObject](directoryobject.md) collection|Directory objects that are owned by the user. Read-only. Nullable.|
|people|Coleção [person](person.md)| Somente leitura. As pessoas mais relevantes para o usuário. A coleção é ordenada por relevância para o usuário, que é determinado pela comunicação e colaboração e pelas relações comerciais do usuário. Uma pessoa é uma agregação de informações provenientes de emails, contatos e redes sociais.|
|photo|[profilePhoto](profilephoto.md)| The user's profile photo. Read-only.|
|photos|coleção de [fotos](photo.md)| Read-only. Nullable.|
|planner|[plannerUser](planneruser.md)| Serviços de planejador seletivo disponíveis para o usuário. Somente leitura. Anulável. |
|scopedRoleMemberOf|Coleção [scopedRoleMembership](scopedrolemembership.md)| As associações de unidade administrativa de função com escopo deste usuário. Somente leitura. Anulável.|
|settings|[userSettings](usersettings.md) | Read-only. Nullable.|
|registeredDevices|Coleção [directoryObject](directoryobject.md)|Devices that are registered for the user. Read-only. Nullable.|

### <a name="user-preferences-for-languages-and-regional-formats"></a>Preferências do usuário para idiomas e formatos regionais
O recurso **User** contém uma propriedade [mailboxSettings](../resources/mailboxsettings.md) que inclui o idioma preferencial do usuário, a formatação de data e hora, o fuso horário padrão e outras configurações especificamente para sua caixa de correio principal do Exchange. Essas preferências são direcionadas para clientes de email e só estarão disponíveis se o usuário tiver uma caixa de correio configurada. Você pode optar por usar o **mailboxSettings** se seu cenário se concentrar apenas em emails, calendário, contatos ou tarefas pendentes do Outlook.

Além do **mailboxSettings**, o **usuário** inclui uma relação por [UserSettings](../resources/usersettings.md) para [regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md), o superconjunto de preferências de formatação regional e de idioma que pode ser usado por qualquer aplicativo para fornecer ao usuário a melhor experiência de formatação regional e de idioma. Use **UserSettings** para uma experiência consistente entre aplicativos que tocam o perfil de usuário do Azure ad para refletir as mesmas preferências do usuário.

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
  "creationType": "string",
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
  "otherMails": ["string"],
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
  "registeredDevices": [{"@odata.type": "microsoft.graph.directoryObject"}],
  "signInActivity": {"@odata.type": "microsoft.graph.signInActivity"}
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
