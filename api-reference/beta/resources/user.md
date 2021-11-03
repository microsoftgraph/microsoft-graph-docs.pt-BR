---
title: Tipo de recurso de usuário
description: Representa uma conta de usuário do Azure AD. Herda de directoryObject.
author: jpettere
ms.localizationpriority: high
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 60aa133d42842aeaa9121151bf2603223eefbff0
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60689036"
---
# <a name="user-resource-type"></a>Tipo de recurso de usuário

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma conta de usuário do Azure Active Directory (Azure AD). Herda de [directoryObject](directoryobject.md).

O recurso **usuário** permite que os aplicativos especifiquem as preferências do usuário para idiomas e formatos de data/hora para as caixas de correio primárias do Exchange e para o perfil do Azure AD do usuário. Para obter mais detalhes, consulte [preferências do usuário para idiomas e formatos regionais](#user-preferences-for-languages-and-regional-formats).

Por motivos de desempenho, as operações [create](../api/user-post-users.md), [get](../api/user-get.md) e [list](../api/user-list.md) retornam por padrão apenas um subconjunto das propriedades usadas com mais frequência. Essas propriedades padrão estão listadas na seção [Propriedades](#properties). Para obter as propriedades não retornadas por padrão, especifique-as em uma opção de consulta `$select` do OData.

Esse recurso permite:

- Adicionar seus próprios dados às propriedades personalizadas como [extensions](/graph/extensibility-overview).
- Assinar as [notificações de alteração](/graph/webhooks).
- Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/user-delta.md).

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:------ |:----------- |:----------- |
| [Listar usuários](../api/user-list.md) | Coleção [user](user.md) | Recuperar uma lista de objetos user. |
| [Criar usuário](../api/user-post-users.md) | [user](user.md) | Criar um novo objeto user. |
| [Obter usuário](../api/user-get.md) | [user](user.md) | Ler propriedades e relações do objeto user. |
| [Atualizar usuário](../api/user-update.md) | [user](user.md) | Atualizar o objeto user. |
| [Excluir usuário](../api/user-delete.md) | Nenhum | Excluir o objeto user. |
| [Obter delta](../api/user-delta.md) | coleção de usuários | Obter as alterações incrementais para usuários. |
| [changePassword](../api/user-changepassword.md) | Nenhum | Atualize sua senha. |
| [invalidateAllRefreshTokens](../api/user-invalidateallrefreshtokens.md) | Nenhum | Invalidar todos os tokens de atualização do usuário emitidos para as aplicações. |
| [validatePassword](../api/user-validatepassword.md)|[passwordValidationInformation](../resources/passwordvalidationinformation.md)|Valide a senha de um usuário na política de validação de senha da organização e informe se a senha é válida. |
| **Atribuição de funções do aplicativo**|||
| [List appRoleAssignments](../api/user-list-approleassignments.md) | [appRoleAssignment](approleassignment.md) collection | Obter os aplicativos e funções do aplicativo atribuídos a esse usuário. |
| [Adicionar uma atribuição de função do aplicativo](../api/user-post-approleassignments.md) | [appRoleAssignment](approleassignment.md) | Atribuir uma função do aplicativo a esse usuário. |
| [Remover uma atribuição de função do aplicativo](../api/user-delete-approleassignments.md) | Nenhum | Remover uma atribuição de função do aplicativo desse usuário. |
| **Calendar** |||
| [Criar calendário](../api/user-post-calendars.md) | [Calendar](calendar.md) | Criar um novo Calendar postando na coleção calendars. |
| [Criar calendarGroup](../api/user-post-calendargroups.md) | [CalendarGroup](calendargroup.md) | Criar um novo CalendarGroup postando na coleção calendarGroups. |
| [Criar evento](../api/user-post-events.md) | [event](event.md) | Criar um novo Event postando na coleção de eventos. |
| [findMeetingTimes](../api/user-findmeetingtimes.md) | [meetingTimeSuggestionsResult](meetingtimesuggestionsresult.md) | Encontrar o tempo e locais para reunião com base na disponibilidade dos participantes, localização ou restrições de tempo. |
| [findRooms](../api/user-findrooms.md) | Coleção [emailaddress.md](emailaddress.md) | Obter todas as salas de reunião no locatário do usuário ou em uma lista de salas específica. |
| [findRoomLists](../api/user-findroomlists.md) | Coleção [emailaddress.md](emailaddress.md) | Obter as listas de salas definidas em um locatário. |
| [getSchedule](../api/calendar-getschedule.md) | [scheduleInformation](scheduleinformation.md) | Adquira as informações de disponibilidade para um conjunto de usuários, listas de distribuição ou recursos (salas e equipamentos) para um período de tempo especificado. |
| [Listar calendários](../api/user-list-calendars.md) | Coleção [Calendar](calendar.md) | Obter uma coleção de objetos Calendar. |
| [Listar calendarGroups](../api/user-list-calendargroups.md) | Coleção [CalendarGroup](calendargroup.md) | Obter uma coleção de objetos CalendarGroup. |
| [Listar calendarView](../api/user-list-calendarview.md) | Coleção [event](event.md) | Obter uma coleção de objetos de evento. |
| [Listar eventos](../api/user-list-events.md) | Coleção [event](event.md) | Obter uma lista de objetos event na caixa de correio do usuário. A lista contém reuniões de instância única e reuniões mestres em série. |
| [reminderView](../api/user-reminderview.md) | Coleção [Reminder](reminder.md) | Retorna uma lista de lembretes de calendário nas horas de início e término especificadas.|
| **Contatos**|||
| [Criar contato](../api/user-post-contacts.md)| [contato](contact.md) | Crie um novo contato postando na coleção de contatos. |
| [Criar contactFolder](../api/user-post-contactfolders.md) | [contactFolder](contactfolder.md) | Crie um novo contactFolder postando na coleção contactFolders. |
| [Listar contatos](../api/user-list-contacts.md) | Coleção [Contact](contact.md) | Obter uma coleção de contatos da pasta padrão de contatos do usuário conectado. |
| [Listar contactFolders](../api/user-list-contactfolders.md) | Coleção [ContactFolder](contactfolder.md) | Obtenha a coleção de pastas de contatos na pasta de contatos padrão do usuário conectado. |
| **Objetos de diretório**|||
| [activateServicePlan](../api/user-activateserviceplan.md) | Nenhum | Ative um serviço com um determinado`servicePlanId` e `skuId`para um determinado[ usuário](user.md). |
| [assignLicense](../api/user-assignlicense.md) | [user](user.md) | Adicionar ou remover assinaturas para o usuário. Você também pode habilitar e desabilitar planos específicos associados a uma assinatura. |
| [checkMemberGroups](../api/user-checkmembergroups.md) | Coleção de cadeias de caracteres | Verifique se há uma associação em uma lista de grupos. A verificação é transitiva. |
| [checkMemberObjects](../api/user-checkmemberobjects.md) | Coleção de cadeias de caracteres | Verifique se há associação em uma lista de objetos de grupo, função de diretório ou unidade administrativa. A verificação é transitiva. |
| [exportPersonalData](../api/user-exportpersonaldata.md) | Nenhum | Envia uma solicitação de operação de política de dados, realizada por um administrador da empresa para exportar os dados de um usuário da organização. |
| [getByIds](../api/directoryobject-getbyids.md) | Coleção de cadeias de caracteres | Retorna os objetos de diretório especificados a partir de uma lista de ids. |
| [getMemberGroups](../api/user-getmembergroups.md) | Coleção de cadeias de caracteres | Retorne todos os grupos dos quais o usuário é membro. A verificação é transitiva. |
| [getMemberObjects](../api/user-getmemberobjects.md) | Coleção String | Retorna todos os grupos, funções de diretório e unidades administrativas dos quais o usuário é membro. A verificação é transitiva. |
| [Get transitiveReports](../api/user-get-transitivereports.md) | Inteiro | Obtenha a contagem de relatórios transitivos para um usuário na propriedade de navegação transitiveReports. |
| [Listar createdObjects](../api/user-list-createdobjects.md) | Coleção [directoryObject](directoryobject.md) | Obter os objetos directory criados pelo usuário da propriedade de navegação createdObjects. |
| [Listar licenseDetails](../api/user-list-licensedetails.md) | Coleção [licenseDetails](licensedetails.md) | Obtenha uma coleção de objetos licenseDetails. |
| [Listar ownedDevices](../api/user-list-owneddevices.md) | Coleção [directoryObject](directoryobject.md) | Obter os dispositivos que pertencem ao usuário da propriedade de navegação ownedDevices. |
| [Listar ownedObjects](../api/user-list-ownedobjects.md) | Coleção [directoryObject](directoryobject.md) | Obter os objetos directory que pertencem ao usuário da propriedade de navegação ownedObjects. |
| [Listar registeredDevices](../api/user-list-registereddevices.md) | Coleção [directoryObject](directoryobject.md) | Obter os dispositivos que estão registrados para o usuário da propriedade de navegação registeredDevices. |
| [Listar associações de função com escopo](../api/user-list-scopedrolememberof.md) | Coleção [scopedRoleMembership](scopedrolemembership.md) | Obter as associações de unidades administrativas de função com escopo deste usuário. |
| [List usageRights](../api/user-list-usagerights.md) | Coleção [usageRight](usageright.md) | Obtenha uma coleção de direitos de uso concedidos ao usuário. |
| [reprocessLicense](../api/user-reprocesslicenseassignment.md) | [user](user.md) | Reprocessar as atribuições de assinatura do usuário. |
| [revokeSignInSessions](../api/user-revokesigninsessions.md) | Nenhum | Revoga todos os tokens de sessão e de atualização do usuário emitidos para aplicativos, redefinindo a propriedade do usuário **signInSessionsValidFromDateTime** para data e a hora atuais. Força o usuário a entrar novamente nesses aplicativos. Este método substitui **invalidateAllRefreshTokens**. |
| **Unidade** |||
| [Obter unidade](../api/drive-get.md) | [unidade](drive.md) | Recuperar as propriedades e as relações de um recurso Drive. |
| [Filhos de lista](../api/driveitem-list-children.md) | [DriveItems](driveitem.md) | Retornar uma coleção de DriveItems no relacionamento filho de um DriveItem. |
| **Grupos** |||
| [Listar joinedTeams](../api/user-list-joinedteams.md) | Coleção [team](team.md) | Obter as equipes do Microsoft Teams no qual o usuário é membro direto da propriedade de navegação joinedTeams. |
| [Listar memberOf](../api/user-list-memberof.md) | Coleção [directoryObject](directoryobject.md) | Obter os grupos, funções de diretório e as unidades administrativas dos quais esse usuário é membro direto, da propriedade de navegação memberOf. |
| [Listar memberOf transitivos](../api/user-list-transitivememberof.md) | Coleção [directoryObject](directoryobject.md) | Lista os grupos e funções de diretório e unidades administrativas dos quais o usuário é membro. Essa operação é transitiva e inclui os grupos dos quais o usuário é membro aninhado. |
| **Percepções** |||
| [Listar compartilhado](../api/insights-list-shared.md) | coleção [sharedInsight](insights-shared.md) | Visão calculada que retorna a lista de arquivos compartilhados com um usuário. |
| [Listar tendências](../api/insights-list-trending.md) | coleção [tendências](insights-trending.md)  | Insights calculados que retornam a lista de itens de tendências do usuário. |
| [Listar usados](../api/insights-list-used.md) | coleção [usedInsight](insights-used.md) | Visão calculada que retorna a lista de arquivos usados com um usuário. |
| **Email** |||
| [Create inferenceClassificationOverride](../api/inferenceclassification-post-overrides.md) | Nenhum | Criar uma substituição da Caixa de Entrada Destaques para um remetente identificado por um endereço SMTP. |
| [Criar MailFolder](../api/user-post-mailfolders.md) | [mailFolder](mailfolder.md) | Criar uma nova MailFolder postando na coleção mailFolders |
| [Criar mensagem](../api/user-post-messages.md) | [message](message.md) | Crie uma mensagem postando na coleção de mensagens. |
| [Criar messageRule](../api/mailfolder-post-messagerules.md) | [messageRule](messagerule.md) | Crie um objeto messageRule especificando um conjunto de condições e ações. |
| [getMailTips](../api/user-getmailtips.md) | Coleção [mailTips](mailtips.md) | Retornar dicas de email de um ou mais destinatários conforme disponíveis para o usuário conectado. |
| [Listar mailFolders](../api/user-list-mailfolders.md) | Coleção [mailFolder](mailfolder.md) | Obter o conjunto de pastas de email sob a pasta raiz do usuário conectado. |
| [Listar mensagens](../api/user-list-messages.md) | Coleção [message](message.md) | Obter todas as mensagens na caixa de correio do usuário conectado. |
| [List overrides](../api/inferenceclassification-list-overrides.md) | Coleção [inferenceClassificationOverride](inferenceclassificationoverride.md) | Obtenha as substituições da Caixa de Entrada Destaques que um usuário configurou para sempre classificar as mensagens de determinados remetentes de maneiras específicas. |
| [Listar regras](../api/mailfolder-list-messagerules.md) | Coleção [messageRule](messagerule.md) | Obtenha todos os objetos messageRule definidos para a caixa de entrada do usuário. |
| [Enviar email](../api/user-sendmail.md) | Nenhum | Enviar a mensagem especificada no corpo da solicitação. |
| **Anotações** |||
| [Criar bloco de anotações](../api/onenote-post-notebooks.md) | [bloco de anotações](notebook.md) | Crie um novo bloco de anotações do OneNote. |
| [Listar blocos de anotações](../api/onenote-list-notebooks.md) | Coleção [bloco de anotações](notebook.md) | Recuperar uma lista de objetos do bloco de anotações. |
| **Extensões abertas** |||
| [Criar extensão aberta](../api/opentypeextension-post-opentypeextension.md) | [openTypeExtension](opentypeextension.md) | Crie uma extensão aberta e adicione propriedades personalizadas a uma instância nova ou existente de um recurso. |
| [Obter extensão aberta](../api/opentypeextension-get.md) | Coleção [openTypeExtension](opentypeextension.md) | Obtenha uma extensão aberta identificada pelo nome da extensão. |
| **Hierarquia da organização** |||
| [Atribuir gerenciador](../api/user-post-manager.md) | Nenhum | Atribuir um gerenciador de usuário. |
| [Obter gerenciador](../api/user-list-manager.md) | [directoryObject](directoryobject.md) | Obter o usuário ou contato que é o gerente do usuário da propriedade de navegação manager. |
| [Listar directReports](../api/user-list-directreports.md) | Coleção [directoryObject](directoryobject.md) | Obter os usuários ou contatos subordinados ao usuário da propriedade de navegação directReports. |
| **Configurações do Outlook** |||
| [Criar categoria do Outlook](../api/outlookuser-post-mastercategories.md) | [outlookCategory](outlookcategory.md) | Cria um objeto outlookCategory na lista mestra de categorias do usuário. |
| [Obter supportedLanguages](../api/outlookuser-supportedlanguages.md), | Coleção [localeInfo](localeinfo.md) | Obtém a lista de locais e idiomas com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário. |
| [Obter supportedTimeZones](../api/outlookuser-supportedtimezones.md) | [timeZoneInformation](timezoneinformation.md collection) | Obtém a lista de fusos horários com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário. |
| [Obtém configurações de caixa de correio do usuário](../api/user-get-mailboxsettings.md) | [mailboxSettings](mailboxsettings.md) | Obtém as configurações de caixa de correio do usuário. |
| [Listar as categorias do Outlook](../api/outlookuser-list-mastercategories.md) | Coleção [outlookCategory](outlookcategory.md)                                 | Obtém todas as categorias que foram definidas para o usuário. |
| [Converter IDs do Exchange](../api/user-translateexchangeids.md) | coleção [convertIdResult](convertidresult.md) | Traduzir os identificadores de recursos relacionados ao Outlook entre formatos. |
| [Atualizar configurações da caixa de correio do usuário](../api/user-update-mailboxsettings.md) | [mailboxSettings](mailboxsettings.md) | Habilitar, configurar ou desabilitar o mailboxSettings de um ou mais usuários. |
| **Pessoas** |||
| [Listar pessoas](../api/user-list-people.md) | [person](person.md) | Recupere uma lista de objetos person ordenados por relevância para o usuário, o que é determinado pelos padrões de comunicação e colaboração e pelas relações comerciais do usuário. |
| **Foto** |||
| [Obter foto](../api/profilephoto-get.md) | [profilePhoto](profilephoto.md) | Obtém o profilePhoto especificado ou seus metadados (propriedades profilePhoto). |
| [Atualizar profilephoto](../api/profilephoto-update.md) | Nenhum | Atualiza a foto de qualquer usuário no locatário, incluindo o usuário conectado ou o grupo ou contato especificado. |
| **Planner** |||
| [Obter plannerUser](../api/planneruser-get.md) | [plannerUser](planneruser.md) | Recupere as propriedades e relações de um objeto plannerUser. |
| [Listar favoritePlans](../api/planneruser-list-favoriteplans.md) | coleção [plannerPlan](plannerplan.md) | Recupere uma lista de plannerPlans marcados como favoritos por um usuário. |
| [Listar recentPlans](../api/planneruser-list-recentplans.md) | coleção [plannerPlan](plannerplan.md) | Recupere uma lista de plannerPlans recentemente exibida por um usuário. |
| [Listar tarefas](../api/planneruser-list-tasks.md) | Coleção [plannerTask](plannertask.md) | Obter o plannerTasks atribuído ao usuário.|
| [Atualizar plannerUser](../api/planneruser-update.md) | Nenhum | Atualize as propriedades de um objeto plannerUser. |
| **Perfil** |||
| [Obter perfil](../api/profile-get.md) | [perfil](profile.md) | Recupere as propriedades e relações de um objeto de perfil para um determinado usuário. |
| [Excluir perfil](../api/profile-delete.md) | Nenhum | Exclua o objeto de perfil de uma conta de usuário. |
| **Extensões de esquema** |||
| [Adicionar valores de extensões de esquema](/graph/extensibility-schema-groups) | Nenhum | Cria uma definição para a extensão de esquema e usa-a para adicionar dados digitados personalizados a um recurso. |
| **Teamwork** |||
|[Lista de aplicativos instalados para o usuário](../api/userteamwork-list-installedapps.md) | Coleção[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) | Os aplicativos instalados no escopo pessoal desse usuário.|
|[Obter o aplicativo instalado para o usuário](../api/userteamwork-get-installedapps.md)| [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) | Lista o aplicativo especificado instalado no escopo pessoal de um usuário. |
|[Adicionar o aplicativo para o usuário](../api/userteamwork-post-installedapps.md) | Nenhum | Adiciona (instala) um aplicativo no escopo pessoal de um usuário.|
|[Remover o aplicativo para o usuário](../api/userteamwork-delete-installedapps.md) | Nenhum | Remove (desinstala) um aplicativo no escopo pessoal de um usuário.|
|[Atualizar o aplicativo instalado para o usuário](../api/userteamwork-teamsappinstallation-upgrade.md) | Nenhum | Atualizações para a versão mais recente do aplicativo instalada no escopo pessoal de um usuário.|
|[Obter chat entre o usuário e o aplicativo](../api/userscopeteamsappinstallation-get-chat.md)| [Chat](chat.md)| Lista um chat entre o usuário e o aplicativo. |
| **Tarefas pendentes** |||
|[Criar tarefa](../api/todotasklist-post-tasks.md)|[todoTask](todotask.md)| Crie um [todoTask](todotask.md) na lista de tarefas especificada.|
|[Criar uma lista de tarefas](../api/todo-post-lists.md) | [todoTaskList](todotasklist.md) | Criar uma lista de tarefas To Dona caixa de correio do usuário. |
|[Listar tarefas](../api/todotasklist-list-tasks.md)|Coleção [todoTask](todotask.md)|Obtenha todos os recursos [todoTask](todotask.md) na lista especificada.|
|[Lista de listas de tarefas](../api/todo-list-lists.md) | Coleção [todoTaskList](todotasklist.md) | Obtenha todas as listas de tarefas na caixa de correio do usuário. |
| **Configurações do usuário** |||
| [Obter configurações](../api/usersettings-get.md) | [userSettings](usersettings.md) | Leia o usuário e o objeto de configurações da organização. |
| [Atualizar configurações](../api/usersettings-update.md) | [userSettings](usersettings.md) | Atualize as propriedades do objeto de configurações. |
| **Tarefas do Outlook** (obsoleto)|||
| [Criar outlookTask](../api/outlookuser-post-tasks.md)(obsoleto) | [outlookTask](outlooktask.md) | Criar uma tarefa do Outlook no grupo de tarefas padrão (Minhas Tarefas) e pasta de tarefas padrão (Tarefas) na caixa de correio do usuário. |
| [Listar de tarefas](../api/outlookuser-list-tasks.md) (obsoleto) | coleção [outlookTask](outlooktask.md) | Obtenha todas as tarefas do Outlook na caixa de correio do usuário. |


## <a name="properties"></a>Propriedades

> [!IMPORTANT]
> O uso específico de `$filter` e o parâmetro de consulta `$search` é suportado somente quando se usa o cabeçalho **ConsistencyLevel** definido como `eventual` e `$count`. Para obter mais informações, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).

| Propriedade       | Tipo    | Descrição |
|:---------------|:--------|:------------|
| aboutMe | String | Um campo de entrada de texto em forma livre para o usuário se descrever. <br><br>Retornado apenas em `$select`. |
| accountEnabled | Booliano | `true` se a conta estiver habilitada. Caso contrário, `false`. Essa propriedade é obrigatória quando um usuário é criado.<br><br>Suporte `$filter` (`eq`, `ne`, `NOT` e `in`). |
| ageGroup | [ageGroup](#agegroup-values) | Define a faixa etária do usuário. Valores permitidos: `null`, `minor`, `notAdult` e `adult`. Confira as [definições de propriedades da faixa etária legal](#legal-age-group-property-definitions) para obter mais informações. <br><br>Suporte `$filter` (`eq`, `ne`, `NOT` e `in`). |
| assignedLicenses | Coleção [assignedLicense](assignedlicense.md) | As licenças atribuídas ao usuário, incluindo licenças herdadas (baseadas em grupo). <br><br>Não anulável. Suporte para `$filter` (`eq` e `NOT`). |
| assignedPlans | Coleção [assignedPlan](assignedplan.md) | Os planos que são atribuídos ao usuário. Somente leitura. Não anulável.<br><br>Suporte para `$filter` (`eq` e `NOT`). |
| birthday | DateTimeOffset | O aniversário do usuário. O tipo de carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é `2014-01-01T00:00:00Z` <br><br>Retornado apenas em `$select`. |
| businessPhones | Coleção de cadeias de caracteres | Números de telefone para o usuário. Somente um número pode ser definido para essa propriedade.<br><br>Somente leitura para usuários sincronizados do diretório local. Suporte para `$filter` (`eq` e `NOT`).|
| city | Cadeia de caracteres | A cidade em que o usuário está localizado. O comprimento máximo é de 128 caracteres. <br><br>Suporta `$filter` (`eq`, `ne`, `NOT`, `ge`, `le`, `in`, `startsWith`). |
| companyName | String | O nome da empresa em que o usuário está associado. Essa propriedade pode ser útil para descrever a empresa de onde procede um usuário externo. O comprimento máximo do nome da empresa é 64 caracteres.<br><br>Suporta `$filter` (`eq`, `ne`, `NOT`, `ge`, `le`, `in`, `startsWith`).|
| consentProvidedForMinor | [consentProvidedForMinor](#consentprovidedforminor-values) | Define se o consentimento foi obtido para menores. Valores permitidos: `null`, `granted`, `denied` e `notRequired`. Confira as [definições de propriedades da faixa etária legal](#legal-age-group-property-definitions) para obter mais informações. <br><br>Suporte `$filter` (`eq`, `ne`, `NOT` e `in`).|
| country | Cadeia de caracteres | O país/região em que o usuário está localizado; por exemplo, `US` ou `UK`. O comprimento máximo é de 128 caracteres. <br><br>Suporta `$filter` (`eq`, `ne`, `NOT`, `ge`, `le`, `in`, `startsWith`). |
| createdDateTime | DateTimeOffset | A data e hora que o usuário foi criado. Não é possível modificar o valor e ele é preenchido automaticamente quando a entidade é criada. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. A propriedade é anulável. Um valor nulo indica que uma hora de criação exata não pode ser determinada pelo usuário. Somente leitura. <br><br>Suporta `$filter` (`eq`, `ne`, `NOT` , `ge`, `le` e operadores `in` ). |
| creationType | String | Indica se a conta do usuário foi criada por meio de um dos seguintes métodos: <br/> <ul><li>Como uma conta corporativa ou de estudante (`null`). <li>Como uma conta externa (`Invitation`). <li>Como uma conta local para um locatário do Azure Active Directory B2C (`LocalAccount`). <li>Por meio da inscrição de autoatendimento feita por um usuário interno usando a verificação por email (`EmailVerified`). <li>Por meio da inscrição de autoatendimento feita por um usuário externo que se inscreveu usando um link que faz parte de um fluxo do usuário (`SelfServiceSignUp`). </ul> <br>Somente leitura.<br>Suporte `$filter` (`eq`, `ne`, `NOT` e `in`). |
| deletedDateTime | DateTimeOffset | A data e hora que o usuário foi excluído. <br><br>Suporta `$filter` (`eq`, `ne`, `NOT`, `ge`, `le`, e `in`). |
| departamento | String | O nome do departamento no qual o usuário trabalha. O comprimento máximo é de 64 caracteres.<br><br>Suporta `$filter` (`eq`, `ne`, `NOT` , `ge`, `le`e operadores `in` ). |
| displayName | String | O nome exibido no catálogo de endereços para o usuário. Geralmente é a combinação do nome do usuário, inicial do meio e sobrenome. Esta propriedade é necessária quando um usuário é criado e não pode ser limpa durante as atualizações. O comprimento máximo é de 256 caracteres.<br><br>Suporta `$filter` (`eq`, `ne`, `NOT` , `ge`, `le`, `in`, `startsWith`), `$orderBy`e `$search`.|
| employeeHireDate | DateTimeOffset | A data e a hora em que o usuário foi contratado ou começará a trabalhar em caso de futura contratação. <br><br>Suporta `$filter` (`eq`, `ne`, `NOT` , `ge`, `le`, `in`).|
| employeeId | String | O identificador de funcionário atribuído ao usuário pela organização. <br><br>Suporta `$filter` (`eq`, `ne`, `NOT` , `ge`, `le`, `in`, `startsWith`).|
|employeeOrgData|[employeeOrgData](employeeorgdata.md) |Representa os dados da organização (por exemplo, divisão e costCenter) associados a um usuário. <br><br>Suporta `$filter` (`eq`, `ne`, `NOT` , `ge`, `le`, `in`).|
| employeeType | String | Captura o tipo de trabalhador corporativo. Por exemplo, `Employee`, `Contractor`, `Consultant` ou `Vendor`. Suporta `$filter` (`eq`, `ne`, `NOT` , `ge`, `le`, `in`, `startsWith`).|
| externalUserState | String | Para um usuário externo convidado para o locatário usando a [API de convite](../api/invitation-post.md), essa propriedade representa o status do convite do usuário convidado. Para usuários convidados, o estado pode ser `PendingAcceptance` ou `Accepted` ou `null` para todos os outros usuários. <br><br>Suporta `$filter` (`eq`, `ne`, `NOT` , `in`). |
| externalUserStateChangeDateTime | String | Mostra o carimbo de hora da alteração mais recente da propriedade externalUserState. <br><br>Suporta `$filter` (`eq`, `ne`, `NOT` , `in`). |
| FaxNumber | String | O número de fax do usuário. <br><br>Suporta `$filter` (`eq`, `ne`, `NOT` , `ge`, `le`, `in`, `startsWith`). |
| givenName | String | O nome fornecido (nome) do usuário. O comprimento máximo é de 64 caracteres. Suporta `$filter` (`eq`, `ne`, `NOT` , `ge`, `le`, `in`, `startsWith`).|
| hireDate | DateTimeOffset | A data de contratação do usuário. O tipo de carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é `2014-01-01T00:00:00Z` <br><br> Retornado apenas em `$select`. <br> **Observação:** essa propriedade é específica do SharePoint Online. É recomendável usar a propriedade **employeeHireDate** nativa para definir e atualizar valores de data de contratação usando as APIs do Microsoft Graph. |
| id | String | O identificador exclusivo do usuário. Deve ser tratado como um identificador opaco. Herdado de [directoryObject](directoryobject.md). Não anulável. Somente leitura. <br><br>Suporta `$filter` (`eq`, `ne`, `NOT`, `in`). |
| Identidades | Coleção [objectIdentity](objectIdentity.md) | Representa as identidades que podem ser usadas para entrar nesta conta de usuário. Uma identidade pode ser fornecida pela Microsoft (também conhecida como conta local), por organizações ou por provedores de identidade social, como o Facebook, Google e Microsoft, e está vinculada a uma conta de usuário. Pode conter vários itens com o mesmo valor **signInType**. <br><br>Suporta `$filter` (`eq`) apenas quando o **signInType** não é `userPrincipalName`. |
| imAddresses | Coleção de cadeias de caracteres | Os endereços do Protocolo de Início de Sessão (SIP) de VoIP (Voice over IP) da mensagem instantânea para o usuário. Somente leitura. Dá suporte a `$filter` (`eq`, `NOT`, `ge`, `le`, `startsWith`).|
| infoCatalogs | Conjunto de cadeias de caracteres | Identifica os segmentos de informações atribuídos ao usuário. Dá suporte a `$filter` (`eq`, `NOT`, `ge`, `le`, `startsWith`). |
| interests | Coleção de cadeias de caracteres | Uma lista para o usuário descrever os interesses dele. <br><br>Retornado apenas em `$select`. |
| isResourceAccount | Boolean | Não use – reservado para uso futuro. |
| jobTitle | String | O cargo do usuário. O comprimento máximo é de 128 caracteres. <br><br>Suporta `$filter` (`eq`, `ne`, `NOT` , `ge`, `le`, `in`, `startsWith`).|
| lastPasswordChangeDateTime | DateTimeOffset | A hora em que esse usuário do Azure AD alterou a senha pela última vez ou quando a senha foi criada, seja qual for a data em que a ação mais recente foi executada. O tipo de carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.<br><br>Retornado apenas em `$select`.  |
| legalAgeGroupClassification | [legalAgeGroupClassification](#legalagegroupclassification-values) | Usado por aplicativos empresariais para determinar a faixa etária legal do usuário. Essa propriedade é somente leitura e calculada com base nas propriedades **ageGroup** e **consentProvidedForMinor**. Valores permitidos: `null`, `minorWithOutParentalConsent`, `minorWithParentalConsent`, `minorNoParentalConsentRequired`, `notAdult` e `adult`. Confira as [definições de propriedades da faixa etária legal](#legal-age-group-property-definitions) para obter mais informações. <br><br>Retornado apenas em `$select`. |
| licenseAssignmentStates | Coleção [licenseAssignmentState](licenseassignmentstate.md) | Estado das atribuições de licença para este usuário. Somente leitura.<br><br>Retornado apenas em `$select`. |
| email | String | O endereço SMTP do usuário, por exemplo, `admin@contoso.com`. As alterações feitas nessa propriedade também atualizarão a coleção **proxyAddresses** do usuário para incluir o valor como um endereço SMTP. Para contas do Azure AD B2C, esta propriedade só pode ser atualizada até dez vezes com endereços SMTP exclusivos. Esta propriedade não pode conter caracteres de destaque. <br><br> Suporta `$filter` (`eq`, `ne`, `NOT`, `ge`, `le`, `in`, `startsWith`, `endsWith`). |
| mailboxSettings | [mailboxSettings](mailboxsettings.md) | Configurações da caixa de correio principal do usuário conectado. Você pode [obter](../api/user-get-mailboxsettings.md) ou [atualizar](../api/user-update-mailboxsettings.md) as configurações de localidade, fuso horário ou de envio de respostas automáticas a mensagens de entrada.<br><br>Retornado apenas em `$select`. |
| mailNickname | String | O alias de email do usuário. Essa propriedade deve ser especificada quando um usuário é criado. O comprimento máximo é de 64 caracteres.<br><br>Suporta `$filter` (`eq`, `ne`, `NOT`, `ge`, `le`, `in`, `startsWith`). |
| mobilePhone | String | O número de celular principal do usuário. Somente leitura para usuários sincronizados do diretório local. <br><br> Suporta `$filter` (`eq`, `ne`, `NOT`, `ge`, `le`, `in`, `startsWith`).|
| mySite | String | A URL do site pessoal do usuário. <br><br>Retornado apenas em `$select`. |
| officeLocation | String | A localização do escritório no local de trabalho do usuário. O comprimento máximo é de 128 caracteres. <br><br>Suporta `$filter` (`eq`, `ne`, `NOT`, `ge`, `le`, `in`, `startsWith`). |
| onPremisesDistinguishedName | String | Contém `distinguished name` ou `DN` do Active Directory local. A propriedade somente é preenchida para os clientes que estejam sincronizando o seu diretório local com o Azure Active Directory pelo Azure AD Connect. Somente leitura.  |
| onPremisesDomainName | String | Contém o `domainFQDN` local, também chamado dnsDomainName sincronizado do diretório local. A propriedade só é populada para clientes que estão sincronizando seu diretório local para Azure Active Directory via Azure AD Connect. Somente leitura. |
| onPremisesExtensionAttributes | [onPremisesExtensionAttributes](onpremisesextensionattributes.md) | Contém extensionAttributes 1-15 para o usuário. Observe que os atributos de extensão individuais não são selecionáveis nem filtráveis. Para um usuário do `onPremisesSyncEnabled`, a fonte de autoridade desse conjunto de propriedades é o local e é somente leitura. Para um usuário somente na nuvem (onde `onPremisesSyncEnabled` é falso), essas propriedades podem ser definidas durante a criação ou atualização. Esses atributos de extensão também são conhecidos como atributos personalizados do Exchange 1-15. <br><br>Suporta `$filter` (`eq`, `NOT`, `ge`, `le`, `in`).  |
| onPremisesImmutableId | String | Essa propriedade é usada para associar uma conta de usuário do Active Directory local com seu objeto de usuário do Azure AD. Essa propriedade deverá ser especificada ao criar uma nova conta de usuário no Graph se você estiver usando um domínio federado para a propriedade `userPrincipalName` (UPN) do usuário. **OBSERVAÇÃO:** Os caracteres **$** e **\_** não podem ser usados ao especificar essa propriedade. <br><br>Suporta `$filter` (`eq`, `ne`, `NOT`, `ge`, `le`, `in`). |
| onPremisesLastSyncDateTime | DateTimeOffset | Indica a última vez em que o objeto foi sincronizado com o diretório local. Por exemplo: "2013-02-16T03:04:54Z". O tipo de carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura. <br><br>Suporta `$filter` (`eq`, `ne`, `NOT`, `ge`, `le`, `in`). |
| onPremisesProvisioningErrors | coleção [OnPremisesProvisioningError](onpremisesprovisioningerror.md) | Erros ao usar o produto de sincronização da Microsoft durante a configuração. <br> Suporta `$filter` (`eq`, `NOT`, `ge`, `le`).|
| onPremisesSamAccountName | String | Contém o `sAMAccountName` local sincronizado do diretório local. A propriedade somente é preenchida para os clientes que estejam sincronizando o diretório local com o Azure Active Directory pelo Azure AD Connect. Somente leitura.<br><br> Suporta `$filter` (`eq`, `ne`, `NOT`, `ge`, `le`, `in`, `startsWith`).|
| onPremisesSecurityIdentifier | String | Contém o identificador de segurança (SID) local do usuário que foi sincronizado do local com a nuvem. Somente leitura. |
| onPremisesSyncEnabled | Booliano | `true` se esse objeto está sincronizado de um diretório local; `false` se esse objeto foi originalmente sincronizado de um diretório local, mas não está mais sincronizado; `null` se esse objeto nunca foi sincronizado de um diretório local (padrão). Somente leitura. <br><br>Suporta `$filter` (`eq`, `ne`, `NOT`, `in`). |
| onPremisesUserPrincipalName | String | Contém o `userPrincipalName` local sincronizado do diretório local. A propriedade somente é preenchida para os clientes que estejam sincronizando o diretório local com o Azure Active Directory pelo Azure AD Connect. Somente leitura.<br><br>Suporta `$filter` (`eq`, `ne`, `NOT`, `ge`, `le`, `in`, `startsWith`). |
| otherMails | Coleção String | Uma lista de endereços de email adicional para o usuário; Por exemplo: `["bob@contoso.com", "Robert@fabrikam.com"]`.<br>NOTA: Esta propriedade não pode conter caracteres de destaque.<br><br>Suporta `$filter` (`eq`, `NOT`, `ge`, `le`, `in`, `startsWith`). |
| passwordPolicies | String | Especifica políticas de senha para o usuário. Esse valor é uma enumeração com um valor possível sendo`DisableStrongPassword`, que permite que senhas mais fracas do que a política padrão sejam especificadas. `DisablePasswordExpiration` também pode ser  especificado. Os dois podem ser especificados juntos. Por exemplo:`DisablePasswordExpiration, DisableStrongPassword`. Para obter mais informações sobre as políticas de senha padrão, consulte as [políticas de senha do Azure AD](/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts). <br><br>Suporta `$filter` (`ne`, `NOT`).|
| passwordProfile | [passwordProfile](passwordprofile.md) | Especifica o perfil de senha do usuário. O perfil contém a senha do usuário. Essa propriedade é obrigatória quando um usuário é criado. A senha no perfil deve atender a requisitos mínimos, conforme especificado pela propriedade **passwordPolicies**. Por padrão, é obrigatória uma senha forte. **OBSERVAÇÃO:** Para locatários B2C do Azure, a propriedade **forceChangePasswordNextSignIn** deve ser definida como `false` e, em vez disso, usar políticas personalizadas e fluxos de usuário para forçar a redefinição de senha no primeiro logon. Confira [Forçar a redefinição de senha no primeiro logon](https://github.com/azure-ad-b2c/samples/tree/master/policies/force-password-reset-first-logon). <br><br>Suporta `$filter` (`eq`, `ne`, `NOT`, `in`).|
| pastProjects | Coleção de cadeias de caracteres | Uma lista para o usuário enumerar seus projetos anteriores. <br><br>Retornado apenas em `$select`. |
| postalCode | String | O código postal do endereço postal do usuário. O código postal é específico para o país/região do usuário. Nos Estados Unidos da América, este atributo contém o Código postal. O comprimento máximo é de 40 caracteres.<br><br>Suporta `$filter` (`eq`, `ne`, `NOT`, `ge`, `le`, `in`, `startsWith`).|
| preferredDataLocation | String | O local de dados preferido para o usuário. Para saber mais, confira [OneDrive Online Multi-Geo](/sharepoint/dev/solution-guidance/multigeo-introduction).|
| preferredLanguage | Cadeia de caracteres | O idioma preferencial do usuário. Deve seguir o Código ISO 639-1; por exemplo, `en-US`.<br><br>Suporta `$filter` (`eq`, `ne`, `NOT`, `ge`, `le`, `in`, `startsWith`). |
| preferredName | String | O nome preferencial do usuário. <br><br>Retornado apenas em `$select`. |
| provisionedPlans | coleção [provisionedPlan](provisionedplan.md) | Os planos que estão provisionados para o usuário. Somente leitura. Não anulável. Dá suporte a `$filter` (`eq`, `NOT`, `ge`, `le`).|
| proxyAddresses | Coleção de cadeias de caracteres | Por exemplo: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]`. Para contas do Azure AD B2C, essa propriedade tem um limite de dez endereços exclusivos. Somente leitura, Não anulável. <br><br>Suporta `$filter` (`eq`, `NOT`, `ge`, `le`, `startsWith`). |
| refreshTokensValidFromDateTime | DateTimeOffset | Os tokens de atualização ou de sessão (cookies de sessão) emitidos antes dessa hora são inválidos e os aplicativos recebem um erro ao usar um token de atualização ou de sessão inválido para adquirir um token de acesso delegado (para acessar APIs como o Microsoft Graph).  Se isso acontecer, o aplicativo precisará adquirir um novo token de atualização, fazendo uma solicitação ao ponto de extremidade de autorização. Somente leitura. Use [invalidateAllRefreshTokens](../api/user-invalidateallrefreshtokens.md) para redefinir.|
| responsibilities | Coleção de cadeias de caracteres | Uma lista para o usuário enumerar suas responsabilidades. <br><br>Retornado apenas em `$select`. |
| schools | Coleção de cadeias de caracteres | Uma lista para o usuário enumerar as escolas que frequentou. <br><br>Retornado apenas em `$select`. |
| showInAddressList | Booliano | `true` se a lista de endereços global do Outlook deve conter o usuário, caso contrário `false`. Se não estiver configurado, isso será tratado como `true`. Para os usuários convidados por meio do Gerenciador de convites, essa propriedade será definida como `false`. <br><br>Suporta `$filter` (`eq`, `ne`, `NOT`, `in`). |
| signInSessionsValidFromDateTime | DateTimeOffset | Os tokens de atualização ou de sessão (cookies de sessão) emitidos antes dessa hora são inválidos e os aplicativos recebem um erro ao usar um token de atualização ou de sessão inválido para adquirir um token de acesso delegado (para acessar APIs como o Microsoft Graph).  Se isso acontecer, o aplicativo precisará adquirir um novo token de atualização, fazendo uma solicitação ao ponto de extremidade de autorização. Somente leitura. Use [revokeSignInSessions](../api/user-revokesigninsessions.md) para redefinir.|
| skills | Coleção de cadeias de caracteres | Uma lista para o usuário enumerar suas qualificações. <br><br>Retornado apenas em `$select`. |
| signInActivity | [signInActivity](signinactivity.md) | Obter a última data de login e solicitar a ID de login para um determinado usuário. Somente leitura.<br><br>Retornado apenas em `$select`. Suporta `$filter` (`eq`, `ne`, `NOT`, `ge`, `le`) *mas*, não com quaisquer outras propriedades filtráveis. **Observação:** os detalhes dessa propriedade exigem uma licença do Azure Active Directory Premium P1/P2 e a permissão **AuditLog.Read.All**.<br><br>**Observação**: há um [problema conhecido](/graph/known-issues#azure-ad-activity-reports) ao recuperar esta propriedade.|
| estado | String | O estado ou município no endereço do usuário. O comprimento máximo é de 128 caracteres. <br><br>Suporta `$filter` (`eq`, `ne`, `NOT`, `ge`, `le`, `in`, `startsWith`). |
| streetAddress | String | O endereço do local de trabalho do usuário. O comprimento máximo é de 1024 caracteres. <br><br>Suporta `$filter` (`eq`, `ne`, `NOT`, `ge`, `le`, `in`, `startsWith`).|
| surname | String | O sobrenome do usuário (nome de família ou sobrenome). O comprimento máximo é de 64 caracteres. <br><br>Suporta `$filter` (`eq`, `ne`, `NOT`, `ge`, `le`, `in`, `startsWith`). |
| usageLocation | String | Um código de duas letras (padrão ISO 3166). Obrigatório para os usuários que receberão licenças devido à exigência legal de verificar a disponibilidade de serviços nos países/regiões. Por exemplo: `US`, `JP`, e `GB`. Não anulável.<br><br>Suporta `$filter` (`eq`, `ne`, `NOT`, `ge`, `le`, `in`, `startsWith`).|
| userPrincipalName | Cadeia de caracteres | O nome UPN do usuário. O nome UPN é um nome de logon para o usuário ao estilo da Internet com base na RFC 822 padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email do usuário. O formato geral é alias@domain, em que o domínio deve estar presente na coleção de domínios verificados do locatário. Essa propriedade é obrigatória quando um usuário é criado. Os domínios verificados para o locatário podem ser acessados pela propriedade **verifiedDomains** da [organização](organization.md).<br>NOTA: Esta propriedade não pode conter caracteres de destaque. <br><br>Suporta `$filter` (`eq`, `ne`, `NOT`, `ge`, `le`, `in`, `startsWith`, `endsWith`) e `$orderBy`.
| userType | String | Um valor de String que pode ser usado para classificar tipos de usuário em seu diretório, como `Member` e `Guest`. <br><br>Suporta `$filter` (`eq`, `ne`, `NOT`, `in`,). **OBSERVAÇÃO:** Para obter mais informações sobre as permissões para usuários membros e convidados, consulte [Quais são as permissões padrão de usuário em Azure Active Directory?](/azure/active-directory/fundamentals/users-default-permissions#member-and-guest-users) |

### <a name="legal-age-group-property-definitions"></a>Definições de propriedade da faixa etária legal

Esta seção explica como as três propriedades de grupo idade (**legalAgeGroupClassification**, **ageGroup** e **consentProvidedForMinor**) são usadas por administradores do Azure Active Directory e desenvolvedores de aplicativos empresariais para atender às regulamentações relacionadas à idade:
- A propriedade legal **AgeGroupClassification** é somente leitura. É usado por desenvolvedores de aplicativos corporativos para garantir o tratamento correto de um usuário com base em sua faixa etária legal. É calculado com base nas propriedades **ageGroup** e **consentProvidedForMinor** do usuário.
- **ageGroup** e **consentProvidedForMinor** são propriedades opcionais usadas pelos administradores do Azure Active Directory para ajudar a garantir que o uso de uma conta seja tratado corretamente com base nas regras regulatórias relacionadas à idade que regem o país ou região do usuário.

Por exemplo: Cameron é o administrador de um diretório em uma escola de ensino fundamental em Holyport, no Reino Unido. No início do ano letivo ele usa a documentação de admissão para obter o consentimento dos pais dos menores baseado nos regulamentos relacionadas com a idade no Reino Unido. O consentimento obtido do pai permite que a conta do menor seja usado pela escola de Holyport e os aplicativos da Microsoft. Cameron cria todas as contas e define o ageGroup para "menor" e consentProvidedForMinor para "concedido". Os aplicativos usados por seus alunos poderão, então suprimir recursos que não são adequados para menores.
<!-- Note that the following 3 sub-sections are only documented like enums for a consistent user experience.
For some reason they are not defined as enums in the CSDL.
Hence the type of the corresponding 3 properties remain as String type in the Properties table.
-->

#### <a name="legalagegroupclassification-values"></a>legalAgeGroupClassification values

| Member    | Descrição|
|:---------------|:----------|
|null|Valor padrão, nenhum **ageGroup** foi definido para o usuário.|
|minorWithoutParentalConsent |(Reservado para uso futuro)|
|minorWithParentalConsent| O usuário é considerado menor baseado nos regulamentos relacionados com a idade de seu país ou região, e o administrador da conta obteve o consentimento apropriado dos pais ou responsável.|
|adult|O usuário é considerado adulto baseado nos regulamentos relacionadas com a idade do seu país ou região.|
|notAdult|O usuário é de um país ou região com regulamentos adicionais relacionados à idade (por exemplo, Estados Unidos, Reino Unido, União Europeia ou Coreia do Sul) e a idade do usuário está entre menor e adulto (como estipulado com base no país ou região). Em geral, isso significa que adolescentes são considerados como `notAdult` nos países/regiões regulamentados.|
|minorNoParentalConsentRequired|O usuário é menor de idade, mas é de um país ou região que não tem com regulamentações relacionadas com a idade.|

#### <a name="agegroup-values"></a>ageGroup values

| Member    | Descrição|
|:---------------|:--------|
|null|Valor padrão, nenhum **ageGroup** foi definido para o usuário.|
|menor|O usuário é considerado um menor.|
|notAdult|O usuário é de um país que possui regulamentos legais (como Estados Unidos, Reino Unido, União Europeia ou Coreia do Sul) e a idade do usuário é superior ao limite superior de idade infantil (conforme o país) e inferior ao limite inferior de adulto idade (conforme estipulado com base no país ou região). Basicamente, os adolescentes são considerados como `notAdult` nos países/regiões regulamentados.|
|adult|O usuário deve ser tratado como um adulto.|

#### <a name="consentprovidedforminor-values"></a>consentProvidedForMinor values

| Member    | Descrição|
|:---------------|:----------|
|null|Valor padrão, nenhum **consentimentoProvidedForMinor** foi definido para o usuário.|
|concedido|O consentimento foi obtido para o usuário ter uma conta.|
|denied|O consentimento não foi obtido para o usuário ter uma conta.|
|notRequired|O usuário é de um local que não exige consentimento.|

## <a name="relationships"></a>Relações

| Relação | Tipo |Descrição|
|:---------------|:--------|:----------|
|agreementAcceptances|Coleção [agreementAcceptance](agreementacceptance.md)| Status de aceitação dos termos de uso do usuário. Somente leitura. Anulável.|
|appRoleAssignments|[appRoleAssignment](approleassignment.md) collection|Representa as funções de aplicativo que um usuário recebeu para um aplicativo. Dá suporte a `$expand`. |
|calendar|[calendar](calendar.md)|O calendário principal do usuário. Somente leitura.|
|calendarGroups|Coleção [CalendarGroup](calendargroup.md)|Os grupos de calendários do usuário. Somente leitura. Anulável.|
|calendarView|Coleção [event](event.md)|O modo de exibição do calendário. Somente leitura. Anulável.|
|calendars|Coleção [calendar](calendar.md)|Os calendários do usuário. Somente leitura. Anulável.|
|contactFolders|Coleção [ContactFolder](contactfolder.md)|As pastas de contatos do usuário. Somente leitura. Anulável.|
|contacts|Coleção [Contact](contact.md)|Os contatos do usuário. Somente leitura. Anulável.|
|createdObjects|Coleção [directoryObject](directoryobject.md)|Objetos directory que foram criados pelo usuário. Somente leitura. Anulável.|
|directReports|Coleção [directoryObject](directoryobject.md)|Os usuários e contatos subordinados ao usuário. (Os usuários e contatos cuja propriedade de gerenciamento está definida para esse usuário.) Somente leitura. Anulável. Dá suporte a `$expand`. |
|Unidade|[drive](drive.md)|O OneDrive do usuário. Somente leitura.|
|unidades|Coleção [drive](drive.md)| Uma coleção de unidades disponíveis para este usuário. Somente leitura. |
|eventos|Coleção [event](event.md)|Os eventos do usuário. O padrão é mostrar eventos no Calendário Padrão. Somente leitura. Anulável.|
|extensions|Coleção [extension](extension.md)|A coleção de extensões abertas definidas para o usuário. Anulável.|
|inferenceClassification|[inferenceClassification](inferenceclassification.md)| Classificação de relevância das mensagens do usuário com base em designações explícitas que substituem a relevância ou importância deduzida. |
|insights|[itemInsights](iteminsights.md) | Somente leitura. Anulável.|
|joinedGroups|Coleção [group](group.md)| Somente leitura. Anulável.|
|mailFolders|Coleção [mailFolder](mailfolder.md)| As pastas de email do usuário. Somente leitura. Anulável.|
|manager|[directoryObject](directoryobject.md)|O usuário ou contato que é o gerente deste usuário. Somente leitura. (Métodos HTTP: GET, PUT, DELETE.). Dá suporte a `$expand`.|
|memberOf|Coleção [directoryObject](directoryobject.md)|Os grupos, funções de diretório e unidades administrativas dos quais o usuário é membro. Somente leitura. Anulável. Dá suporte a `$expand`.  |
|joinedTeams|Coleção [team](team.md)|O Microsoft Teams do qual o usuário é membro. Somente leitura. Anulável.|
|messages|Coleção [message](message.md)|As mensagens em uma caixa de correio ou pasta. Somente leitura. Anulável.|
|onenote|[onenote](onenote.md)| Somente leitura.|
|outlook|[outlookUser](outlookuser.md)| Os serviços seletivos do Outlook disponíveis para o usuário. Somente leitura. Anulável.|
|ownedDevices|Coleção [directoryObject](directoryobject.md)|Dispositivos que pertencem ao usuário. Somente leitura. Anulável. Dá suporte a `$expand`.|
|ownedObjects|Coleção [directoryObject](directoryobject.md)|Objetos de diretório que pertencem ao usuário. Somente leitura. Anulável. Dá suporte a `$expand`.|
|pendingAccessReviewInstances|[accessReviewInstance](accessreviewinstance.md) | Propriedade de navegação para obter a lista de análises de acesso com aprovação pendente do revisor. |
|people|Coleção [person](person.md)| Somente leitura. As pessoas mais relevantes para o usuário. A coleção é ordenada por relevância para o usuário, que é determinado pela comunicação e colaboração e pelas relações comerciais do usuário. Uma pessoa é uma agregação de informações provenientes de emails, contatos e redes sociais.|
|photo|[profilePhoto](profilephoto.md)| A foto de perfil do usuário. Somente leitura.|
|photos|coleção de [fotos](photo.md)| Somente leitura. Anulável.|
|planner|[plannerUser](planneruser.md)| Serviços de Planejador seletivo disponíveis para o usuário. Somente leitura. Anulável. |
|perfil |[perfil](profile.md) | Representa propriedades que são descritivas de um usuário em um locatário. |
|registeredDevices|Coleção [directoryObject](directoryobject.md)|Dispositivos que estão registrados para o usuário. Somente leitura. Anulável. Suporta `$expand`.|
|scopedRoleMemberOf|Coleção [scopedRoleMembership](scopedrolemembership.md)| As associações de unidade administrativa de função com escopo deste usuário. Somente leitura. Anulável.|
|settings|[userSettings](usersettings.md) | Somente leitura. Anulável.|
|trabalho em equipe|[userTeamwork](userteamwork.md)| Um contêiner dos recursos do Microsoft Teams disponíveis para o usuário. Somente leitura. Anulável.|
|todo|[todo](todo.md)|Representa os serviços To Do disponíveis para um usuário. |
|transitiveReports|Coleção [directoryObject](directoryobject.md) | Os relatórios transitivos para um usuário. Somente leitura.|
|usageRight|Coleção [usageRight](usageright.md)|Representa os direitos de uso concedidos a um usuário. |

### <a name="user-preferences-for-languages-and-regional-formats"></a>Preferências do usuário para idiomas e formatos regionais.
O recurso do **usuário** contém uma propriedade [mailboxSettings](../resources/mailboxsettings.md), que inclui o idioma, a formatação de data e hora, o fuso horário padrão e outras configurações preferidas do usuário especificamente para a caixa de correio principal do Exchange. Essas preferências são direcionadas para os clientes de email e só estarão disponíveis se o usuário tiver uma caixa de correio provisionada. Você pode optar por usar **mailboxSettings** se o seu cenário se concentrar apenas em emails, calendários, contatos ou tarefas pendentes do Outlook.

Além de **mailboxSettings**, **usuário** inclui uma relação por meio de [userSettings](../resources/usersettings.md) para [regionalAndLanguageSettings](../resources/regionalandlanguagesettings.md), o superconjunto de preferências de formatação regional e de idioma, que pode ser usado por qualquer aplicativo para oferecer ao usuário uma experiência de formatação regional e de idioma melhor. Use **userSettings** para uma experiência consistente entre aplicativos que tocam no perfil de usuário do Azure AD para refletir as mesmas preferências do usuário.

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
    "profile",
    "registeredDevices"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}-->

```json
{
  "aboutMe": "String",
  "accountEnabled": true,
  "ageGroup": "String",
  "assignedLicenses": [{"@odata.type": "microsoft.graph.assignedLicense"}],
  "assignedPlans": [{"@odata.type": "microsoft.graph.assignedPlan"}],
  "birthday": "String (timestamp)",
  "businessPhones": ["String"],
  "city": "String",
  "companyName": "String",
  "consentProvidedForMinor": "String",
  "country": "String",
  "createdDateTime": "2019-02-07T21:53:13.067Z",
  "creationType": "String",
  "deletedDateTime": "String (timestamp)",
  "department": "String",
  "displayName": "String",
  "employeeHireDate": "2020-01-01T00:00:00Z",
  "employeeId": "String",
  "employeeOrgData": {"@odata.type": "microsoft.graph.employeeOrgData"},
  "employeeType": "String",
  "externalUserState": "PendingAcceptance",
  "externalUserStateChangeDateTime": "2018-11-12T01:13:13Z",
  "faxNumber": "String",
  "givenName": "String",
  "hireDate": "String (timestamp)",
  "id": "String (identifier)",
  "identities": [{"@odata.type": "microsoft.graph.objectIdentity"}],
  "interests": ["String"],
  "isResourceAccount": false,
  "jobTitle": "String",
  "legalAgeGroupClassification": "String",
  "licenseAssignmentStates": [{"@odata.type": "microsoft.graph.licenseAssignmentState"}],
  "mail": "String",
  "mailboxSettings": {"@odata.type": "microsoft.graph.mailboxSettings"},
  "mailNickname": "String",
  "mobilePhone": "String",
  "mySite": "String",
  "officeLocation": "String",
  "onPremisesDistinguishedName": "String",
  "onPremisesDomainName": "String",
  "onPremisesExtensionAttributes": {"@odata.type": "microsoft.graph.onPremisesExtensionAttributes"},
  "onPremisesImmutableId": "String",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSamAccountName": "String",
  "onPremisesSecurityIdentifier": "String",
  "onPremisesSyncEnabled": true,
  "onPremisesUserPrincipalName": "String",
  "otherMails": ["String"],
  "passwordPolicies": "String",
  "passwordProfile": {"@odata.type": "microsoft.graph.passwordProfile"},
  "pastProjects": ["String"],
  "postalCode": "String",
  "preferredDataLocation": "String",
  "preferredLanguage": "String",
  "preferredName": "String",
  "provisionedPlans": [{"@odata.type": "microsoft.graph.provisionedPlan"}],
  "proxyAddresses": ["String"],
  "refreshTokensValidFromDateTime": "2019-02-07T21:53:13.084Z",
  "responsibilities": ["String"],
  "schools": ["String"],
  "showInAddressList": true,
  "signInSessionsValidFromDateTime": "2019-02-07T21:53:13.084Z",
  "skills": ["String"],
  "state": "String",
  "streetAddress": "String",
  "surname": "String",
  "usageLocation": "String",
  "userPrincipalName": "String",
  "userType": "String",
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
  "insights": {"@odata.type": "microsoft.graph.itemInsights"},
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
  "profile": {"@odata.type": "microsoft.graph.profile"},
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
