---
title: tipo de recurso de grupo
description: 'Representa um grupo do Azure Active Directory (Azure AD), que pode ser um grupo do Office 365 ou um grupo de segurança. '
localization_priority: Priority
author: yyuank
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 03c366f8597d678cf875083067c96af6187fabb2
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845646"
---
# <a name="group-resource-type"></a>tipo de recurso de grupo

Namespace: microsoft.graph

Representa um grupo do Azure Active Directory (Azure AD), que pode ser um grupo do Office 365 ou um grupo de segurança.

Herda de [directoryObject](directoryobject.md).

Por motivos de desempenho, as operações [create](../api/group-post-groups.md), [get](../api/group-get.md) e [list](../api/group-list.md) retornam por padrão apenas um subconjunto das propriedades usadas com mais frequência. Essas propriedades _padrão_ estão listadas na seção [Propriedades](#properties). Para obter as propriedades não retornadas por padrão, especifique-as em uma opção de consulta `$select` do OData.

Esse recurso permite:

- Adicionar seus próprios dados às propriedades personalizadas como [extensions](/graph/extensibility-overview).
- Assinar as [notificações de alteração](/graph/webhooks).
- Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/user-delta.md).


## <a name="methods"></a>Métodos

| Método                                                                      | Tipo de retorno                                                | Descrição                                                                                                                                                                                                       |
|:----------------------------------------------------------------------------|:-----------------------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Gerenciamento de grupos**                                                        |                                                            |                                                                                                                                                                                                                   |
| [Criar grupo](../api/group-post-groups.md)                                 | [group](group.md)                                          | Criar um novo grupo. Pode ser um grupo do Office 365, um grupo dinâmico ou um grupo de segurança.                                                                                                                              |
| [Obter grupo](../api/group-get.md)                                            | [grupo](group.md)                                          | Ler as propriedades de um objeto group.                                                                                                                                                                                |
| [Listar grupos](../api/group-list.md)                                         | Coleção [group](group.md)                               | Listar objetos group e suas propriedades.                                                                                                                                                                          |
| [Atualizar grupo](../api/group-update.md)                                      | Nenhum                                                       | Atualizar as propriedades de um objeto group.                                                                                                                                                                          |
| [Excluir grupo](../api/group-delete.md)                                      | Nenhum                                                       | Excluir um objeto group.                                                                                                                                                                                              |
| [delta](../api/group-delta.md)                                              | Coleção group                                           | Obter alterações incrementais para grupos.                                                                                                                                                                               |
| [Listar groupLifecyclePolicies](../api/group-list-grouplifecyclepolicies.md)  | Coleção [groupLifecyclePolicy](grouplifecyclepolicy.md) | Listar políticas de ciclo de vida de grupo.                                                                                                                                                                                    |
| [Renovar](../api/group-renew.md)                                              | Booliano                                                    | Renova o período de validade de um grupo. Após renovar um grupo, o período de validade é estendido de acordo com o número de dias definido na política.                                                                               |
| [Adicionar proprietário](../api/group-post-owners.md)                                    | Nenhum                                                       | Adicionar um novo proprietário para o grupo postando na propriedade de navegação **owners** (com suporte somente para grupos de segurança e grupos de segurança habilitados para email).                                                             |
| [Listar proprietários](../api/group-list-owners.md)                                  | [directoryObject](directoryobject.md) collection           | Obter os proprietários do grupo da propriedade de navegação **owners**.                                                                                                                                              |
| [Remover proprietário](../api/group-delete-owners.md)                               | Nenhum                                                       | Remover um proprietário de um grupo do Office 365, grupo de segurança ou grupo de segurança habilitado para email por meio da propriedade de navegação **owners**.                                                                           |
| [Adicionar membro](../api/group-post-members.md)                                  | Nenhum                                                       | Adicionar um usuário ou grupo a esse grupo postando na propriedade de navegação **members** (com suporte somente para grupos de segurança e grupos de segurança habilitados para email).                                                        |
| [Listar membros](../api/group-list-members.md)                                | Coleção [directoryObject](directoryobject.md)           | Obter os usuários e grupos que são membros diretos desse grupo da propriedade de navegação **members**.                                                                                                          |
| [Listar membros transitivos](../api/group-list-transitivemembers.md)           | Coleção [directoryObject](directoryobject.md)           | Obtenha os usuários, grupos e dispositivos que são membros, inclusive membros aninhados desse grupo.                                                                                                                       |
| [Listar memberOf transitivos](../api/group-list-transitivememberof.md)         | Coleção [directoryObject](directoryobject.md)           | Lista os grupos dos quais este grupo é membro. Essa operação é transitiva e inclui os grupos que são membros aninhados desse grupo.                                                                       |
| [Remover membro](../api/group-delete-members.md)                             | Nenhum                                                       | Remove a member from an Office 365 group, a security group or a mail-enabled security group through the **members** navigation property. You can remove users or other groups.                                    |
| [checkMemberGroups](../api/group-checkmembergroups.md)                      | Coleção de cadeias de caracteres                                          | Check this group for membership in a list of groups. The function is transitive.                                                                                                                                  |
| [checkMemberObjects](../api/group-checkmemberobjects.md)                    | Coleção de cadeias de caracteres                                          | Verifique se há associação em uma lista de grupo, função de diretório ou objetos de unidade administrativa. Essa função é transitiva.                                                                                              |
| [getMemberGroups](../api/group-getmembergroups.md)                          | Coleção de cadeias de caracteres                                          | Return all the groups that the group is a member of. The function is transitive.                                                                                                                                  |
| [getMemberObjects](../api/group-getmemberobjects.md)                        | String collection                                          | Return all of the groups that the group is a member of. The function is transitive.                                                                                                                               |
| [Criar configuração](../api/groupsetting-post-groupsettings.md)                 | [groupSetting](groupsetting.md)                            | Create a setting object based on a groupSettingTemplate. The POST request must provide settingValues for all the settings defined in the template. Only groups specific templates may be used for this operation. |
| [Obter configuração](../api/groupsetting-get.md)                                   | [groupSetting](groupsetting.md)                            | Ler propriedades de um objeto de configuração específico.                                                                                                                                                                     |
| [Listar configurações](../api/groupsetting-list.md)                                | Conjunto [groupSetting](groupsetting.md)                 | Lista propriedades de todos os objetos de configuração.                                                                                                                                                                           |
| [Atualizar configuração](../api/groupsetting-update.md)                             | [groupSetting](groupsetting.md)                            | Atualizar um objeto de configuração.                                                                                                                                                                                          |
| [Excluir configuração](../api/groupsetting-delete.md)                             | None                                                       | Excluir um objeto de configuração.                                                                                                                                                                                          |
| [validateProperties](../api/group-validateproperties.md)                    | JSON                                                       | Valide se o nome de exibição do grupo do Office 365 ou apelido de email está em conformidade com as políticas de nomenclatura.                                                                                                                  |
| [assignLicense](../api/group-assignlicense.md)                              | [group](group.md)                                          | Adicione ou remova assinaturas para o grupo. Você também pode habilitar e desabilitar planos específicos associados a uma assinatura.                                                                                         |
| **Atribuições de função de aplicativo**                                                    |                                                            |                                                                                                                                                                                                                   |
| [List appRoleAssignments](../api/group-list-approleassignments.md)          | [appRoleAssignment](approleassignment.md) collection       | Obtenha os aplicativos e as funções de aplicativo que esse grupo foi atribuído.                                                                                                                                                    |
| [Adicionar appRoleAssignment](../api/group-post-approleassignments.md)            | [appRoleAssignment](approleassignment.md)                  | Atribuir uma função de aplicativo a este grupo.                                                                                                                                                                                 |
| [Remover appRoleAssignment](../api/group-delete-approleassignments.md)       | Nenhum                                                      | Remova uma atribuição de função de aplicativo deste grupo.                                                                                                                                                                    |
| **Calendar**                                                                |                                                            |                                                                                                                                                                                                                   |
| [Criar evento](../api/group-post-events.md)                                 | [evento](event.md)                                          | Criar um novo Event postando na coleção de eventos.                                                                                                                                                           |
| [Obter evento](../api/group-get-event.md)                                      | [event](event.md)                                          | Ler as propriedades de um objeto event.                                                                                                                                                                               |
| [Listar eventos](../api/group-list-events.md)                                  | Coleção [event](event.md)                               | Obter uma coleção de objetos de evento.                                                                                                                                                                                   |
| [Atualizar evento](../api/group-update-event.md)                                | Nenhum                                                       | Atualizar as propriedades de um objeto event.                                                                                                                                                                         |
| [Excluir evento](../api/group-delete-event.md)                                | Nenhum                                                       | Excluir o objeto event.                                                                                                                                                                                              |
| [Listar calendarView](../api/group-list-calendarview.md)                      | Coleção [event](event.md)                               | Obter um conjunto de eventos em uma janela de tempo especificada.                                                                                                                                                            |
| **Conversas**                                                           |                                                            |                                                                                                                                                                                                                   |
| [Criar conversa](../api/group-post-conversations.md)                   | [conversa](conversation.md)                            | Crie uma nova conversa postando na coleção de conversas.                                                                                                                                             |
| [Obter conversa](../api/group-get-conversation.md)                        | [conversation](conversation.md)                            | Ler as propriedades de um objeto conversation.                                                                                                                                                                         |
| [Listar conversas](../api/group-list-conversations.md)                    | Coleção [conversation](conversation.md)                 | Obter uma coleção de objetos Conversation.                                                                                                                                                                             |
| [Excluir conversa](../api/group-delete-conversation.md)                  | Nenhuma                                                       | Excluir objeto conversation.                                                                                                                                                                                       |
| [Criar thread](../api/group-post-threads.md)                               | [conversationThread](conversationthread.md)                | Criar um novo thread de conversa.                                                                                                                                                                                 |
| [Acessar thread](../api/group-get-thread.md)                                    | [conversationThread](conversationthread.md)                | Ler as propriedades de um objeto thread.                                                                                                                                                                               |
| [Listar threads](../api/group-list-threads.md)                                | Coleção [conversationThread](conversationthread.md)     | Obter todos os threads de um grupo.                                                                                                                                                                                   |
| [Atualizar thread](../api/group-update-thread.md)                              | Nenhum                                                       | Atualizar as propriedades de um objeto thread.                                                                                                                                                                             |
| [Excluir thread](../api/group-delete-thread.md)                              | Nenhum                                                       | Excluir objeto thread.                                                                                                                                                                                             |
| [Listar acceptedSenders](../api/group-list-acceptedsenders.md)                | Coleção [directoryObject](directoryobject.md)           | Obtenha uma lista de usuários ou grupos que estão na lista de remetentes aceitos para este grupo.                                                                                                                               |
| [Adicionar acceptedSender](../api/group-post-acceptedsenders.md)                  | [directoryObject](directoryobject.md)                      | Adicionar um Usuário ou Grupo à coleção acceptSenders.                                                                                                                                                              |
| [Remover acceptedSender](../api/group-delete-acceptedsenders.md)             | [directoryObject](directoryobject.md)                      | Remover um Usuário ou Grupo da coleção acceptedSenders.                                                                                                                                                       |
| [Listar rejectedSenders](../api/group-list-rejectedsenders.md)                | Coleção [directoryObject](directoryobject.md)           | Obtenha uma lista de usuários ou grupos que estão na lista de remetentes rejeitados para este grupo.                                                                                                                               |
| [Adicionar rejectedSender](../api/group-post-rejectedsenders.md)                  | [directoryObject](directoryobject.md)                      | Adicionar um novo Usuário ou Grupo à coleção rejectedSenders.                                                                                                                                                        |
| [Remover rejectedSender](../api/group-delete-rejectedsenders.md)             | [directoryObject](directoryobject.md)                      | Remover um novo Usuário ou Grupo da coleção Remetentesrejeitados.                                                                                                                                                     |
| [Criar configuração](../api/groupsetting-post-groupsettings.md)                 | [groupSetting](groupsetting.md)                            | Create a setting object based on a groupSettingTemplate. The POST request must provide settingValues for all the settings defined in the template. Only groups specific templates may be used for this operation. |
| [Obter configuração](../api/groupsetting-get.md)                                   | [groupSetting](groupsetting.md)                            | Ler propriedades de um objeto de configuração específico.                                                                                                                                                                     |
| [Listar configurações](../api/groupsetting-list.md)                                | Conjunto [groupSetting](groupsetting.md)                 | Lista propriedades de todos os objetos de configuração.                                                                                                                                                                           |
| [Atualizar configuração](../api/groupsetting-update.md)                             | Nenhum                                                       | Atualizar um objeto setting.                                                                                                                                                                                          |
| [Excluir configuração](../api/groupsetting-delete.md)                             | None                                                       | Excluir um objeto de configuração.                                                                                                                                                                                          |
| [Obter modelo de configuração](../api/groupsettingtemplate-get.md)                  | Nenhum                                                       | Ler as propriedades de um modelo de configuração.                                                                                                                                                                            |
| [Listar modelo de configuração](../api/groupsettingtemplate-list.md)                | Nenhum                                                       | Listar propriedades de todos os modelos de configuração.                                                                                                                                                                         |
| **Extensões abertas**                                                         |                                                            |                                                                                                                                                                                                                   |
| [Criar extensão aberta](../api/opentypeextension-post-opentypeextension.md) | [openTypeExtension](opentypeextension.md)                  | Crie uma extensão aberta e adicione propriedades personalizadas a uma instância nova ou existente de um recurso.                                                                                                                                 |
| [Obter extensão aberta](../api/opentypeextension-get.md)                       | Coleção [openTypeExtension](opentypeextension.md)       | Obtenha uma extensão aberta identificada pelo nome da extensão.                                                                                                                                                           |
| **Extensões de esquema**                                                       |                                                            |                                                                                                                                                                                                                   |
| [Adicionar valores de extensões de esquema](/graph/extensibility-schema-groups)           |                                                            | Cria uma definição para a extensão de esquema e usa-a para adicionar dados digitados personalizados a um recurso.                                                                                                                      |
| **Outros recursos de grupo**                                                   |                                                            |                                                                                                                                                                                                                   |
| [Listar fotos](../api/group-list-photos.md)                                  | Coleção [profilePhoto](photo.md)                        | Obter um conjunto de fotos de perfil para o grupo.                                                                                                                                                                 |
| [Listar plannerPlans](../api/plannergroup-list-plans.md)                      | Coleção [plannerPlan](plannerplan.md)                   | Obter os planos de planejador pertencentes ao grupo.                                                                                                                                                                             |
| **Configurações do usuário**                                                           |                                                            |                                                                                                                                                                                                                   |
| [addFavorite](../api/group-addfavorite.md)                                  | Nenhum                                                       | Adicionar o grupo à lista de grupos de favoritos do usuário conectado. Com suporte apenas para grupos do Office 365.                                                                                                          |
| [removeFavorite](../api/group-removefavorite.md)                            | Nenhum                                                       | Remover o grupo da lista de grupos favoritos do usuário conectado. Com suporte apenas para grupos do Office 365.                                                                                                     |
| [Listar memberOf](../api/group-list-memberof.md)                              | Coleção [directoryObject](directoryobject.md)           | Obtenha os grupos e as unidades administrativas dos quais esse usuário é membro direto, da propriedade de navegação **memberOf** .                                                                                           |
| [subscribeByMail](../api/group-subscribebymail.md)                          | Nenhum                                                       | Definir a propriedade isSubscribedByMail como **true**. Permitir que o usuário conectado receba conversas por email. Com suporte apenas para grupos do Office 365.                                                                |
| [unsubscribeByMail](../api/group-unsubscribebymail.md)                      | Nenhum                                                       | Definir a propriedade isSubscribedByMail como **false**. Desabilitar o recebimento de conversas por email do usuário conectado. Com suporte apenas para grupos do Office 365.                                                            |
| [resetUnseenCount](../api/group-resetunseencount.md)                        | Nenhum                                                       | Redefinir unseenCount como 0 para todas as postagens que o usuário conectado não tenha visto desde a última visita. Com suporte apenas para grupos do Office 365.                                                                    |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|allowExternalSenders|Booliano| Indica se as pessoas externas à empresa podem enviar mensagens para o grupo. O valor padrão é **false**. <br><br>Retornado apenas em $select. |
|assignedLicenses|Coleção [assignedLicense](assignedlicense.md)|As licenças que são atribuídas ao grupo. <br><br>Retornado apenas em $select. Somente leitura.|
|autoSubscribeNewMembers|Booliano|Indica se novos membros adicionados ao grupo serão automaticamente inscritos para receberem notificações por email. Você pode definir essa propriedade em uma solicitação PATCH para o grupo. Não a defina na solicitação POST inicial que cria esse grupo. O valor padrão é **false**. <br><br>Retornado apenas em $select.|
|classificação|String|Describes a classification for the group (such as low, medium or high business impact). Valid values for this property are defined by creating a ClassificationList [setting](groupsetting.md) value, based on the [template definition](groupsettingtemplate.md).<br><br>Retornado por padrão.|
|createdDateTime|DateTimeOffset| Carimbo de data/hora da ocasião em que o grupo foi criado. Não é possível modificar o valor e ele é preenchido automaticamente quando o grupo é criado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. <br><br>Retornado por padrão. Somente leitura. |
|deletedDateTime|DateTimeOffset| Para alguns objetos do Azure Active Directory (usuário, grupo, aplicativo), se o objeto for excluído, ele será excluído primeiro logicamente e essa propriedade será atualizada com a data e a hora em que o objeto foi excluído. Caso contrário, essa propriedade é nula. Se o objeto for restaurado, essa propriedade será atualizada para nula. |
|description|String|Uma descrição opcional para o grupo. <br><br>Retornado por padrão.|
|displayName|String|O nome de exibição do grupo. Essa propriedade é obrigatória quando um grupo é criado e não pode ser apagado durante as atualizações. <br><br>Retornado por padrão. Oferece suporte a $filter e $orderby. |
|groupTypes|Coleção de cadeias de caracteres| Especifica o tipo de grupo e sua associação.  <br><br>Se a coleção contiver `Unified`, o grupo será um grupo do Office 365; caso contrário, será um grupo de segurança.  <br><br>Se a coleção inclui `DynamicMembership`, o grupo tem associação dinâmica; caso contrário, a associação é estática.  <br><br>Retornado por padrão. Oferece suporte a $filter.|
|hasMembersWithLicenseErrors|Booliano|Indica se existem membros neste grupo com erros de licença da sua atribuição de licença baseada em grupo. <br><br>Esta propriedade nunca é retornada em uma operação GET. Você pode usá-lo como um argumento $filter para acessar os grupos que têm membros com erros de licença (ou seja, o filtro para essa propriedade é true). Veja um [exemplo](../api/group-list.md).|
|hideFromAddressLists |Boleano |Verdadeiro se o grupo não for exibido em certas partes da interface do usuário do Outlook: **Catálogo de endereços**, listas de endereços para selecionar os destinatários da mensagem e na caixa de diálogo **Procurar grupos** para pesquisar grupos; caso contrário, falso. O valor padrão é **false**. <br><br>Retornado apenas em $select.|
|hideFromOutlookClients |Boolean |Verdadeiro se o grupo não for exibido nos clientes do Outlook, como Outlook para Windows e Outlook na Web; caso contrário, falso. O valor padrão é **false**. <br><br>Retornado apenas em $select.|
|id|Cadeia de caracteres|O identificador exclusivo do grupo. <br><br>Retornado por padrão. Herdado de [directoryObject](directoryobject.md). Chave. Não anulável. Somente leitura.|
|isSubscribedByMail|Boolean|Indica se o usuário conectado está inscrito para receber conversas de email. O valor padrão é **true**. <br><br>Retornado apenas em $select. |
|licenseProcessingState|String|Indica o status da atribuição de licença de grupo para todos os membros do grupo. O valor padrão é **false**. Somente leitura. Valores possíveis: `QueuedForProcessing`, `ProcessingInProgress` e `ProcessingComplete`.<br><br>Retornado apenas em $select. Somente leitura.|
|email|Cadeia de caracteres|O endereço SMTP do grupo, por exemplo, "serviceadmins@contoso.onmicrosoft.com". <br><br>Retornado por padrão. Apenas leitura. Oferece suporte a $filter.|
|mailEnabled|Boolean|Especifica se o grupo está habilitado para email. <br><br>Retornado por padrão.|
|mailNickname|String|O alias de email do grupo, exclusivo na organização. Essa propriedade deve ser especificada quando um grupo é criado. <br><br>Retornado por padrão. Oferece suporte a $filter.|
|onPremisesDomainName|String|Contém o **nome de domínio totalmente qualificado (FQDN)** local, também chamado de **dnsDomainName** sincronizado no diretório local. A propriedade somente é preenchida para os clientes que estejam sincronizando o seu diretório local com o Azure Active Directory pelo Azure AD Connect.<br><br>Retornado por padrão. Apenas leitura. |
|onPremisesLastSyncDateTime|DateTimeOffset|Indica a última vez em que o grupo foi sincronizado com o diretório local. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. <br><br>Retornado por padrão. Apenas leitura. Oferece suporte a $filter.|
|onPremisesNetBiosName|String|Contém o **netBios name** local sincronizado no diretório local. A propriedade somente é preenchida para os clientes que estejam sincronizando o seu diretório local com o Azure Active Directory pelo Azure AD Connect.<br><br>Retornado por padrão. Somente leitura. |
|onPremisesProvisioningErrors|coleção [OnPremisesProvisioningError](onpremisesprovisioningerror.md)| Erros ao usar o produto de sincronização da Microsoft durante a configuração. <br><br>Retornado por padrão.|
|onPremisesSamAccountName|Cadeia de Caracteres|Contém o **nome da conta SAM** local sincronizado no diretório local. A propriedade somente é preenchida para os clientes que estejam sincronizando o seu diretório local com o Azure Active Directory pelo Azure AD Connect.<br><br>Retornado por padrão. Apenas leitura. |
|onPremisesSecurityIdentifier|String|Contém o identificador de segurança (SID) local do grupo que foi sincronizado do local com a nuvem. <br><br>Retornado por padrão. Apenas leitura. |
|onPremisesSyncEnabled|Booliano|**True** se esse grupo está sincronizado de um diretório local; **false** se esse grupo foi originalmente sincronizado de um diretório local, mas não está mais sincronizado; **null** se esse objeto nunca foi sido sincronizado de um diretório local (padrão). <br><br>Retornado por padrão. Apenas leitura. Oferece suporte a $filter.|
|preferredDataLocation|String|O local de data preferido para o grupo. Saiba mais em [OneDrive Online com Multi-Geo](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction). <br><br>Retornado por padrão.|
|proxyAddresses|String collection| Endereços de email para o grupo que direcionam para a mesma caixa de correio do grupo. Por exemplo: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]`. O operador **any** é obrigatório para filtrar expressões em propriedades de vários valores. <br><br>Retornado por padrão. Apenas leitura. Não anulável. Oferece suporte a $filter. |
|renewedDateTime|DateTimeOffset| Carimbo de data/hora da ocasião em que o grupo foi renovado pela última vez. Não é possível modificar isso diretamente e a atualização ocorre apenas por meio da [ação de renovação de serviço](../api/group-renew.md). O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. <br><br>Retornado por padrão. Apenas leitura.|
|securityEnabled|Boolean|Especifica se o grupo é um grupo de segurança. <br><br>Retornado por padrão. Oferece suporte a $filter.|
|securityIdentifier|Cadeia de Caracteres|Identificador de segurança do grupo, usado em cenários do Windows. <br><br>Retornado por padrão.|
|unseenCount|Int32|Contagem das conversas que receberam novas postagens desde que o usuário conectado visitou o grupo pela última vez. <br><br>Retornado apenas em $select. |
|visibility|String| Especifica a visibilidade de um grupo do Office 365. Valores possíveis são: `Private`, `Public`, ou `Hiddenmembership`; valores em branco são tratados como públicos.  Saiba mais em [Opções de visibilidade do grupo](#group-visibility-options).<br>A visibilidade só pode ser configurada quando um grupo é criado, ela não é editável.<br>A visibilidade tem suporte apenas para grupos unificados; Não há suporte para grupos de segurança. <br><br>Retornado por padrão.|


### <a name="group-visibility-options"></a>Opções de visibilidade do grupo

Veja o que cada valor da propriedade de **visibilidade** significa:

|Valor|Descrição|
|:----|-----------|
| Público | Qualquer pessoa pode ingressar no grupo sem precisar de permissão de proprietário.<br>Qualquer pessoa pode exibir o conteúdo do grupo.|
| Privado | A permissão de proprietário é necessária para ingressar no grupo.<br>Não membros não podem exibir o conteúdo do grupo.|
| Hiddenmembership | A permissão de proprietário é necessária para ingressar no grupo.<br>Não membros não podem exibir o conteúdo do grupo.<br>Não membros não podem ver os membros do grupo.<br>Administradores (global, empresa, usuário e helpdesk) podem visualizar a associação do grupo.<br>O grupo aparece no catálogo de endereços global (GAL).|


## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|acceptedSenders|Coleção [directoryObject](directoryobject.md)|The list of users or groups that are allowed to create post's or calendar events in this group. If this list is non-empty then only users or groups listed here are allowed to post.|
|calendário|[calendar](calendar.md)|The group's calendar. Read-only.|
|calendarView|Coleção [event](event.md)|The calendar view for the calendar. Read-only.|
|conversations|Coleção [conversation](conversation.md)|As conversas do grupo.|
|createdOnBehalfOf|[directoryObject](directoryobject.md)| The user (or application) that created the group. NOTE: This is not set if the user is an administrator. Read-only.|
|Unidade|[unidade](drive.md)|Unidade padrão do grupo. Somente leitura.|
|unidades|Coleção [drive](drive.md)|As unidades do grupo. Somente leitura.|
|events|Coleção [event](event.md)|Os eventos de calendário do grupo.|
|extensions|Coleção [extension](extension.md)|The collection of open extensions defined for the group. Read-only. Nullable.|
|groupLifecyclePolicies|Coleção [groupLifecyclePolicy](grouplifecyclepolicy.md)|O conjunto de políticas de ciclo de vida para esse grupo. Somente leitura. Anulável.|
|memberOf|Coleção [directoryObject](directoryobject.md)|Groups that this group is a member of. HTTP Methods: GET (supported for all groups). Read-only. Nullable.|
|membros|Coleção [directoryObject](directoryobject.md)| Users and groups that are members of this group. HTTP Methods: GET (supported for all groups), POST (supported for Office 365 groups, security groups and mail-enabled security groups), DELETE (supported for Office 365 groups and security groups) Nullable.|
|membersWithLicenseErrors|Coleção [user](user.md)|Uma lista de membros do grupo com erros de licença desse grupo baseado em atribuição de licença. Somente leitura.|
|onenote|[Onenote](onenote.md)| Somente leitura.|
|owners|[directoryObject](directoryobject.md) collection|Os proprietários do grupo. Os proprietários são um conjunto de usuários não administradores e que têm permissão para modificar esse objeto. Limitado a 100 proprietários. Métodos HTTP: GET (com suporte para todos os grupos), POST (com suporte para grupos do Office 365, grupos de segurança e grupos de segurança habilitados para email), DELETE (com suporte para grupos do Office 365 e grupos de segurança). Anulável.|
|photo|[profilePhoto](profilephoto.md)| A foto de perfil do grupo |
|fotos|Coleção [profilePhoto](profilephoto.md)| The profile photos owned by the group. Read-only. Nullable.|
|planejador|[plannerGroup](plannergroup.md)| Ponto de entrada para o recurso Planejador que pode existir para um Grupo unificado.|
|rejectedSenders|Coleção [directoryObject](directoryobject.md)|The list of users or groups that are not allowed to create posts or calendar events in this group. Nullable|
|configurações|Conjunto [groupSetting](groupsetting.md)| Read-only. Nullable.|
|sites|conjunto de [sites](site.md)|The list of SharePoint sites in this group. Access the default site with /sites/root.|
|threads|Coleção [conversationThread](conversationthread.md)| The group's conversation threads. Nullable.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true,
  "optionalProperties": [
    "acceptedSenders",
    "appRoleAssignments",
    "calendar",
    "calendarView",
    "conversations",
    "createdOnBehalfOf",
    "drive",
    "drives",
    "events",
    "extensions",
    "groupLifecyclePolicies",
    "memberOf",
    "members",
    "onenote",
    "owners",
    "photo",
    "photos",
    "planner",
    "rejectedSenders",
    "settings",
    "sites",
    "threads",

    "allowExternalSenders",
    "assignedLicenses",
    "autoSubscribeNewMembers",
    "hasMembersWithLicenseErrors",
    "isSubscribedByMail",
    "licenseProcessingState",
    "unseenCount"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.group",
  "@odata.annotations": [
    {
      "capabilities": {
        "changeTracking": true
      }
    },
    {
      "property": "acceptedSenders",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false,
        "updatable": false
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
      "property": "calendarView",
      "capabilities": {
        "changeTracking": true,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "conversations",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "updatable": false
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
    },
    {
      "property": "rejectedSenders",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "threads",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "allowExternalSenders": false,
  "assignedLicenses": [{"@odata.type": "microsoft.graph.assignedLicense"}],
  "autoSubscribeNewMembers": true,
  "classification": "string",
  "createdDateTime": "String (timestamp)",
  "description": "string",
  "displayName": "string",
  "groupTypes": ["string"],
  "hasMembersWithLicenseErrors": "Boolean",
  "hideFromAddressLists": false,
  "hideFromOutlookClients": false,
  "id": "string (identifier)",
  "isSubscribedByMail": true,
  "licenseProcessingState": "string",
  "mail": "string",
  "mailEnabled": true,
  "mailNickname": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
  "preferredDataLocation": "string",
  "proxyAddresses": ["string"],
  "renewedDateTime": "String (timestamp)",
  "securityEnabled": true,
  "securityIdentifier": "String",
  "unseenCount": 1024,
  "visibility": "string",
  "acceptedSenders": [ { "@odata.type": "microsoft.graph.directoryObject"} ],
  "calendar": { "@odata.type": "microsoft.graph.calendar" },
  "calendarView": [{ "@odata.type": "microsoft.graph.event" }],
  "conversations": [ { "@odata.type": "microsoft.graph.conversation" }],
  "createdOnBehalfOf": { "@odata.type": "microsoft.graph.directoryObject" },
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "events": [ { "@odata.type": "microsoft.graph.event" }],
  "memberOf": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "members": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "membersWithLicenseErrors": [{"@odata.type": "microsoft.graph.user"}],
  "owners": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "photo": { "@odata.type": "microsoft.graph.profilePhoto" },
  "rejectedSenders": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "sites": [ { "@odata.type": "microsoft.graph.site" } ],
  "threads": [ { "@odata.type": "microsoft.graph.conversationThread" }]
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
  "description": "group resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
