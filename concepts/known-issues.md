---
title: Problemas conhecidos com o Microsoft Graph
description: Este artigo descreve os problemas conhecidos com o Microsoft Graph.
author: MSGraphDocsVTeam
ms.localizationpriority: high
ms.openlocfilehash: 925fa2538496b20b5b22a99823ea80fed8d9b1a0
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688097"
---
# <a name="known-issues-with-microsoft-graph"></a>Problemas conhecidos com o Microsoft Graph

Este artigo descreve os problemas conhecidos com o Microsoft Graph. 

Para relatar um problema conhecido, confira a página [Suporte Microsoft Graph](https://developer.microsoft.com/graph/support).

Para saber mais sobre as atualizações mais recentes da API do Microsoft Graph, confira o [changelog do Microsoft Graph](changelog.md).

## <a name="applications"></a>Aplicativos

### <a name="some-limitations-apply-to-the-application-and-serviceprincipal-resources"></a>Algumas limitações se aplicam ao aplicativo e aos recursos servicePrincipal

As alterações para os recursos [application](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true) e [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true) estão atualmente em desenvolvimento. A seguir, encontra-se um resumo das limitações atuais e os recursos da API em desenvolvimento.

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

### <a name="azure-ad-v20-endpoint-is-not-supported-for-csp-apps"></a>O ponto de extremidade do Azure AD v2.0 não é compatível com aplicativos CSP

Aplicativos de provedor de solução de nuvem (CSP) devem adquirir tokens de pontos de extremidade do Azure AD (v1) para chamar a Microsoft Graph com êxito em seus clientes gerenciados por parceiros. Atualmente, não há suporte para aquisição de um token pelo ponto de extremidade Azure AD v 2.0 mais recente.

### <a name="pre-consent-for-csp-apps-doesnt-work-in-some-customer-tenants"></a>A pré-autorização para aplicativos CSP não funciona em alguns locatários do cliente

Sob certas circunstâncias, o pré-consentimento para aplicativos de provedor de soluções na nuvem (CSP) pode não funcionar para alguns de seus locatários de clientes.

- Para aplicativos que usam permissões delegadas, ao usar o aplicativo pela primeira vez com um novo locatário do cliente, você poderá receber esse erro após o logon: `AADSTS50000: There was an error issuing a token`.
- Para aplicativos que usam permissões de aplicativos, seu aplicativo pode adquirir um token, mas inesperadamente receber uma mensagem de acesso negado ao chamar o Microsoft Graph.

Estamos trabalhando para corrigir esse problema o mais rápido possível, de modo que a pré-autorização funcionará para todos os seus locatários de clientes.

Enquanto isso, para desbloquear o desenvolvimento e os testes, você pode usar a seguinte solução alternativa.

>**Observação:** esta não é uma solução permanente e destina-se apenas a desbloquear o desenvolvimento. Esta solução alternativa não será necessária uma vez que o problema for corrigido. Esta solução alternativa não precisa ser desfeita após a correção.

1. Abra uma sessão do Azure AD v2 PowerShell e conecte-se ao locatário do parceiro `customer`digitando suas credenciais de administrador na janela de entrada. Você pode baixar e instalar o Azure AD PowerShell V2 [aqui](https://www.powershellgallery.com/packages/AzureAD).

    ```PowerShell
    Connect-AzureAd -TenantId {customerTenantIdOrDomainName}
    ```

2. Crie o servicePrincipal do Microsoft Graph.

    ```PowerShell
    New-AzureADServicePrincipal -AppId 00000003-0000-0000-c000-000000000000
    ```
## <a name="bookings"></a>Reservas

### <a name="error-when-querying-bookingbusinesses"></a>Erro ao consultar bookingBusinesses

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
## <a name="calendar"></a>Calendário

### <a name="error-accessing-a-shared-calendar"></a>Erro ao acessar um calendário compartilhado

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

### <a name="partial-support-for-adding-and-accessing-ics-based-calendars-in-users-mailbox"></a>Suporte parcial para adicionar e acessar calendários baseados em ICS na caixa de correio do usuário

Atualmente, calendários com base em uma Inscrição em Calendário da Internet (ICS) têm apenas suporte parcial:

* Você pode adicionar um calendário baseado em ICS para uma caixa de correio do usuário por meio da interface do usuário, mas não através da API do Microsoft Graph.
* [Listar os calendários do usuário](/graph/api/user-list-calendars) permite que você obtenha as propriedades **name**, **color** e **id** de cada [calendar](/graph/api/resources/calendar) no grupo de calendários padrão do usuário ou em um grupo de calendários especificado, inclusive todos os calendários com base em ICS. Não é possível armazenar ou acessar a URL da ICS no recurso de calendário.
* Você também pode [listar os eventos](/graph/api/calendar-list-events) de um calendário baseado em ICS.

### <a name="error-attaching-large-files-to-events"></a>Erro ao anexar arquivos grandes a eventos
Um aplicativo com permissões delegadas retorna `HTTP 403 Forbidden` ao tentar [anexar arquivos grandes](outlook-large-attachments.md) a uma mensagem ou evento do Outlook que está em uma caixa de correio compartilhada ou delegada. Com as permissões delegadas, [createUploadSession](/graph/api/attachment-createuploadsession) só é bem sucedida se a mensagem ou o evento estiver na caixa de correio do usuário conectado.

### <a name="onlinemeetingurl-property-is-not-supported-for-microsoft-teams"></a>A propriedade onlineMeetingUrl não é compatível com o Microsoft Teams

Atualmente, a propriedade **onlineMeetingUrl** de um [evento](/graph/api/resources/event) de reunião do Skype indica a URL da reunião online. No entanto, essa propriedade para um evento de reunião do Microsoft Teams está definida como nula.

A versão beta oferece uma solução alternativa, na qual é possível usar a propriedade **onlineMeetingProvider** de um [evento](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true) para verificar se o provedor é o Microsoft Teams. Por meio da propriedade **onlineMeeting** do **evento**, você pode acessar o **joinUrl**.

## <a name="change-notifications"></a>Notificações de alteração

### <a name="update-notifications-occur-on-creation-and-soft-deletion-of-users"></a>As notificações de atualização ocorrem na criação e exclusão reversível de usuários

As [assinaturas](/graph/api/resources/subscription) de alterações para o **usuário** com o **changeType** definido como **atualizado** também receberão notificações de **changeType**: **atualizado** na criação do usuário e exclusão reversível do usuário.

### <a name="update-notifications-occur-on-creation-and-soft-deletion-of-groups"></a>As notificações de atualização ocorrem na criação e exclusão reversível de grupos

As [assinaturas](/graph/api/resources/subscription) de alterações no **grupo** com o **changeType** definido como **atualizado** também receberão notificações **changeType**: **atualizado** na criação do grupo e exclusão reversível do grupo.

## <a name="cloud-communications"></a>Comunicações na nuvem 

### <a name="view-meeting-details-menu-is-not-available-on-microsoft-teams-client"></a>O menu "Exibir detalhes da reunião" não está disponível no cliente Microsoft Teams

O cliente do Microsoft Teams não mostra o menu **Exibir detalhes da Reunião** para reuniões de canal criadas por meio da API de comunicações na nuvem.

## <a name="compliance"></a>Conformidade

### <a name="subject-rights-request-api-permissions-are-not-currently-available"></a>As permissões da API de solicitação de direitos do titular dos dados não estão disponíveis no momento

No momento, as entidades da API de solicitação de direitos do titular dos dados na API de privacidade do Microsoft Graph não têm permissões disponíveis. Esse problema pode impedir que os usuários vejam permissões e consentam com o uso da API em seu ambiente. 

## <a name="contacts"></a>Contatos

### <a name="get-operation-does-not-return-default-contacts-folder"></a>A operação GET não retorna a pasta de contatos padrão

Na versão `/v1.0`, `GET /me/contactFolders` não inclui a pasta de contatos do usuário padrão.

Uma correção será disponibilizada. Enquanto isso, você pode usar a seguinte consulta [list contacts](/graph/api/user-list-contacts) e a propriedade **parentFolderId** como uma solução alternativa para obter a ID da pasta de contatos padrão:

```http
GET https://graph.microsoft.com/v1.0/me/contacts?$top=1&$select=parentFolderId
```

Nesta solicitação:

1. `/me/contacts?$top=1` obtém as propriedades de um [contato](/graph/api/resources/contact) na pasta de contatos padrão.
2. A anexação de `&$select=parentFolderId` retorna apenas a propriedade **parentFolderId** do contato, que é a ID da pasta de contatos padrão.


### <a name="accessing-contacts-via-a-contact-folder-doesnt-work-in-beta"></a>Acessar contatos por meio de uma pasta de contatos não funciona na versão beta

Na versão `/beta`, um problema impede o acesso a um [contato](/graph/api/resources/contact?view=graph-rest-beta&preserve-view=true) especificando sua pasta pai na URL de solicitação REST, conforme mostrado nos dois cenários a seguir.

Acessando um contato a partir de um [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-beta&preserve-view=true) de nível superior de um usuário:

```http
GET /me/contactfolders/{id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```

Acessando um contato contido em uma pasta filha de um **contactFolder**: 

```http
GET /me/contactFolders/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```

O exemplo anterior mostra um nível de aninhamento, mas um contato pode estar localizado em um filho de um filho e assim por diante.

Como alternativa, você pode simplesmente [obter](/graph/api/contact-get?view=graph-rest-beta&preserve-view=true) o contato, especificando sua identificação conforme mostrado, porque o GET /contacts na versão `/beta` se aplica a todos os contatos na caixa de correio do usuário:

```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
## <a name="delta-query"></a>Consulta delta

### <a name="odata-context-is-returned-incorrectly"></a>O contexto OData é retornado incorretamente

O contexto de OData às vezes é retornado incorretamente ao controlar alterações nas relações.

### <a name="schema-extensions-are-not-returned-with-select"></a>Extensões de esquema não são retornadas com `select`

As extensões de esquema (herdadas) não são retornadas com instrução `$select`, mas são retornadas sem `$select`.

### <a name="clients-cannot-track-changes-to-open-extensions"></a>Os clientes não podem controlar as alterações nas extensões abertas

Os clientes não podem controlar alterações em extensões abertas ou extensões de esquema.

## <a name="devices-and-apps--device-updates-windows-updates"></a>Dispositivos e aplicativos | Atualizações do dispositivo (atualizações do Windows)

### <a name="accessing-and-updating-deployment-audiences-is-not-supported"></a>Não há suporte para acessar e atualizar audiências de implantação

Acessando e atualizando audiências de implantação em recursos de **implantação** criados por meio do Intune não são suportados atualmente.

* [Listando membros da audiência de implantação](/graph/api/windowsupdates-deploymentaudience-list-members) e [listando exclusões da audiência de implantação](/graph/api/windowsupdates-deploymentaudience-list-exclusions) retornos `404 Not Found`.
* [Atualizar membros da audiência de implantação e exclusões](/graph/api/windowsupdates-deploymentaudience-updateaudience) ou [atualizar por ID](/graph/api/windowsupdates-deploymentaudience-updateaudiencebyid) retorna `202 Accepted`, mas a audiência não é atualizada.

## <a name="extensions"></a>Extensões

### <a name="change-tracking-is-not-supported"></a>Não há suporte para o controle de alterações

O controle de alterações (consulta delta) não tem suporte nas propriedades de extensão do esquema ou abrir.

### <a name="unable-to-create-a-resource-and-open-extension-at-the-same-time"></a>Não é possível criar um recurso e uma extensão aberta ao mesmo tempo

Você não pode especificar uma extensão aberta ao mesmo tempo que cria uma instância de **administrativeUnit**, **device**, **group**, **organization** ou **user**. Primeiro você deve criar a instância e, depois, especificar os dados da extensão aberta em uma solicitação ``POST`` subsequente nessa instância.

### <a name="unable-to-create-a-resource-instance-and-add-schema-extension-data-at-the-same-time"></a>Não é possível criar uma instância de recurso e adicionar dados de extensão de esquema ao mesmo tempo

Não é possível especificar uma extensão de esquema na mesma operação, como criar uma instância de **contato**, **evento**, **mensagem** ou **postagem**.
Você deve primeiro criar a instância de recurso e, em seguida, fazer um `PATCH` para essa instância para adicionar uma extensão de esquema e dados personalizados.

### <a name="limit-of-100-schema-extension-property-values-allowed-per-resource-instance"></a>Limite de 100 valores de propriedade de extensão de esquema permitido por instância de recursos

Recursos de diretório, como **dispositivo**, **grupo** e **usuário**, atualmente limitam o número total de valores de propriedade de extensão de esquema que podem ser definidas em um recurso até 100.

### <a name="owner-must-be-specified-when-updating-a-schemaextension-definition-using-microsoft-graph-explorer"></a>O proprietário deve ser especificado ao atualizar uma definição de schemaExtension usando o Microsoft Graph Explorer

Ao usar `PATCH` para atualizar uma schemaExtension usando o Graph Explorer, você deve especificar a propriedade de **proprietário** e defini-la com seu valor `appid` atual (que será necessário ser uma `appId` de um aplicativo que você tenha). Esse também é o caso de qualquer aplicativo de cliente cuja `appId` não seja a mesma que a do **proprietário**.

### <a name="filtering-on-schema-extension-properties-is-not-supported-on-all-entity-types"></a>Não há suporte a filtragem em propriedades de extensão de esquema em todos os tipos de entidade

Não há suporte a filtragem em propriedades de extensão de esquema (usando a expressão `$filter`) para tipos de entidade do Outlook – **contato**, **evento**, **mensagem** ou **postagem**.

## <a name="files-onedrive"></a>Arquivos (OneDrive)

### <a name="accessing-a-users-drive-before-user-accesses-it-leads-to-error"></a>Acessar a unidade de um usuário antes que o usuário a acesse leva a um erro

O primeiro acesso a uma unidade pessoal de um usuário pelo Microsoft Graph antes que ele acesse o próprio site pessoal por um navegador resulta em uma resposta `401`.

## <a name="groups"></a>Grupos

### <a name="admins-must-consent-to-permissions-for-groups-and-microsoft-teams"></a>Os administradores devem consentir com as permissões para grupos e Microsoft Teams

O Microsoft Graph expõe duas permissões ([*Group.Read.All*](permissions-reference.md#group-permissions) e [*Group.ReadWrite.All*](permissions-reference.md#group-permissions)) para obter acesso a APIs de grupos e Microsoft Teams.
As permissões do aplicativo devem ser consentidas por um administrador.
No futuro, pretendemos adicionar novas permissões para grupos e equipes que possam ser consentidas pelos usuários.

### <a name="some-group-apis-dont-support-delegated-or-app-only-permissions"></a>Algumas APIs de grupo não oferecem suporte para permissões delegadas ou somente de aplicativo

Somente a API para administração de grupo principal e gerenciamento suporta acesso usando permissões delegadas ou somente para aplicativos. Todos os outros recursos da API do grupo dão suporte apenas a permissões delegadas.

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

### <a name="microsoft-graph-bypasses-group-policies-configured-through-outlook-on-the-web"></a>O Microsoft Graph ignora as políticas de grupo configuradas por meio do Outlook na Web

Usar o Microsoft Graph para criar e nomear um grupo do Microsoft 365 ignora qualquer política de grupo do Microsoft 365 configurada por meio do Outlook na Web.

### <a name="allowexternalsenders-property-cannot-be-set-in-a-post-or-patch-operation"></a>A propriedade allowExternalSenders não pode ser definida em uma operação POST ou PATCH

Atualmente, há um problema que impede a configuração da propriedade **allowExternalSenders** de um grupo em uma operação de POST ou PATCH no `/v1.0` e no `/beta`.

### <a name="removing-a-group-owner-also-removes-the-user-as-a-group-member"></a>Remover um proprietário de grupo também remove o usuário como um membro do grupo

Quando [DELETE /groups/{id}/owners](/graph/api/group-delete-owners.md) é chamado para um grupo que está associado a uma [equipe](/graph/api/resources/team.md), o usuário também é removido da lista /groups/{id}/members. Para contornar isso, remova o usuário tanto dos proprietários quanto dos membros, espere 10 segundos e o adicione de volta aos membros.

## <a name="identity-and-access"></a>Identidade e acesso

### <a name="conditional-access-policy-requires-consent-to-permission"></a>A política de acesso condicional requer consentimento para a permissão

Atualmente, a API [conditionalAccessPolicy](/graph/api/resources/conditionalaccesspolicy) requer o consentimento da permissão **Policy.Read.All** para chamar os métodos POST e PATCH. No futuro, a permissão **Policy.ReadWrite.ConditionalAccess** permitirá que você leia as políticas do diretório.

### <a name="claims-mapping-policy-might-require-consent-to-permissions"></a>A política de mapeamento de declarações pode exigir consentimento para permissões

A API [claimsMappingPolicy](/graph/api/resources/claimsmappingpolicy) pode exigir o consentimento das permissões **Policy.Read.All** e **Policy.ReadWrite.ConditionalAccess** para os métodos `LIST /policies/claimsMappingPolicies` e `GET /policies/claimsMappingPolicies/{id}`, da seguinte forma:

+ Se nenhum objeto **claimsMappingPolicy** estiver disponível para ser recuperado em uma operação LIST, qualquer permissão será suficiente para chamar esse método.
+ Se houver objetos **claimsMappingPolicy** a serem recuperados, seu aplicativo deverá consentir com ambas as permissões. Caso contrário, um erro `403 Forbidden` será retornado.

No futuro, qualquer permissão será suficiente para chamar ambos os métodos.

## <a name="json-batching"></a>Envio em lote JSON

### <a name="nested-batches-are-not-supported"></a>Não há suporte para lotes aninhados.

Solicitações de lote JSON não devem conter quaisquer solicitações em lotes aninhados.

### <a name="all-individual-requests-must-be-synchronous"></a>Todas as solicitações individuais devem ser síncronas

Todas as solicitações contidas em uma solicitação de lote devem ser executadas de forma síncrona. Se estiver presente, a preferência `respond-async` será ignorada.

### <a name="transactional-processing-of-requests-is-not-supported"></a>Não há suporte para o processamento transacional de solicitações

No momento o Microsoft Graph não oferece suporte a processamento transacional de solicitações individuais. A propriedade **atomicityGroup** em solicitações individuais será ignorada.

### <a name="uris-must-be-relative"></a>URIs devem ser relativas

Sempre especifique URIs relativas em solicitações de lote. O Microsoft Graph então torna essas URLs absolutas usando o ponto de extremidade de versão incluído na URL de lote.

### <a name="batch-size-is-limited"></a>O tamanho do lote é limitado

No momento, as solicitações de lote JSON estão limitadas a 20 solicitações individuais.

### <a name="request-dependencies-are-limited"></a>As dependências de solicitação são limitadas

Solicitações individuais podem depender de outras solicitações individuais. Atualmente, solicitações só podem depender de uma única outra solicitação e devem seguir um destes três padrões:

- Paralelo - nenhuma solicitação individual indica uma dependência na propriedade **dependsOn**.
- Serial – todas as solicitações individuais dependem da solicitação individual anterior.
- Mesmo - todas as solicitações individuais que indicam uma dependência na propriedade **dependsOn** declaram a mesma dependência. **Observação**: as solicitações feitas usando este padrão serão executadas sequencialmente.

Conforme o processamento em lotes JSON amadurece, essas limitações são removidas.

## <a name="mail-outlook"></a>Email (Outlook)

### <a name="attaching-large-files-to-messages-with-delegated-permissions-can-fail"></a>A anexação de arquivos grandes a mensagens com permissões delegadas pode falhar
Um aplicativo com permissões delegadas retorna `HTTP 403 Forbidden` ao tentar [anexar arquivos grandes](outlook-large-attachments.md) a uma mensagem ou evento do Outlook que está em uma caixa de correio compartilhada ou delegada. Com as permissões delegadas, [createUploadSession](/graph/api/attachment-createuploadsession) só é bem sucedida se a mensagem ou o evento estiver na caixa de correio do usuário conectado.

### <a name="the-comment-parameter-for-creating-a-draft-does-not-become-part-of-the-message-body"></a>O parâmetro de comentário para criar um rascunho não se torna parte do corpo da mensagem

O parâmetro **comment** para criar uma resposta ou rascunho de encaminhamento ([createReply](/graph/api/message-createreply), [createReplyAll](/graph/api/message-createreplyall), [createForward](/graph/api/message-createforward)) não se torna parte do corpo do rascunho de mensagem resultante.

### <a name="get-messages-returns-chats-in-microsoft-teams"></a>As mensagens GET retornam chats no Microsoft Teams

Em pontos de extremidade beta e v1.0, a resposta de `GET /users/id/messages` inclui chats do usuário no Microsoft Teams que ocorreu fora do escopo de uma equipe ou de um canal. Essas mensagens de chat tem "IM" como o assunto.

## <a name="reports"></a>Relatórios

### <a name="azure-ad-activity-reports-can-return-an-error"></a>Os relatórios de atividade do Azure AD podem retornar um erro

Quando você tiver uma licença válida do Azure AD Premium e chamar [directoryAudit](/graph/api/resources/directoryaudit), [signIn](/graph/api/resources/signin)ou [provisionar](/graph/api/resources/provisioningobjectsummary) as APIs de relatórios de atividade do Azure AD, você ainda poderá encontrar uma mensagem de erro semelhante à seguinte:

```json
{
    "error": {
        "code": "Authentication_RequestFromNonPremiumTenantOrB2CTenant",
        "message": "Neither tenant is B2C or tenant doesn't have premium license",
        "innerError": {
            "date": "2021-09-02T17:15:30",
            "request-id": "73badd94-c0ca-4b09-a3e6-20c1f5f9a307",
            "client-request-id": "73badd94-c0ca-4b09-a3e6-20c1f5f9a307"
        }
    }
}
```
Esse erro também pode ocorrer ao recuperar a propriedade **signInActivity** do recurso do [usuário](/graph/api/resources/user?view=graph-rest-beta&preserve-view=true); por exemplo, `https://graph.microsoft.com/beta/users?$select=signInActivity`.

Esse erro ocorre por causa das falhas de verificação de licença intermitentes, que estamos trabalhando para corrigir. Como solução alternativa temporária, adicione a permissão **Directory.Read.All**. Essa solução alternativa temporária não será necessária quando o problema for resolvido.


## <a name="teamwork-microsoft-teams"></a>Trabalho em equipe (Microsoft Teams)

### <a name="get-teams-is-not-supported"></a>GET /teams não tem suporte

Para obter uma lista de equipes, confira [listar todas as equipes](teams-list-all-teams.md) e [listar suas equipes](/graph/api/user-list-joinedteams).

### <a name="unable-to-filter-team-members-by-roles"></a>Não é possível filtrar os membros da equipe por funções
Filtros de consulta de função junto com outros filtros `GET /teams/team-id/members?$filter=roles/any(r:r eq 'owner') and displayName eq 'dummy'` podem não funcionar. O servidor pode responder com uma.`BAD REQUEST`

### <a name="requests-to-filter-team-members-by-role-require-a-parameter"></a>Solicitações para filtrar membros da equipe por função exigem um parâmetro

Todas as solicitações para filtrar membros da equipe por funções esperam um parâmetro _skipToken_ ou um parâmetro _top_ na solicitação, mas não ambos. Se ambos os parâmetros forem passados na solicitação, o parâmetro _top_ será ignorado.

### <a name="some-properties-for-chat-members-might-be-missing-in-the-response-to-a-get-request"></a>Algumas propriedades para membros do chat podem estar ausentes na resposta a uma solicitação GET
Em certos casos, a `tenantId` / `email` / `displayName` propriedade para os membros individuais de um bate-papo pode não ser preenchida em uma solicitação `GET /chats/chat-id/members` ou `GET /chats/chat-id/members/membership-id`.

### <a name="properties-are-missing-in-the-list-of-teams-that-a-user-has-joined"></a>Faltam propriedades na lista de equipes que um usuário ingressou
A chamada à API para [me/joinedTeams](/graph/api/user-list-joinedteams) retorna apenas as propriedades **id**, **displayName** e **description** de uma [equipe](/graph/api/resources/team). Para obter todas as propriedades, use a operação[obter a equipe](/graph/api/team-get).

## <a name="users"></a>Usuários

### <a name="use-the-dollar--symbol-in-the-userprincipalname"></a>Usar o símbolo de cifrão ($) no userPrincipalName

O Microsoft Graph permite que o **userPrincipalName** comece com um caractere de cifrão (`$`). No entanto, ao consultar usuários por userPrincipalName, a url de solicitação `/users/$x@y.com` falha. Isso porque essa URL de solicitação viola a convenção de URL OData que espera que apenas as opções de consulta do sistema sejam prefixadas com um caractere `$`. Como alternativa, remova a barra (/) após `/users` e coloque o **userPrincipalName** entre parênteses e aspas simples como a seguir: `/users('$x@y.com')`

### <a name="access-to-user-resources-is-delayed-after-creation"></a>O acesso aos recursos do usuário é aiado após a criação

Os usuários podem ser criados imediatamente por um POST na entidade do usuário. Uma licença do Office 365 deve ser atribuída a um usuário primeiro para que ele possa ter acesso aos serviços do Microsoft 365. Mesmo assim, devido à natureza distribuída do serviço, pode demorar 15 minutos antes que os arquivos, as mensagens e as entidades de eventos fiquem disponíveis para uso por esse usuário na API do Microsoft Graph. Durante esse período, os aplicativos receberão uma resposta de erro HTTP `404`.

### <a name="access-to-a-users-profile-photo-is-limited"></a>O acesso à foto de perfil de um usuário é limitado

A leitura e a atualização da foto do perfil do usuário só serão possíveis se o usuário tiver uma caixa de correio. Além disso, quaisquer fotos que *possam* ter sido armazenadas anteriormente usando a propriedade **thumbnailPhoto** (usando a API do Azure AD Graph (preterido) ou por meio da sincronização do AD Connect) não estarão mais acessíveis por meio da propriedade de **foto** do Microsoft Graph do recurso de [usuário](/graph/api/resources/user).
Falha ao ler ou atualizar uma foto, nesse caso, resulta no seguinte erro:

```javascript
{
  "error": {
    "code": "ErrorNonExistentMailbox",
    "message": "The SMTP address has no mailbox associated with it."
  }
}
```

### <a name="revoke-sign-in-sessions-returns-wrong-http-code"></a>A revogação de sessões de entrada retorna um código HTTP errado

O [usuário: revokeSignInSessions API](/graph/api/user-revokesigninsessions) deve retornar uma resposta `204 No content` para ter revogações bem-sucedidas e um código de erro HTTP (4xx ou 5xx) se algo der errado com a solicitação.  No entanto, devido a um problema de serviço, essa API retorna um parâmetro `200 OK` e um parâmetro booleano que é sempre `true`.  Até que isso seja corrigido, você pode tratar qualquer código de retorno 2xx como bem-sucedido para esta API.

### <a name="incomplete-objects-are-returned-when-using-getbyids-request"></a>Objetos incompletos são retornados ao usar a solicitação getByIds

A solicitação de objetos usando a opção de [Obter objetos de diretório de uma lista de IDs](/graph/api/directoryobject-getbyids) deve retornar objetos completos. No entanto, atualmente, os objetos de [usuário](/graph/api/resources/user) no ponto de extremidade v1.0 são retornados com um conjunto limitado de propriedades. Como solução temporária, ao usar a operação em combinação com a opção de consulta `$select`, objetos de [usuário](/graph/api/resources/user) mais completos serão retornados. Esse comportamento não está de acordo com as especificações do OData. Como esse comportamento pode ser atualizado no futuro, use esta solução alternativa apenas quando fornecer `$select=` com todas as propriedades de seu interesse e somente se futuras alterações nessa solução alternativa forem aceitáveis.

## <a name="query-parameters"></a>Parâmetros de consulta 

### <a name="some-limitations-apply-to-query-parameters"></a>Algumas limitações se aplicam aos parâmetros de consulta

As seguintes limitações se aplicam aos parâmetros de consulta:

* Não há suporte para vários namespaces.
* Não há suporte para as solicitações GET no `$ref` e também para transmissão em usuários, grupos, dispositivos, entidades de serviço e aplicativos.
* `@odata.bind` não é compatível. Isso significa que os você não pode definir corretamente as propriedades de navegação **acceptedSenders** ou **rejectedSenders** em um grupo.
* `@odata.id` não está presente na navegação sem confinamento (como mensagens) quando há o uso de metadados mínimos.
* `$expand`:
  * Retorna um máximo de 20 objetos.
  * Sem suporte para `@odata.nextLink`.
  * Sem suporte para mais de um nível de expansão.
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


## <a name="functionality-available-only-in-office-365-rest-or-azure-ad-graph-apis-deprecated"></a>Funcionalidade disponível somente nas APIs rest do Office 365 ou do Graph do Azure Active Directory (preterida)

Alguns recursos ainda não estão disponíveis no Microsoft Graph. Se você não vir a funcionalidade que está procurando, poderá usar as [APIs REST do Office 365](/previous-versions/office/office-365-api/) específicas do ponto de extremidade. Para o Azure Active Directory Graph, consulte [Migrar aplicativos do Graph do Azure Active Directory (Azure AD) para Microsoft Graph](./migrate-azure-ad-graph-overview.md).
