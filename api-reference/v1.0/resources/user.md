---
title: Tipo de recurso de usuário
description: Representa uma conta de usuário do Azure AD. Herda de directoryObject.
author: jpettere
ms.localizationpriority: high
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: a21cfb34d99142f88eb8651e6df241677844765c
ms.sourcegitcommit: dab085b74666e190974a35e6a124d3ff1645fa25
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/05/2022
ms.locfileid: "64646533"
---
# <a name="user-resource-type"></a>Tipo de recurso de usuário

Namespace: microsoft.graph

Representa uma conta de usuário do Azure Active Directory (Azure AD). Esse recurso é um tipo aberto que permite que outras propriedades sejam passadas. Herda de [directoryObject](directoryobject.md).

Esse recurso permite:

- Adicionar seus próprios dados às propriedades personalizadas como [extensions](/graph/extensibility-overview).
- Assinar as [notificações de alteração](/graph/webhooks).
- Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/user-delta.md).

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:-|:-|:-|
| [Listar usuários](../api/user-list.md) | Coleção [user](user.md) | Recuperar uma lista de objetos user. |
| [Criar usuário](../api/user-post-users.md) | [user](user.md) | Criar um novo objeto user. |
| [Obter usuário](../api/user-get.md) | [user](user.md) | Ler propriedades e relações do objeto user. |
| [Atualizar usuário](../api/user-update.md) | [user](user.md) | Atualizar o objeto user. |
| [Excluir usuário](../api/user-delete.md) | Nenhum | Excluir o objeto user. |
| [Obter delta](../api/user-delta.md) | Coleção [usuário](user.md) | Obter as alterações incrementais para usuários. |
| [changePassword](../api/user-changepassword.md) | Nenhum | Atualize sua senha. |
| **Atribuição de funções do aplicativo** |  |  |
| [List appRoleAssignments](../api/user-list-approleassignments.md) | [appRoleAssignment](approleassignment.md) collection | Obter os aplicativos e funções do aplicativo atribuídos a esse usuário. |
| [Adicionar uma atribuição de função do aplicativo](../api/user-post-approleassignments.md) | [appRoleAssignment](approleassignment.md) | Atribuir uma função do aplicativo a esse usuário. |
| [Remover uma atribuição de função do aplicativo](../api/user-delete-approleassignments.md) | Nenhum | Remover uma atribuição de função do aplicativo desse usuário. |
| **Calendar** |  |  |
| [Criar calendário](../api/user-post-calendars.md) | [Calendar](calendar.md) | Criar um novo Calendar postando na coleção calendars. |
| [Criar calendarGroup](../api/user-post-calendargroups.md) | [CalendarGroup](calendargroup.md) | Criar um novo CalendarGroup postando na coleção calendarGroups. |
| [Criar evento](../api/user-post-events.md) | [event](event.md) | Criar um novo Event postando na coleção de eventos. |
| [findMeetingTimes](../api/user-findmeetingtimes.md) | [meetingTimeSuggestionsResult](meetingtimesuggestionsresult.md) | Encontrar o tempo e locais para reunião com base na disponibilidade dos participantes, localização ou restrições de tempo. |
| [getSchedule](../api/calendar-getschedule.md) | [scheduleInformation](scheduleinformation.md) | Adquira as informações de disponibilidade para um conjunto de usuários, listas de distribuição ou recursos (salas e equipamentos) para um período de tempo especificado. |
| [Listar calendários](../api/user-list-calendars.md) | Coleção [calendar](calendar.md) | Obter uma coleção de objetos Calendar. |
| [Listar calendarGroups](../api/user-list-calendargroups.md) | Coleção de [CalendarGroup](calendargroup.md) | Obter uma coleção de objetos CalendarGroup. |
| [Listar calendarView](../api/user-list-calendarview.md) | Coleção [event](event.md) | Obtenha uma coleção do objeto Event. |
| [Listar eventos](../api/user-list-events.md) | Coleção [event](event.md) | Obter uma lista de objetos event na caixa de correio do usuário. A lista contém reuniões de instância única e reuniões mestres em série. |
| [reminderView](../api/user-reminderview.md) | Coleção [Reminder](reminder.md) | Retorna uma lista de lembretes de calendário nas horas de início e término especificadas. |
| **Contatos** |  |  |
| [Criar contato](../api/user-post-contacts.md) | [contato](contact.md) | Criar um novo Contact postando na coleção contacts. |
| [Criar contactFolder](../api/user-post-contactfolders.md) | [pastadeContatos](contactfolder.md) | Criar uma nova ContactFolder postando na coleção contactFolders. |
| [Listar contatos](../api/user-list-contacts.md) | Coleção de[contato](contact.md) | Obter uma coleção de contatos da pasta Contatos padrão do usuário conectado. |
| [Listar contactFolders](../api/user-list-contactfolders.md) | Coleção de [pastadeContatos](contactfolder.md) | Obter a coleção de pastas de contatos na pasta Contatos padrão do usuário conectado. |
| **Objetos de diretório** |  |  |
| [assignLicense](../api/user-assignlicense.md) | [user](user.md) | Adicionar ou remover assinaturas para o usuário. Você também pode habilitar e desabilitar planos específicos associados a uma assinatura. |
| [checkMemberGroups](../api/directoryobject-checkmembergroups.md) | Coleção de cadeias de caracteres | Verifique se há uma associação em uma lista de grupos. A verificação é transitiva. |
| [checkMemberObjects](../api/directoryobject-checkmemberobjects.md) | Coleção de cadeias de caracteres | Verifique se há associação em uma lista de objetos de grupo, função de diretório ou unidade administrativa. A função é transitiva. |
| [exportPersonalData](../api/user-exportpersonaldata.md) | Nenhum | Envia uma solicitação de operação de política de dados, realizada por um administrador da empresa para exportar os dados de um usuário da organização. |
| [getByIds](../api/directoryobject-getbyids.md) | Coleção de cadeias de caracteres | Retorna os objetos de diretório especificados a partir de uma lista de ids. |
| [getMemberGroups](../api/directoryobject-getmembergroups.md) | Coleção de cadeias de caracteres | Retorne todos os grupos dos quais o usuário é membro. A verificação é transitiva. |
| [getMemberObjects](../api/directoryobject-getmemberobjects.md) | Coleção de cadeias de caracteres | Retorna todos os grupos e funções de diretório e unidades administrativas dos quais o usuário é membro. A verificação é transitiva. |
| [Listar createdObjects](../api/user-list-createdobjects.md) | Coleção [directoryObject](directoryobject.md) | Obter os objetos directory criados pelo usuário da propriedade de navegação createdObjects. |
| [Listar licenseDetails](../api/user-list-licensedetails.md) | Coleção [licenseDetails](licensedetails.md) | Obtenha uma coleção de objetos licenseDetails. |
| [Listar ownedDevices](../api/user-list-owneddevices.md) | Coleção [directoryObject](directoryobject.md) | Obter os dispositivos que pertencem ao usuário da propriedade de navegação ownedDevices. |
| [Listar ownedObjects](../api/user-list-ownedobjects.md) | Coleção [directoryObject](directoryobject.md) | Obter os objetos directory que pertencem ao usuário da propriedade de navegação ownedObjects. |
| [Listar registeredDevices](../api/user-list-registereddevices.md) | Coleção [directoryObject](directoryobject.md) | Obter os dispositivos que estão registrados para o usuário da propriedade de navegação registeredDevices. |
| [reprocessLicense](../api/user-reprocesslicenseassignment.md) | [user](user.md) | Reprocessar as atribuições de assinatura do usuário. |
| [revokeSignInSessions](../api/user-revokesigninsessions.md) | Nenhum | Revoga todos os tokens de sessão e de atualização do usuário emitidos para aplicativos, redefinindo a propriedade do usuário **signInSessionsValidFromDateTime** para data e a hora atuais. Força o usuário a entrar novamente nesses aplicativos. |
| [Listar grupos excluídos](../api/directory-deleteditems-list.md) | Coleção [directoryObject](directoryobject.md) | Recupere os grupos excluídos no locatário nos últimos 30 dias. |
| [Listar grupos excluídos pertencentes ao usuário](../api/directory-deleteditems-user-owned.md) | Coleção [directoryObject](directoryobject.md) | Recupere os grupos excluídos no locatário nos últimos 30 dias e que pertencem a um usuário. |
| [Obter grupo excluído](../api/directory-deleteditems-get.md) | Coleção [directoryObject](directoryobject.md) | Recupere um grupo excluído por ID. |
| [Restaurar grupo excluído](../api/directory-deleteditems-delete.md) | Coleção [directoryObject](directoryobject.md) | Restaure um grupo excluído no locatário nos últimos 30 dias. |
| [Excluir permanentemente um grupo](../api/directory-deleteditems-restore.md) | Coleção [directoryObject](directoryobject.md) | Exclua permanentemente um grupo excluído do locatário. |
| **Unidade** |  |  |
| [Obter unidade](../api/drive-get.md) | [unidade](drive.md) | Recuperar as propriedades e as relações de um recurso Drive. |
| [Filhos de lista](../api/driveitem-list-children.md) | [DriveItems](driveitem.md) | Retornar uma coleção de DriveItems no relacionamento filho de um DriveItem. |
| **Grupos** |  |  |
| [Listar joinedTeams](../api/user-list-joinedteams.md) | Coleção [team](team.md) | Obter as equipes do Microsoft Teams no qual o usuário é membro direto da propriedade de navegação joinedTeams. |
| [Listar memberOf](../api/user-list-memberof.md) | Coleção [directoryObject](directoryobject.md) | Obter os grupos e as funções de diretório dos quais o usuário é membro direto da propriedade de navegação memberOf. |
| [Listar memberOf transitivos](../api/user-list-transitivememberof.md) | Coleção [directoryObject](directoryobject.md) | Enumera os grupos e as funções de diretório dos quais o usuário é membro. Essa operação é transitiva e inclui os grupos dos quais o usuário é membro aninhado. |
| **Email** |  |  |
| [Create inferenceClassificationOverride](../api/inferenceclassification-post-overrides.md) | Criar uma substituição da Caixa de Entrada Destaques para um remetente identificado por um endereço SMTP. |  |
| [Criar MailFolder](../api/user-post-mailfolders.md) | [mailFolder](mailfolder.md) | Criar uma nova MailFolder postando na coleção mailFolders. |
| [Criar mensagem](../api/user-post-messages.md) | [message](message.md) | Criar uma nova Mensagem postando na coleção messages. |
| [Criar messageRule](../api/mailfolder-post-messagerules.md) | [messageRule](messagerule.md) | Crie um objeto messageRule especificando um conjunto de condições e ações. |
| [getMailTips](../api/user-getmailtips.md) | Coleção [mailTips](mailtips.md) | Retornar dicas de email de um ou mais destinatários conforme disponíveis para o usuário conectado. |
| [Listar mailFolders](../api/user-list-mailfolders.md) | Coleção [mailFolder](mailfolder.md) | Obter o conjunto de pastas de email sob a pasta raiz do usuário conectado. |
| [Listar mensagens](../api/user-list-messages.md) | Coleção [message](message.md) | Obter todas as mensagens na caixa de correio do usuário conectado. |
| [List overrides](../api/inferenceclassification-list-overrides.md) | Coleção [inferenceClassificationOverride](inferenceclassificationoverride.md) | Obtenha as substituições da Caixa de Entrada Destaques que um usuário configurou para sempre classificar as mensagens de determinados remetentes de maneiras específicas. |
| [Listar regras](../api/mailfolder-list-messagerules.md) | Coleção [messageRule](messagerule.md) | Obtenha todos os objetos messageRule definidos para a caixa de entrada do usuário. |
| [Enviar email](../api/user-sendmail.md) | Nenhum | Enviar a mensagem especificada no corpo da solicitação. |
| **Anotações** |  |  |
| [Criar bloco de anotações](../api/onenote-post-notebooks.md) | [bloco de anotações](notebook.md) | Crie um novo bloco de anotações do OneNote. |
| [Listar blocos de anotações](../api/onenote-list-notebooks.md) | Coleção [bloco de anotações](notebook.md) | Recuperar uma lista de objetos do bloco de anotações. |
| **Extensões abertas** |  |  |
| [Criar extensão aberta](../api/opentypeextension-post-opentypeextension.md) | [openTypeExtension](opentypeextension.md) | Crie uma extensão aberta e adicione propriedades personalizadas a uma instância nova ou existente de um recurso. |
| [Obter extensão aberta](../api/opentypeextension-get.md) | Coleção [openTypeExtension](opentypeextension.md) | Obtenha uma extensão aberta identificada pelo nome da extensão. |
| **Hierarquia da organização** |  |  |
| [Atribuir gerente](../api/user-post-manager.md) | [directoryObject](directoryobject.md) | Atribuir um usuário ou um contato organizacional como o gerente do usuário. |
| [Obter gerenciador](../api/user-list-manager.md) | [directoryObject](directoryobject.md) | Obter o usuário ou o contato organizacional que é o gerente do usuário da propriedade de navegação do gerente. |
| [Listar directReports](../api/user-list-directreports.md) | Coleção [directoryObject](directoryobject.md) | Obter os usuários ou contatos subordinados ao usuário da propriedade de navegação directReports. |
| **Configurações do Outlook** |  |  |
| [Criar categoria do Outlook](../api/outlookuser-post-mastercategories.md) | [outlookCategory](outlookcategory.md) | Cria um objeto outlookCategory na lista mestra de categorias do usuário. |
| [Obter supportedLanguages](../api/outlookuser-supportedlanguages.md), | Coleção [localeInfo](localeinfo.md) | Obtém a lista de locais e idiomas com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário. |
| [Obter supportedTimeZones](../api/outlookuser-supportedtimezones.md) | [timeZoneInformation](timezoneinformation.md collection) | Obtém a lista de fusos horários com suporte para o usuário, conforme configurado no servidor de caixa de correio do usuário. |
| [Obtém configurações de caixa de correio do usuário](../api/user-get-mailboxsettings.md) | [mailboxSettings](mailboxsettings.md) | Obtém as configurações de caixa de correio do usuário. |
| [Listar as categorias do Outlook](../api/outlookuser-list-mastercategories.md) | Coleção [outlookCategory](outlookcategory.md) | Obtém todas as categorias que foram definidas para o usuário. |
| [Converter IDs do Exchange](../api/user-translateexchangeids.md) | coleção [convertIdResult](convertidresult.md) | Traduzir os identificadores de recursos relacionados ao Outlook entre formatos. |
| [Atualizar configurações da caixa de correio do usuário](../api/user-update-mailboxsettings.md) | [mailboxSettings](mailboxsettings.md) | Habilitar, configurar ou desabilitar o mailboxSettings de um ou mais usuários. |
| **Foto** |  |  |
| [Obter foto](../api/profilephoto-get.md) | [profilePhoto](profilephoto.md) | Obtém o profilePhoto especificado ou seus metadados (propriedades profilePhoto). |
| [Atualizar profilephoto](../api/profilephoto-update.md) | Nenhum | Atualiza a foto de qualquer usuário no locatário, incluindo o usuário conectado ou o grupo ou contato especificado. |
| **Planejador** |  |  |
| [Listar tarefas](../api/planneruser-list-tasks.md) | Coleção [plannerTask](plannertask.md) | Obter o plannerTasks atribuído ao usuário. |
| **Extensões de esquema** |  |  |
| [Adicionar valores de extensões de esquema](/graph/extensibility-schema-groups) | Nenhum | Cria uma definição para a extensão de esquema e usa-a para adicionar dados digitados personalizados a um recurso. |
| **Teamwork** |  |  |
| [Lista de aplicativos instalados para o usuário](../api/userteamwork-list-installedapps.md) | Coleção[userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) | Lista os aplicativos instalados no escopo pessoal de um usuário. |
| [Obtém o aplicativo instalado para o usuário](../api/userteamwork-get-installedapps.md) | [userScopeTeamsAppInstallation](userscopeteamsappinstallation.md) | Lista o aplicativo especificado instalado no escopo pessoal de um usuário. |
| [Adicionar o aplicativo para o usuário](../api/userteamwork-post-installedapps.md) | Nenhum | Adiciona (instala) um aplicativo no escopo pessoal de um usuário. |
| [Remover o aplicativo para o usuário](../api/userteamwork-delete-installedapps.md) | Nenhum | Remove (desinstala) um aplicativo no escopo pessoal de um usuário. |
| [Atualizar o aplicativo instalado para o usuário](../api/userteamwork-teamsappinstallation-upgrade.md) | Nenhum | Atualizações para a versão mais recente do aplicativo instalada no escopo pessoal de um usuário. |
| [Obter chat entre o usuário e o aplicativo](../api/userscopeteamsappinstallation-get-chat.md) | [Chat](chat.md) | Lista um chat entre o usuário e o aplicativo. |
| **Tarefas pendentes** |  |  |
| [Criar tarefa](../api/todotasklist-post-tasks.md) | [todoTask](todotask.md) | Crie um [todoTask](todotask.md) na lista de tarefas especificada. |
| [Criar uma lista de tarefas](../api/todo-post-lists.md) | [todoTaskList](todotasklist.md) | Criar uma lista de tarefas To Dona caixa de correio do usuário. |
| [Listar tarefas](../api/todotasklist-list-tasks.md) | Coleção [todoTask](todotask.md) | Obtenha todos os recursos [todoTask](todotask.md) na lista especificada. |
| [Lista de listas de tarefas](../api/todo-list-lists.md) | Coleção [todoTaskList](todotasklist.md) | Obtenha todas as listas de tarefas na caixa de correio do usuário. |
| **Configurações do usuário** |  |  |
| [Obter configurações](../api/usersettings-get.md) | [userSettings](usersettings.md) | Leia o usuário e o objeto de configurações da organização. |
| [Atualizar configurações](../api/usersettings-update.md) | [userSettings](usersettings.md) | Atualize as propriedades do objeto de configurações. |


## <a name="properties"></a>Propriedades

> [!IMPORTANT]
> O uso específico de `$filter` e o parâmetro de consulta `$search` é suportado somente quando se usa o cabeçalho **ConsistencyLevel** definido como `eventual` e `$count`. Para obter mais informações, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries#user-properties).

| Propriedade       | Tipo    |Descrição|
|:---------------|:--------|:----------|
|aboutMe|String|Um campo de entrada de texto de forma livre para o usuário se descrever. Retornado apenas em `$select`.|
|accountEnabled|Booliano| `true` se a conta estiver habilitada. Caso contrário, `false`. Essa propriedade é obrigatória quando um usuário é criado.<br><br>Retornado apenas em `$select`. Suporte `$filter` (`eq`, `ne`, `not` e `in`).    |
|ageGroup|[ageGroup](#agegroup-values)|Define a faixa etária do usuário. Valores permitidos: `null`, `Minor`, `NotAdult` e `Adult`. Confira as [definições de propriedades da faixa etária legal](#legal-age-group-property-definitions) para obter mais informações. <br><br>Retornado apenas em `$select`. Suporte `$filter` (`eq`, `ne`, `not` e `in`).|
|assignedLicenses|Coleção [assignedLicense](assignedlicense.md)|As licenças atribuídas ao usuário, incluindo licenças herdadas (baseadas em grupo).  Não anulável. Retornado apenas em `$select`. Suporte para `$filter` (`eq` e `not`).           |
|assignedPlans|Coleção [assignedPlan](assignedplan.md)|Os planos que são atribuídos ao usuário. Somente leitura. Não anulável.<br><br>Retornado apenas em `$select`. Suporte para `$filter` (`eq` e `not`). |
|birthday|DateTimeOffset|O aniversário do usuário. O tipo de carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é: `2014-01-01T00:00:00Z` <br><br>Retornado apenas em `$select`.|
|businessPhones|Coleção de cadeias de caracteres|Os números de telefone do usuário. OBSERVAÇÃO: Embora esta seja uma coleção de cadeia de caracteres, somente um número pode ser definido para esta propriedade. Somente leitura para usuários sincronizados do diretório local.<br><br>Retornado por padrão. Suporta `$filter` (`eq`, `not`, `ge`, `le`, `startsWith`).|
|city|Cadeia de caracteres|A cidade em que o usuário está localizado. O comprimento máximo é de 128 caracteres. <br><br>Retornado apenas em `$select`. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`, e `eq` em `null` valores).|
|CompanyName | String | O nome da empresa em que o usuário está associado. Essa propriedade pode ser útil para descrever a empresa de onde procede um usuário externo. O tamanho máximo é de 64 caracteres.<br><br>Retornado apenas em `$select`. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`, e `eq` em `null` valores).|
|consentProvidedForMinor|[consentProvidedForMinor](#consentprovidedforminor-values)|Define se o consentimento foi obtido para menores. Valores permitidos: `null`, `Granted`, `Denied` e `NotRequired`. Confira as [definições de propriedades da faixa etária legal](#legal-age-group-property-definitions) para obter mais informações. <br><br>Retornado apenas em `$select`. Suporte `$filter` (`eq`, `ne`, `not` e `in`).|
|country|Cadeia de caracteres|O país/região em que o usuário está localizado; por exemplo, `US` ou `UK`. O comprimento máximo é de 128 caracteres. <br><br>Retornado apenas em `$select`. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`, e `eq` em `null` valores).|
|createdDateTime | DateTimeOffset |A data de criação do objeto de usuário. Somente leitura.<br><br>Retornado apenas em `$select`. Suporta `$filter` (`eq`, `ne`, `not` , `ge`, `le`, `in`).|
| creationType | String | Indica se a conta do usuário foi criada por meio de um dos seguintes métodos: <br/> <ul><li>Como uma conta corporativa ou de estudante (`null`). <li>Como uma conta externa (`Invitation`). <li>Como uma conta local para um locatário do Azure Active Directory B2C (`LocalAccount`). <li>Por meio da inscrição de autoatendimento feita por um usuário interno usando a verificação por email (`EmailVerified`). <li>Por meio da inscrição de autoatendimento feita por um usuário externo que se inscreveu usando um link que faz parte de um fluxo do usuário (`SelfServiceSignUp`).</ul> <br>Somente leitura.<br>Retornado apenas em `$select`. Suporta `$filter` (`eq`, `ne`, `not`, `in`). |
|deletedDateTime| DateTimeOffset | A data e hora que o usuário foi excluído. <br><br>Retornado apenas em `$select`. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`). |
|department|String|O nome do departamento no qual o usuário trabalha. O comprimento máximo é de 64 caracteres. <br><br>Retornado apenas em `$select`. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `eq` em `null` valores).|
|displayName|String|O nome exibido no catálogo de endereços para o usuário. Geralmente é a combinação do nome do usuário, inicial do meio e sobrenome. Esta propriedade é necessária quando um usuário é criado e não pode ser limpa durante as atualizações. O comprimento máximo é de 256 caracteres.<br><br>Retornado por padrão. Suporta `$filter` (`eq`, `ne`, `not` , `ge`, `le`, `in`, `startsWith`, e `eq` em `null` valores), `$orderBy`, e `$search`.|
| employeeHireDate | DateTimeOffset | A data e a hora em que o usuário foi contratado ou começará a trabalhar em caso de futura contratação. <br><br>Retornado apenas em `$select`. Suporta `$filter` (`eq`, `ne`, `not` , `ge`, `le`, `in`).|
| employeeId | String | O identificador de funcionário atribuído ao usuário pela organização. O comprimento máximo é de 16 caracteres. <br><br>Retornado apenas em `$select`. Suporta `$filter` (`eq`, `ne`, `not` , `ge`, `le`, `in`, `startsWith`, e `eq` em `null` valores).|
|employeeOrgData|[employeeOrgData](employeeorgdata.md) |Representa os dados da organização (por exemplo, divisão e costCenter) associados a um usuário. <br><br>Retornado apenas em `$select`. Suporta `$filter` (`eq`, `ne`, `not` , `ge`, `le`, `in`).|
| employeeType | String | Captura o tipo de trabalhador corporativo. Por exemplo, `Employee`, `Contractor`, `Consultant` ou `Vendor`. Retornado apenas em `$select`. Suporta `$filter` (`eq`, `ne`, `not` , `ge`, `le`, `in`, `startsWith`).|
|externalUserState|String|Para um usuário externo convidado para o locatário usando a [API de convite](../api/invitation-post.md), essa propriedade representa o status do convite do usuário convidado. Para usuários convidados, o estado pode ser `PendingAcceptance` ou `Accepted` ou `null` para todos os outros usuários. <br><br>Retornado apenas em `$select`. Suporta `$filter` (`eq`, `ne`, `not` , `in`).|
|externalUserStateChangeDateTime|DateTimeOffset|Mostra o carimbo de data/hora da alteração mais recente da propriedade **externalUserState**. <br><br>Retornado apenas em `$select`. Suporta `$filter` (`eq`, `ne`, `not` , `in`).|
|FaxNumber|String|O número de fax do usuário. <br><br>Retornado apenas em `$select`. Suporta `$filter` (`eq`, `ne`, `not` , `ge`, `le`, `in`, `startsWith`, e `eq` em `null` valores).|
|givenName|String|O nome fornecido (nome) do usuário. O comprimento máximo é de 64 caracteres. <br><br>Retornado por padrão. Suporta `$filter` (`eq`, `ne`, `not` , `ge`, `le`, `in`, `startsWith`, e `eq` em `null` valores).|
| hireDate | DateTimeOffset | A data de contratação do usuário. O tipo de carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é `2014-01-01T00:00:00Z` <br><br>Retornado apenas em `$select`. <br> **Observação:** essa propriedade é específica do SharePoint Online. É recomendável usar a propriedade **employeeHireDate** nativa para definir e atualizar valores de data de contratação usando as APIs do Microsoft Graph. |
|id|String|O identificador exclusivo do usuário. Deve ser tratado como um identificador opaco. Herdado de [directoryObject](directoryobject.md). Chave. Não anulável. Somente leitura. <br><br>Retornado por padrão. Dá suporte `$filter` (`eq`, `ne`, `not`, `in`).|
|Identidades|Coleção [objectIdentity](objectIdentity.md)| Representa as identidades que podem ser usadas para entrar nesta conta de usuário. Uma identidade pode ser fornecida pela Microsoft (também conhecida como conta local), por organizações ou por provedores de identidade social, como o Facebook, Google e Microsoft, e está vinculada a uma conta de usuário. Pode conter vários itens com o mesmo valor **signInType**. <br><br>Retornado apenas em `$select`. Dá suporte a `$filter` (`eq`) incluindo em valores`null`, somente quando o **signInType** não é `userPrincipalName`.|
|imAddresses|String collection|Os endereços do Protocolo de Início de Sessão (SIP) de VoIP (Voice over IP) da mensagem instantânea para o usuário. Somente leitura.<br><br>Retornado apenas em `$select`. Suporta `$filter` (`eq`, `not`, `ge`, `le`, `startsWith`).|
|interests|Coleção de cadeias de caracteres|Uma lista para o usuário descrever os interesses dele. <br><br>Retornado apenas em `$select`.|
|isResourceAccount|Boolean| Não use – reservado para uso futuro.|
|jobTitle|String|O cargo do usuário. O comprimento máximo é de 128 caracteres. <br><br>Retornado por padrão. Suporta `$filter` (`eq`, `ne`, `not` , `ge`, `le`, `in`, `startsWith`, e `eq` em `null` valores).|
|lastPasswordChangeDateTime| DateTimeOffset | A hora em que esse usuário do Azure Active Directory alterou sua senha pela última vez ou quando sua senha foi criada, qualquer que seja a data em que a ação mais recente foi realizada. As informações de data e hora usam o formato ISO 8601 e estão sempre no horário UTC. Por exemplo, meia-noite UTC de 1º de janeiro de 2014 é `2014-01-01T00:00:00Z`. <br><br>Retornado apenas em `$select`.|
|legalAgeGroupClassification|[legalAgeGroupClassification](#legalagegroupclassification-values)| Usado por aplicativos empresariais para determinar a faixa etária legal do usuário. Essa propriedade é somente leitura e calculada com base nas propriedades **ageGroup** e **consentProvidedForMinor**. Valores permitidos: `null`, `MinorWithOutParentalConsent`, `MinorWithParentalConsent`, `MinorNoParentalConsentRequired`, `NotAdult` e `Adult`. Confira as [definições de propriedades da faixa etária legal](#legal-age-group-property-definitions) para obter mais informações. <br><br>Retornado apenas em `$select`.|
|licenseAssignmentStates|Coleção [licenseAssignmentState](licenseassignmentstate.md)|Estado das atribuições de licença para este usuário. Somente leitura.<br><br>Retornado apenas em `$select`.|
|email|String|O endereço SMTP do usuário, por exemplo, `jeff@contoso.onmicrosoft.com`.<br>As alterações feitas nessa propriedade também atualizarão a coleção **proxyAddresses** do usuário para incluir o valor como um endereço SMTP. Para contas do Azure AD B2C, esta propriedade só pode ser atualizada até dez vezes com endereços SMTP exclusivos. Esta propriedade não pode conter caracteres de ênfase.<br><br>Retornado por padrão. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`, `endsWith`e `eq` em `null` valores).|
|mailboxSettings|[mailboxSettings](mailboxsettings.md)|Configurações da caixa de correio principal do usuário conectado. Você pode [obter](../api/user-get-mailboxsettings.md) ou [atualizar](../api/user-update-mailboxsettings.md) as configurações de localidade, fuso horário ou de envio de respostas automáticas a mensagens de entrada.<br><br>Retornado apenas em `$select`.|
|mailNickname|String|O alias de email do usuário. Essa propriedade deve ser especificada quando um usuário é criado. O comprimento máximo é de 64 caracteres.<br><br>Retornado apenas em `$select`. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`, e `eq` em `null` valores).|
|mobilePhone|String|O número de celular principal do usuário. Somente leitura para usuários sincronizados do diretório local. O comprimento máximo é de 64 caracteres. <br><br>Retornado por padrão. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`, e `eq` em `null` valores). |
|mySite|String|A URL do site pessoal do usuário. <br><br>Retornado apenas em `$select`.|
|officeLocation|String|A localização do escritório no local de trabalho do usuário. <br><br>Retornado por padrão. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`, e `eq` em `null` valores).|
|onPremisesDistinguishedName|String| Contém `distinguished name` ou `DN` do Active Directory local. A propriedade somente é preenchida para os clientes que estejam sincronizando o seu diretório local com o Azure Active Directory pelo Azure AD Connect. Somente leitura.<br><br>Retornado apenas em `$select`. |
|onPremisesDomainName|String| Contém o `domainFQDN` local, também chamado dnsDomainName, sincronizado do diretório local. A propriedade é preenchida apenas para clientes que estão sincronizando seu diretório local com o Azure Active Directory por meio do Azure AD Connect. Somente leitura. <br><br>Retornado apenas em `$select`.|
|onPremisesExtensionAttributes|[onPremisesExtensionAttributes](onpremisesextensionattributes.md)|Contém extensionAttributes1-15 para o usuário. Os atributos de extensão individuais não são selecionáveis nem filtráveis. <br><li>Para um usuário **onPremisesSyncEnabled**, a fonte de autoridade para este conjunto de propriedades é o local e é somente leitura. </li><li>Para um usuário apenas na nuvem (onde **onPremisesSyncEnabled** é `false`), essas propriedades podem ser definidas durante a criação ou atualização de um objeto de usuário.  </li><li>Para um usuário somente na nuvem previamente sincronizado a partir do Active Directory local, essas propriedades são somente leitura no Microsoft Graph, mas podem ser totalmente gerenciadas através do Centro de Administração do Exchange ou do módulo Exchange Online V2 no PowerShell.</li><br> Esses atributos de extensão também são conhecidos como atributos personalizados do Exchange 1-15. |
|onPremisesImmutableId|String|Essa propriedade é usada para associar uma conta de usuário do Active Directory local com seu objeto de usuário do Azure AD. Essa propriedade deverá ser especificada ao criar uma nova conta de usuário no Graph se você estiver usando um domínio federado para a propriedade **userPrincipalName** (UPN) do usuário. **OBSERVAÇÃO:** Os caracteres **$** e **\_** não podem ser usados ao especificar essa propriedade.<br><br>Retornado apenas em `$select`. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`)..                            |
|onPremisesLastSyncDateTime|DateTimeOffset|Indica a última vez em que o objeto foi sincronizado com o diretório no local; por exemplo: `2013-02-16T03:04:54Z`. O tipo de carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é: `2014-01-01T00:00:00Z`. Somente leitura. <br><br>Retornado apenas em `$select`. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`).|
|onPremisesProvisioningErrors|coleção [OnPremisesProvisioningError](onpremisesprovisioningerror.md)| Erros ao usar o produto de sincronização da Microsoft durante a configuração. <br><br>Retornado apenas em `$select`. Suporta `$filter` (`eq`, `not`, `ge`, `le`).|
|onPremisesSamAccountName|String| Contém o `samAccountName` local sincronizado do diretório local. A propriedade somente é preenchida para os clientes que estejam sincronizando o diretório local com o Azure Active Directory pelo Azure AD Connect. Somente leitura.<br><br>Retornado apenas em `$select`. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`).|
|onPremisesSecurityIdentifier|String|Contém o identificador de segurança (SID) local do usuário que foi sincronizado do local com a nuvem. Somente leitura.<br><br>Retornado apenas em `$select`.  Suporta `$filter` (`eq` incluindo valores `null` ). |
|onPremisesSyncEnabled|Booliano| `true` se esse objeto está sincronizado de um diretório local; `false` se esse objeto foi originalmente sincronizado de um diretório local, mas não está mais sincronizado; `null` se esse objeto nunca foi sincronizado de um diretório local (padrão). Somente leitura. <br><br>Retornado apenas em `$select`. Suporta `$filter` (`eq`, `ne`, `not`, `in` e `eq` em `null` valores).|
|onPremisesUserPrincipalName|String| Contém o `userPrincipalName` local sincronizado do diretório local. A propriedade somente é preenchida para os clientes que estejam sincronizando o diretório local com o Azure Active Directory pelo Azure AD Connect. Somente leitura.<br><br>Retornado apenas em `$select`. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`).|
|otherMails|Coleção String| Uma lista de endereços de email adicional para o usuário; Por exemplo: `["bob@contoso.com", "Robert@fabrikam.com"]`. <br>OBSERVAÇÃO: esta propriedade não pode conter caracteres de ênfase. <br><br>Retornado apenas em `$select`. Suporta `$filter` (`eq`, `not`, `ge`, `le`, `in`, `startsWith`).|
|passwordPolicies|String|Especifica as políticas de senha do usuário. Esse valor é uma enumeração cujo um dos valores possíveis é `DisableStrongPassword`, o que permite especificar senhas mais fracas do que a política padrão. Também é possível especificar `DisablePasswordExpiration`. Ambos podem ser especificados juntos; por exemplo: `DisablePasswordExpiration, DisableStrongPassword`.<br><br>Retornado apenas em `$select`. Para mais informações sobre as políticas de senha padrão, confira [Políticas de senha do Azure AD](/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts). Dá suporte a `$filter` (`ne`, `not` e `eq` em valores `null`). |
|passwordProfile|[passwordProfile](passwordprofile.md)|Especifica o perfil de senha do usuário. O perfil contém a senha do usuário. Essa propriedade é obrigatória quando um usuário é criado. A senha no perfil deve atender a requisitos mínimos, conforme especificado pela propriedade **passwordPolicies**. Por padrão, é obrigatória uma senha forte. **OBSERVAÇÃO:** Para locatários B2C do Azure, a propriedade **forceChangePasswordNextSignIn** deve ser definida como `false` e, em vez disso, usar políticas personalizadas e fluxos de usuário para forçar a redefinição de senha no primeiro logon. Confira [Forçar a redefinição de senha no primeiro logon](https://github.com/azure-ad-b2c/samples/tree/master/policies/force-password-reset-first-logon).<br><br>Retornado apenas em `$select`. Suporta `$filter` (`eq`, `ne`, `not`, `in` e `eq` em `null` valores).|
|pastProjects|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar seus projetos anteriores. <br><br>Retornado apenas em `$select`.|
|postalCode|String|O código postal do endereço postal do usuário. O código postal é específico para o país/região do usuário. Nos Estados Unidos da América, este atributo contém o Código postal. O comprimento máximo é de 40 caracteres.<br><br>Retornado apenas em `$select`. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`, e `eq` em `null` valores).|
| preferredDataLocation | String | O local de dados preferido para o usuário. Para saber mais, confira [OneDrive Online Multi-Geo](/sharepoint/dev/solution-guidance/multigeo-introduction).|
|preferredLanguage|Cadeia de caracteres|O idioma preferencial do usuário. Deve seguir o Código ISO 639-1; por exemplo, `en-US`.<br><br>Devolvido por padrão. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` e `eq` em valores `null`)|
|preferredName|String|O nome preferencial do usuário. <br><br>Retornado apenas em `$select`.|
|provisionedPlans|coleção [provisionedPlan](provisionedplan.md)|Os planos que estão provisionados para o usuário. Somente leitura. Não anulável.<br><br>Retornado apenas em `$select`. Suporta `$filter` (`eq`, `not`, `ge`, `le`).|
|proxyAddresses|Coleção de cadeias de caracteres|Por exemplo: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]`. As alterações na propriedade **mail** também atualizarão essa coleção para incluir o valor como um endereço SMTP. Para obter mais informações, consulte propriedades de [email e proxyAddresses](#mail-and-proxyaddresses-properties). O endereço proxy prefixado com `SMTP` (em maiúsculas) é o endereço proxy primário, enquanto aqueles prefixados com `smtp` são os endereços proxy secundários. Para contas do Azure AD B2C, essa propriedade tem um limite de dez endereços exclusivos. Somente leitura no Microsoft Graph; você pode atualizar essa propriedade somente por meio do [Microsoft 365 de administração](/exchange/recipients-in-exchange-online/manage-user-mailboxes/add-or-remove-email-addresses). Não anulável. <br><br>Retornado apenas em `$select`. Suporta `$filter` (`eq`, `not`, `ge`, `le`, `startsWith`).|
|refreshTokensValidFromDateTime|DateTimeOffset|Os tokens de atualização ou de sessão (cookies de sessão) emitidos antes dessa hora são inválidos e os aplicativos recebem um erro ao usar um token de atualização ou de sessão inválido para adquirir um token de acesso delegado (para acessar APIs como o Microsoft Graph).  Se isso acontecer, o aplicativo precisará adquirir um novo token de atualização, fazendo uma solicitação ao ponto de extremidade de autorização. <br><br>Retornado apenas em `$select`. Somente leitura. |
|responsibilities|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar suas responsabilidades. <br><br>Retornado apenas em `$select`.|
|schools|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar as escolas que frequentou. <br><br>Retornado apenas em `$select`.|
|showInAddressList|Booliano|`true` se a lista de endereços global do Outlook deve conter o usuário, caso contrário `false`. Se não estiver configurado, isso será tratado como `true`. Para os usuários convidados por meio do Gerenciador de convites, essa propriedade será definida como `false`. <br><br>Retornado apenas em `$select`. Suporta `$filter` (`eq`, `ne`, `not`, `in`).|
|skills|Coleção de cadeias de caracteres|Uma lista para o usuário enumerar suas qualificações. <br><br>Retornado apenas em `$select`.|
|signInSessionsValidFromDateTime|DateTimeOffset| Os tokens de atualização ou de sessão (cookies de sessão) emitidos antes dessa hora são inválidos e os aplicativos recebem um erro ao usar um token de atualização ou de sessão inválido para adquirir um token de acesso delegado (para acessar APIs como o Microsoft Graph).  Se isso acontecer, o aplicativo precisará adquirir um novo token de atualização, fazendo uma solicitação ao ponto de extremidade de autorização. Somente leitura. Use [revokeSignInSessions](../api/user-revokesigninsessions.md) para redefinir. <br><br>Retornado apenas em `$select`.|
|state|String|O estado ou município no endereço do usuário. O comprimento máximo é de 128 caracteres. <br><br>Retornado apenas em `$select`. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`, e `eq` em `null` valores).|
|streetAddress|String|O endereço do local de trabalho do usuário. O comprimento máximo é de 1024 caracteres. <br><br>Retornado apenas em `$select`. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`, e `eq` em `null` valores).|
|surname|String|O sobrenome do usuário (nome de família ou sobrenome). O comprimento máximo é de 64 caracteres. <br><br>Retornado por padrão. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`, e `eq` em `null` valores).|
|usageLocation|String|Um código de duas letras (padrão ISO 3166). Obrigatório para os usuários que receberão licenças devido à exigência legal de verificar a disponibilidade de serviços nos países/regiões. Por exemplo: `US`, `JP`, e `GB`. Não anulável.<br><br>Retornado apenas em `$select`. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`, e `eq` em `null` valores).|
|userPrincipalName|Cadeia de caracteres|O nome UPN do usuário. O nome UPN é um nome de logon para o usuário ao estilo da Internet com base na RFC 822 padrão da Internet. Por convenção, ele deve ser mapeado para o nome de email do usuário. O formato geral é alias@domain, em que o domínio deve estar presente na coleção de domínios verificados do locatário. Essa propriedade é obrigatória quando um usuário é criado. Os domínios verificados para o locatário podem ser acessados pela propriedade **verifiedDomains** da [organização](organization.md).<br>OBSERVAÇÃO: esta propriedade não pode conter caracteres de ênfase. Somente os seguintes caracteres são permitidos `A - Z`, `a - z`, `0 - 9`, ` ' . - _ ! # ^ ~`. Para obter a lista completa de caracteres permitidos, consulte as [políticas de nome de usuário](/azure/active-directory/authentication/concept-sspr-policy#userprincipalname-policies-that-apply-to-all-user-accounts). <br><br>Retornado por padrão. Suporta `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith`, `endsWith`) e `$orderBy`.
|userType|String|Um valor de string que pode ser usado para classificar tipos de usuário em seu diretório, como `Member` e `Guest`. <br><br>Retornado apenas em `$select`. Suporta `$filter` (`eq`, `ne`, `not`, `in` e `eq` em `null` valores). **OBSERVAÇÃO:** Para obter mais informações sobre as permissões para usuários membros e convidados, consulte [Quais são as permissões padrão de usuário em Azure Active Directory?](/azure/active-directory/fundamentals/users-default-permissions#member-and-guest-users)         |

### <a name="mail-and-proxyaddresses-properties"></a>propriedades mail e proxyAddresses
**email** e **proxyAddresses** são propriedades relacionadas a email. **proxyAddresses** é uma coleção de endereços relevantes apenas para o servidor do Microsoft Exchange. Ele é usado para armazenar uma lista de endereços de email para um usuário que está vinculado a uma única caixa de correio. **email** propriedade é usada como o endereço de email do usuário para várias finalidades, incluindo a entrada do usuário e define o endereço proxy principal.
 
**email** e **proxyAddresses** podem ser recuperados por meio da API de [usuário GET](/graph/api/user-get) no MS Graph. **email** pode ser atualizado por meio do método [PATCH da API de usuário de atualização](/graph/api/user-update), mas **proxyAddresses** não pode ser atualizado por meio do Microsoft Graph. Quando a propriedade de **email** de um usuário é atualizada, ela aciona o recálculo de **proxyAddresses** e o email recém-atualizado é definido como o endereço de proxy primário, exceto nos seguintes cenários: 
 
1. Se um usuário tiver uma licença que inclua o Microsoft Exchange, todos os endereços proxy deverão pertencer a um domínio verificado no locatário. Qualquer um que não pertença a domínios verificados é removido silenciosamente.
2. O email de um usuário NÃO será definido como o endereço de proxy primário se o usuário for um convidado e o endereço de proxy primário contiver a cadeia de caracteres UPN do usuário convidado com #EXT#.
3. O email de um usuário NÃO será removido, mesmo que ele não tenha mais endereços proxy, se o usuário for um convidado.
 
**proxyAddresses** são exclusivos entre objetos de diretório (usuários, grupos e contatos organizacionais). Se a propriedade **mail** de um usuário estiver em conflito com um dos **proxyAddresses** de outro objeto, você atualizará com êxito a propriedade **mail**. No entanto, o novo valor de email não será adicionado à coleção **proxyAddresses**.

### <a name="legal-age-group-property-definitions"></a>Definições de propriedade da faixa etária legal

Esta seção explica como as três propriedades de grupo idade (**legalAgeGroupClassification**, **ageGroup** e **consentProvidedForMinor**) são usadas por administradores do Azure Active Directory e desenvolvedores de aplicativos empresariais para atender às regulamentações relacionadas à idade:
- A propriedade legal **AgeGroupClassification** é somente leitura. É usado por desenvolvedores de aplicativos corporativos para garantir o tratamento correto de um usuário com base em sua faixa etária legal. É calculado com base nas propriedades **ageGroup** e **consentProvidedForMinor** do usuário.
- **ageGroup** e **consentProvidedForMinor** são propriedades opcionais usadas pelos administradores do Azure Active Directory para ajudar a garantir que o uso de uma conta seja tratado corretamente com base nas regras regulatórias relacionadas à idade que regem o país ou região do usuário.

Por exemplo: Cameron é o administrador de um diretório em uma escola de ensino fundamental em Holyport, no Reino Unido. No início do ano letivo ele usa a documentação de admissão para obter o consentimento dos pais dos menores baseado nos regulamentos relacionadas com a idade no Reino Unido. O consentimento obtido do pai permite que a conta do menor seja usado pela escola de Holyport e os aplicativos da Microsoft. Cameron cria todas as contas e define **ageGroup** como `minor` e **consentProvidedForMinor** como `granted`. Os aplicativos usados ​​por seus alunos podem suprimir recursos que não são adequados para menores.

<!-- Note that the following 3 sub-sections are only documented like enums for a consistent user experience but they are String types.-->

#### <a name="legalagegroupclassification-values"></a>legalAgeGroupClassification values

| Member    | Descrição|
|:---------------|:----------|
|null|Valor padrão, nenhum **ageGroup** foi definido para o usuário.|
|MenorSemConsentimentoDosPais |(Reservado para uso futuro)|
|MenorComConsentimentoDosPais| O usuário é considerado menor baseado nos regulamentos relacionados com a idade de seu país ou região, e o administrador da conta obteve o consentimento apropriado dos pais ou responsável.|
|Adulto|O usuário é considerado adulto baseado nos regulamentos relacionadas com a idade do seu país ou região.|
|NãoAdulto|O usuário é de um país ou região com regulamentos adicionais relacionados à idade (por exemplo, Estados Unidos, Reino Unido, União Europeia ou Coreia do Sul) e a idade do usuário está entre menor e adulto (como estipulado com base no país ou região). Em geral, isso significa que adolescentes são considerados como `notAdult` nos países/regiões regulamentados.|
|MenorSemExigênciaDeConsentimentoDosPais|O usuário é menor de idade, mas é de um país ou região que não tem com regulamentações relacionadas com a idade.|

#### <a name="agegroup-values"></a>ageGroup values

| Member    | Descrição|
|:---------------|:--------|
|null|Valor padrão, nenhum **ageGroup** foi definido para o usuário.|
|Secundária|O usuário é considerado um menor.|
|NãoAdulto|O usuário é de um país que possui regulamentos legais (como Estados Unidos, Reino Unido, União Europeia ou Coreia do Sul) e a idade do usuário é superior ao limite superior de idade infantil (conforme o país) e inferior ao limite inferior de adulto idade (conforme estipulado com base no país ou região). Basicamente, os adolescentes são considerados como `notAdult` nos países/regiões regulamentados.|
|Adulto|O usuário deve ser tratado como um adulto.|

#### <a name="consentprovidedforminor-values"></a>consentProvidedForMinor values

| Member    | Descrição|
|:---------------|:----------|
|null|Valor padrão, nenhum **consentimentoProvidedForMinor** foi definido para o usuário.|
|Concedido|O consentimento foi obtido para o usuário ter uma conta.|
|Negado|O consentimento não foi obtido para o usuário ter uma conta.|
|NãoExigido|O usuário é de um local que não exige consentimento.|

## <a name="relationships"></a>Relações

| Relação | Tipo    |Descrição|
|:---------------|:--------|:----------|
|agreementAcceptances|Coleção [agreementAcceptance](agreementacceptance.md)| Status de aceitação dos termos de uso do usuário. Somente leitura. Anulável.|
|activities|Coleção [userActivity](projectrome-activity.md)|As atividades do usuário em todos os dispositivos. Somente leitura. Anulável.|
|appRoleAssignments|[appRoleAssignment](approleassignment.md) collection|Representa as funções de aplicativo que um usuário recebeu para um aplicativo. Dá suporte a `$expand`. |
|autenticação|[autenticação](../resources/authentication.md)| Os métodos de autenticação com suporte para o usuário.|
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
|events|Coleção [event](event.md)|Os eventos do usuário. O padrão é mostrar eventos no Calendário Padrão. Somente leitura. Anulável.|
|extensions|[extension](extension.md) collection|A coleção de extensões abertas definidas para o usuário. Somente leitura. Anulável.|
|inferenceClassification | [inferenceClassification](inferenceclassification.md) | Classificação de relevância das mensagens do usuário com base em designações explícitas que substituem a relevância ou importância deduzida. |
|insights|[officeGraphInsights](officegraphinsights.md) | Somente leitura. Anulável.|
|licenseDetails|Coleção de[licenseDetails](licensedetails.md)|Uma coleção dos detalhes da licença deste usuário. Somente leitura.|
|mailFolders|Coleção [mailFolder](mailfolder.md)| As pastas de email do usuário. Somente leitura. Anulável.|
|manager|[directoryObject](directoryobject.md)|O usuário ou contato que é o gerente deste usuário. Somente leitura. (Métodos HTTP: GET, PUT, DELETE.). Dá suporte a `$expand`.|
|memberOf|Coleção [directoryObject](directoryobject.md)|Os grupos e as funções de diretório dos quais o usuário é membro. Somente leitura. Anulável. Dá suporte a `$expand`. |
|messages|Coleção [message](message.md)|As mensagens em uma caixa de correio ou pasta. Somente leitura. Anulável.|
|onenote|[onenote](onenote.md)| Somente leitura.|
|outlook|[outlookUser](outlookuser.md)| Somente leitura.|
|ownedDevices|Coleção [directoryObject](directoryobject.md)|Dispositivos que pertencem ao usuário. Somente leitura. Anulável. Dá suporte a `$expand`.|
|ownedObjects|Coleção [directoryObject](directoryobject.md)|Objetos de diretório que pertencem ao usuário. Somente leitura. Anulável. Dá suporte a `$expand`.|
|people|Coleção [person](person.md)| Pessoas que são relevantes para o usuário. Somente leitura. Anulável.
|photo|[profilePhoto](profilephoto.md)| A foto de perfil do usuário. Somente leitura.|
|planner|[plannerUser](planneruser.md)| Ponto de entrada para o recurso do Planner que pode existir para um usuário. Somente leitura.|
|registeredDevices|Coleção [directoryObject](directoryobject.md)|Dispositivos que estão registrados para o usuário. Somente leitura. Anulável. Suporta `$expand`.|
|todo|[todo](todo.md)|Representa os serviços To Do disponíveis para um usuário. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

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
  "createdDateTime": "String (timestamp)",
  "creationType": "String",
  "department": "String",
  "displayName": "String",
  "employeeHireDate": "2020-01-01T00:00:00Z",
  "employeeId": "String",
  "employeeOrgData": {"@odata.type": "microsoft.graph.employeeOrgData"},
  "employeeType": "String",
  "faxNumber" : "String",
  "givenName": "String",
  "hireDate": "String (timestamp)",
  "id": "String (identifier)",
  "identities": [{"@odata.type": "microsoft.graph.objectIdentity"}],
  "imAddresses": ["String"],
  "interests": ["String"],
  "isResourceAccount": false,
  "jobTitle": "String",
  "legalAgeGroupClassification": "String",
  "licenseAssignmentStates": [{"@odata.type": "microsoft.graph.licenseAssignmentState"}],
  "lastPasswordChangeDateTime": "String (timestamp)",
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
  "responsibilities": ["String"],
  "schools": ["String"],
  "showInAddressList": true,
  "signInSessionsValidFromDateTime": "String (timestamp)",
  "skills": ["String"],
  "state": "String",
  "streetAddress": "String",
  "surname": "String",
  "usageLocation": "String",
  "userPrincipalName": "String",
  "userType": "String",

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

