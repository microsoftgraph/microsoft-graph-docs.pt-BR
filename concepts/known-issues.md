---
title: Problemas conhecidos com o Microsoft Graph
description: Este artigo descreve os problemas conhecidos com o Microsoft Graph.
author: MSGraphDocsVTeam
localization_priority: Priority
ms.openlocfilehash: 925baa0705d7747136f6dc1b60a9c34c72b59d7d
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58248132"
---
# <a name="known-issues-with-microsoft-graph"></a>Problemas conhecidos com o Microsoft Graph

Este artigo descreve os problemas conhecidos com o Microsoft Graph. 

Para relatar um problema conhecido, confira a página [Suporte Microsoft Graph](https://developer.microsoft.com/graph/support).

Para saber mais sobre as atualizações mais recentes da API do Microsoft Graph, confira o [changelog do Microsoft Graph](changelog.md).

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

```http
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Fabrikam
```
## <a name="calendars"></a>Calendários

### <a name="accessing-a-shared-calendar"></a>Acessar um calendário compartilhado

Ao tentar acessar eventos em um calendário compartilhado por outro usuário usando a operação a seguir:

```http
GET /users/{id}/calendars/{id}/events
```

Você pode receber HTTP 500 com o código de erro `ErrorInternalServerTransientError`. O erro ocorre porque:

- Historicamente, há duas maneiras de compartilhar o calendário, que são chamadas de "antiga" e "nova" abordagens, para fins de diferenciá-las.
- A nova abordagem está disponível atualmente para compartilhamento de calendários, com permissões de exibição ou edição, mas não com permissões de representante.
- Você pode usar a API REST de calendário para exibir ou editar calendários compartilhados somente quando os calendários são compartilhados de acordo com a **nova** abordagem.
- Não é possível usar a API REST de calendário para exibir ou editar esses calendários ou os respectivos eventos quando eles são compartilhados de acordo com a **antiga** abordagem.


Se você compartilhar o calendário com permissões de exibição ou edição usando a abordagem antiga, poderá resolver o problema e atualizar manualmente o compartilhamento do calendário para usar a nova abordagem.
Com o tempo, o Outlook atualizará automaticamente todos os calendários compartilhados para usar a nova abordagem, incluindo calendários compartilhados com permissões delegadas.

Para atualizar manualmente um calendário compartilhado e usar a nova abordagem, faça os seguintes procedimentos:
1.  O destinatário remove o calendário previamente compartilhado com ele.
2.  O proprietário compartilha novamente o calendário no Outlook na Web, no Outlook para iOS ou no Outlook para Android.
3.  O destinatário aceita novamente o calendário compartilhado usando o Outlook na Web. Em breve você poderá usar outros clientes do Outlook.
4.  O destinatário verifica se o calendário foi compartilhado novamente com êxito por meio da nova abordagem, com permissão para exibi-lo no Outlook para iOS ou no Outlook para Android.

Um calendário compartilhado com você na nova abordagem é exibido como qualquer outro na sua caixa de correio. Você pode usar a API REST de calendário para visualizar e editar eventos no calendário compartilhado, como se fosse seu próprio calendário. Como exemplo:

```http
GET /me/calendars/{id}/events
```

### <a name="adding-and-accessing-ics-based-calendars-in-users-mailbox"></a>Adicionar e acessar calendários baseados em ICS na caixa de correio do usuário

Atualmente, há suporte parcial para um calendário com base em uma Inscrição em Calendário da Internet (ICS):

* Você pode adicionar um calendário baseado em ICS para uma caixa de correio do usuário por meio da interface do usuário, mas não através da API do Microsoft Graph.
* [Listar os calendários do usuário](/graph/api/user-list-calendars) permite que você obtenha as propriedades **name**, **color** e **id** de cada [calendar](/graph/api/resources/calendar) no grupo de calendários padrão do usuário ou em um grupo de calendários especificado, inclusive todos os calendários com base em ICS. Não é possível armazenar ou acessar a URL da ICS no recurso de calendário.
* Você também pode [listar os eventos](/graph/api/calendar-list-events) de um calendário baseado em ICS.

### <a name="attaching-large-files-to-events"></a>Anexar arquivos grandes a eventos
Um aplicativo com permissões delegadas retorna `HTTP 403 Forbidden` ao tentar [anexar arquivos grandes](outlook-large-attachments.md) a uma mensagem ou evento do Outlook que está em uma caixa de correio compartilhada ou delegada. Com as permissões delegadas, [createUploadSession](/graph/api/attachment-createuploadsession) só é bem sucedida se a mensagem ou o evento estiver na caixa de correio do usuário conectado.

### <a name="onlinemeetingurl-property-support-for-microsoft-teams"></a>Suporte de propriedade onlineMeetingUrl do Microsoft Teams

Atualmente, a propriedade **onlineMeetingUrl** de um [evento](/graph/api/resources/event) de reunião do Skype indica a URL da reunião online. No entanto, essa propriedade para um evento de reunião do Microsoft Teams está definida como nula.

A versão beta oferece uma solução alternativa, na qual é possível usar a propriedade **onlineMeetingProvider** de um [evento](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true)para verificar se o provedor é o Microsoft Teams. Por meio da propriedade **onlineMeeting** do **evento**, você pode acessar o **joinUrl**.

## <a name="change-notifications"></a>Notificações de alteração

### <a name="additional-notifications-for-users"></a>Notificações adicionais para usuários

As [assinaturas](/graph/api/resources/subscription) de alterações para o **usuário** com o **changeType** definido como **atualizado** também receberão notificações de **changeType**: **atualizado** na criação do usuário e exclusão reversível do usuário.

### <a name="additional-notifications-for-groups"></a>Notificações adicionais para grupos

As [assinaturas](/graph/api/resources/subscription) de alterações no **grupo** com o **changeType** definido como **atualizado** também receberão notificações **changeType**: **atualizado** na criação do grupo e exclusão reversível do grupo.

## <a name="cloud-communications"></a>Comunicações na nuvem 

O cliente do Microsoft Teams não mostra o menu **Exibir detalhes da Reunião** para reuniões de canal criadas por meio da API de comunicações na nuvem.

## <a name="cloud-solution-provider-apps"></a>Aplicativos de Provedor de Soluções na Nuvem

### <a name="csp-apps-must-use-azure-ad-endpoint"></a>Os aplicativos CSP devem usar o ponto de extremidade do Azure AD

Aplicativos de provedor de solução de nuvem (CSP) devem adquirir tokens de pontos de extremidade do Azure AD (v1) para chamar a Microsoft Graph com êxito em seus clientes gerenciados por parceiros. Atualmente, não há suporte para aquisição de um token pelo ponto de extremidade Azure AD v 2.0 mais recente.

### <a name="pre-consent-for-csp-apps-doesnt-work-in-some-customer-tenants"></a>A pré-autorização para aplicativos CSP não funciona em alguns locatários do cliente

Sob certas circunstâncias, o pré-consentimento para aplicativos CSP pode não funcionar para alguns de seus locatários de clientes.

- Para aplicativos que usam permissões delegadas, ao usar o aplicativo pela primeira vez com um novo locatário do cliente, você poderá receber esse erro após o logon: `AADSTS50000: There was an error issuing a token`.
- Para aplicativos que usam permissões de aplicativos, seu aplicativo pode adquirir um token, mas inesperadamente receber uma mensagem de acesso negado ao chamar o Microsoft Graph.

Estamos trabalhando para corrigir esse problema o mais rápido possível, de modo que a pré-autorização funcionará para todos os seus locatários de clientes.

Enquanto isso, para desbloquear o desenvolvimento e testes, você pode usar a seguinte solução alternativa.

>**OBSERVAÇÃO:** esta não é uma solução permanente e destina-se apenas a desbloquear o desenvolvimento.  Esta solução alternativa não será necessária uma vez que a questão acima mencionada seja corrigida.  Esta solução alternativa não precisa ser desfeita após a correção.

1. Abra uma sessão do Azure AD v2 PowerShell e conecte-se ao locatário do parceiro `customer`digitando suas credenciais de administrador na janela de entrada. Você pode baixar e instalar o Azure AD PowerShell V2 [aqui](https://www.powershellgallery.com/packages/AzureAD).

    ```PowerShell
    Connect-AzureAd -TenantId {customerTenantIdOrDomainName}
    ```

2. Crie o servicePrincipal do Microsoft Graph.

    ```PowerShell
    New-AzureADServicePrincipal -AppId 00000003-0000-0000-c000-000000000000
    ```
## <a name="contacts"></a>Contatos

### <a name="organization-contacts-available-in-only-beta"></a>Contatos de organização disponíveis somente na versão beta

Somente os contatos pessoais têm suporte no momento. Os contatos organizacionais atualmente não têm suporte na `/v1.0`, mas podem ser encontrados na versão `/beta`.

### <a name="default-contacts-folder"></a>Pasta Contatos padrão

Na versão `/v1.0`, `GET /me/contactFolders` não inclui a pasta de contatos do usuário padrão.

Uma correção será disponibilizada. Enquanto isso, você pode usar a seguinte consulta [list contacts](/graph/api/user-list-contacts) e a propriedade **parentFolderId** como uma solução alternativa para obter a ID da pasta de contatos padrão:

```http
GET https://graph.microsoft.com/v1.0/me/contacts?$top=1&$select=parentFolderId
```

Na consulta acima:

1. `/me/contacts?$top=1` obtém as propriedades de um [contato](/graph/api/resources/contact) na pasta de contatos padrão.
2. A anexação de `&$select=parentFolderId` retorna apenas a propriedade **parentFolderId** do contato, que é a ID da pasta de contatos padrão.


### <a name="accessing-contacts-via-a-contact-folder-in-beta"></a>Acessar contatos por meio de uma pasta de contatos na versão beta

Atualmente, não há na versão `/beta` um problema que impeça o acesso a um [contato](/graph/api/resources/contact?view=graph-rest-beta&preserve-view=true) especificando sua pasta pai na URL de solicitação REST, conforme mostrado nos dois cenários abaixo.

* Acessando um contato a partir de um nível superior do [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-beta&preserve-view=true) do usuário.

```http
GET /me/contactfolders/{id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```

* Acessando um contato contido em uma pasta filha de um **contactFolder**.  O exemplo a seguir mostra um nível de aninhamento, mas um contato pode estar localizado em um filho de um filho e assim por diante.

```http
GET /me/contactFolders/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```

Como alternativa, você pode simplesmente [obter](/graph/api/contact-get?view=graph-rest-beta&preserve-view=true) o contato, especificando sua identificação conforme mostrado abaixo, uma vez que o GET /contacts na versão `/beta` se aplica a todos os contatos na caixa de correio do usuário:

```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
## <a name="delta-query"></a>Consulta delta

* O contexto de OData às vezes é retornado incorretamente ao controlar alterações nas relações.
* As extensões de esquema (herdadas) não são retornadas com instrução $select, mas são retornadas sem $select.
* Os clientes não podem controlar alterações em extensões abertas ou extensões de esquema.

## <a name="devices-and-apps--device-updates-windows-updates"></a>Dispositivos e aplicativos | Atualizações do dispositivo (atualizações do Windows)

### <a name="accessing-and-updating-deployment-audiences"></a>Acessando e atualizando audiências de implantação

Acessando e atualizando audiências de implantação em recursos de **implantação** criados por meio do Intune não são suportados atualmente.

* [Listando membros da audiência de implantação](/graph/api/windowsupdates-deploymentaudience-list-members) e [listando exclusões da audiência de implantação](/graph/api/windowsupdates-deploymentaudience-list-exclusions) retornos `404 Not Found`.
* [Atualizar membros da audiência de implantação e exclusões](/graph/api/windowsupdates-deploymentaudience-updateaudience) ou [atualizar por ID](/graph/api/windowsupdates-deploymentaudience-updateaudiencebyid) retorna `202 Accepted`, mas a audiência não é atualizada.

## <a name="extensions"></a>Extensões

### <a name="change-tracking-is-not-supported"></a>Não há suporte para o controle de alterações

O controle de alterações (consulta delta) não tem suporte nas propriedades de extensão do esquema ou abrir.

### <a name="creating-a-resource-and-open-extension-at-the-same-time"></a>Criar um recurso e uma extensão aberta ao mesmo tempo

Você não pode especificar uma extensão aberta ao mesmo tempo que cria uma instância de **administrativeUnit**, **device**, **group**, **organization** ou **user**. Primeiro você deve criar a instância e, depois, especificar os dados da extensão aberta em uma solicitação ``POST`` subsequente nessa instância.

### <a name="creating-a-resource-instance-and-adding-schema-extension-data-at-the-same-time"></a>Criar uma instância de recurso e adicionar dados de extensão de esquema ao mesmo tempo

Não é possível especificar uma extensão de esquema na mesma operação, como criar uma instância de **contato**, **evento**, **mensagem** ou **postagem**.
Você deve primeiro criar a instância de recurso e, em seguida, fazer um `PATCH` para essa instância para adicionar uma extensão de esquema e dados personalizados.

### <a name="limit-of-100-schema-extension-property-values-allowed-per-resource-instance"></a>Limite de 100 valores de propriedade de extensão de esquema permitido por instância de recursos

Recursos de diretório, como **dispositivo**, **grupo** e **usuário**, atualmente limitam o número total de valores de propriedade de extensão de esquema que podem ser definidas em um recurso, até 100.

### <a name="updating-a-schemaextension-definition-using-microsoft-graph-explorer"></a>Atualizar uma definição de schemaExtension usando o Microsoft Graph Explorer

Ao usar `PATCH` para atualizar uma schemaExtension usando o Graph Explorer, você deve especificar a propriedade de **proprietário** e defini-la com seu valor `appid` atual (que será necessário ser uma `appId` de um aplicativo que você tenha). Esse também é o caso de qualquer aplicativo de cliente que `appId` não seja o mesmo que o do **proprietário**.

### <a name="filtering-on-schema-extension-properties-not-supported-on-all-entity-types"></a>Não há suporte a filtragem em propriedades de extensão de esquema em todos os tipos de entidade

Não há suporte a filtragem em propriedades de extensão de esquema (usando a expressão `$filter`) para tipos de entidade do Outlook – **contato**, **evento**, **mensagem** ou **postagem**.

## <a name="files-onedrive"></a>Arquivos (OneDrive)

* O primeiro acesso a uma unidade pessoal de um usuário pelo Microsoft Graph antes que ele acesse o próprio site pessoal por um navegador resulta em uma resposta 401.

## <a name="groups"></a>Grupos

### <a name="permissions-for-groups-and-microsoft-teams"></a>Permissões para grupos e Microsoft Teams

O Microsoft Graph expõe duas permissões ([*Group.Read.All*](permissions-reference.md#group-permissions) e [*Group.ReadWrite.All*](permissions-reference.md#group-permissions)) para obter acesso a APIs de grupos e Microsoft Teams.
As permissões do aplicativo devem ser consentidas por um administrador.
No futuro, pretendemos adicionar novas permissões para grupos e equipes que possam ser consentidas pelos usuários.

Além disso, somente a API para administração de grupo principal e gerenciamento suporta acesso usando permissões delegadas ou somente para aplicativos. Todos os outros recursos da API do grupo dão suporte apenas a permissões delegadas.

Exemplos de recursos de grupo que oferecem suporte a permissões delegadas e somente para aplicativos:

* Criar e excluir grupos
* Obter e atualizar propriedades do grupo pertencentes ao gerenciamento ou administração de grupo
* [Definições do diretório](/graph/api/resources/directoryobject), tipo e sincronização do grupo
* Membros e proprietários de grupo
* Como obter conversas de grupo e threads

Exemplos de recursos de grupo que oferecem suporte somente a permissões delegadas:

* Eventos de grupo, foto
* Remetentes externos, remetentes aceitos ou rejeitados e assinatura de grupo
* Favoritos do usuário e contagem de não vistos

### <a name="policy"></a>Política

Usar o Microsoft Graph para criar e nomear um grupo do Microsoft 365 ignora qualquer política de grupo do Microsoft 365 configurada por meio do Outlook na Web.

### <a name="setting-the-allowexternalsenders-property"></a>Definir a propriedade allowExternalSenders

Atualmente, há um problema que impede a configuração da propriedade **allowExternalSenders** de um grupo em uma operação de POST ou PATCH no `/v1.0` e no `/beta`.

### <a name="using-delta-query"></a>Uso da consulta delta

Para saber mais sobre problemas conhecidos com o uso da consulta delta, veja a [seção da consulta delta](#delta-query) deste artigo.

## <a name="identity-and-access--application-and-service-principal-apis"></a>Identidade e acesso | APIs da entidade de serviço e aplicativo

Há alterações para as entidades [application](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true) e [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true) atualmente em desenvolvimento. A seguir, encontra-se um resumo das limitações atuais e os recursos da API em desenvolvimento:

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

Todas as solicitações contidas em uma solicitação em lote devem ser executadas de forma síncrona. Se estiver presente, a preferência `respond-async` será ignorada.

### <a name="no-transactions"></a>Sem transações

No momento o Microsoft Graph não oferece suporte a processamento transacional de solicitações individuais. A propriedade `atomicityGroup` em solicitações individuais será ignorada.

### <a name="uris-must-be-relative"></a>URIs devem ser relativas

Sempre especifique URIs relativas em solicitações de lote. O Microsoft Graph então torna essas URLs absolutas usando o ponto de extremidade de versão incluído na URL de lote.

### <a name="limit-on-batch-size"></a>Limite de tamanho de lote

No momento, as solicitações de lote JSON estão limitadas a 20 solicitações individuais.

### <a name="simplified-dependencies"></a>Dependências simplificadas

Solicitações individuais podem depender de outras solicitações individuais. Atualmente, solicitações só podem depender de uma única outra solicitação e devem seguir um destes três padrões:

1. Paralelo - nenhuma solicitação individual indica uma dependência na propriedade **dependsOn**.
2. Serial – todas as solicitações individuais dependem da solicitação individual anterior.
3. Mesmo - todas as solicitações individuais que indicam uma dependência na propriedade **dependsOn** declaram a mesma dependência. **Observação**: as solicitações feitas usando este padrão serão executadas sequencialmente.

Conforme o processamento em lotes JSON amadurece, essas limitações são removidas.

## <a name="mail-outlook"></a>Email (Outlook)

### <a name="attaching-large-files-to-messages"></a>Anexando grandes arquivos a mensagens
Um aplicativo com permissões delegadas retorna `HTTP 403 Forbidden` ao tentar [anexar arquivos grandes](outlook-large-attachments.md) a uma mensagem ou evento do Outlook que está em uma caixa de correio compartilhada ou delegada. Com as permissões delegadas, [createUploadSession](/graph/api/attachment-createuploadsession) só é bem sucedida se a mensagem ou o evento estiver na caixa de correio do usuário conectado.

### <a name="the-comment-parameter-for-creating-a-draft"></a>O parâmetro de comentário para criar um rascunho

O parâmetro **comment** para criar uma resposta ou rascunho de encaminhamento ([createReply](/graph/api/message-createreply), [createReplyAll](/graph/api/message-createreplyall), [createForward](/graph/api/message-createforward)) não se torna parte do corpo do rascunho de mensagem resultante.

### <a name="get-messages-returns-chats-in-microsoft-teams"></a>As mensagens GET retornam chats no Microsoft Teams

Em pontos de extremidade beta e v1, a resposta de `GET /users/id/messages` inclui chats do usuário no Microsoft Teams que ocorreu fora do escopo de uma equipe ou de um canal. Essas mensagens de chat tem "IM" como o assunto.

## <a name="teamwork-microsoft-teams"></a>Trabalho em equipe (Microsoft Teams)

### <a name="get-teams-is-not-supported"></a>GET /teams não tem suporte

Para obter uma lista de equipes, confira [listar todas as equipes](teams-list-all-teams.md) e [listar suas equipes](/graph/api/user-list-joinedteams).

### <a name="unable-to-filter-team-members-by-roles"></a>Não é possível filtrar os membros da equipe por funções
A consulta de filtro para obter membros de uma equipe com base em suas funções `GET /teams/team-id/members?$filter=roles/any(r:r eq 'owner')`pode não funcionar. O servidor pode responder com uma.`BAD REQUEST`

### <a name="missing-properties-for-chat-members"></a>Propriedades ausentes para membros do bate-papo
Em certos casos, a `tenantId` / `email` / `displayName` propriedade para os membros individuais de um bate-papo pode não ser preenchida em uma solicitação `GET /chats/chat-id/members` ou `GET /chats/chat-id/members/membership-id`.

### <a name="missing-properties-in-the-list-of-teams-that-a-user-has-joined"></a>Propriedades ausentes na lista de equipes que um usuário ingressou
A chamada à API para [me/joinedTeams](/graph/api/user-list-joinedteams) retorna apenas as propriedades **id**, **displayName** e **description** de uma [equipe](/graph/api/resources/team). Para obter todas as propriedades, use a operação[obter a equipe](/graph/api/team-get).

## <a name="users"></a>Usuários

### <a name="use-the-dollar--symbol-in-the-userprincipalname"></a>Usar o símbolo de cifrão ($) no userPrincipalName

O Microsoft Graph permite que o **userPrincipalName** comece com um caractere de cifrão (`$`). No entanto, ao consultar usuários por userPrincipalName, a url de solicitação `/users/$x@y.com` falha. Isso porque essa URL de solicitação viola as convenções de URL OData que espera que apenas as opções de consulta do sistema sejam prefixadas com um caractere `$`. Como alternativa, remova a barra (/) após `/users` e coloque o **userPrincipalName** entre parênteses e aspas simples como a seguir: `/users('$x@y.com')`

### <a name="no-instant-access-after-creation"></a>Sem acesso instantâneo após a criação

Os usuários podem ser criados imediatamente por um POST na entidade do usuário. Uma licença do Office 365 deve ser atribuída a um usuário primeiro para que ele possa ter acesso aos serviços do Microsoft 365. Mesmo assim, devido à natureza distribuída do serviço, pode demorar 15 minutos antes que os arquivos, as mensagens e as entidades de eventos fiquem disponíveis para uso por esse usuário na API do Microsoft Graph. Durante esse período, os aplicativos receberão uma resposta de erro HTTP 404.

### <a name="photo-restrictions"></a>Restrições de foto

A leitura e a atualização da foto do perfil do usuário só serão possíveis se o usuário tiver uma caixa de correio. Além disso, as fotos que *possam* ter sido previamente armazenadas usando a propriedade **thumbnailPhoto** (usando o Azure AD Graph ou por meio da sincronização do AD Connect) deixarão de estar acessíveis por meio da propriedade **foto** do recurso [usuário](/graph/api/resources/user) do Microsoft Graph.
A falha na leitura ou na atualização de uma foto, nesse caso, resultaria no seguinte erro:

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

O [usuário: revokeSignInSessions API](/graph/api/user-revokesigninsessions) deve retornar uma resposta `204 No content` para ter revogações bem-sucedidas e um código de erro HTTP (4xx ou 5xx) se algo der errado com a solicitação.  No entanto, devido a um problema de serviço, essa API retorna um parâmetro `200 OK` e um parâmetro booleano que é sempre true.  Até que isso seja corrigido, é recomendado que desenvolvedores simplesmente tratem qualquer código de retorno 2xx como bem-sucedido para esta API.

### <a name="incomplete-objects-when-using-getbyids-request"></a>Objetos incompletos ao usar a solicitação getByIds

A solicitação de objetos usando a opção de [Obter objetos de diretório de uma lista de IDs](/graph/api/directoryobject-getbyids) deve retornar objetos completos. No entanto, atualmente, os objetos de [usuário](/graph/api/resources/user) no ponto de extremidade v1.0 são retornados com um conjunto limitado de propriedades. Como solução temporária, ao usar a operação em combinação com a opção de consulta `$select`, objetos de [usuário](/graph/api/resources/user) mais completos serão retornados. Esse comportamento não está de acordo com as especificações do OData. Como esse comportamento pode ser atualizado no futuro, use esta solução alternativa apenas quando fornecer `$select=` com todas as propriedades de seu interesse e somente se futuras alterações nessa solução alternativa forem aceitáveis.

## <a name="query-parameter-limitations"></a>Limitações de parâmetro de consulta

* Não há suporte para vários namespaces.
* Não há suporte para GETs no `$ref` e também para transmissão em usuários, grupos, dispositivos, entidades de serviço e aplicativos.
* `@odata.bind` não é compatível. Isso significa que os desenvolvedores não poderão definir corretamente a propriedade de navegação **acceptedSenders** ou **rejectedSenders** em um grupo.
* `@odata.id` não está presente na navegação sem confinamento (como mensagens) quando há o uso de metadados mínimos.
* `$expand`:
  * Retorna um máximo de 20 objetos.
  * Sem suporte para `@odata.nextLink`.
  * Sem suporte para mais de 1 nível de expansão.
  * Sem suporte com parâmetros extras (`$filter`, `$select`).
* `$filter`:
  * Não há suporte para filtros no ponto de extremidade `/attachments`. Se presente, o parâmetro `$filter` é ignorado.
  * Não há suporte para filtragem de carga de trabalho cruzada.
* `$search`:
  * A pesquisa de texto completo só está disponível para um subconjunto de entidades, como mensagens.
  * Não há suporte para pesquisa de carga de trabalho cruzada.
  * A pesquisa não é suportada nos locatários do Azure AD B2C.
* `$count`:
  * Não é apoiado em locatários do Azure AD B2C.
  * Ao usar a cadeia de consulta `$count=true` ao consultar recursos de diretório, a propriedade `@odata.count` estará presente apenas na primeira página dos dados paginados.
* Os parâmetros de consulta especificados em uma solicitação podem falhar silenciosamente. Isto pode ser verdade tanto para parâmetros de consulta não suportados quanto para combinações não suportadas de parâmetros de consulta..


## <a name="functionality-available-only-in-office-365-rest-or-azure-ad-graph-apis"></a>Funcionalidade disponível apenas nas APIs Graph do Azure AD ou REST do Office 365

Alguns recursos ainda não estão disponíveis no Microsoft Graph. Se você não vir a funcionalidade que está procurando, poderá usar as [APIs REST do Office 365](/previous-versions/office/office-365-api/) específicas do ponto de extremidade. Para o Azure Active Directory, confira [Migrar aplicativos do Azure AD Graph para o Microsoft Graph](./migrate-azure-ad-graph-planning-checklist.md).
