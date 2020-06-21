---
title: Problemas conhecidos com o Microsoft Graph
description: Este artigo descreve os problemas conhecidos do Microsoft Graph.
author: MSGraphDocsVTeam
localization_priority: Priority
ms.openlocfilehash: 98c61991ec99b1f7776c03f5fa5bc2400b5950a6
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/16/2020
ms.locfileid: "44744052"
---
# <a name="known-issues-with-microsoft-graph"></a>Problemas conhecidos com o Microsoft Graph

Este artigo descreve os problemas conhecidos do Microsoft Graph. 

Para relatar um problema conhecido, confira a página de [suporte do Microsoft Graph](https://developer.microsoft.com/graph/support) .

Para obter informações sobre as atualizações mais recentes para a API do Microsoft Graph, consulte o [changelog do Microsoft Graph](changelog.md).

## <a name="bookings"></a>Reservas

### <a name="errorexceededfindcountlimit-when-querying-bookingbusinesses"></a>ErrorExceededFindCountLimit ao consultar bookingBusinesses

A obtenção da lista de `bookingBusinesses` falha com o seguinte código de erro quando a organização tem várias empresas de Reservas e a conta que está fazendo a solicitação não é um administrador:

```json
{
  "error": {
    "code": "ErrorExceededFindCountLimit",
    "message":
      "The GetBookingMailboxes request returned too many results. Please specify a query to limit the results.",
  }
}
```

Como alternativa, você pode limitar o conjunto de empresas retornadas pela solicitação, incluindo um parâmetro `query`, por exemplo:

```
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Fabrikam
```
## <a name="calendars"></a>Calendários

### <a name="accessing-a-shared-calendar"></a>Acessar um calendário compartilhado

Ao tentar acessar eventos em um calendário compartilhado por outro usuário usando a operação a seguir:

```http
GET /users/{id}/calendars/{id}/events
```

You may get HTTP 500 with the error code `ErrorInternalServerTransientError`. The error occurs because:

- Historicamente, há duas maneiras de compartilhar o calendário, que são chamadas de "antiga" e "nova" abordagens, para fins de diferenciá-las.
- A nova abordagem está disponível atualmente para compartilhamento de calendários, com permissões de exibição ou edição, mas não com permissões de representante.
- Você pode usar a API REST de calendário para exibir ou editar calendários compartilhados somente quando os calendários são compartilhados de acordo com a **nova** abordagem.
- Não é possível usar a API REST de calendário para exibir ou editar esses calendários ou os respectivos eventos quando eles são compartilhados de acordo com a **antiga** abordagem.


Se você compartilhar o calendário com permissões de exibição ou edição usando a abordagem antiga, poderá resolver o problema e atualizar manualmente o compartilhamento do calendário para usar a nova abordagem.
Com o tempo, o Outlook atualizará automaticamente todos os calendários compartilhados para usar a nova abordagem, incluindo calendários compartilhados com permissões delegadas.

Para atualizar manualmente um calendário compartilhado e usar a nova abordagem, faça os seguintes procedimentos:
1.  O destinatário remove o calendário previamente compartilhado com ele.
2.  O proprietário compartilha novamente o calendário no Outlook na Web, no Outlook para iOS ou no Outlook para Android.
3.  The recipient re-accepts the shared calendar using Outlook on the web. (It will be possible to use other Outlook clients soon.)
4.  O destinatário verifica se o calendário foi compartilhado novamente com êxito por meio da nova abordagem, com permissão para exibi-lo no Outlook para iOS ou no Outlook para Android.

A calendar shared with you in the new approach appears as just another calendar in your mailbox. You can use the calendar REST API to view or edit events in the shared calendar, as if it's your own calendar. As an example:

```http
GET /me/calendars/{id}/events
```

### <a name="adding-and-accessing-ics-based-calendars-in-users-mailbox"></a>Adicionar e acessar calendários baseados em ICS na caixa de correio do usuário

Atualmente, há suporte parcial para um calendário com base em uma Inscrição em Calendário da Internet (ICS):

* Você pode adicionar um calendário baseado em ICS para uma caixa de correio do usuário por meio da interface do usuário, mas não através da API do Microsoft Graph.
* [Listing the user's calendars](/graph/api/user-list-calendars?view=graph-rest-1.0) lets you get the **name**, **color** and **id** properties of each [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) in the user's default calendar group, or a specified calendar group, including any ICS-based calendars. You cannot store or access the ICS URL in the calendar resource.
* Você também pode [listar os eventos](/graph/api/calendar-list-events?view=graph-rest-1.0) de um calendário baseado em ICS.

### <a name="attaching-large-files-to-events"></a>Anexar arquivos grandes a eventos
Um aplicativo com permissões delegadas retorna `HTTP 403 Forbidden` ao tentar [anexar arquivos grandes](outlook-large-attachments.md) a uma mensagem ou evento do Outlook que está em uma caixa de correio compartilhada ou delegada. Com as permissões delegadas, [createUploadSession](/graph/api/attachment-createuploadsession?view=graph-rest-1.0) só é bem sucedida se a mensagem ou o evento estiver na caixa de correio do usuário conectado.

### <a name="onlinemeetingurl-property-support-for-microsoft-teams"></a>Suporte de propriedade onlineMeetingUrl do Microsoft Teams

Atualmente, a propriedade **onlineMeetingUrl** de um [evento](/graph/api/resources/event?view=graph-rest-1.0) de reunião do Skype indica a URL da reunião online. No entanto, essa propriedade para um evento de reunião do Microsoft Teams está definida como nula.

A versão beta oferece uma solução alternativa, na qual é possível usar a propriedade **onlineMeetingProvider** de um [evento](/graph/api/resources/event?view=graph-rest-beta)para verificar se o provedor é o Microsoft Teams. Por meio da propriedade **onlineMeeting** do **evento**, você pode acessar o **joinUrl**.

## <a name="change-notifications"></a>Notificações de alteração

### <a name="additional-notifications-for-users"></a>Notificações adicionais para usuários

As [assinaturas](/graph/api/resources/subscription) de alterações para o **usuário** com o **changeType** definido como **atualizado** também receberão notificações de **changeType**: **atualizado** na criação do usuário e exclusão reversível do usuário.

### <a name="additional-notifications-for-groups"></a>Notificações adicionais para grupos

As [assinaturas](/graph/api/resources/subscription) de alterações no **grupo** com o **changeType** definido como **atualizado** também receberão notificações **changeType**: **atualizado** na criação do grupo e exclusão reversível do grupo.

## <a name="cloud-communications"></a>Comunicações na nuvem 

O cliente do Microsoft Teams não mostra o menu **Exibir detalhes da Reunião** para reuniões de canal criadas por meio da API de comunicações na nuvem.

## <a name="cloud-solution-provider-apps"></a>Aplicativos de Provedor de Soluções na Nuvem

### <a name="csp-apps-must-use-azure-ad-endpoint"></a>Os aplicativos CSP devem usar o ponto de extremidade do Azure AD

Cloud solution provider (CSP) apps must acquire tokens from the Azure AD (v1) endpoints to successfully call Microsoft Graph in their partner-managed customers. Currently, acquiring a token through the newer Azure AD v2.0 endpoint is not supported.

### <a name="pre-consent-for-csp-apps-doesnt-work-in-some-customer-tenants"></a>A pré-autorização para aplicativos CSP não funciona em alguns locatários do cliente

Sob certas circunstâncias, o pré-consentimento para aplicativos CSP pode não funcionar para alguns de seus locatários de clientes.

- Para aplicativos que usam permissões delegadas, ao usar o aplicativo pela primeira vez com um novo locatário do cliente, você poderá receber esse erro após o logon: `AADSTS50000: There was an error issuing a token`.
- Para aplicativos que usam permissões de aplicativos, seu aplicativo pode adquirir um token, mas inesperadamente receber uma mensagem de acesso negado ao chamar o Microsoft Graph.

Estamos trabalhando para corrigir esse problema o mais rápido possível, de modo que a pré-autorização funcionará para todos os seus locatários de clientes.

Enquanto isso, para desbloquear o desenvolvimento e testes, você pode usar a seguinte solução alternativa.

>**NOTE:** This is not a permanent solution and is only intended to unblock development.  This workaround will not be required once the aforementioned issue is fixed.  This workaround does not need to be undone once the fix is in place.

1. Open an Azure AD v2 PowerShell session and connect to your `customer` tenant by entering your admin credentials into the sign-in window. You can download and install Azure AD PowerShell V2 from [here](https://www.powershellgallery.com/packages/AzureAD).

    ```PowerShell
    Connect-AzureAd -TenantId {customerTenantIdOrDomainName}
    ```

2. Crie o servicePrincipal do Microsoft Graph.

    ```PowerShell
    New-AzureADServicePrincipal -AppId 00000003-0000-0000-c000-000000000000
    ```
## <a name="contacts"></a>Contatos

### <a name="organization-contacts-available-in-only-beta"></a>Contatos de organização disponíveis somente na versão beta

Only personal contacts are currently supported. Organizational contacts are not currently supported in `/v1.0`, but can be found in `/beta`.

### <a name="default-contacts-folder"></a>Pasta Contatos padrão

Na versão `/v1.0`, `GET /me/contactFolders` não inclui a pasta de contatos do usuário padrão.

A fix will be made available. Meanwhile, you can use the following [list contacts](/graph/api/user-list-contacts?view=graph-rest-1.0) query and the **parentFolderId** property as a workaround to get the folder ID of the default contacts folder:

```http
GET https://graph.microsoft.com/v1.0/me/contacts?$top=1&$select=parentFolderId
```

Na consulta acima:

1. `/me/contacts?$top=1` obtém as propriedades de um [contato](/graph/api/resources/contact?view=graph-rest-1.0) na pasta de contatos padrão.
2. A anexação de `&$select=parentFolderId` retorna apenas a propriedade **parentFolderId** do contato, que é a ID da pasta de contatos padrão.


### <a name="accessing-contacts-via-a-contact-folder-in-beta"></a>Acessar contatos por meio de uma pasta de contatos na versão beta

Atualmente, não há na versão `/beta` um problema que impeça o acesso a um [contato](/graph/api/resources/contact?view=graph-rest-beta) especificando sua pasta pai na URL de solicitação REST, conforme mostrado nos dois cenários abaixo.

* Acessando um contato a partir de um nível superior do [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-beta) do usuário.

```http
GET /me/contactfolders/{id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```

* Accessing a contact contained in a child folder of a **contactFolder**.  The example below shows one level of nesting, but a contact can be located in a child of a child and so on.

```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```

Como alternativa, você pode simplesmente [obter](/graph/api/contact-get?view=graph-rest-beta) o contato, especificando sua identificação conforme mostrado abaixo, uma vez que o GET /contacts na versão `/beta` se aplica a todos os contatos na caixa de correio do usuário:

```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
## <a name="delta-query"></a>Consulta delta

* O contexto de OData às vezes é retornado incorretamente ao controlar alterações nas relações.
* As extensões de esquema (herdadas) não são retornadas com instrução $select, mas são retornadas sem $select.
* Os clientes não podem controlar alterações em extensões abertas ou extensões de esquema.

## <a name="extensions"></a>Extensões

### <a name="change-tracking-is-not-supported"></a>Não há suporte para o controle de alterações

O controle de alterações (consulta delta) não tem suporte nas propriedades de extensão do esquema ou abrir.

### <a name="creating-a-resource-and-open-extension-at-the-same-time"></a>Criar um recurso e uma extensão aberta ao mesmo tempo

You cannot specify an open extension at the same time you create an instance of **administrativeUnit**, **device**, **group**, **organization** or **user**. You must first create the instance and then specify the open extension data in a subsequent ``POST`` request on that instance.

### <a name="creating-a-resource-instance-and-adding-schema-extension-data-at-the-same-time"></a>Criar uma instância de recurso e adicionar dados de extensão de esquema ao mesmo tempo

Não é possível especificar uma extensão de esquema na mesma operação, como criar uma instância de **contato**, **evento**, **mensagem** ou **postagem**.
Você deve primeiro criar a instância de recurso e, em seguida, fazer um `PATCH` para essa instância para adicionar uma extensão de esquema e dados personalizados.

### <a name="limit-of-100-schema-extension-property-values-allowed-per-resource-instance"></a>Limite de 100 valores de propriedade de extensão de esquema permitido por instância de recursos

Recursos de diretório, como **dispositivo**, **grupo** e **usuário**, atualmente limitam o número total de valores de propriedade de extensão de esquema que podem ser definidas em um recurso, até 100.

### <a name="filtering-on-schema-extension-properties-not-supported-on-all-entity-types"></a>Não há suporte a filtragem em propriedades de extensão de esquema em todos os tipos de entidade

Não há suporte a filtragem em propriedades de extensão de esquema (usando a expressão `$filter`) para tipos de entidade do Outlook – **contato**, **evento**, **mensagem** ou **postagem**.

## <a name="files-onedrive"></a>Arquivos (OneDrive)

* O primeiro acesso a uma unidade pessoal de um usuário pelo Microsoft Graph antes que ele acesse o próprio site pessoal por um navegador resulta em uma resposta 401.

## <a name="groups"></a>Grupos

### <a name="permissions-for-groups-and-microsoft-teams"></a>Permissões para grupos e Microsoft Teams

O Microsoft Graph expõe duas permissões ([*Group.Read.All*](permissions-reference.md#group-permissions) e [*Group.ReadWrite.All*](permissions-reference.md#group-permissions)) para obter acesso a APIs de grupos e Microsoft Teams.
As permissões do aplicativo devem ser consentidas por um administrador.
No futuro, pretendemos adicionar novas permissões para grupos e equipes que possam ser consentidas pelos usuários.

Also, only the API for core group administration and management supports access using delegated or app-only permissions. All other features of the group API support only delegated permissions.

Exemplos de recursos de grupo que oferecem suporte a permissões delegadas e somente para aplicativos:

* Criar e excluir grupos
* Obter e atualizar propriedades do grupo pertencentes ao gerenciamento ou administração de grupo
* [Definições do diretório](/graph/api/resources/directoryobject?view=graph-rest-1.0), tipo e sincronização do grupo
* Membros e proprietários de grupo
* Obtendo conversas de grupo e threads

Exemplos de recursos de grupo que oferecem suporte somente a permissões delegadas:

* Agrupar eventos, foto
* Remetentes externos, remetentes aceitos ou rejeitados e assinatura de grupo
* Favoritos do usuário e contagem de não vistos

### <a name="policy"></a>Política

O uso do Microsoft Graph para criar e nomear um grupo do Office 365 ultrapassa qualquer política de grupo do Office 365 que seja configurada pelo Outlook Web App.

### <a name="setting-the-allowexternalsenders-property"></a>Definir a propriedade allowExternalSenders

Atualmente, há um problema que impede a configuração da propriedade **allowExternalSenders** de um grupo em uma operação de POST ou PATCH no `/v1.0` e no `/beta`.

### <a name="using-delta-query"></a>Uso da consulta delta

Para saber mais sobre problemas conhecidos com o uso da consulta delta, veja a [seção da consulta delta](#delta-query) deste artigo.

## <a name="identity-and-access--application-and-service-principal-apis"></a>Identidade e acesso | APIs da entidade de serviço e aplicativo

There are changes to the [application](/graph/api/resources/application?view=graph-rest-beta) and [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) entities currently in development. The following is a summary of current limitations and in-development API features.

Limitações atuais:

* Algumas propriedades do aplicativo (como appRoles e addIns) não estarão disponíveis até que todas as alterações sejam concluídas.
* Somente aplicativos multilocatários podem ser registrados.
* Atualizar aplicativos é restrito aos aplicativos registrados após a atualização inicial beta.
* Usuários do Azure Active Directory podem registrar aplicativos e adicionar proprietários adicionais.
* Suporte para protocolos OpenID Connect e OAuth.
* Atribuições de política para uma falha de aplicativo.
* Falha em operações em ownedObjects que exigem appId (por exemplo, users/{id|userPrincipalName}/ownedObjects/{id}/...).

Em desenvolvimento:

* Capacidade de registrar aplicativos de um único locatário.
* Atualizações para o servicePrincipal.
* Migração de aplicativos Azure AD existentes para um modelo atualizado.
* Suporte para appRoles, clientes pré-autorizados, reivindicações opcionais, reivindicações de associação de grupo e identidade visual.
* Os usuários de conta Microsoft (MSA) podem registrar aplicativos.
* Suporte para protocolos SAML e WsFed.

## <a name="identity-and-access--conditional-access"></a>Identidade e acesso | Acesso condicional

### <a name="permissions"></a>Permissões

Atualmente, a permissão Policy.Read.All é necessária para chamar as APIs POST e PATCH. No futuro, a permissão Policy.ReadWrite.ConditionalAccess possibilitará que você leia as políticas do diretório.

## <a name="json-batching"></a>Envio em lote JSON

### <a name="no-nested-batch"></a>Nenhum lote aninhado

Solicitações de lote JSON não devem conter quaisquer solicitações em lotes aninhados.

### <a name="all-individual-requests-must-be-synchronous"></a>Todas as solicitações individuais devem ser síncronas

All requests contained in a batch request must be executed synchronously. If present, the `respond-async` preference will be ignored.

### <a name="no-transactions"></a>Sem transações

Microsoft Graph does not currently support transactional processing of individual requests. The `atomicityGroup` property on individual requests will be ignored.

### <a name="uris-must-be-relative"></a>URIs devem ser relativas

Always specify relative URIs in batch requests. Microsoft Graph then makes these URLs absolute by using the version endpoint included in the batch URL.

### <a name="limit-on-batch-size"></a>Limite de tamanho de lote

No momento, as solicitações de lote JSON estão limitadas a 20 solicitações individuais.

### <a name="simplified-dependencies"></a>Dependências simplificadas

Individual requests can depend on other individual requests. Currently, requests can only depend on a single other request, and must follow one of these three patterns:

1. Paralelo – nenhuma solicitação individual declara uma dependência na propriedade `dependsOn`.
2. Serial – todas as solicitações individuais dependem da solicitação individual anterior.
3. Mesmo – todas as solicitações individuais indicam que uma dependência na propriedade `dependsOn` declaram a mesma dependência.

Conforme o processamento em lotes JSON amadurece, essas limitações são removidas.

## <a name="mail-outlook"></a>Email (Outlook)

### <a name="attaching-large-files-to-messages"></a>Anexando grandes arquivos a mensagens
Um aplicativo com permissões delegadas retorna `HTTP 403 Forbidden` ao tentar [anexar arquivos grandes](outlook-large-attachments.md) a uma mensagem ou evento do Outlook que está em uma caixa de correio compartilhada ou delegada. Com as permissões delegadas, [createUploadSession](/graph/api/attachment-createuploadsession?view=graph-rest-1.0) só é bem sucedida se a mensagem ou o evento estiver na caixa de correio do usuário conectado.

### <a name="the-comment-parameter-for-creating-a-draft"></a>O parâmetro de comentário para criar um rascunho

O parâmetro **comment** para criar uma resposta ou rascunho de encaminhamento ([createReply](/graph/api/message-createreply?view=graph-rest-1.0), [createReplyAll](/graph/api/message-createreplyall?view=graph-rest-1.0), [createForward](/graph/api/message-createforward?view=graph-rest-1.0)) não se torna parte do corpo do rascunho de mensagem resultante.

### <a name="get-messages-returns-chats-in-microsoft-teams"></a>As mensagens GET retornam chats no Microsoft Teams

Em pontos de extremidade beta e v1, a resposta de `GET /users/id/messages` inclui chats do usuário no Microsoft Teams que ocorreu fora do escopo de uma equipe ou de um canal. Essas mensagens de chat tem "IM" como o assunto.

## <a name="teamwork-microsoft-teams"></a>Trabalho em equipe (Microsoft Teams)

### <a name="get-teams-is-not-supported"></a>GET /teams não tem suporte

Para obter uma lista de equipes, confira [listar todas as equipes](teams-list-all-teams.md) e [listar suas equipes](/graph/api/user-list-joinedteams?view=graph-rest-1.0).

### <a name="post-teams-is-only-available-in-beta"></a>POST /teams está disponível apenas na versão beta
Para criar equipes no v 1.0, confira [criar equipe](/graph/api/team-put-teams?view=graph-rest-1.0).

### <a name="missing-teams-in-list-all-teams"></a>Equipes ausentes em listas todas as equipes

Algumas equipes que foram criadas no passado mas não foram usadas recentemente por um usuário do Microsoft Teams não são listadas por [listar todas as equipes](teams-list-all-teams.md).
Novas equipes serão listadas.
Algumas equipes antigas não têm uma propriedade **resourceProvisioningOptions** que contém “Equipe”, que é configurada em equipes recém-criadas e equipes que são visitadas no Microsoft Teams.
No futuro, vamos configurar **resourceProvisioningOptions** em equipes existentes que não foram abertas no Microsoft Teams.

## <a name="users"></a>Usuários

### <a name="no-instant-access-after-creation"></a>Sem acesso instantâneo após a criação

Users can be created immediately through a POST on the user entity. An Office 365 license must first be assigned to a user, in order to get access to Office 365 services. Even then, due to the distributed nature of the service, it might take 15 minutes before files, messages and events entities are available for use for this user, through the Microsoft Graph API. During this time, apps will receive a 404 HTTP error response.

### <a name="photo-restrictions"></a>Restrições de foto

Reading and updating a user's profile photo is only possible if the user has a mailbox. Additionally, any photos that *may* have been previously stored using the **thumbnailPhoto** property (using the Office 365 unified API preview, or the Azure AD Graph, or through AD Connect synchronization) are no longer accessible through the Microsoft Graph **photo** property of the [user](/graph/api/resources/user?view=graph-rest-1.0) resource.
Failure to read or update a photo, in this case, would result in the following error:

```javascript
{
  "error": {
    "code": "ErrorNonExistentMailbox",
    "message": "The SMTP address has no mailbox associated with it."
  }
}
```

### <a name="using-delta-query"></a>Uso da consulta delta

Para saber mais sobre problemas conhecidos com o uso da consulta delta, veja a [seção da consulta delta](#delta-query) deste artigo.

### <a name="revoke-sign-in-sessions-returns-wrong-http-code"></a>A revogação de sessões de entrada retorna um código HTTP errado

O [usuário: revokeSignInSessions API](/graph/api/user-revokesigninsessions?view=graph-rest-1.0) deve retornar uma resposta `204 No content` para ter revogações bem-sucedidas e um código de erro HTTP (4xx ou 5xx) se algo der errado com a solicitação.  No entanto, devido a um problema de serviço, essa API retorna um parâmetro `200 OK` e um parâmetro booleano que é sempre true.  Até que isso seja corrigido, é recomendado que desenvolvedores simplesmente tratem qualquer código de retorno 2xx como bem-sucedido para esta API.

### <a name="incomplete-objects-when-using-getbyids-request"></a>Objetos incompletos ao usar a solicitação getByIds

A solicitação de objetos usando a opção de [Obter objetos de diretório de uma lista de IDs](/graph/api/directoryobject-getbyids?view=graph-rest-1.0) deve retornar objetos completos. No entanto, atualmente, os objetos de [usuário](/graph/api/resources/user?view=graph-rest-1.0) no ponto de extremidade v1.0 são retornados com um conjunto limitado de propriedades. Como solução temporária, ao usar a operação em combinação com a opção de consulta `$select`, objetos de [usuário](/graph/api/resources/user?view=graph-rest-1.0) mais completos serão retornados. Esse comportamento não está de acordo com as especificações do OData. Como esse comportamento pode ser atualizado no futuro, use esta solução alternativa apenas quando fornecer `$select=` com todas as propriedades de seu interesse e somente se futuras alterações nessa solução alternativa forem aceitáveis.

## <a name="query-parameter-limitations"></a>Limitações de parâmetro de consulta

* Não há suporte para vários namespaces.
* Não há suporte para GETs em `$ref` e conversão em usuários, grupos, dispositivos, entidades de serviço e aplicativos.
* `@odata.bind` is not supported.  This means that developers won’t be able to properly set the **acceptedSenders** or **rejectedSenders** navigation property on a group.
* `@odata.id` não está presente na navegação sem confinamento (como mensagens) quando há o uso de metadados mínimos.
* `$expand`:
  * Não há suporte para `nextLink`
  * Não há suporte para mais de um nível de expansão
  * Não há suporte com parâmetros adicionais (`$filter`, `$select`)
* `$filter`:
  * Não há suporte para filtros no ponto de extremidade `/attachments`. Se presente, o parâmetro `$filter` é ignorado.
  * Não há suporte para filtragem de carga de trabalho cruzada.
* `$search`:
  * A pesquisa de texto completo só está disponível para um subconjunto de entidades, como mensagens.
  * Não há suporte para pesquisa de carga de trabalho cruzada.


## <a name="functionality-available-only-in-office-365-rest-or-azure-ad-graph-apis"></a>Funcionalidade disponível apenas nas APIs Graph do Azure AD ou REST do Office 365

Alguns recursos ainda não estão disponíveis no Microsoft Graph. Se você não vir a funcionalidade que está procurando, poderá usar as [APIs REST do Office 365](https://docs.microsoft.com/previous-versions/office/office-365-api/) específicas do ponto de extremidade. Para o Azure Active Directory, confira [Migrar aplicativos do Azure AD Graph para o Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview). 
