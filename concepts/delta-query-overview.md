---
title: Usar a consulta delta para controlar alterações nos dados do Microsoft Graph
description: Delta query enables applications to discover newly created, updated, or deleted entities without performing a full read of the target resource with every request. Microsoft Graph applications can use delta query to efficiently synchronize changes with a local data store.
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 7e969858b7537ea36189d24c449803d2a00b125e
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "44990035"
---
# <a name="use-delta-query-to-track-changes-in-microsoft-graph-data"></a>Usar a consulta delta para controlar alterações nos dados do Microsoft Graph

Delta query enables applications to discover newly created, updated, or deleted entities without performing a full read of the target resource with every request. Microsoft Graph applications can use delta query to efficiently synchronize changes with a local data store.

> [!div class="nextstepaction"]
> [Tutorial: usar notificações de alteração e controlar alterações com o Microsoft Graph](/learn/modules/msgraph-changenotifications-trackchanges)

## <a name="use-delta-query-to-track-changes-in-a-resource-collection"></a>Usar solicitação delta para rastrear alterações em uma coleção resource

O padrão típico de chamada corresponde ao que segue:

1. O aplicativo começa chamando uma solicitação GET com a função delta no recurso desejado.
2. O Microsoft Graph envia uma resposta que contém o recurso solicitado e um [token de estado](#state-tokens).

     a.  If a `nextLink` URL is returned, there may be additional pages of data to be retrieved in the session. The application continues making requests using the `nextLink` URL to retrieve all pages of data until a `deltaLink` URL is returned in the response.

     b.  If a `deltaLink` URL is returned, there is no more data about the existing state of the resource to be returned. For future requests, the application uses the `deltaLink` URL to learn about changes to the resource.

3. When the application needs to learn about changes to the resource, it makes a new request using the `deltaLink` URL received in step 2. This request *may* be made immediately after completing step 2 or when the application checks for changes.
4. O Microsoft Graph retorna uma resposta, descrevendo alterações no recurso desde a solicitação anterior e em uma URL `nextLink` ou uma URL `deltaLink`.

>**Observação:** recursos armazenados no Azure Active Directory (por exemplo, usuários e grupos) dão suporte a cenários do tipo "sincronizar a partir de agora". Isso permite que você ignore as etapas 1 e 2 acima (se você não está interessado em recuperar o estado completo do recurso) e peça para conferir o último `deltaLink` em vez disso. Acrescente `$deltaToken=latest` à função `delta`, e a resposta conterá um `deltaLink` e nenhum dado do recurso.

>**Observação:** a função de consulta Delta geralmente é referida ao acrescentar `/delta` ao nome do recurso. No entanto, `/delta` é um atalho para o nome totalmente qualificado `/microsoft.graph.delta` que você vê em solicitações geradas pelos SDKs do Microsoft Graph.

>**Observação:** A solicitação inicial para a função de consulta Delta (sem token Delta ou Skip) retornará os recursos que existem atualmente na coleção. Os recursos que foram criados e excluídos antes da consulta Delta inicial não serão retornados. As atualizações feitas antes da solicitação inicial são resumidas no recurso retornado como seu estado mais recente.

### <a name="state-tokens"></a>Tokens de estado

A delta query GET response always includes a URL specified in a `nextLink` or `deltaLink` response header.
The `nextLink` URL includes a _skipToken_, and a `deltaLink` URL includes a _deltaToken_.

These tokens are opaque to the client. The following details are what you need to know about them:

- Cada token reflete o estado e representa um instantâneo do recurso dessa fase do controle de alterações.

- The state tokens also encode and include other query parameters (such as `$select`) specified in the initial delta query request. Therefore, it's not required to repeat them in subsequent delta query requests.

- Ao realizar a consulta delta, você pode copiar e aplicar a URL `nextLink` ou `deltaLink` à próxima chamada de função **delta** sem precisar inspecionar o conteúdo da URL, incluindo seu token de estado.

### <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

If a client uses a query parameter, it must be specified in the initial request. Microsoft Graph automatically encodes the specified parameter into the `nextLink` or `deltaLink` provided in the response. The calling application only needs to specify the query parameters once upfront. Microsoft Graph adds the specified parameters automatically for all subsequent requests.

Observe o suporte geral limitado dos seguintes parâmetros de consulta opcionais:

- `$orderby`

    Não assuma que uma sequência específica das respostas tenha retornado de uma consulta delta. Suponha que o mesmo item possa aparecer em qualquer lugar na sequência do `nextLink` e leve isso em conta em sua lógica de mesclagem.
- `$top`

    O número de objetos em cada página pode variar dependendo do tipo de recurso e do tipo de alterações feitas no recurso.

Para obter o recurso[mensagem](/graph/api/resources/message?view=graph-rest-1.0), consulte os detalhes do [suporte aos parâmetros de consulta em uma consulta delta](delta-query-messages.md#use-query-parameters-in-a-delta-query-for-messages).

Para os recursos de [usuário](/graph/api/resources/user?view=graph-rest-1.0) e [grupo](/graph/api/resources/group?view=graph-rest-1.0), há restrições no uso de alguns parâmetros de consulta:

- Não há suporte para `$expand`.
- Não há suporte para `$top`.
- Não há suporte para `$orderby`.
- If a `$select` query parameter is used, the parameter indicates that the client prefers to only track changes on the properties or relationships specified in the `$select` statement. If a change occurs to a property that is not selected, the resource for which that property changed does not appear in the delta response after a subsequent request.
- O `$select` também tem suporte para `manager` e `members` propriedade de navegação para usuários e grupos, respectivamente. A seleção dessas propriedades permite controlar as alterações feitas no gerenciador de usuário e nas associações de grupo.

- Os filtros de escopo permitem controlar alterações para um ou mais usuários ou grupos específicos por ID de objeto. Por exemplo, a solicitação a seguir retorna alterações para os grupos que correspondem às IDs especificadas no filtro de consulta.

<!-- {
  "blockType": "request",
  "name": "group_delta"
}-->
```http
https://graph.microsoft.com/beta/groups/delta/?$filter=id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ae5f' or id eq '004d6a07-fe70-4b92-add5-e6e37b8acd8e'
```

## <a name="resource-representation-in-the-delta-query-response"></a>Representação de recurso na resposta da consulta delta

- Instâncias de um recurso recém-criadas de um recurso para o qual há suporte são representadas na resposta da consulta delta usando sua representação-padrão.

- Instâncias atualizadas são representadas por seus **id** com *pelo menos* as propriedades que foram atualizadas, mas podem ser incluídas propriedades adicionais.

- Relationships on users and groups are represented as annotations on the standard resource representation. These annotations use the format `propertyName@delta`. The annotations are included in the response of the initial delta query request.

As instâncias removidas são representadas por sua **id** e um objeto `@removed`. O objeto `@removed` pode incluir informações adicionais sobre o porquê de a instância ter sido removida. Por exemplo,  "@removido": {"motivo": “alterado”}.

Possíveis motivos @removed podem ser *changed* ou *deleted*.

- *Alterado* indica que o item foi excluído e poderá ser restaurado de [deletedItems](/graph/api/resources/directory).

- *Deleted* indica que o item foi excluído e não pode ser restaurado.

The `@removed` object can be returned in the initial delta query response and in tracked (deltaLink) responses. Clients using delta query requests should be designed to handle these objects in the responses.

>**Observação:** é possível que uma única entidade seja incluída várias vezes na resposta, caso essa entidade tenha sido alterada várias vezes e sob determinadas condições. As consultas Delta permitem aos aplicativos listar todas as alterações, mas não garantem que as entidades sejam unificadas em uma única resposta.

## <a name="supported-resources"></a>Recursos com suporte

A consulta delta é compatível atualmente com os seguintes recursos.

| **Coleção de recursos**                                        | **API**                                                                                                                                                                                          |
|:---------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Aplicativos                                                   | Função [delta](/graph/api/application-delta) do recurso [aplicativo](/graph/api/resources/application)                                                                                   |
| Unidades administrativas (visualização)                                 | função [delta](/graph/api/administrativeunit-delta) do recurso [administrativeUnit](/graph/api/resources/administrativeunit) (visualização)                                                    |
| Mensagens de chat em um canal (visualização)                           | função [delta](/graph/api/chatmessage-delta) do recurso [chatMessage](/graph/api/resources/chatmessage)                                                                                            |
| Classes (pré-visualização)                                              | Função [delta](/graph/api/educationclass-delta) do recurso [educationClass](/graph/api/resources/educationclass) (visualização)                                                                |
| Objetos de diretório (visualização)                                    | Função [delta](/graph/api/directoryobject-delta) do recurso [directoryObjects](/graph/api/resources/directoryobject) (visualização)                                                             |
| Funções de diretório                                                | Função [delta](/graph/api/directoryrole-delta?view=graph-rest-1.0) do recurso [directoryRole](/graph/api/resources/directoryrole?view=graph-rest-1.0)                                     |
| Itens de unidade\*                                                  | Função [delta](/graph/api/driveitem-delta?view=graph-rest-1.0) do recurso [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0)                                                 |
| Usuários da educação (pré-visualização)                                      | Função [delta](/graph/api/educationuser-delta) do recurso [educationUser](/graph/api/resources/educationuser) (visualização)                                                                   |
| Eventos em um modo de exibição de calendário (intervalo de datas) do calendário principal | função [delta](/graph/api/event-delta?view=graph-rest-1.0) do recurso [evento](/graph/api/resources/event?view=graph-rest-1.0)                                                             |
| Grupos                                                         | Função [delta](/graph/api/group-delta?view=graph-rest-1.0) do recurso [group](/graph/api/resources/group?view=graph-rest-1.0)                                                             |
| Pastas de email                                                   | função [delta](/graph/api/mailfolder-delta?view=graph-rest-1.0) do recurso [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0)                                               |
| Mensagens de uma pasta                                           | função [delta](/graph/api/message-delta?view=graph-rest-1.0) do recurso [mensagem](/graph/api/resources/message?view=graph-rest-1.0)                                                        |
| Contatos organizacionais                                        | função [delta](/graph/api/orgcontact-delta?view=graph-rest-1.0) do recurso [orgContact](/graph/api/resources/orgcontact?view=graph-rest-1.0)                                              |
| OAuth2PermissionGrants (visualização)                               | Função [delta](/graph/api/oauth2permissiongrant-delta?view=graph-rest-beta) do recurso [oauth2permissiongrant](/graph/api/resources/oauth2permissiongrant?view=graph-rest-beta) (visualização) |
| Pastas de contatos pessoais                                       | função [delta](/graph/api/contactfolder-delta?view=graph-rest-1.0) do recurso [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0)                                     |
| Contatos pessoais em uma pasta                                  | Função [delta](/graph/api/contact-delta?view=graph-rest-1.0) do recurso [contato](/graph/api/resources/contact?view=graph-rest-1.0)                                                       |
| Itens do Planner\*\* (pré-visualização)                                    | função [delta](/graph/api/planneruser-list-delta) de todos os segmentos do recurso [plannerUser](/graph/api/resources/planneruser) (visualização)                                                     |
| Escolas (pré-visualização)                                              | Função [delta](/graph/api/educationschool-delta) do recurso [educationSchool](/graph/api/resources/educationschool) (visualização)                                                             |
| Entidades de serviço (visualização)                                   | Função [delta](/graph/api/serviceprincipal-delta) do recurso [servicePrincipal](/graph/api/resources/serviceprincipal) (visualização)                                                          |
| Usuários                                                          | função [delta](/graph/api/user-delta?view=graph-rest-1.0) do recurso [usuário](/graph/api/resources/user?view=graph-rest-1.0)                                                                |


> \* O padrão de uso dos recursos do OneDrive é semelhante a outros recursos compatíveis com algumas pequenas diferenças de sintaxe. A consulta delta para unidades será atualizada no futuro para serem consistentes com outros tipos de recursos. Confira mais detalhes sobre a sintaxe atual em [Controlar alterações para uma unidade](/graph/api/driveitem-delta?view=graph-rest-1.0).

> \*\* O padrão de uso dos recursos do Planner é semelhante a outros recursos compatíveis, mas com algumas diferenças.  Para saber mais, consulte [Controlar alterações para o Planner](/graph/api/planneruser-list-delta).

## <a name="limitations"></a>Limitações

### <a name="properties-stored-outside-of-the-main-data-store"></a>Propriedades armazenadas fora do repositório de dados principal

Alguns recursos contêm propriedades armazenadas fora do repositório de dados principal do recurso (por exemplo, o recurso de usuário é armazenado no sistema Azure AD, enquanto algumas propriedades, como **skills**, são armazenadas no SharePoint Online). Atualmente, não há suporte para essas propriedades como parte do controle de alterações; uma alteração em uma dessas propriedades não resultará em um objeto aparecendo na resposta de consulta Delta. Atualmente, apenas as propriedades armazenadas no repositório de dados principal disparam alterações na consulta Delta.

Para verificar se uma propriedade pode ser usada na consulta Delta, experimente executar uma operação de `GET` regular na coleção de recursos e selecione a propriedade que você está interessado. Por exemplo, você pode usar a propriedade **skills** na coleção de usuários.

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/?$select=skills
```

Como a propriedade **skills** é armazenada fora do Azure AD, a seguinte é a resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->

```http
HTTP/1.1 501 Not Implemented
Content-type: application/json

{
    "error": {
        "code": "NotImplemented",
        "message": "This operation target is not yet supported.",
        "innerError": {
            "request-id": "...",
            "date": "2019-09-20T21:47:50"
        }
    }
}
```

Isso informa que não há suporte para a propriedade **skills** para a consulta Delta no recurso **user**.

### <a name="navigation-properties"></a>Propriedades de navegação

Não há suporte para propriedades de navegação. Por exemplo, você não pode controlar alterações na coleção de usuários que incluiriam alterações na propriedade **photo**; **photo** é uma propriedade de navegação armazenada fora da entidade do usuário, e as alterações feitas nela não fazem com que o objeto de usuário seja incluído na resposta Delta.

### <a name="processing-delays"></a>Atrasos de processamento

Esperar atrasos variáveis entre o tempo que uma alteração é feita em uma instância de recurso, que pode ser por meio de uma interface de aplicativo ou API, e o tempo em que a alteração controlada é refletida em uma resposta de consulta Delta.

### <a name="national-clouds"></a>Nuvens nacionais

As consultas Delta estão disponíveis para os clientes hospedados na nuvem pública e o Microsoft Graph na China operado apenas pela 21Vianet.

### <a name="token-duration"></a>Duração do token

Os tokens Delta só são válidos para um período específico, antes que o aplicativo cliente precise executar uma sincronização total novamente. Para objetos de diretório (**Application**, **administrativeUnit**, **directoryobject**, **directoryRole**, **Group**, **orgContact**, **oauth2permissiongrant**, **servicePrincipalName**e **User**), o limite é de sete dias. Para objetos de educação (**educationSchool**, **educationUser**e **educationClass**), o limite é de sete dias.

## <a name="prerequisites"></a>Pré-requisitos

As mesmas [permissões](./permissions-reference.md) necessárias para ler um recurso específico também são necessárias para executar a consulta delta nesse recurso.

## <a name="delta-query-request-examples"></a>Exemplos de solicitação de consulta delta

- [Obter as alterações incrementais para os eventos em um modo de exibição de calendário](delta-query-events.md)
- [Obter as alterações incrementais para as mensagens em uma pasta](./delta-query-messages.md)
- [Obter as alterações incrementais para grupos](./delta-query-groups.md)
- [Obter as alterações incrementais para usuários](./delta-query-users.md)
