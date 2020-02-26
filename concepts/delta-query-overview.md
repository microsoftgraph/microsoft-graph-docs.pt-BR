---
title: Usar a consulta delta para controlar alterações nos dados do Microsoft Graph
description: A consulta delta permite que aplicativos localizem entidades recém-criadas, atualizadas ou excluídas sem executar uma leitura completa do recurso de destino com cada solicitação. Os aplicativos do Microsoft Graph podem usar consulta delta para sincronizar, com eficiência, alterações com armazenamento de dados local.
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 3ec98035d3d5e0de6a7ddd316446f3bd226930cf
ms.sourcegitcommit: 6144934d4f6cf8c9797aa19e62285217220c7f45
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/25/2020
ms.locfileid: "42268425"
---
# <a name="use-delta-query-to-track-changes-in-microsoft-graph-data"></a>Usar a consulta delta para controlar alterações nos dados do Microsoft Graph

A consulta delta permite que aplicativos localizem entidades recém-criadas, atualizadas ou excluídas sem executar uma leitura completa do recurso de destino com cada solicitação. Os aplicativos do Microsoft Graph podem usar consulta delta para sincronizar, com eficiência, alterações com armazenamento de dados local.

## <a name="use-delta-query-to-track-changes-in-a-resource-collection"></a>Usar solicitação delta para rastrear alterações em uma coleção resource

O padrão típico de chamada corresponde ao que segue:

1. O aplicativo começa chamando uma solicitação GET com a função delta no recurso desejado.
2. O Microsoft Graph envia uma resposta que contém o recurso solicitado e um [token de estado](#state-tokens).

     a.  Se uma URL `nextLink` é retornada, poderá haver páginas de dados adicionais a serem recuperadas na sessão. O aplicativo continua fazendo solicitações usando a URL `nextLink` para recuperar todas as páginas de dados até que uma URL `deltaLink` seja retornada na resposta.

     b.  Se uma URL `deltaLink` é retornada, não há mais nenhum dado sobre o estado do recurso a ser retornado. Em solicitações futuras, o aplicativo usa a URL `deltaLink` para inteirar-se das alterações feitas no recurso.

3. Quando o aplicativo precisa saber das alterações no recurso, ele faz uma nova solicitação usando a URL `deltaLink` recebida na etapa 2. Esta solicitação *pode* ser feita imediatamente após concluir a etapa 2 ou quando o aplicativo verifica as alterações.
4. O Microsoft Graph retorna uma resposta, descrevendo alterações no recurso desde a solicitação anterior e em uma URL `nextLink` ou uma URL `deltaLink`.

>**Observação:** recursos armazenados no Azure Active Directory (por exemplo, usuários e grupos) dão suporte a cenários do tipo "sincronizar a partir de agora". Isso permite que você ignore as etapas 1 e 2 acima (se você não está interessado em recuperar o estado completo do recurso) e peça para conferir o último `deltaLink` em vez disso. Acrescente `$deltaToken=latest` à função `delta`, e a resposta conterá um `deltaLink` e nenhum dado do recurso.  

>**Observação:** a função de consulta Delta geralmente é referida ao acrescentar `/delta` ao nome do recurso. No entanto, `/delta` é um atalho para o nome totalmente qualificado `/microsoft.graph.delta` que você vê em solicitações geradas pelos SDKs do Microsoft Graph.

### <a name="state-tokens"></a>Tokens de estado

Um GET de consulta delta sempre inclui uma URL especificada em um cabeçalho de resposta `nextLink` ou `deltaLink`. A URL `nextLink` inclui um _skipToken_ e uma URL `deltaLink` inclui um _deltaToken_.

Esses tokens são opacos para o cliente. Os seguintes detalhes são o que você precisa saber sobre eles:

- Cada token reflete o estado e representa um instantâneo do recurso dessa fase do controle de alterações.

- Os tokens de estado também codificam e incluem outros parâmetros da consulta (como `$select`) especificados na solicitação de consulta delta inicial. Portanto, ele não é necessário repeti-los em solicitações de consulta delta subsequentes.

- Ao realizar a consulta delta, você pode copiar e aplicar a URL `nextLink` ou `deltaLink` à próxima chamada de função **delta** sem precisar inspecionar o conteúdo da URL, incluindo seu token de estado.

### <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Se um cliente usa um parâmetro de consulta, ele deve ser especificado na solicitação inicial. O Microsoft Graph codifica automaticamente o parâmetro especificado em `nextLink` ou `deltaLink` fornecidos na resposta. O aplicativo de chamada só precisa especificar os parâmetros de consulta desejados uma vez antecipados. O Microsoft Graph adiciona os parâmetros especificados automaticamente para todas as solicitações subsequentes.

Observe o suporte geral limitado dos seguintes parâmetros de consulta opcionais:

- `$orderby` 
    
    Não assuma que uma sequência específica das respostas tenha retornado de uma consulta delta. Suponha que o mesmo item possa aparecer em qualquer lugar na sequência do `nextLink` e leve isso em conta em sua lógica de mesclagem.
- `$top` 
    
    O número de objetos em cada página pode variar dependendo do tipo de recurso e do tipo de alterações feitas no recurso.

Para obter o recurso[mensagem](/graph/api/resources/message?view=graph-rest-1.0), consulte os detalhes do [suporte aos parâmetros de consulta em uma consulta delta](delta-query-messages.md#use-query-parameters-in-a-delta-query-for-messages).

Para os recursos de [usuário](/graph/api/resources/user?view=graph-rest-1.0) e [grupo](/graph/api/resources/group?view=graph-rest-1.0), há restrições no uso de alguns parâmetros de consulta:

- Não há suporte para `$top`.
- Não há suporte para `$orderby`.
- Se um parâmetro de consulta `$select` for usado, isso indica que o cliente prefere somente controlar alterações nas propriedades ou relações especificadas na instrução `$select`. Se ocorrer uma alteração em uma propriedade que não esteja selecionada, o recurso por meio do qual essa propriedade foi alterada não aparecerá na resposta delta após uma solicitação subsequente.
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

- Relações entre os usuários e os grupos são representadas como anotações na representação do recurso padrão. Essas anotações usam o formato `propertyName@delta`. As anotações são incluídas na resposta da solicitação de consulta inicial delta.

As instâncias removidas são representadas por sua **id** e um objeto `@removed`. O objeto `@removed` pode incluir informações adicionais sobre o porquê de a instância ter sido removida. Por exemplo,  "@removido": {"motivo": “alterado”}.

Possíveis motivos @removed podem ser *changed* ou *deleted*.

- *Alterado* indica que o item foi excluído e poderá ser restaurado de [deletedItems](/graph/api/resources/directory?view=graph-rest-beta).

- *Deleted* indica que o item foi excluído e não pode ser restaurado.

O objeto `@removed` pode ser retornado na resposta de consulta delta inicial e nas respostas rastreadas (deltaLink). Os clientes que usam solicitações de consulta delta devem ser designados para lidar com esses objetos nas respostas.

>**Observação:** é possível que uma única entidade seja incluída várias vezes na resposta, caso essa entidade tenha sido alterada várias vezes e sob determinadas condições. As consultas Delta permitem aos aplicativos listar todas as alterações, mas não garantem que as entidades sejam unificadas em uma única resposta.

## <a name="supported-resources"></a>Recursos com suporte

A consulta delta é compatível atualmente com os seguintes recursos.

| **Coleção de recursos**                                        | **API**                                                                                                                                                                                |
| :------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Aplicativos (visualização)                                         | Função [delta](/graph/api/application-delta?view=graph-rest-beta) do recurso [application](/graph/api/resources/application?view=graph-rest-beta) (visualização)                     |
| Mensagens de chat em um canal (visualização)                            | função [delta](/graph/api/chatmessage-delta?view=graph-rest-beta) do recurso [chatMessage](/graph/api/resources/chatmessage?view=graph-rest-beta) |
| Classes (pré-visualização)                                              | Função [delta](/graph/api/educationclass-delta?view=graph-rest-beta) do recurso [educationClass](/graph/api/resources/educationclass?view=graph-rest-beta) (visualização)                     |
| Objetos de diretório (visualização)                                    | Função [delta](/graph/api/directoryobject-delta?view=graph-rest-beta) do recurso [directoryObjects](/graph/api/resources/directoryobject?view=graph-rest-beta) (visualização)        |
| Funções de diretório                                                | Função [delta](/graph/api/directoryrole-delta?view=graph-rest-1.0) do recurso [directoryRole](/graph/api/resources/directoryrole?view=graph-rest-1.0)                           |
| Itens de unidade\*                                                  | Função [delta](/graph/api/driveitem-delta?view=graph-rest-1.0) do recurso [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0)                                       |
| Usuários da educação (pré-visualização)                                      | Função [delta](/graph/api/educationuser-delta?view=graph-rest-beta) do recurso [educationUser](/graph/api/resources/educationuser?view=graph-rest-beta) (visualização)             |
| Eventos em um modo de exibição de calendário (intervalo de datas) do calendário principal | função [delta](/graph/api/event-delta?view=graph-rest-1.0) do recurso [evento](/graph/api/resources/event?view=graph-rest-1.0)                                                   |
| Grupos                                                         | Função [delta](/graph/api/group-delta?view=graph-rest-1.0) do recurso [group](/graph/api/resources/group?view=graph-rest-1.0)                                                   |
| Pastas de email                                                   | função [delta](/graph/api/mailfolder-delta?view=graph-rest-1.0) do recurso [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0)                                     |
| Mensagens de uma pasta                                           | função [delta](/graph/api/message-delta?view=graph-rest-1.0) do recurso [mensagem](/graph/api/resources/message?view=graph-rest-1.0)                                              |
| Pastas de contatos pessoais                                       | função [delta](/graph/api/contactfolder-delta?view=graph-rest-1.0) do recurso [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0)                           |
| Contatos pessoais em uma pasta                                  | Função [delta](/graph/api/contact-delta?view=graph-rest-1.0) do recurso [contato](/graph/api/resources/contact?view=graph-rest-1.0)    
| Itens do Planner\*\* (pré-visualização)                                    | função [delta](/graph/api/planneruser-list-delta?view=graph-rest-beta) de todos os segmentos do recurso [plannerUser](/graph/api/resources/planneruser?view=graph-rest-beta) (visualização)|                                         |
| Escolas (pré-visualização)                                              | Função [delta](/graph/api/educationschool-delta?view=graph-rest-beta) do recurso [educationSchool](/graph/api/resources/educationschool?view=graph-rest-beta) (visualização)                  |
| Entidades de serviço (visualização)                                   | Função [delta](/graph/api/serviceprincipal-delta?view=graph-rest-beta) do recurso [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) (visualização)      |
| Usuários                                                          | função [delta](/graph/api/user-delta?view=graph-rest-1.0) do recurso [usuário](/graph/api/resources/user?view=graph-rest-1.0) |


> \* O padrão de uso dos recursos do OneDrive é semelhante a outros recursos compatíveis com algumas pequenas diferenças de sintaxe. A consulta delta para unidades será atualizada no futuro para serem consistentes com outros tipos de recursos. Confira mais detalhes sobre a sintaxe atual em [Controlar alterações para uma unidade](/graph/api/driveitem-delta?view=graph-rest-1.0).

> \*\* O padrão de uso dos recursos do Planner é semelhante a outros recursos compatíveis, mas com algumas diferenças.  Para saber mais, consulte [Controlar alterações para o Planner](/graph/api/planneruser-list-delta?view=graph-rest-beta).

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

Os tokens Delta só são válidos para um período específico, antes que o aplicativo cliente precise executar uma sincronização total novamente. Para objetos de identidade (**directoryobject**, **directoryRole**, **Group**, **User**), o limite é 30 dias.

## <a name="prerequisites"></a>Pré-requisitos

As mesmas [permissões](./permissions-reference.md) necessárias para ler um recurso específico também são necessárias para executar a consulta delta nesse recurso.

## <a name="delta-query-request-examples"></a>Exemplos de solicitação de consulta delta

- [Obter as alterações incrementais para os eventos em um modo de exibição de calendário](delta-query-events.md)
- [Obter as alterações incrementais para as mensagens em uma pasta](./delta-query-messages.md)
- [Obter as alterações incrementais para grupos](./delta-query-groups.md)
- [Obter as alterações incrementais para usuários](./delta-query-users.md)
