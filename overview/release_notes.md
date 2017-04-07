# <a name="known-issues-with-microsoft-graph"></a>Problemas conhecidos com o Microsoft Graph

Este artigo descreve os problemas conhecidos com o Microsoft Graph. Para obter informações sobre as atualizações mais recentes, confira o [Log de alterações do Microsoft Graph](http://graph.microsoft.io/en-us/changelog).

## <a name="graph-explorer"></a>Explorador do Graph
Desativamos os logons da conta da Microsoft para o Explorer Graph devido a um problema de serviço. Estamos trabalhando ativamente em uma correção e atualizaremos este texto quando ela estiver pronta.  

Não era possível entrar pelo Internet Explorer e o Microsoft Edge. Esse problema foi resolvido no dia 2 de fevereiro de 2017.

## <a name="users"></a>Usuários
#### <a name="no-instant-access-after-creation"></a>Sem acesso instantâneo após a criação
Os usuários podem ser criados imediatamente por um POST na entidade do usuário. Uma licença do Office 365 deve ser atribuída a um usuário primeiro para que ele possa ter acesso aos serviços do Office 365. Mesmo assim, devido à natureza distribuída do serviço, pode demorar 15 minutos antes que os arquivos, as mensagens e as entidades de eventos fiquem disponíveis para uso por esse usuário na API do Microsoft Graph. Durante esse período, os aplicativos receberão uma resposta de erro 404 HTTP. 

#### <a name="photo-restrictions"></a>Restrições de foto
A leitura e a atualização da foto do perfil do usuário só serão possíveis se o usuário tiver uma caixa de correio. Além disso, as fotos que *possam* ter sido previamente armazenadas usando a propriedade **thumbnailPhoto** (usando a visualização da API unificada do Office 365, o Azure AD Graph ou por meio da sincronização do AD Connect) deixarão de estar acessíveis com a propriedade das fotos do usuário do Microsoft Graph. A falha na leitura ou na atualização de uma foto, nesse caso, resultaria no seguinte erro:

```javascript
    {
      "error": {
        "code": "ErrorNonExistentMailbox",
        "message": "The SMTP address has no mailbox associated with it."
      }
    }
```

 > **Observação**:  logo após a GA, o armazenamento e a recuperação de fotos de perfil de usuário serão habilitados, mesmo que o usuário não tenha uma caixa de correio, e esse erro deve desaparecer.


#### <a name="adding-and-accessing-ics-based-calendars-in-users-mailbox"></a>Adicionar e acessar calendários baseados em ICS na caixa de correio do usuário
Atualmente, há suporte parcial para um calendário com base em uma Inscrição em Calendário da Internet (ICS):

* Você pode adicionar um calendário baseado em ICS para uma caixa de correio do usuário por meio da interface do usuário, mas não através da API do Microsoft Graph. 
* [Listar os calendários do usuário](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_list_calendars) permite que você obtenha as propriedades **name**, **color** e **id** de cada [calendar](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/calendar) no grupo de calendários padrão do usuário ou em um grupo de calendários especificado, inclusive todos os calendários com base em ICS. Não é possível armazenar ou acessar a URL da ICS no recurso de calendário.
* Você também pode [listar os eventos](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/calendar_list_events) de um calendário baseado em ICS.

## <a name="groups"></a>Grupos
#### <a name="policy"></a>Política
O uso do Microsoft Graph para criar e nomear um grupo do Office 365 ultrapassa qualquer política de grupo do Office 365 que seja configurada pelo Outlook Web App. 

#### <a name="group-permission-scopes"></a>Escopos de permissão de grupo
O Microsoft Graph expõe dois escopos de permissão (*Group.Read.All* e *Group.ReadWrite.All*) para o acesso a APIs de grupos.  
Esses escopos de permissão devem ser permitidos por um administrador (que é uma alteração da visualização).  No futuro, pretendemos adicionar novos escopos para grupos que possam ser permitidos pelos usuários.

Além disso, somente a API para administração de grupo principal e gerenciamento suporta acesso usando permissões delegadas ou somente para aplicativos. Todos os outros recursos da API do grupo dão suporte apenas a permissões delegadas. 

Exemplos de recursos de grupo que oferecem suporte a permissões delegadas e somente para aplicativos: 

* Criar e excluir grupos
* Obter e atualizar propriedades do grupo pertencentes ao gerenciamento ou administração de grupo
* [Definições do diretório](../api-reference/v1.0/resources/directoryobject.md), tipo e sincronização do grupo
* Membros e proprietários de grupo


Exemplos de recursos de grupo que oferecem suporte somente a permissões delegadas:

* Conversas, eventos e foto de grupo
* Remetentes externos, remetentes aceitos ou rejeitados e assinatura de grupo
* Favoritos do usuário e contagem de não vistos


#### <a name="adding-and-getting-attachments-of-group-posts"></a>Adicionando e obtendo anexos de postagens de grupo
A [adição](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/post_post_attachments) de anexos a postagens de grupo a [listagem](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/post_list_attachments) e a obtenção de anexos de postagens do grupo atualmente retornam a mensagem de erro "A solicitação de OData não tem suporte." Uma correção foi implementada nas versões `/v1.0` e `/beta`, e deve estar amplamente disponível até o final de janeiro de 2016.


#### <a name="setting-the-allowexternalsenders-property"></a>Definir a propriedade allowExternalSenders
Atualmente, há um problema que impede a configuração da propriedade **allowExternalSenders** de um grupo em uma operação de POST ou PATCH no `/v1.0` e no `/beta`.


## <a name="contacts"></a>Contatos

#### <a name="organization-contacts-available-in-only-beta"></a>Contatos de organização disponíveis somente na versão beta
Somente os contatos pessoais têm suporte no momento. Os contatos organizacionais atualmente não têm suporte na `/v1.0`, mas podem ser encontrados na versão `/beta`.

#### <a name="default-contacts-folder"></a>Pasta Contatos padrão

Na versão `/v1.0`, `GET /me/contactFolders` não inclui a pasta de contatos do usuário padrão. 

Uma correção será disponibilizada. Enquanto isso, você pode usar a seguinte consulta [list contacts](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_list_contacts) e a propriedade **parentFolderId** como uma solução alternativa para obter a ID da pasta de contatos padrão:

```
GET https://graph.microsoft.com/v1.0/me/contacts?$top=1&$select=parentFolderId
```
Na consulta acima:
1. `/me/contacts?$top=1` obtém as propriedades de um [contato](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/contact) na pasta de contatos padrão.
2. A anexação de `&$select=parentFolderId` retorna apenas a propriedade **parentFolderId** do contato, que é a ID da pasta de contatos padrão.


#### <a name="accessing-contacts-via-a-contact-folder-in-beta"></a>Acessar contatos por meio de uma pasta de contatos na versão beta
Atualmente, não há na versão `/beta` um problema que impeça o acesso a um [contato](../api-reference/beta/resources/contact.md) especificando sua pasta pai na URL de solicitação REST, conforme mostrado nos dois cenários abaixo.

* Acessando um contato a partir de um nível superior do [contactFolder](../api-reference/beta/resources/contactfolder.md) do usuário.
```http
GET /me/contactfolders/{id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```
* Acessando um contato contido em uma pasta filha de um **contactFolder**.  O exemplo a seguir mostra um nível de aninhamento, mas um contato pode estar localizado em um filho de um filho e assim por diante.
```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```

Como alternativa, você pode simplesmente [obter](../api-reference/beta/api/contact_get.md) o contato, especificando sua identificação conforme mostrado abaixo, uma vez que o GET /contacts na versão `/beta` se aplica a todos os contatos na caixa de correio do usuário:

```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```

## <a name="messages"></a>Mensagens
#### <a name="the-comment-parameter-for-creating-a-draft"></a>O parâmetro de comentário para criar um rascunho
O parâmetro **comment** para criar uma resposta ou rascunho de encaminhamento ([createReply](../api-reference/v1.0/api/message_createreply.md), [createReplyAll](../api-reference/v1.0/api/message_createreplyall.md), [createForward](../api-reference/v1.0/api/message_createforward.md)) não se torna parte do corpo do rascunho de mensagem resultante.  


## <a name="drives-files-and-content-streaming"></a>Unidades, arquivos e streaming de conteúdo
* O acesso pela primeira vez a uma unidade pessoal de um usuário pelo Microsoft Graph antes que ele acesse seu site pessoal por um navegador resulta em uma resposta 401.

## <a name="functionality-available-only-in-office-365-rest-apis"></a>Funcionalidade disponível apenas nas APIs REST do Office 365

Alguns recursos ainda não estão disponíveis no Microsoft Graph. Se você não vir a funcionalidade que está procurando, poderá usar as [APIs REST do Office 365](https://msdn.microsoft.com/en-us/office/office365/api/api-catalog) específicas do ponto de extremidade.


#### <a name="batching"></a>Envio em lote
O envio em lote não tem suporte do Microsoft Graph. No entanto, você pode usar o ponto de extremidade do Outlook beta e [enviar as chamadas REST do Outlook em lote](https://msdn.microsoft.com/en-us/office/office365/api/batch-outlook-rest-requests). 

#### <a name="availability-in-china"></a>Disponibilidade na China
O serviço Microsoft Graph é operado pela 21Vianet (e agora está disponível na China). Revise [Implantações na nuvem soberana do Microsoft Graph](http://developer.microsoft.com/en-us/graph/docs/overview/deployments) para obter mais detalhes, incluindo restrições.

#### <a name="service-actions-and-functions"></a>Funções e ações de serviço
`isMemberOf` e `getObjectsById` não estão disponíveis no Microsoft Graph

## <a name="microsoft-graph-permissions"></a>Permissões do Microsoft Graph
Para obter os detalhes mais recentes sobre as permissões delegadas e os aplicativos com suporte do Microsoft Graph, examine os [Escopos de permissão](http://developer.microsoft.com/en-us/graph/docs/authorization/permission_scopes). Além disso, as seguintes limitações aplicam-se a `v1.0`:

|Permissão |    Tipo de permissão | Limitação |    Alternativa |
|-----------|-----------------|------------|--------------|
|_User.ReadWrite_| Delegado    | Não é possível atualizar o número de celular|    Selecione também `Directory.AccessAsUser.All`| 
|_User.ReadWrite.All_|    Delegado|    Não é possível realizar operações de CRUD no `User` além de atualizar a foto do usuário em alta definição e as propriedades de perfil avançadas|    Também selecione `Directory.ReadWrite.All` ou `Directory.AccessAsUser.All` se a exclusão do usuário é obrigatória.|
|_User.Read.All_|    Aplicativo    |Não é possível executar operações de leitura em outros usuários|    Selecione também `Directory.Read.All`|
| _User.ReadWrite.All_ |    Aplicativo |    Não é possível realizar operações de CRUD no `User` além de atualizar a foto do usuário em alta definição e as propriedades de perfil avançadas |    Selecione também`Directory.ReadWrite.All`. **OBSERVAÇÃO**: Não será possível excluir o usuário.|
|_Group.Read.All_    | Aplicativo |    Não é possível enumerar grupos ou associações de grupo.  Ainda pode ler o conteúdo de grupo para Grupos do Office    | Selecione também `Directory.Read.All` |
|_Group.ReadWrite.All_    | Aplicativo    | Não é possível enumerar associações de grupo ou grupos, criar grupos, atualizar associações de grupo ou excluir grupos.  Ainda é possível ler e atualizar o conteúdo de grupo para os Grupos do Office.    | Selecione também `Directory.ReadWrite.All`. **OBSERVAÇÃO**:  Não será possível excluir o grupo.|

Além disso, existem as seguintes limitações da `/beta`:

|Permissão |    Tipo de permissão | Limitação |    Alternativa |
|-----------|-----------------|------------|--------------|
| _Group.ReadWrite.All_    | Delegado    | Não é possível ler ou atualizar tarefas do Planejador nos Grupos do Office    | Selecione também `Tasks.ReadWrite`|
|_Tasks.ReadWrite_    | Delegado    | Não é possível ler ou atualizar tarefas do usuário conectado| Selecione também `Group.ReadWrite.All`|

## <a name="odata-related-limitations"></a>Limitações relacionadas ao OData
* Limitações **$expand**: 
 * Sem suporte para `nextLink`
 * Não há suporte para mais de um nível de expansão
 * Não há suporte com parâmetros adicionais (**$filter**, **$select**)
* Não há suporte para vários namespaces
* GETs em `$ref` e conversão não têm suporte em usuários, grupos, dispositivos, entidades de serviço e aplicativos.
* Não há suporte para `@odata.bind`.  Isso significa que os desenvolvedores não serão capazes de definir corretamente `Accepted` ou `RejectedSenders` em um grupo.
* `@odata.id` não está presente na navegação sem confinamento (como mensagens) quando há o uso de metadados mínimos
* Filtragem/pesquisa entre cargas não disponível. 
* A pesquisa de texto completo (usando **$search**) só está disponível para alguns entidades, como mensagens.

  >  Seus comentários são importantes para nós. Junte-se a nós na página [Stack Overflow](http://stackoverflow.com/questions/tagged/office365). Marque as suas perguntas com {MicrosoftGraph} e {office365}.


