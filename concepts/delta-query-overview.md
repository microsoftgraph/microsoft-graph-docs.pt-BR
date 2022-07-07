---
title: Usar a consulta delta para controlar alterações nos dados do Microsoft Graph
description: Usar a consulta delta para habilitar os aplicativos a localizarem entidades recém-criadas, atualizadas ou excluídas sem executar uma leitura completa do recurso de destino com cada solicitação.
author: Jumaodhiss
ms.localizationpriority: high
ms.custom: graphiamtop20
ms.openlocfilehash: 844b86023c216b215530e1d0fc685185c73179d4
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671385"
---
# <a name="use-delta-query-to-track-changes-in-microsoft-graph-data"></a>Usar a consulta delta para controlar alterações nos dados do Microsoft Graph

A consulta delta permite que aplicativos localizem entidades recém-criadas, atualizadas ou excluídas sem executar uma leitura completa do recurso de destino com cada solicitação. Os aplicativos do Microsoft Graph podem usar consulta delta para sincronizar, com eficiência, alterações com armazenamento de dados local.

> [!div class="nextstepaction"]
> [Tutorial: usar notificações de alteração e controlar alterações com o Microsoft Graph](/learn/modules/msgraph-changenotifications-trackchanges)

## <a name="use-delta-query-to-track-changes-in-a-resource-collection"></a>Usar solicitação delta para rastrear alterações em uma coleção resource

O padrão típico de chamada corresponde ao que segue:

1. O aplicativo começa chamando uma solicitação GET com a função delta no recurso desejado.
2. O Microsoft Graph envia uma resposta que contém o recurso solicitado e um [token de estado](#state-tokens).

     a.  Se uma URL `@odata.nextLink` é retornada, poderá haver páginas de dados adicionais a serem recuperadas na sessão. O aplicativo continua fazendo solicitações usando a URL `@odata.nextLink` para recuperar todas as páginas de dados até que uma URL `@odata.deltaLink` seja retornada na resposta.

     b.  Se uma URL `@odata.deltaLink` é retornada, não há mais nenhum dado sobre o estado do recurso a ser retornado. Em solicitações futuras, o aplicativo usa a URL `@odata.deltaLink` para inteirar-se das alterações feitas no recurso.

3. Quando o aplicativo precisa saber das alterações no recurso, ele faz uma nova solicitação usando a URL `@odata.deltaLink` recebida na etapa 2. Esta solicitação *pode* ser feita imediatamente após concluir a etapa 2 ou quando o aplicativo verifica as alterações.
4. O Microsoft Graph retorna uma resposta, descrevendo alterações no recurso desde a solicitação anterior e em uma URL `@odata.nextLink` ou uma URL `@odata.deltaLink`.

> [!NOTE]
> Recursos armazenados no Azure Active Directory (tais como usuários e grupos) dão suporte a cenários do tipo "sincronizar a partir de agora". Isso permite que você ignore as etapas 1 e 2 acima (se você não está interessado em recuperar o estado completo do recurso) e peça para conferir o último `@odata.deltaLink` em vez disso. Acrescente `$deltaToken=latest` à função `delta`, e a resposta conterá um `@odata.deltaLink` e nenhum dado do recurso. Os recursos do OneDrive e do Microsoft Office SharePoint Online também oferecem suporte a esse recurso. Para recursos no OneDrive e no Microsoft Office SharePoint Online, anexe `token=latest` em vez disso.

> [!NOTE]
> A função de consulta Delta é geralmente referida ao anexar `/delta` o nome do recurso. No entanto, `/delta` é um atalho para o nome totalmente qualificado `/microsoft.graph.delta` que você vê em solicitações geradas pelos SDKs do Microsoft Graph.

> [!NOTE]
> A solicitação inicial para a função de consulta delta (sem `$deltaToken` ou `$skipToken`) devolverá os recursos que existem atualmente na coleção. Os recursos que foram criados e excluídos antes da consulta delta inicial não serão retornados. As atualizações feitas antes da solicitação inicial são resumidas no recurso retornado como seu estado mais recente.

### <a name="state-tokens"></a>Tokens de estado

Um GET de consulta delta sempre inclui uma URL especificada em um cabeçalho de resposta `@odata.nextLink` ou `@odata.deltaLink`. A URL `@odata.nextLink` inclui um `$skipToken` e uma URL `@odata.deltaLink` inclui um `$deltaToken`.

Esses tokens são opacos para o cliente. Os seguintes detalhes são o que você precisa saber sobre eles:

- Cada token reflete o estado e representa um instantâneo do recurso dessa fase do controle de alterações.

- Os tokens de estado também codificam e incluem outros parâmetros da consulta (como `$select`) especificados na solicitação de consulta delta inicial. Portanto, ele não é necessário repeti-los em solicitações de consulta delta subsequentes.

- Ao realizar a consulta delta, você pode copiar e aplicar a URL `@odata.nextLink` ou `@odata.deltaLink` à próxima chamada de função **delta** sem precisar inspecionar o conteúdo da URL, incluindo seu token de estado.

### <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Se um cliente usa um parâmetro de consulta, ele deve ser especificado na solicitação inicial. O Microsoft Graph codifica automaticamente o parâmetro especificado em `@odata.nextLink` ou `@odata.deltaLink` fornecidos na resposta. O aplicativo de chamada só precisa especificar os parâmetros de consulta desejados uma vez antecipados. O Microsoft Graph adiciona os parâmetros especificados automaticamente para todas as solicitações subsequentes.

Observe o suporte geral limitado dos seguintes parâmetros de consulta opcionais:

- `$orderby`

    Não assuma uma sequência específica das respostas retornadas de uma consulta delta. Suponha que o mesmo item possa aparecer em qualquer lugar na sequência `@odata.nextLink` e trate isso em sua lógica de mesclagem.
- `$top`

    O número de objetos em cada página pode variar dependendo do tipo de recurso e do tipo de alterações feitas no recurso.

Para obter o recurso[mensagem](/graph/api/resources/message), consulte os detalhes do [suporte aos parâmetros de consulta em uma consulta delta](delta-query-messages.md#use-query-parameters-in-a-delta-query-for-messages).

Para os recursos de [usuário](/graph/api/resources/user) e [grupo](/graph/api/resources/group), há restrições no uso de alguns parâmetros de consulta:

- Não há suporte para `$expand`.
- Não há suporte para `$top`.
- Não há suporte para `$orderby`.
- Se um parâmetro de consulta `$select` for usado, isso indica que o cliente prefere somente controlar alterações nas propriedades ou relações especificadas na instrução `$select`. Se ocorrer uma alteração em uma propriedade que não esteja selecionada, o recurso por meio do qual essa propriedade foi alterada não aparecerá na resposta delta após uma solicitação subsequente.
- `$select` também suporta às propriedades de navegação do **gerente** e **membros** para usuários e grupos, respectivamente. A seleção dessas propriedades permite controlar as alterações feitas no gerenciador de usuário e nas associações de grupo.

- Os filtros de escopo permitem controlar alterações para um ou mais usuários ou grupos específicos por ID de objeto. Por exemplo, a seguinte solicitação retorna alterações para os grupos que correspondem às IDs especificadas no filtro de consulta.

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

- Os relacionamentos nos usuários e grupos são representados como anotações na representação de recursos padrão. Essas anotações usam o formato **propertyName@delta**. As anotações estão incluídas na resposta da solicitação da consulta delta inicial.

As instâncias removidas são representadas pela sia **ID** e um objeto **@removido**. O objeto **@removido** pode incluir informações adicionais sobre por que a instância foi removida. Por exemplo,  `"@removed": {"reason": "changed"}`.

Os possíveis motivos de ser **@removido** podem ser `changed` ou `deleted`.

- `changed` indica que o item foi excluído e poderá ser restaurado de [deletedItems](/graph/api/resources/directory).

- `deleted` indica que o item foi excluído e não pode ser restaurado.

O objeto **@removido** pode ser retornado na resposta inicial da consulta delta e nas respostas rastreadas (deltaLink). Os clientes que usam solicitações de consulta delta devem ser projetados para lidar com esses objetos nas respostas.

> [!NOTE]
> É possível que uma única entidade seja incluída várias vezes na resposta, caso essa entidade tenha sido alterada várias vezes e sob determinadas condições. As consultas Delta permitem aos aplicativos listar todas as alterações, mas não garantem que as entidades sejam unificadas em uma única resposta.

## <a name="supported-resources"></a>Recursos com suporte

Atualmente, a consulta delta é compatível com os recursos a seguir. Observe que alguns recursos que estão disponíveis na v1.0 têm suas funções **delta** correspondentes ainda em status de versão prévia, conforme indicado.

| **Coleção de recursos**                                        | **API**                                                                                                                                            |
| :------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------- |
| Aplicativos                                                   | Função [delta](/graph/api/application-delta) do recurso [aplicativo](/graph/api/resources/application)                                     |
| Unidades administrativas (visualização)                                 | Função [delta](/graph/api/administrativeunit-delta) (visualização) do recurso [administrativeUnit](/graph/api/resources/administrativeunit)      |
| Mensagens de chat em um canal.                                     | Função [delta](/graph/api/chatmessage-delta) (visualização) do [chatMessage](/graph/api/resources/chatmessage)                                    |
| Funções de diretório                                                | Função [delta](/graph/api/directoryrole-delta) do recurso [directoryRole](/graph/api/resources/directoryrole) |
| Itens de unidade\*                                                  | Função [delta](/graph/api/driveitem-delta) do recurso [driveItem](/graph/api/resources/driveitem)             |
| Atribuições de educação                                          | função [delta](/graph/api/educationassignment-delta) do recurso [educationAssignment](/graph/api/resources/educationassignment)             |
| Categorias educacionais                                           | função [delta](/graph/api/educationcategory-delta) do recurso [educationCategory](/graph/api/resources/educationcategory)                   |
| Aulas de educação                                              | Função [delta](/graph/api/educationclass-delta) do recurso [educationClass](/graph/api/resources/educationclass)                            |
| Escolas da Educação                                              | Função [delta](/graph/api/educationschool-delta) do recurso [educationSchool](/graph/api/resources/educationschool)                         |
| Usuários da educação                                                | Função [delta](/graph/api/educationuser-delta) do recurso [educationUser](/graph/api/resources/educationuser)                               |
| Eventos em um modo de exibição de calendário (intervalo de datas) do calendário principal | função [delta](/graph/api/event-delta) do recurso [evento](/graph/api/resources/event)                         |
| Grupos                                                         | Função [delta](/graph/api/group-delta) do recurso [group](/graph/api/resources/group)                         |
| Listar itens\*                                                   | função [delta](/graph/api/listitem-delta) do recurso [listItem](/graph/api/resources/listitem)                |
| Pastas de email                                                   | função [delta](/graph/api/mailfolder-delta) do recurso [mailFolder](/graph/api/resources/mailfolder)           |
| Mensagens de uma pasta                                           | função [delta](/graph/api/message-delta) do recurso [mensagem](/graph/api/resources/message)                    |
| Contatos organizacionais                                        | função [delta](/graph/api/orgcontact-delta) do recurso [orgContact](/graph/api/resources/orgcontact)          |
| OAuth2PermissionGrants                                         | Função [delta](/graph/api/oauth2permissiongrant-delta) do recurso [oauth2permissiongrant](/graph/api/resources/oauth2permissiongrant)         |
| Pastas de contatos pessoais                                       | função [delta](/graph/api/contactfolder-delta) do recurso [contactFolder](/graph/api/resources/contactfolder) |
| Contatos pessoais em uma pasta                                  | Função [delta](/graph/api/contact-delta) do recurso [contato](/graph/api/resources/contact)                   |
| Itens do Planner\*\* (pré-visualização)                                    | Função [delta](/graph/api/planneruser-list-delta) (visualização) de todos os segmentos do recurso [plannerUser](/graph/api/resources/planneruser)        |
| Entidades de serviço                                             | Função [delta](/graph/api/serviceprincipal-delta) do recurso [servicePrincipal](/graph/api/resources/serviceprincipal)                       |
| Tarefas pendente em uma lista de tarefas                                     | Função [delta](/graph/api/todotask-delta) do recurso [todoTask](/graph/api/resources/todotask)                                               |
| Listas de tarefas pendentes                                               | Função [delta](/graph/api/todotasklist-delta) do recurso [todoTaskList](/graph/api/resources/todotasklist)                                   |
| Usuários                                                          | função [delta](/graph/api/user-delta) do recurso [usuário](/graph/api/resources/user)                            |


> \* O padrão de uso para recursos do OneDrive e do SharePoint é semelhante aos outros recursos com suporte com algumas pequenas diferenças de sintaxe. A consulta delta para unidades e listas será atualizada no futuro para ser consistente com outros tipos de recursos. Para obter mais detalhes sobre a sintaxe atual, consulte [driveItem: delta](/graph/api/driveitem-delta) e [listItem: delta](/graph/api/listitem-delta).

> \*\* O padrão de uso dos recursos do Planner é semelhante a outros recursos com suporte com algumas diferenças. Para obter detalhes, consulte [planner: delta](/graph/api/planneruser-list-delta).

## <a name="limitations"></a>Limitações

### <a name="properties-stored-outside-of-the-main-data-store"></a>Propriedades armazenadas fora do repositório de dados principal

Alguns recursos contêm propriedades armazenadas fora do repositório de dados principal do recurso (por exemplo, o recurso de usuário é armazenado no sistema Azure AD, enquanto algumas propriedades, como **skills**, são armazenadas no SharePoint Online). Atualmente, não há suporte para essas propriedades como parte do controle de alterações; uma alteração em uma dessas propriedades não resultará em um objeto aparecendo na resposta de consulta Delta. Atualmente, apenas as propriedades armazenadas no repositório de dados principal disparam alterações na consulta Delta.

Para verificar se uma propriedade pode ser usada na consulta delta, tente executar uma operação `GET` regular na coleção de recursos e selecione a propriedade na qual você está interessado. Por exemplo, você pode tentar a propriedade **skills** na coleção de usuários.

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

As propriedades de navegação não são suportadas. Por exemplo, você não pode rastrear alterações na coleção de usuários que incluam alterações na propriedade da **foto**; **photo** é uma propriedade de navegação armazenada fora da entidade do usuário e as alterações nela não fazem com que o objeto do usuário seja incluído na resposta delta.

### <a name="processing-delays"></a>Atrasos de processamento

Esperar atrasos variáveis entre o tempo que uma alteração é feita em uma instância de recurso, que pode ser por meio de uma interface de aplicativo ou API, e o tempo em que a alteração controlada é refletida em uma resposta de consulta Delta.

Às vezes, as alterações que ocorreram no objeto podem não ser indicadas ao selecionar `@odata.nextLink` ou `@odata.deltaLink`. Isso porque algumas solicitações podem ter atrasos de replicação para objetos que foram criados, atualizados ou excluídos recentemente. Repita `@odata.nextLink` ou `@odata.deltaLink` depois de algum tempo para recuperar as alterações mais recentes.

### <a name="national-clouds"></a>Nuvens nacionais

As consultas Delta estão disponíveis para os clientes hospedados na nuvem pública e o Microsoft Graph na China operado apenas pela 21Vianet.

### <a name="replays"></a>Repetições

O aplicativo deve estar preparado para repetições, que ocorrem quando a mesma alteração aparece nas respostas subsequentes. Embora a consulta delta se esforce ao máximo para reduzir as repetições, elas ainda são possíveis.

### <a name="synchronization-reset"></a>Sincronização redefinida

A consulta Delta pode retornar um código de resposta de `410 (gone)` e um cabeçalho de **Localização** contendo um URL de solicitação com um `$deltaToken` vazio (o mesmo que a consulta inicial). Isso é uma indicação de que o aplicativo deve reiniciar com uma sincronização completa do locatário de destino. Isso geralmente acontece para evitar inconsistência de dados devido à manutenção interna ou migração do locatário de destino.

### <a name="token-duration"></a>Duração do token

Os tokens Delta só são válidos para um período específico, antes que o aplicativo cliente precise executar uma sincronização total novamente.
- Para [objetos de diretório](/graph/api/resources/directoryobject), o limite é de sete dias. 
- Para objetos educacionais (**educationSchool**, **educationUser** e **educationClass**), o limite é de sete dias.
- Para entidades do Outlook (**message**, **mailFolder**, **event**, **contact**, **contactFolder**, **todoTask**, and **todoTaskList**), o limite superior não é corrigido; depende do tamanho do cache de tokens do delta interno. Enquanto os novos tokens delta são adicionados ao cache, após a capacidade do cache ser excedida, os tokens delta mais antigos são excluídos.

No caso de um token expirado, o serviço deve responder com um erro da série 40X com códigos de erro como `syncStateNotFound`. Para obter mais informações, consulte [Códigos de erro no Microsoft Graph](/graph/errors#code-property).

## <a name="prerequisites"></a>Pré-requisitos

As mesmas [permissões](./permissions-reference.md) necessárias para ler um recurso específico também são necessárias para executar a consulta delta nesse recurso.

## <a name="delta-query-request-examples"></a>Exemplos de solicitação de consulta delta

- [Obter as alterações incrementais para os eventos em um modo de exibição de calendário](delta-query-events.md)
- [Obter as alterações incrementais para as mensagens em uma pasta](./delta-query-messages.md)
- [Obter as alterações incrementais para grupos](./delta-query-groups.md)
- [Obter as alterações incrementais para usuários](./delta-query-users.md)
