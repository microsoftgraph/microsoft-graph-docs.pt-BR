---
title: Usar a API de Pesquisa da Microsoft para consultar dados
description: Utilizando a API de pesquisa, os aplicativos podem pesquisar os dados do Microsoft 365 no contexto do usuário autenticado
localization_priority: Priority
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: b363031992b58808d79747cdd122d56a98ebdb77
ms.sourcegitcommit: 366178d3fc37439791061082da80a63fba2c27df
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2020
ms.locfileid: "48921799"
---
# <a name="use-the-microsoft-search-api-to-query-data"></a>Usar a API de Pesquisa da Microsoft para consultar dados

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode utilizar a API de Pesquisa da Microsoft para consultar os dados do Microsoft 365 nos seus aplicativos.

As solicitações de pesquisa são executadas no contexto do usuário conectado, identificado usando um [token de acesso com permissões delegadas](/graph/auth-v2-user).

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

## <a name="common-use-cases"></a>Casos de uso comuns

A API de pesquisa da Microsoft fornece um método de [consulta](../api/search-query.md) para pesquisar os dados na Pesquisa da Microsoft, no qual você passa um[searchRequest](searchRequest.md) no corpo da solicitação, definindo as especificações da pesquisa.

Essa seção lista os casos de uso comuns do método de **consulta** , com base nas propriedades e parâmetros definidos no corpo da **consulta** [searchRequest](searchRequest.md).

Search requests run on behalf of the user. Search results are scoped to enforce any access control applied to the items.  For example, in the context of files, permissions on the files are evaluated as part of the search request. Users cannot access more items in a search than they can otherwise obtain from a corresponding GET operation with the same permissions and access control.

| Casos de uso | Propriedades a serem definidas no corpo da solicitação de consulta |
|:------------------|:---------|
|[ Resultados da pesquisa de escopo com base em tipos de entidade](#scope-search-based-on-entity-types)| **entityTypes** |
|[Resultados da página](#page-search-results) | **from** e **size** |
|[Obter os emails mais relevantes](#get-the-most-relevant-emails) | **enableTopResults** |
|[Obter as propriedades selecionadas](#get-selected-properties) | **campos** |
|[Usar KQL em termos de consulta](#keyword-query-language-kql-support) | **query** |
|[Classificar resultados de pesquisa](#sort-search-results)| **sort** |
|[Refinar os resultados usando agregações](#refine-results-using-aggregations)| **aggregations** |
|[Pesquisar entre conectores do Graph](/graph/search-concept-custom-types)| **contentSources** |

## <a name="scope-search-based-on-entity-types"></a>Pesquisa de escopo com base em tipos de entidade

Define the scope of the search request using the **entityTypes** property in the **query** request payload. The following table describes the types available to query and the supported permissions to access the data.

| EntityType | Escopo de permissão necessário para acessar os itens| Origem| Comentário|
|:------------------|:---------|:---------|:---------|
|[message](message.md)|Mail.Read, Mail.ReadWrite| Exchange Online| Mensagens de email.|
|[event](event.md) |Calendars.Read, Calendars.ReadWrite| Exchange Online|Eventos do calendário. |
|[unidade](drive.md)|Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All| SharePoint | Bibliotecas de documentos.|
|[driveItem](driveitem.md)|Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All| SharePoint e OneDrive | Arquivos, pastas, páginas e notícias. |
|[list](list.md)|Sites.Read.All, Sites.ReadWrite.All| SharePoint e OneDrive | Lists. Note that document libraries are also returned as lists. |
|[listItem](listitem.md)|Sites.Read.All, Sites.ReadWrite.All| SharePoint e OneDrive | List items. Note that files and folders are also returned as list items; **listItem** is the super class of **driveItem**. |
|[site](site.md)|Sites.Read.All, Sites.ReadWrite.All| SharePoint | Sites no SharePoint.|
|[externalItem](externalitem.md)|ExternalItem.Read.All| Conectores do Microsoft Graph| Todo o conteúdo está absorvido pela API dos conectores do Microsoft Graph.|

## <a name="page-search-results"></a>Resultados da pesquisa de página

Para controlar a paginação dos resultados da pesquisa, especifique as duas seguintes propriedades no corpo da solicitação **query** :

- **from** - An integer that indicates the 0-based starting point to list search results on the page. The default value is 0.

- **size** - An integer that indicates the number of results to be returned for a page. The default value is 25.

Observe os seguintes limites se você estiver pesquisando a entidade **event** ou **message** :

- **from** deve começar em zero na primeira solicitação de página; caso contrário, a solicitação resultará em um HTTP 400 `Bad request`.
- O máximo de resultados por página ( **size** ) é 25 por **mensagem** e **evento**. 

There is no upper limit for SharePoint or OneDrive items. A reasonable page size is 200. A larger page size generally incurs higher latency.

Práticas recomendadas:

- Specify a smaller first page in the initial request. For example, specify **from** as 0, **size** as 25.
- Paginate subsequent pages by updating the **from** and **size** properties. You can increase the page size in each subsequent request. The following table shows an example.

    | Page | from | size |
    |:-----|:-----|:-----|
    | 1    | 0 | 25 |
    | 2    | 25 | 50 |
    | 3    | 75 | 75 |
    | 4    | 150 | 100 |

## <a name="get-the-most-relevant-emails"></a>Obter os emails mais relevantes

Quando você pesquisa na entidade **mensagem** , a especificação de **enableTopResults** como`true` retorna uma lista híbrida de mensagens: as três primeiras mensagens na resposta são classificadas por relevância; as mensagens restantes são classificadas por data/hora.

## <a name="get-selected-properties"></a>Obter as propriedades selecionadas

When searching an entity type, such as **message** , **event** , **drive** , **driveItem** , **list** , **listItem** , **site** , **externalItem** , you can include in the **fields** property specific entity properties to return in the search results. This is similar to using the [OData system query option, $select](/graph/query-parameters#select-parameter) in REST requests. The search API does not technically support these query options because the behavior is expressed in the POST body.

Para todos esses tipos de entidade, especificar a propriedade **campos** reduz o número de propriedades retornadas na resposta, melhorando a carga na conexão.

The **listItem** and **externalItem** entities are the only supported entities that allow getting extended fields configured in the schema. You cannot retrieve extended properties from all the other entities. For example, if you created a field for **externalItem** in the search schema, or if you have a custom column on a **listItem** , you can retrieve these properties from search. To retrieve an extended property on a file, specify the **listItem** type in the request.

If the **fields** specified in the request are not present in the schema, they will not be returned in the response. Invalid fields in the request are silently ignored.

If you do not specify any **fields** in the request,  you will get the default set of properties for all types. For extended properties, **listItem** and **externalItem** behave differently when no **fields** are passed in the request:

- **listItem** não retornará nenhum campo personalizado.
- **externalItem** retornará todos os campos marcados com o atributo **recuperável** no esquema do conector do Microsoft Graph para essa conexão em particular.

## <a name="keyword-query-language-kql-support"></a>Suporte a KQL (Linguagem de Consulta de Palavra-chave)

Specify free text keywords, operators (such as `AND`, `OR`), and property restrictions in KQL syntax in the actual search query string ( **query** property of the **query** request body). The syntax and command depend on the entity types (in the **entityTypes** property) you target in the same **query** request body.

Depending on the entity type, the searchable properties vary. For details, see:

- [Propriedades do email](/microsoft-365/compliance/keyword-queries-and-search-conditions#searchable-email-properties)
- [Propriedades do site](/microsoft-365/compliance/keyword-queries-and-search-conditions#searchable-site-properties)

## <a name="sort-search-results"></a>Classificar resultados de pesquisa

Os resultados da pesquisa na resposta são classificados na ordem de classificação padrão a seguir:

- **mensagem** e **evento** são classificados por data.
- Todos os tipos de conectores SharePoint e OneDrive são classificados por relevância.

The [query](../api/search-query.md) method lets you customize the search order by specifying the **sortProperties** on the `requests` parameter, which is a collection of [searchRequest](./searchrequest.md) objects. This allows you to specify a list of one or more sortable properties and the sort order.

Atualmente, só há suporte para a classificação de resultados nos seguintes tipos de SharePoint e OneDrive: [driveItem](driveitem.md), [listItem](listitem.md), [list](list.md) e [site](site.md).

The properties on which the sort clause are applied need to be sortable in the SharePoint [search schema](/sharepoint/manage-search-schema). If the property specified in the request is not sortable or does not exist, the response will return an error, `HTTP 400 Bad Request`. Note that you cannot specify to sort documents by relevance using [sortProperty](sortproperty.md).

Ao especificar o **nome** de um objeto [sortProperty](sortproperty.md), você pode usar o nome da propriedade do tipo Microsoft Graph (por exemplo, em [driveItem](driveitem.md)) ou o nome da propriedade gerenciada no índice de pesquisa.

Confira [classificar resultados de pesquisa](/graph/search-concept-sort) para obter exemplos que mostram como classificar resultados.

## <a name="refine-results-using-aggregations"></a>Refinar os resultados usando agregações

Aggregations (also known as refiners in SharePoint) are a very popular way to enhance a search experience. In addition to the results, they provide some level of aggregate information on the matching set of search results. For example, you can provide information on the most represented authors of the documents matching the query, or the most represented file types, etc.

In the [searchRequest](./searchrequest.md), specify the aggregations that should be returned in addition to the search results. The description of each aggregation is defined in the [aggregationOption](./aggregationoption.md), which specifies the property on which the aggregation should be computed, and the number of [searchBucket](searchBucket.md) to be returned in the response.

The properties on which the aggregation is requested need to be refinable in the SharePoint [search schema](/sharepoint/manage-search-schema). If the property specified is not refinable or does not exist, the response returns `HTTP 400 Bad Request`.

Uma vez que a resposta retorne contendo a coleção de objetos [searchBucket](searchBucket.md), é possível refinar a solicitação de pesquisa somente aos elementos correspondentes contidos em uma [searchBucket](searchBucket.md). Isso é alcançado passando o valor **aggregationsFilterToken** na propriedade **aggregationFilters** da subsequente [searchRequest](./searchrequest.md).

As agregações atualmente têm suporte para qualquer propriedade refinável nos seguintes tipos do SharePoint e OneDrive: [driveItem](driveitem.md), [listItem](listitem.md), [list](list.md), [site](site.md). e nos conectores do Microsoft Graph [externalItem](externalItem.md).

Consulte [refinar os resultados da pesquisa](/graph/search-concept-aggregation) para obter exemplos que mostram como usar a agregação para melhorar e restringir os resultados da pesquisa.

## <a name="error-handling"></a>Tratamento de erros

A API de pesquisa retorna respostas de erro conforme estipulado pela [definição de objeto de erro OData](http://docs.oasis-open.org/odata/odata-json-format/v4.01/cs01/odata-json-format-v4.01-cs01.html#sec_ErrorResponse). Cada uma delas é um objeto JSON que contém um código e uma mensagem.

<!---TODOSEARCHAPI Describe the know errors: bad requests.--->

## <a name="known-limitations"></a>Limitações conhecidas

A API de pesquisa tem as seguintes limitações:

- The **query** method is defined to allow passing a collection of one or more **searchRequest** instances at once. However, the service currently supports only a single [searchRequest](./searchrequest.md) at a time.

- The [searchRequest](./searchrequest.md) resource supports passing multiple types of entities at a time. However, currently the only supported combination is for SharePoint and OneDrive entityTypes: **driveItem** , **drive** , **site** , **list** , **listItem**. Any combinations involving **message** , **event** , SharePoint and OneDrive types , or **externalItem** are currently not supported.  

- A propriedade **contentSource** , que define a conexão a ser usada, só será aplicável quando **entityType** for especificada como `externalItem`.

- A API de pesquisa não dá suporte à classificação personalizada para **mensagem** , **evento** ou  **externalItem**.

- A API de pesquisa não dá suporte a agregações para **mensagem** , **evento** , **site** ou **unidade**.

## <a name="schema-change-deprecation-warning"></a>Aviso de preterição de mudança de esquema

Properties used in a search request and response have been renamed or removed. In most cases, the original properties are being deprecated and replaced by the current properties, as listed in the table below.

Start updating any existing apps to use current property and type names, and to get current property names in the response. For backward compatibility, the original properties and types are accessible and functional until **December 31, 2020** , after which they will be removed.

| Recurso                           | Tipo de alteração   | Propriedade original | Propriedade atual|
|:-----------------------------------|:--------------|:------------------|:----------------|
| [searchRequest](./searchrequest.md)| Renomear Propriedade | **stored_fields** | **campos**      |
| [searchQuery](./searchquery.md)    | Renomear propriedade | **query_string** | **queryString** |
| [searchQueryString](./searchquerystring.md) | Substituir recurso | Não aplicável | Não aplicável |
| [searchHit](./searchhit.md)        | Renomear propriedade | **_id** | **hitId** |
| [searchHit](./searchhit.md)        | Renomear propriedade | **_score** | **classificação** |
| [searchHit](./searchhit.md)        | Remover propriedade | **_sortField** | Não aplicável |
| [searchHit](./searchhit.md)        | Renomear propriedade | **_source** | **recurso** |
| [searchHit](./searchhit.md)        | Renomear propriedade | **_summary**  | **resumo**  |

## <a name="search-samples"></a>Exemplos de pesquisa

- Saiba mais sobre alguns dos principais casos de uso:
  - [Pesquisar mensagens do Outlook](/graph/search-concept-messages)
  - [Pesquisar eventos do calendário](/graph/search-concept-events)
  - [Pesquisar conteúdo no OneDrive e Microsoft Office SharePoint Online](/graph/search-concept-files)
  - [Pesquisar conteúdo externo](/graph/search-concept-custom-types)
  - [Classificar resultados de pesquisa](/graph/search-concept-sort)
  - [Refinar resultados de pesquisa](/graph/search-concept-aggregation)

- Explore as APIs no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).


## <a name="whats-new"></a>O que há de novo

Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.