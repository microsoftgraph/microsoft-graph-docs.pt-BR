---
title: Tipo de recurso de usuário
description: Representa uma conta de usuário do Azure AD. Herda de directoryObject.
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 8a3ccac297741ad85d1f74119047becb2da46274
ms.sourcegitcommit: 9bc1652890fe49d7ad5e5b7177c8a682b1759b75
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/30/2021
ms.locfileid: "52100076"
---
# <a name="user-resource-type"></a>Tipo de recurso de usuário

Namespace: microsoft.graph

Representa uma conta de usuário do Azure AD. Herda de [directoryObject](directoryobject.md).

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
| **Atribuição de funções do aplicativo**                                                                   |                                                                                  |                                                                                                                                                                                                                                     |
| [List appRoleAssignments](../api/user-list-approleassignments.md)                          | [appRoleAssignment](approleassignment.md) collection                             | Obter os aplicativos e funções do aplicativo atribuídos a esse usuário.                                                                                                                                                                       |
| [Adicionar uma atribuição de função do aplicativo](../api/user-post-approleassignments.md)                            | [appRoleAssignment](approleassignment.md)                                        | Atribuir uma função do aplicativo a esse usuário.                                                                                                                                                                                                    |
| [Remover uma atribuição de função do aplicativo](../api/user-delete-approleassignments.md)                       | Nenhum                                                                             | Remover uma atribuição de função do aplicativo desse usuário.                                                                                                                                                                                       |
| **Calendar**                                                                               |                                                                                  |                                                                                                                                                                                                                                     |
| [Criar calendário](../api/user-post-calendars.md)                                           | [Calendar](calendar.md)                                                          | Criar um novo Calendar postando na coleção calendars.                                                                                                                                                                       |
| [Criar calendarGroup](../api/user-post-calendargroups.md)                                 | [CalendarGroup](calendargroup.md)                                                | Criar um novo CalendarGroup postando na coleção calendarGroups.                                                                                                                                                             |
| [Criar evento](../api/user-post-events.md)                                                 | [event](event.md)                                                                | Criar um novo Event postando na coleção de eventos.                                                                                                                                                                             |
| [findMeetingTimes](../api/user-findmeetingtimes.md)                                        | [meetingTimeSuggestionsResult](meetingtimesuggestionsresult.md)                  | Encontrar o tempo e locais para reunião com base na disponibilidade dos participantes, localização ou restrições de tempo.                                                                                                                                      |
| [getSchedule](../api/calendar-getschedule.md)                                              | [scheduleInformation](scheduleinformation.md)                                    | Adquira as informações de disponibilidade para um conjunto de usuários, listas de distribuição ou recursos (salas e equipamentos) para um período de tempo especificado.                                                                           |
| [Listar calendários](../api/user-list-calendars.md)                                            | Coleção [calendar](calendar.md)                                               | Obter uma coleção de objetos Calendar.                                                                                                                                                                                                   |
| [Listar calendarGroups](../api/user-list-calendargroups.md)                                  | Coleção de [CalendarGroup](calendargroup.md)                                     | Obter uma coleção de objetos CalendarGroup.                                                                                                                                                                                              |
| [Listar calendarView](../api/user-list-calendarview.md)                                      | Coleção [event](event.md)                                                     | Obtenha uma coleção do objeto Event.                                                                                                                                                                                                      |
| [Listar eventos](../api/user-list-events.md)                                                  | Coleção [event](event.md)                                                     | Obter uma lista de objetos event na caixa de correio do usuário. A lista contém reuniões de instância única e reuniões mestres em série.                                                                                                                   |
| [reminderView](../api/user-reminderview.md)                                                | Coleção [Reminder](reminder.md)                                               | Retorna uma lista de lembretes de calendário nas horas de início e término especificadas.                                                                                                                                                       |
| **Contatos**                                                                               |                                                                                  |                                                                                                                                                                                                                                     |
| [Criar contato](../api/user-post-contacts.md)                                             | [contato](contact.md)                                                            | Criar um novo Contact postando na coleção contacts.                                                                                                                                                                         |
| [Criar contactFolder](../api/user-post-contactfolders.md)                                 | [pastadeContatos](contactfolder.md)                                                | Criar uma nova ContactFolder postando na coleção contactFolders.                                                                                                                                                             |
| [Listar contatos](../api/user-list-contacts.md)                                              | Coleção de[contato](contact.md)                                                 | Obter uma coleção de contatos da pasta Contatos padrão do usuário conectado.                                                                                                                                                    |
| [Listar contactFolders](../api/user-list-contactfolders.md)                                  | Coleção de [pastadeContatos](contactfolder.md)                                     | Obter a coleção de pastas de contatos na pasta Contatos padrão do usuário conectado.                                                                                                                                             |
| **Objetos de diretório**                                                                      |                                                                                  |                                                                                                                                                                                                                                     |
| [assignLicense](../api/user-assignlicense.md)                                              | [user](user.md)                                                                  | Adicionar ou remover assinaturas para o usuário. Você também pode habilitar e desabilitar planos específicos associados a uma assinatura.                                                                                                            |
| [checkMemberGroups](../api/user-checkmembergroups.md)                                      | Coleção de cadeias de caracteres                                                                | Verifique se há uma associação em uma lista de grupos. A verificação é transitiva.                                                                                                                                                                  |
| [checkMemberObjects](../api/user-checkmemberobjects.md)                                    | Coleção de cadeias de caracteres                                                                | Verifique se há associação em uma lista de objetos de grupo, função de diretório ou unidade administrativa. A função é transitiva.                                                                                                                |
| [exportPersonalData](../api/user-exportpersonaldata.md)                                    | Nenhum                                                                             | Envia uma solicitação de operação de política de dados, realizada por um administrador da empresa para exportar os dados de um usuário da organização.                                                                                                                   |
| [getByIds](../api/directoryobject-getbyids.md)                                             | Coleção de cadeias de caracteres                                                                | Retorna os objetos de diretório especificados a partir de uma lista de ids.                                                                                                                                                                           |
| [getMemberGroups](../api/user-getmembergroups.md)                                          | Coleção de cadeias de caracteres                                                                | Retorne todos os grupos dos quais o usuário é membro. A verificação é transitiva.                                                                                                                                                        |
| [getMemberObjects](../api/user-getmemberobjects.md)                                        | Coleção de cadeias de caracteres                                                                | Retorna todos os grupos e funções de diretório dos quais o usuário é membro. A verificação é transitiva.                                                                                                                                 |
| [Listar createdObjects](../api/user-list-createdobjects.md)                                  | Coleção [directoryObject](directoryobject.md)                                 | Obter os objetos directory criados pelo usuário da propriedade de navegação createdObjects.                                                                                                                                          |
| [Listar licenseDetails](../api/user-list-licensedetails.md)                                  | Coleção [licenseDetails](licensedetails.md)                                   | Obtenha uma coleção de objetos licenseDetails.                                                                                                                                                                                             |
| [Listar ownedDevices](../api/user-list-owneddevices.md)                                      | Coleção [directoryObject](directoryobject.md)                                 | Obter os dispositivos que pertencem ao usuário da propriedade de navegação ownedDevices.                                                                                                                                               |
| [Listar ownedObjects](../api/user-list-ownedobjects.md)                                      | Coleção [directoryObject](directoryobject.md)                                 | Obter os objetos directory que pertencem ao usuário da propriedade de navegação ownedObjects.                                                                                                                                     |
| [Listar registeredDevices](../api/user-list-registereddevices.md)                            | Coleção [directoryObject](directoryobject.md)                                 | Obter os dispositivos que estão registrados para o usuário da propriedade de navegação registeredDevices.                                                                                                                                    |
| [reprocessLicense](../api/user-reprocesslicenseassignment.md)                              | [user](user.md)                                                                  | Reprocessar as atribuições de assinatura do usuário.                                                                                                                                                                                    |
| [revokeSignInSessions](../api/user-revokesigninsessions.md)                                | Nenhum                                                                             | Revoga todos os tokens de sessão e de atualização do usuário emitidos para aplicativos, redefinindo a propriedade do usuário **signInSessionsValidFromDateTime** para data e a hora atuais. Força o usuário a entrar novamente nesses aplicativos. |
| **Drive**                                                                                  |                                                                                  |                                                                                                                                                                                                                                     |
| [Obter unidade](../api/drive-get.md)                                                           | [unidade](drive.md)                                                                | Recuperar as propriedades e as relações de um recurso Drive.                                                                                                                                                                      |
| [Filhos de lista](../api/driveitem-list-children.md)                                         | [DriveItems](driveitem.md)                                                       | Retornar uma coleção de DriveItems no relacionamento filho de um DriveItem.                                                                                                                                                      |
| **Grupos**                                                                                 |                                                                                  |                                                                                                                                                                                                                                     |
| [Listar joinedTeams](../api/user-list-joinedteams.md)                                        | Coleção [team](team.md)                                                       | Obter as equipes do Microsoft Teams no qual o usuário é membro direto da propriedade de navegação joinedTeams.                                                                                                                         |
| [Listar memberOf](../api/user-list-memberof.md)                                              | Coleção [directoryObject](directoryobject.md)                                 | Obter os grupos e as funções de diretório dos quais o usuário é membro direto da propriedade de navegação memberOf.                                                                                                                       |
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
| **Teamwork** |||
|[Lista de aplicativos instalados para o usuário](../api/userteamwork-list-installedapps.md) | Coleção[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) | Lista os aplicativos instalados no escopo pessoal de um usuário.|
|[Obtém o aplicativo instalado para o usuário](../api/userteamwork-get-installedapps.md)| [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) | Lista o aplicativo especificado instalado no escopo pessoal de um usuário. |
|[Adicionar o aplicativo para o usuário](../api/userteamwork-post-installedapps.md) | Nenhum | Adiciona (instala) um aplicativo no escopo pessoal de um usuário.|
|[Remover o aplicativo para o usuário](../api/userteamwork-delete-installedapps.md) | Nenhum | Remove (desinstala) um aplicativo no escopo pessoal de um usuário.|
|[Atualizar o aplicativo instalado para o usuário](../api/userteamwork-teamsappinstallation-upgrade.md) | Nenhum | Atualizações para a versão mais recente do aplicativo instalada no escopo pessoal de um usuário.|
|[Obter chat entre o usuário e o aplicativo](../api/userscopeteamsappinstallation-get-chat.md)| [Chat](chat.md)| Lista um chat entre o usuário e o aplicativo. |
| **Tarefas pendentes** |||
|[Criar tarefa](../api/todotasklist-post-tasks.md)|[todoTask](todotask.md)| Crie um [todoTask](todotask.md) na lista de tarefas especificada.|
|[Criar uma lista de tarefas](../api/todo-post-lists.md) | [todoTaskList](todotasklist.md) | Criar uma lista de tarefas To Dona caixa de correio do usuário. |
|[Listar tarefas](../api/todotasklist-list-tasks.md)|Coleção [todoTask](todotask.md)|Obtenha todos os recursos [todoTask](todotask.md) na lista especificada.|
|[Lista de listas de tarefas](../api/todo-list-lists.md) | Coleção [todoTaskList](todotasklist.md) | Obtenha todas as listas de tarefas na caixa de correio do usuário. |
| **Configurações do usuário**                                                                          |                                                                                  |                                                                                                                                                                                                                                     |
| [Obter configurações](../api/usersettings-get.md)                                                 | [userSettings](usersettings.md)                                                  | Leia o usuário e o objeto de configurações da organização.                                                                                                                                                                                     |
| [Atualizar configurações](../api/usersettings-update.md)                                           | [userSettings](usersettings.md)                                                  | Atualize as propriedades do objeto de configurações.                                                                                                                                                                                       |


## <a name="properties"></a>Propriedades

| Propriedade       | Tipo    |Descrição|
|:---------------|:--------|:----------|
|aboutMe|String|Um campo de entrada de texto em forma livre para o usuário se descrever.|
|accountEnabled|Boolean| **true** se a conta estiver habilitada; caso contrário, **false**. Essa propriedade é obrigatória quando um usuário é criado. Oferece suporte para `$filter`.    |
|ageGroup|[ageGroup](#agegroup-values)|Define a faixa etária do usuário. Valores permitidos: `null`, `minor`, `notAdult` e `adult`. Confira as [definições de propriedades da faixa etária legal](#legal-age-group-property-definitions) para obter mais informações. |
|assignedLicenses|Coleção [assignedLicense](assignedlicense.md)|As licenças que são atribuídas ao usuário. Retornado apenas em `$select`. Não anulável. Oferece suporte para `$filter`.           |
|assignedPlans|Coleção [assignedPlan](assignedplan.md)|Os planos que são atribuídos ao usuário. Somente leitura. Não anulável. |
|birthday|DateTimeOffset|O aniversário do usuário. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|businessPhones|String collection|Números de telefone para o usuário. OBSERVAÇÃO: Embora isso seja uma coleção de cadeias de caracteres, somente um número pode ser definido para essa propriedade. <br><br>Somente leitura para usuários sincronizados do diretório local. Retornado por padrão.|
|city|String|A cidade em que o usuário está localizado. O comprimento máximo é de 128 caracteres. Oferece suporte para `$filter`.|
|companyName | String | O nome da empresa em que o usuário está associado. Essa propriedade pode ser útil para descrever a empresa de onde procede um usuário externo. O comprimento máximo do nome da empresa é 64 caracteres.<br><br>Retornado apenas em `$select`.|
|consentProvidedForMinor|[consentProvidedForMinor](#consentprovidedforminor-values)|Define se o consentimento foi obtido para menores. Valores permitidos: `null`, `granted`, `denied` e `notRequired`. Confira as [definições de propriedades da faixa etária legal](#legal-age-group-property-definitions) para obter mais informações.|
|country|String|País/região em que o usuário está localizado. Por exemplo, "EUA" ou "Reino Unido". O comprimento máximo é de 128 caracteres. Oferece suporte para `$filter`.|
|createdDateTime | DateTimeOffset |Data de criação do objeto do usuário. Suporta o `$filter` com os operadores `eq`,`lt` e`ge`.|
|creationType|String|Indica se a conta de usuário foi criada como uma conta corporativa ou de estudante (`null`), uma conta externa (`Invitation`), uma conta local para um locatário do Azure Active Directory B2C (`LocalAccount`) ou uma inscrição de autoatendimento usando a verificação de email (`EmailVerified`). Somente leitura.|
|deletedDateTime| DateTimeOffset | A data e hora que o usuário foi excluído. <br><br>Retornado apenas em `$select`. |
|department|String|O nome do departamento no qual o usuário trabalha. O comprimento máximo é de 64 caracteres. Oferece suporte para `$filter`.|
|displayName|String|O nome exibido no catálogo de endereços para o usuário. Geralmente é a combinação do nome do usuário, inicial do meio e sobrenome. Esta propriedade é necessária quando um usuário é criado e não pode ser limpa durante as atualizações. O comprimento máximo é de 256 caracteres.<br><br>Retornado por padrão. Oferece suporte para `$filter` e `$orderby`.|
| employeeHireDate | DateTimeOffset | A data e a hora em que o usuário foi contratado ou começará a trabalhar em caso de futura contratação. <br><br>Retornado apenas em `$select`. Oferece suporte para `$filter`.|
| employeeId | String | O identificador de funcionário atribuído ao usuário pela organização. <br><br>Retornado apenas em `$select`. Oferece suporte para `$filter`.|
|employeeOrgData|[employeeOrgData](employeeorgdata.md) |Representa os dados da organização (por exemplo, divisão e costCenter) associados a um usuário. <br><br>Retornado apenas em `$select`.|
| employeeType | String | Captura o tipo de trabalhador corporativo: Empregado, Contratante, Consultor, Fornecedor, etc. <br><br>Retornado apenas em `$select`. Oferece suporte para `$filter`.|
|externalUserState|String|Para um usuário externo convidado para o locatário usando a [API de convite](../api/invitation-post.md), essa propriedade representa o status do convite do usuário convidado. Para usuários convidados, o estado pode ser `PendingAcceptance` ou `Accepted` ou `null` para todos os outros usuários. <br><br>Retornado apenas em `$select`. Suporta o `$filter` com os valores compatíveis. Por exemplo: `$filter=externalUserState eq 'PendingAcceptance'`.|
|externalUserStateChangeDateTime|DateTimeOffset|Mostra o carimbo de data/hora da alteração mais recente da propriedade **externalUserState**. <br><br>Retornado apenas em `$select`.|
|FaxNumber|String|O número de fax do usuário.|
|givenName|String|O nome fornecido (nome) do usuário. Retornado por padrão. O comprimento máximo é de 64 caracteres. Oferece suporte para `$filter`.|
| hireDate | DateTimeOffset | A data de contratação do usuário. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. <br><br>Retornado apenas em `$select`. <br><br> **Observação:** Esta propriedade é específica do SharePoint Online. Recomendamos usar a propriedade nativa **employeeHireDate** para definir e atualizar os valores das datas de contratação usando as APIs do Microsoft Graph. |
|id|String|O identificador exclusivo do usuário. Deve ser tratado como um identificador opaco. Herdado de [directoryObject](directoryobject.md). Chave. <br><br>Não anulável. Somente leitura.|
|Identidades|Coleção [objectIdentity](objectIdentity.md)| Representa as identidades que podem ser usadas para entrar nesta conta de usuário. Uma identidade pode ser fornecida pela Microsoft (também conhecida como conta local), por organizações ou por provedores de identidade social, como o Facebook, Google e Microsoft, e está vinculada a uma conta de usuário. Pode conter vários itens com o mesmo valor **signInType**. Pode conter até dez objetos [objectIdentity](objectIdentity.md). <br>Oferece suporte para `$filter`.|
|imAddresses|String collection|Os endereços do Protocolo de Início de Sessão (SIP) de VoIP (Voice over IP) da mensagem instantânea para o usuário. Somente leitura.|
|interests|Coleção de cadeias de caracteres|Uma lista para o usuário descrever os interesses dele.|
|isResourceAccount|Boolean| Não use – reservado para uso futuro.|
|jobTitle|String|O cargo do usuário. O comprimento máximo é de 128 caracteres. Retornado por padrão. Oferece suporte para `$filter`.|
|lastPasswordChangeDateTime| DateTimeOffset | A hora em que o usuário do Azure AD alterou a senha dele pela última vez. As informações de data e hora usam o formato ISO 8601 e estão sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|legalAgeGroupClassification|[legalAgeGroupClassification](#legalagegroupclassification-values)| Usado por aplicativos empresariais para determinar a faixa etária legal do usuário. Essa propriedade é somente leitura e calculada com base nas propriedades **ageGroup** e **consentProvidedForMinor**. Valores permitidos: `null`, `minorWithOutParentalConsent`, `minorWithParentalConsent`, `minorNoParentalConsentRequired`, `notAdult` e `adult`. Confira as [definições de propriedades da faixa etária legal](#legal-age-group-property-definitions) para obter mais informações.|
|licenseAssignmentStates|Coleção [licenseAssignmentState](licenseassignmentstate.md)|Estado das atribuições de licença para este usuário. Somente leitura.|
|email|String|O endereço SMTP do usuário, por exemplo, "jeff@contoso.onmicrosoft.com".<br>OBSERVAÇÃO: embora essa propriedade possa conter caracteres acentuados, eles podem causar problemas de acesso aos aplicativos primários para o usuário. <br><br>Retornado por padrão. Oferece suporte para `$filter` e `endsWith`.|
|mailboxSettings|[mailboxSettings](mailboxsettings.md)|Configurações da caixa de correio principal do usuário conectado. Você pode [obter](../api/user-get-mailboxsettings.md) ou [atualizar](../api/user-update-mailboxsettings.md) as configurações de localidade, fuso horário ou de envio de respostas automáticas a mensagens de entrada.<br><br>Retornado apenas em `$select`. Com suporte apenas para Obter API de usuário (`GET /users/{id}` ou `GET /me`).|
|mailNickname|String|O alias de email do usuário. Essa propriedade deve ser especificada quando um usuário é criado. O comprimento máximo é de 64 caracteres. Oferece suporte para `$filter`.|
|mobilePhone|String|O número de celular principal do usuário. Somente leitura para usuários sincronizados do diretório local. O comprimento máximo é de 64 caracteres. Retornado por padrão. |
|mySite|String|A URL do site pessoal do usuário.|
|officeLocation|String|A localização do escritório no local de trabalho do usuário. Retornado por padrão.|
|onPremisesDistinguishedName|String| Contém o `distinguished name` do Active Directory no local ou `DN`. A propriedade somente é preenchida para os clientes que estejam sincronizando o seu diretório local ao Azure Active Directory pelo Azure AD Connect. Somente leitura. |
|onPremisesDomainName|String| Contém o `domainFQDN` local, também chamado dnsDomainName sincronizado do diretório local. A propriedade somente é preenchida para os clientes que estejam sincronizando o seu diretório local ao Azure Active Directory pelo Azure AD Connect. Somente leitura. |
|onPremisesExtensionAttributes|[onPremisesExtensionAttributes](onpremisesextensionattributes.md)|Contém extensionAttributes 1-15 para o usuário. Observe que os atributos de extensão individuais não são selecionáveis nem filtráveis. Para um usuário do `onPremisesSyncEnabled`, a fonte de autoridade desse conjunto de propriedades é o local e é somente para leitura. Para um usuário somente na nuvem (onde `onPremisesSyncEnabled` é falso), essas propriedades podem ser definidas durante a criação ou atualização. Esses atributos de extensão também são conhecidos como atributos personalizados do Exchange 1-15. |
|onPremisesImmutableId|String|Essa propriedade é usada para associar uma conta de usuário do Active Directory local com seu objeto de usuário do Azure AD. Esta propriedade deve ser especificada ao criar uma nova conta de usuário no Graph se você estiver usando um domínio federado para a propriedade **userPrincipalName** (UPN). **Importante:** Os caracteres **$** e **\_** não podem ser utilizados ao especificar esta propriedade. Oferece suporte para `$filter`.                            |
|onPremisesLastSyncDateTime|DateTimeOffset|Indica a última vez em que o objeto foi sincronizado com o diretório local; por exemplo: "2013-02-16T03:04:54Z". O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|
|onPremisesProvisioningErrors|coleção [OnPremisesProvisioningError](onpremisesprovisioningerror.md)| Erros ao usar o produto de sincronização da Microsoft durante o provisionamento. |
|onPremisesSamAccountName|String| Contém o `samAccountName` local sincronizado no diretório local. A propriedade somente é preenchida para os clientes que estejam sincronizando o seu diretório local ao Azure Active Directory pelo Azure AD Connect. Somente leitura. |
|onPremisesSecurityIdentifier|String|Contém o identificador de segurança (SID) local do usuário que foi sincronizado do local com a nuvem. Somente leitura.|
|onPremisesSyncEnabled|Booliano| **True** se esse objeto está sincronizado de um diretório local; **false** se esse objeto foi originalmente sincronizado de um diretório local, mas não está mais sincronizado; **null** se esse objeto nunca foi sido sincronizado de um diretório local (padrão). Somente leitura |
|onPremisesUserPrincipalName|String| Contém o `userPrincipalName` local sincronizado no diretório local. A propriedade somente é preenchida para os clientes que estejam sincronizando o seu diretório local ao Azure Active Directory pelo Azure AD Connect. Somente leitura. |
|otherMails|Coleção String| Uma lista de endereços de email adicional para o usuário; Por exemplo: `["bob@contoso.com", "Robert@fabrikam.com"]`. <br>OBSERVAÇÃO: embora essa propriedade possa conter caracteres acentuados, eles podem causar problemas de acesso aos aplicativos primários para o usuário. <br><br> Oferece suporte para o `$filter`.|
|passwordPolicies|String|Especifica as políticas de senha do usuário. Esse valor é uma enumeração cujo um dos valores possíveis é "DisableStrongPassword", o que permite especificar senhas mais fracas do que a política padrão. Também é possível especificar "DisablePasswordExpiration". Ambos podem ser especificados juntos; por exemplo: "DisablePasswordExpiration, DisableStrongPassword".|
|passwordProfile|[passwordProfile](passwordprofile.md)|Especifica o perfil de senha do usuário. O perfil contém a senha do usuário. Essa propriedade é obrigatória quando um usuário é criado. A senha no perfil deve atender a requisitos mínimos, conforme especificado pela propriedade **passwordPolicies**. Por padrão, é obrigatória uma senha forte.|
|pastProjects|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar seus projetos anteriores.|
|postalCode|String|O código postal do endereço postal do usuário. O código postal é específico para o país/região do usuário. Nos Estados Unidos da América, este atributo contém o Código postal. O comprimento máximo é de 40 caracteres.|
|preferredLanguage|String|O idioma preferencial do usuário. Deve seguir o Código ISO 639-1; por exemplo "en-US". Retornado por padrão.|
|preferredName|String|O nome preferencial do usuário.|
|provisionedPlans|coleção [provisionedPlan](provisionedplan.md)|Os planos que estão provisionados para o usuário. Somente leitura. Não anulável. |
|proxyAddresses|String collection|Por exemplo: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` O operador **any** é obrigatório para expressões de filtro em propriedades de vários valores. Somente leitura, não anulável. Oferece suporte para `$filter`.|
|refreshTokensValidFromDateTime|DateTimeOffset|Os tokens de atualização ou de sessão (cookies de sessão) emitidos antes dessa hora são inválidos e os aplicativos recebem um erro ao usar um token de atualização ou de sessão inválido para adquirir um token de acesso delegado (para acessar APIs como o Microsoft Graph).  Se isso acontecer, o aplicativo precisará adquirir um novo token de atualização, fazendo uma solicitação ao ponto de extremidade de autorização. <br><br>Retornado apenas em `$select`. Apenas leitura. |
|responsibilities|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar suas responsabilidades.|
|schools|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar as escolas que frequentou.|
|showInAddressList|Booliano|**true** se a lista de endereços global do Outlook deve conter o usuário, caso contrário **false**. Se não estiver configurado, isso será tratado como **true**. Para os usuários convidados por meio do Gerenciador de convites, essa propriedade será definida como **false**.|
|skills|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar suas qualificações.|
|signInSessionsValidFromDateTime|DateTimeOffset| Os tokens de atualização ou de sessão (cookies de sessão) emitidos antes dessa hora são inválidos e os aplicativos recebem um erro ao usar um token de atualização ou de sessão inválido para adquirir um token de acesso delegado (para acessar APIs como o Microsoft Graph).  Se isso acontecer, o aplicativo precisará adquirir um novo token de atualização, fazendo uma solicitação ao ponto de extremidade de autorização. Somente leitura. Use [revokeSignInSessions](../api/user-revokesigninsessions.md) para redefinir.|
|state|String|O estado ou município no endereço do usuário. O comprimento máximo é de 128 caracteres. Oferece suporte para `$filter`.|
|streetAddress|String|O endereço do local de trabalho do usuário. O comprimento máximo é de 1024 caracteres.|
|surname|String|O sobrenome do usuário (nome de família ou sobrenome). Retornado por padrão. O comprimento máximo é de 64 caracteres. Oferece suporte para `$filter`.|
|usageLocation|String|Um código de duas letras (padrão ISO 3166). Obrigatório para os usuários que receberão licenças devido à exigência legal de verificar a disponibilidade de serviços nos países.  Os exemplos incluem: "US", "JP" e "GB". Não anulável. Oferece suporte para `$filter`.|
|userPrincipalName|String|O nome UPN do usuário. O nome UPN é um nome de logon para o usuário ao estilo da Internet com base na RFC 822 padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email do usuário. O formato geral é alias@domain, onde o domínio deve estar presente na coleta de domínios verificados pelo locatário. Essa propriedade é obrigatória quando um usuário é criado. Os domínios verificados para o locatário podem ser acessados pela propriedade **verifiedDomains** de [organization](organization.md).<br>OBSERVAÇÃO: embora essa propriedade possa conter caracteres acentuados, eles podem causar problemas de acesso aos aplicativos primários para o usuário. <br><br>Retornado por padrão. Oferece suporte para `$filter`, `$orderby` e `endsWith`.
|userType|String|Um valor de cadeia de caracteres que pode ser usado para classificar tipos de usuários no seu diretório, como “Membro” e “Convidado”. Oferece suporte para `$filter`.          |

### <a name="legal-age-group-property-definitions"></a>Definições de propriedade da faixa etária legal

Esta seção explica como as três propriedades de grupo idade (**legalAgeGroupClassification**, **ageGroup** e **consentProvidedForMinor**) são usadas por administradores do Azure Active Directory e desenvolvedores de aplicativos empresariais para atender às regulamentações relacionadas à idade:
- A propriedade legal **AgeGroupClassification** é somente leitura. É usado por desenvolvedores de aplicativos corporativos para garantir o tratamento correto de um usuário com base em sua faixa etária legal. É calculado com base nas propriedades **ageGroup** e **consentProvidedForMinor** do usuário.
- **ageGroup** e **consentProvidedForMinor** são propriedades opcionais usadas pelos administradores do Azure Active Directory para ajudar a garantir que o uso de uma conta seja tratado corretamente com base nas regras regulatórias relacionadas à idade que regem o país ou região do usuário.

Por exemplo: Cameron é o administrador de um diretório em uma escola de ensino fundamental em Holyport, no Reino Unido. No início do ano letivo ele usa a documentação de admissão para obter o consentimento dos pais dos menores baseado nos regulamentos relacionadas com a idade no Reino Unido. O consentimento obtido do pai permite que a conta do menor seja usado pela escola de Holyport e os aplicativos da Microsoft. Cameron cria todas as contas e define **ageGroup** como `minor` e **consentProvidedForMinor** como `granted`. Os aplicativos usados ​​por seus alunos podem suprimir recursos que não são adequados para menores.

<!-- Note that the following 3 sub-sections are only documented like enums for a consistent user experience. 
For some reason they are not defined as enums in the CSDL. 
Hence the type of the corresponding 3 properties remain as string type in the Properties table.
-->

#### <a name="legalagegroupclassification-values"></a>legalAgeGroupClassification values

| Member    | Descrição|
|:---------------|:----------|
|null|Valor padrão, nenhum **ageGroup** foi definido para o usuário.|
|minorWithoutParentalConsent |(Reservado para uso futuro)|
|minorWithParentalConsent| O usuário é considerado menor baseado nos regulamentos relacionados com a idade de seu país ou região, e o administrador da conta obteve o consentimento apropriado dos pais ou responsável.|
|adult|O usuário é considerado adulto baseado nos regulamentos relacionadas com a idade do seu país ou região.|
|notAdult|O usuário é de um país ou região com regulamentações adicionais relacionados à idade (por exemplo, Estados Unidos, Reino Unido, União Europeia ou Coreia do Sul) e a idade do usuário está entre menor e adulto (como estipulado com base no país ou região). Em geral, isso significa que adolescentes são considerados como `notAdult` em países regulamentados.|
|minorNoParentalConsentRequired|O usuário é menor de idade, mas é de um país ou região que não tem com regulamentações relacionadas com a idade.|

#### <a name="agegroup-values"></a>ageGroup values

| Member    | Descrição|
|:---------------|:--------|
|null|Valor padrão, nenhum **ageGroup** foi definido para o usuário.|
|menor|O usuário é considerado um menor.|
|notAdult|O usuário é de um país que possui regulamentos legais (como Estados Unidos, Reino Unido, União Europeia ou Coreia do Sul) e a idade do usuário é superior ao limite superior de idade infantil (conforme o país) e inferior ao limite inferior de adulto idade (conforme estipulado com base no país ou região). Basicamente, adolescentes são considerados como `notAdult` em países regulamentados.|
|adult|O usuário deve ser tratado como um adulto.|

#### <a name="consentprovidedforminor-values"></a>consentProvidedForMinor values

| Member    | Descrição|
|:---------------|:----------|
|null|Valor padrão, nenhum **consentimentoProvidedForMinor** foi definido para o usuário.|
|concedido|O consentimento foi obtido para o usuário ter uma conta.|
|denied|O consentimento não foi obtido para o usuário ter uma conta.|
|notRequired|O usuário é de um local que não exige consentimento.|

## <a name="relationships"></a>Relações

| Relação | Tipo    |Descrição|
|:---------------|:--------|:----------|
|agreementAcceptances|Coleção [agreementAcceptance](agreementacceptance.md)| Status de aceitação dos termos de uso do usuário. Somente leitura. Anulável.|
|activities|Coleção [userActivity](projectrome-activity.md)|As atividades do usuário em todos os dispositivos. Somente leitura. Anulável.|
|appRoleAssignments|[appRoleAssignment](approleassignment.md) collection|Representa as funções de aplicativo que um usuário recebeu para um programa. |
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
|events|Coleção [event](event.md)|Os eventos do usuário. O padrão é mostrar eventos no Calendário Padrão. Somente leitura. Anulável.|
|extensions|[extension](extension.md) collection|A coleção de extensões abertas definidas para o usuário. Somente leitura. Anulável.|
|inferenceClassification | [inferenceClassification](inferenceclassification.md) | Classificação de relevância das mensagens do usuário com base em designações explícitas que substituem a relevância ou importância deduzida. |
|insights|[officeGraphInsights](officegraphinsights.md) | Somente leitura. Anulável.|
|licenseDetails|Coleção de[licenseDetails](licensedetails.md)|Uma coleção dos detalhes da licença deste usuário. Somente leitura.|
|mailFolders|Coleção [mailFolder](mailfolder.md)| As pastas de email do usuário. Somente leitura. Anulável.|
|manager|[directoryObject](directoryobject.md)|O usuário ou contato que é o gerente deste usuário. Somente leitura. (Métodos HTTP: GET, PUT, DELETE.)|
|memberOf|Coleção [directoryObject](directoryobject.md)|Os grupos e as funções de diretório dos quais o usuário é membro. Somente leitura. Anulável.|
|messages|Coleção [message](message.md)|As mensagens em uma caixa de correio ou pasta. Somente leitura. Anulável.|
|onenote|[onenote](onenote.md)| Somente leitura.|
|outlook|[outlookUser](outlookuser.md)| Somente leitura.|
|ownedDevices|Coleção [directoryObject](directoryobject.md)|Dispositivos que pertencem ao usuário. Somente leitura. Anulável.|
|ownedObjects|Coleção [directoryObject](directoryobject.md)|Objetos de diretório que pertencem ao usuário. Somente leitura. Anulável.|
|people|Coleção [person](person.md)| Pessoas que são relevantes para o usuário. Somente leitura. Anulável.
|photo|[profilePhoto](profilephoto.md)| A foto de perfil do usuário. Somente leitura.|
|planner|[plannerUser](planneruser.md)| Ponto de entrada para o recurso do Planner que pode existir para um usuário. Somente leitura.|
|registeredDevices|Coleção [directoryObject](directoryobject.md)|Dispositivos que estão registrados para o usuário. Somente leitura. Anulável.|
|todo|[todo](todo.md)|Representa os serviços To Do disponíveis para um usuário. |

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
  "employeeHireDate": "2020-01-01T00:00:00Z",
  "employeeId": "string",
  "employeeOrgData": {"@odata.type": "microsoft.graph.employeeOrgData"},
  "employeeType": "string",
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
  "otherMails": ["string"],
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
  ],
  "section": "documentation",
  "tocPath": ""
}-->

