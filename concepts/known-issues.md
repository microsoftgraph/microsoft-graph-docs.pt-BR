---
title: Problemas conhecidos com o Microsoft Graph
description: Este artigo descreve os problemas conhecidos com o Microsoft Graph. Confira as informações sobre as atualizações mais recentes no Log de alterações do Microsoft Graph.
author: jthake-msft
localization_priority: Priority
ms.openlocfilehash: 351b02e3d423458fba8dbaec2050530ccaba4df0
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576784"
---
# <a name="known-issues-with-microsoft-graph"></a>Problemas conhecidos com o Microsoft Graph

Este artigo descreve os problemas conhecidos com o Microsoft Graph. Confira as informações sobre as atualizações mais recentes no [Log de alterações do Microsoft Graph](changelog.md).

## <a name="users"></a>Usuários

### <a name="no-instant-access-after-creation"></a>Sem acesso instantâneo após a criação

Os usuários podem ser criados imediatamente por um POST na entidade do usuário. Uma licença do Office 365 deve ser atribuída a um usuário primeiro para que ele possa ter acesso aos serviços do Office 365. Mesmo assim, devido à natureza distribuída do serviço, pode demorar 15 minutos antes que os arquivos, as mensagens e as entidades de eventos fiquem disponíveis para uso por esse usuário na API do Microsoft Graph. Durante esse período, os aplicativos receberão uma resposta de erro 404 HTTP.

### <a name="photo-restrictions"></a>Restrições de foto

A leitura e a atualização da foto do perfil do usuário só serão possíveis se o usuário tiver uma caixa de correio. Além disso, as fotos que *possam* ter sido previamente armazenadas usando a propriedade **thumbnailPhoto** (usando a visualização da API unificada do Office 365, o Azure AD Graph ou por meio da sincronização do AD Connect) deixarão de estar acessíveis com a propriedade **photo** do recurso [usuário](/graph/api/resources/user?view=graph-rest-1.0) do Microsoft Graph. A falha na leitura ou na atualização de uma foto, nesse caso, resultaria no seguinte erro:

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

## <a name="microsoft-teams"></a>Microsoft Teams

### <a name="create-chat-thread-api"></a>Criar API de thread de chat

A API atual para [criar um thread de chat](/graph/api/channel-post-chatthreads?view=graph-rest-beta) será substituída por uma API mais rica, consistente com o esquema para [listar mensagens de canais](/graph/api/channel-list-messages?view=graph-rest-beta).

### <a name="graph-explorer-and-global-admins"></a>Explorador do Graph e administradores globais

Atualmente, o Explorador do Graph permite que administradores globais manipulem equipes das quais não são proprietários ou membros; porém outros aplicativos que tentam fazer as mesmas chamadas de API falharão se o usuário atual não for um membro ou proprietário da equipe.

### <a name="get-teams-and-post-teams-are-not-supported"></a>GET /teams e POST /teams não são suportados

Confira [listar todas as equipes](teams-list-all-teams.md) e [listar suas equipes](/graph/api/user-list-joinedteams?view=graph-rest-1.0) para obter uma lista de equipes.
Confira [criar equipe](/graph/api/team-put-teams?view=graph-rest-1.0) para criar equipes.

### <a name="missing-teams-in-list-all-teams"></a>Equipes ausentes em listas todas as equipes

Algumas equipes que foram criadas no passado mas não foram usadas recentemente por um usuário do Microsoft Teams não são listadas por [listar todas as equipes](teams-list-all-teams.md).
Novas equipes serão listadas.
Algumas equipes antigas não têm uma propriedade **resourceProvisioningOptions** que contém “Equipe”, que é configurada em equipes recém-criadas e equipes que são visitadas no Microsoft Teams.
No futuro, vamos configurar **resourceProvisioningOptions** em equipes existentes que não foram abertas no Microsoft Teams.

## <a name="groups"></a>Grupos

### <a name="permissions-for-groups-and-microsoft-teams"></a>Permissões para grupos e Microsoft Teams

O Microsoft Graph expõe duas permissões ([*Group.Read.All*](permissions-reference.md#group-permissions) e [*Group.ReadWrite.All*](permissions-reference.md#group-permissions)) para obter acesso a APIs de grupos e Microsoft Teams.
As permissões do aplicativo devem ser consentidas por um administrador.
No futuro, pretendemos adicionar novas permissões para grupos e equipes que possam ser consentidas pelos usuários.

Além disso, somente a API para administração de grupo principal e gerenciamento suporta acesso usando permissões delegadas ou somente para aplicativos. Todos os outros recursos da API do grupo dão suporte apenas a permissões delegadas.

Exemplos de recursos de grupo que oferecem suporte a permissões delegadas e somente para aplicativos:

* Criar e excluir grupos
* Obter e atualizar propriedades do grupo pertencentes ao gerenciamento ou administração de grupo
* [Definições do diretório](/graph/api/resources/directoryobject?view=graph-rest-1.0), tipo e sincronização do grupo
* Membros e proprietários de grupo

Exemplos de recursos de grupo que oferecem suporte somente a permissões delegadas:

* Conversas, eventos e foto de grupo
* Remetentes externos, remetentes aceitos ou rejeitados e assinatura de grupo
* Favoritos do usuário e contagem de não vistos

### <a name="policy"></a>Política

O uso do Microsoft Graph para criar e nomear um grupo do Office 365 ultrapassa qualquer política de grupo do Office 365 que seja configurada pelo Outlook Web App.

### <a name="adding-and-getting-attachments-of-group-posts"></a>Adicionando e obtendo anexos de postagens de grupo

A [adição](/graph/api/post-post-attachments?view=graph-rest-1.0) de anexos a postagens de grupo a [listagem](/graph/api/post-list-attachments?view=graph-rest-1.0) e a obtenção de anexos de postagens do grupo atualmente retornam a mensagem de erro "A solicitação de OData não tem suporte." Uma correção foi implementada nas versões `/v1.0` e `/beta`, e deve estar amplamente disponível até o final de janeiro de 2016.

### <a name="setting-the-allowexternalsenders-property"></a>Definir a propriedade allowExternalSenders

Atualmente, há um problema que impede a configuração da propriedade **allowExternalSenders** de um grupo em uma operação de POST ou PATCH no `/v1.0` e no `/beta`.

### <a name="using-delta-query"></a>Uso da consulta delta

Para saber mais sobre problemas conhecidos com o uso da consulta delta, veja a [seção da consulta delta](#delta-query) deste artigo.

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
GET \users('{id}')\calendars('{id}')\events
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
GET \me\calendars('{id}')\events
```

### <a name="adding-and-accessing-ics-based-calendars-in-users-mailbox"></a>Adicionar e acessar calendários baseados em ICS na caixa de correio do usuário

Atualmente, há suporte parcial para um calendário com base em uma Inscrição em Calendário da Internet (ICS):

* Você pode adicionar um calendário baseado em ICS para uma caixa de correio do usuário por meio da interface do usuário, mas não através da API do Microsoft Graph.
* [Listar os calendários do usuário](/graph/api/user-list-calendars?view=graph-rest-1.0) permite que você obtenha as propriedades **name**, **color** e **id** de cada [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) no grupo de calendários padrão do usuário ou em um grupo de calendários especificado, inclusive todos os calendários com base em ICS. Não é possível armazenar ou acessar a URL da ICS no recurso de calendário.
* Você também pode [listar os eventos](/graph/api/calendar-list-events?view=graph-rest-1.0) de um calendário baseado em ICS.

### <a name="onlinemeetingurl-property-support-for-microsoft-teams"></a>Suporte de propriedade onlineMeetingUrl do Microsoft Teams

Atualmente, a propriedade **onlineMeetingUrl** de um [evento](/graph/api/resources/event?view=graph-rest-1.0) de reunião do Skype indica a URL da reunião online. No entanto, essa propriedade para um evento de reunião do Microsoft Teams está definida como nula.

## <a name="calls-and-online-meetings"></a>Chamadas e reuniões online

> **Observação** As chamadas e reuniões online estão atualmente em visualização e estarão disponíveis apenas no ponto de extremidade beta do Microsoft Graph.

- O caminho da navegação `/applications/{id}` não tem suporte. Não é permitido navegar pelo nó de aplicativos globais para o aplicativo, mesmo que seja o seu próprio.  Use o `/app` apenas para navegação.

## <a name="contacts"></a>Contatos

### <a name="organization-contacts-available-in-only-beta"></a>Contatos de organização disponíveis somente na versão beta

Somente os contatos pessoais têm suporte no momento. Os contatos organizacionais atualmente não têm suporte na `/v1.0`, mas podem ser encontrados na versão `/beta`.

### <a name="default-contacts-folder"></a>Pasta Contatos padrão

Na versão `/v1.0`, `GET /me/contactFolders` não inclui a pasta de contatos do usuário padrão.

Uma correção será disponibilizada. Enquanto isso, você pode usar a seguinte consulta [list contacts](/graph/api/user-list-contacts?view=graph-rest-1.0) e a propriedade **parentFolderId** como uma solução alternativa para obter a ID da pasta de contatos padrão:

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

* Acessando um contato contido em uma pasta filha de um **contactFolder**.  O exemplo a seguir mostra um nível de aninhamento, mas um contato pode estar localizado em um filho de um filho e assim por diante.

```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```

Como alternativa, você pode simplesmente [obter](/graph/api/contact-get?view=graph-rest-beta) o contato, especificando sua identificação conforme mostrado abaixo, uma vez que o GET /contacts na versão `/beta` se aplica a todos os contatos na caixa de correio do usuário:

```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```

## <a name="messages"></a>Mensagens

### <a name="the-comment-parameter-for-creating-a-draft"></a>O parâmetro de comentário para criar um rascunho

O parâmetro **comment** para criar uma resposta ou rascunho de encaminhamento ([createReply](/graph/api/message-createreply?view=graph-rest-1.0), [createReplyAll](/graph/api/message-createreplyall?view=graph-rest-1.0), [createForward](/graph/api/message-createforward?view=graph-rest-1.0)) não se torna parte do corpo do rascunho de mensagem resultante.

### <a name="get-messages-returns-chats-in-microsoft-teams"></a>As mensagens GET retornam chats no Microsoft Teams

Em pontos de extremidade beta e v1, a resposta de `GET /users/id/messages` inclui chats do usuário no Microsoft Teams que ocorreu fora do escopo de uma equipe ou de um canal. Essas mensagens de chat tem "IM" como o assunto.


## <a name="drives-files-and-content-streaming"></a>Unidades, arquivos e streaming de conteúdo

* O acesso pela primeira vez a uma unidade pessoal de um usuário pelo Microsoft Graph antes que ele acesse seu site pessoal por um navegador resulta em uma resposta 401.

## <a name="query-parameter-limitations"></a>Limitações de parâmetro de consulta

* Não há suporte para vários namespaces.
* Não há suporte para GETs em `$ref` e conversão em usuários, grupos, dispositivos, entidades de serviço e aplicativos.
* Não há suporte para `@odata.bind`. Isso significa que os desenvolvedores não poderão definir corretamente `Accepted` ou `RejectedSenders` em um grupo.
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

## <a name="delta-query"></a>Consulta delta

* O contexto de OData às vezes é retornado incorretamente ao controlar alterações nas relações.
* As extensões de esquema (herdadas) não são retornadas com instrução $select, mas são retornadas sem $select.
* Os clientes não podem controlar alterações em extensões abertas ou extensões de esquema.

## <a name="application-and-serviceprincipal-api-changes"></a>Alterações do aplicativo e da API servicePrincipal

Há alterações para as entidades [application](/graph/api/resources/application?view=graph-rest-beta) e [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) atualmente em desenvolvimento. A seguir, encontra-se um resumo das limitações atuais e os recursos da API em desenvolvimento:

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

### <a name="filtering-on-schema-extension-properties-not-supported-on-all-entity-types"></a>Não há suporte a filtragem em propriedades de extensão de esquema em todos os tipos de entidade

Não há suporte a filtragem em propriedades de extensão de esquema (usando a expressão `$filter`) para tipos de entidade do Outlook – **contact**, **event**, **message** ou **post**.

## <a name="json-batching"></a>Processamento em lotes JSON

### <a name="no-nested-batch"></a>Nenhum lote aninhado

Solicitações de lote JSON não devem conter quaisquer solicitações em lotes aninhados.

### <a name="all-individual-requests-must-be-synchronous"></a>Todas as solicitações individuais devem ser síncronas

Todas as solicitações contidas em uma solicitação de lote devem ser executadas de forma síncrona. Se estiver presente, a preferência `respond-async` será ignorada.

### <a name="no-transactions"></a>Sem transações

No momento o Microsoft Graph não oferece suporte a processamento transacional de solicitações individuais. A propriedade `atomicityGroup` em solicitações individuais será ignorada.

### <a name="uris-must-be-relative"></a>URIs devem ser relativas

Sempre especifique URIs relativas em solicitações de lote. O Microsoft Graph então torna essas URLs absolutas usando o ponto de extremidade de versão incluído na URL de lote.

### <a name="limit-on-batch-size"></a>Limite de tamanho de lote

No momento, as solicitações de lote JSON estão limitadas a 20 solicitações individuais.

### <a name="simplified-dependencies"></a>Dependências simplificadas

Solicitações individuais podem depender de outras solicitações individuais. Atualmente, solicitações só podem depender de uma única outra solicitação e devem seguir um destes três padrões:

1. Paralelo – nenhuma solicitação individual declara uma dependência na propriedade `dependsOn`.
2. Serial – todas as solicitações individuais dependem da solicitação individual anterior.
3. Mesmo – todas as solicitações individuais indicam que uma dependência na propriedade `dependsOn` declaram a mesma dependência.

Conforme o processamento em lotes JSON amadurece, essas limitações são removidas.

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

## <a name="functionality-available-only-in-office-365-rest-or-azure-ad-graph-apis"></a>Funcionalidade disponível apenas nas APIs Graph do Azure AD ou REST do Office 365

Alguns recursos ainda não estão disponíveis no Microsoft Graph. Se você não vir a funcionalidade que está procurando, poderá usar as [APIs REST do Office 365](https://msdn.microsoft.com/office/office365/api/api-catalog) específicas do ponto de extremidade. Para o Azure Active Directory, veja a postagem no blog [Microsoft Graph ou Azure AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) sobre os recursos que só estão disponíveis pela API do Graph do Azure AD.

