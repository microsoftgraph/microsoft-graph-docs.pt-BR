---
title: Usar a API de Pesquisa da Microsoft para consultar dados
description: Utilizando a API de pesquisa, os aplicativos podem pesquisar os dados do Microsoft 365 no contexto do usuário autenticado
ms.localizationpriority: high
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 04a9f843da8326f257a7a48537353a10ac458a81
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59766933"
---
# <a name="use-the-microsoft-search-api-to-query-data"></a>Usar a API de Pesquisa da Microsoft para consultar dados

Você pode utilizar a API de Pesquisa da Microsoft para consultar os dados do Microsoft 365 nos seus aplicativos.

As solicitações de pesquisa são executadas no contexto do usuário conectado, identificado usando um [token de acesso com permissões delegadas](/graph/auth-v2-user).

## <a name="common-use-cases"></a>Casos de uso comuns

A API de pesquisa da Microsoft fornece um método de [consulta](../api/search-query.md) para pesquisar os dados na Pesquisa da Microsoft, no qual você passa um[searchRequest](searchRequest.md) no corpo da solicitação, definindo as especificações da pesquisa.

Essa seção lista os casos de uso comuns do método de **consulta**, com base nas propriedades e parâmetros definidos no corpo da **consulta** [searchRequest](searchRequest.md).

As solicitações de pesquisa são executadas em nome do usuário. Os resultados da pesquisa têm escopo para impor o controle de acesso aplicado aos itens.  Por exemplo, no contexto de arquivos, as permissões em relação aos arquivos serão avaliadas como parte da solicitação de pesquisa. Os usuários não podem acessar mais itens em uma pesquisa do que eles poderiam obter de uma operação GET correspondente com as mesmas permissões e controle de acesso.

| Casos de uso | Propriedades a serem definidas no corpo da solicitação de consulta |
|:------------------|:---------|
|[ Resultados da pesquisa de escopo com base em tipos de entidade](#scope-search-based-on-entity-types)| **entityTypes** |
|[Resultados da página](#page-search-results) | **from** e **size** |
|[Obter os emails mais relevantes](#get-the-most-relevant-emails) | **enableTopResults** |
|[Obter as propriedades selecionadas](#get-selected-properties) | **campos** |
|[Usar KQL em termos de consulta](#keyword-query-language-kql-support) | **query** |
|[Classificar resultados de pesquisa](#sort-search-results)| **sort** |
|[Refinar os resultados usando agregações](#refine-results-using-aggregations)| **aggregations** |

## <a name="scope-search-based-on-entity-types"></a>Pesquisa de escopo com base em tipos de entidade

Defina o escopo da solicitação de pesquisa usando a propriedade **entityTypes** no conteúdo da solicitação **query**.
A tabela a seguir descreve os tipos disponíveis para consulta e as permissões com suporte para acessar os dados.

| EntityType | Escopo de permissão necessário para acessar os itens| Origem| Comentário|
|:------------------|:---------|:---------|:---------|
|[message](message.md)|Mail.Read, Mail.ReadWrite| Exchange Online| Mensagens de email.|
|[event](event.md) |Calendars.Read, Calendars.ReadWrite| Exchange Online|Eventos do calendário. |
|[unidade](drive.md)|Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All| SharePoint | Bibliotecas de documentos.|
|[driveItem](driveitem.md)|Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All| SharePoint e OneDrive | Arquivos, pastas, páginas e notícias. |
|[list](list.md)|Sites.Read.All, Sites.ReadWrite.All| SharePoint e OneDrive | Listas. Observe que as bibliotecas de documentos também são retornadas como listas. |
|[listItem](listitem.md)|Sites.Read.All, Sites.ReadWrite.All| SharePoint e OneDrive | Listar itens. Observe que os arquivos e as pastas também são retornados como itens de lista; **listItem** é a superclasse de **driveItem**. |
|[site](site.md)|Sites.Read.All, Sites.ReadWrite.All| SharePoint | Sites no SharePoint.|

## <a name="page-search-results"></a>Resultados da pesquisa de página

Para controlar a paginação dos resultados da pesquisa, especifique as duas seguintes propriedades no corpo da solicitação **query**:

- **from** – um número inteiro que indica o ponto de partida baseado em 0 para listar os resultados da pesquisa na página. O valor padrão é 0.

- **size** – um número inteiro que indica o número de resultados a serem retornados para uma página. O valor padrão é 25.

Observe os seguintes limites se você estiver pesquisando a entidade **event** ou **message**:

- **from** deve começar em zero na primeira solicitação de página; caso contrário, a solicitação resultará em um HTTP 400 `Bad request`.
- O máximo de resultados por página (**size**) é 25 por **mensagem** e **evento**. 

Não há um limite superior para itens do SharePoint ou do OneDrive. Um tamanho de página razoável é 200. Um tamanho de página maior geralmente gera uma latência maior.

Práticas recomendadas:

- Especifique uma primeira página menor na solicitação inicial. Por exemplo, especifique **from** como 0 e **size** como 25.
- Pagine as páginas subsequentes atualizando as propriedades **from** e **size**. Você pode aumentar o tamanho de página em cada solicitação subsequente. A tabela a seguir mostra um exemplo.

    | Página | from | size |
    |:-----|:-----|:-----|
    | 1    | 0 | 25 |
    | 2    | 25 | 50 |
    | 3    | 75 | 75 |
    | 4    | 150 | 100 |

## <a name="get-the-most-relevant-emails"></a>Obter os emails mais relevantes

Quando você pesquisa na entidade **mensagem**, a especificação de **enableTopResults** como`true` retorna uma lista híbrida de mensagens: as três primeiras mensagens na resposta são classificadas por relevância; as mensagens restantes são classificadas por data/hora.

## <a name="get-selected-properties"></a>Obter as propriedades selecionadas

Ao pesquisar um tipo de entidade, como **mensagem**, **evento**, **unidade**, **driveItem**, **lista**, **listItem**, **site**, **externalItem**, você pode incluir na propriedade **campos** as propriedades de entidade específica para retornar nos resultados da pesquisa. Isso é semelhante a usar a opção [$select, da consulta do sistema OData](/graph/query-parameters#select-parameter), em solicitações REST. A pesquisa do API não oferece suporte técnico a essas opções de consulta porque o comportamento é expresso no corpo POST.

Para todos esses tipos de entidade, especificar a propriedade **campos** reduz o número de propriedades retornadas na resposta, melhorando a carga na conexão.

As entidades **listItem** e **externalItem** são as únicas entidades suportadas que permitem a obtenção de campos extensíveis de recuperação configurados no esquema. Você não pode recuperar as propriedades estendidas de todas as outras entidades usando a API de pesquisa. Por exemplo, se você criou um campo recuperável para **externalItem** no esquema de pesquisa, ou se você tem uma coluna personalizada recuperável em uma **listItem**, você pode recuperar essas propriedades da pesquisa. Para recuperar uma propriedade estendida de um arquivo, especifique o tipo de **listItem** na solicitação.

Se os **campos** especificados na solicitação não estiverem presentes no esquema ou não estiverem marcados como recuperáveis, eles não serão devolvidos na resposta. Campos inválidos na solicitação são ignorados silenciosamente.

Se você não especificar nenhum **campo** na solicitação, obterá o conjunto padrão de propriedades para todos os tipos. Para propriedades estendidas, **listItem** e **externalItem** se comportam de forma diferente quando nenhum **campo** é passado na solicitação:

- **listItem** não retornará nenhum campo personalizado.
- **externalItem** retornará todos os campos marcados com o atributo **recuperável** no esquema do conector do Microsoft Graph para essa conexão em particular.

## <a name="keyword-query-language-kql-support"></a>Suporte a KQL (Linguagem de Consulta de Palavra-chave)

Especifique palavras-chave de texto livre, operadores (como `AND`, `OR`) e restrições de propriedade na sintaxe KQL na cadeia de caracteres de consulta de pesquisa real (propriedade **query** do corpo da solicitação **query**). A sintaxe e o comando dependem dos tipos de entidade (na propriedade **entityTypes**) que você direciona no corpo da solicitação **query**.

Dependendo do tipo de entidade, as propriedades pesquisáveis variam. Veja mais detalhes em:

- [Propriedades do email](/microsoft-365/compliance/keyword-queries-and-search-conditions#searchable-email-properties)
- [Propriedades do site](/microsoft-365/compliance/keyword-queries-and-search-conditions#searchable-site-properties)

## <a name="sort-search-results"></a>Classificar resultados de pesquisa

Os resultados da pesquisa na resposta são classificados na ordem de classificação padrão a seguir:

- **mensagem** e **evento** são classificados por data.
- Todos os tipos de SharePoint, OneDrive, pessoas e conectores são classificados por relevância.

O método de [consulta](../api/search-query.md) permite que você personalize a ordem de pesquisa especificando as **sortProperties** no parâmetro `requests`, que é uma coleção de objetos [searchRequest](./searchrequest.md). Isso permite especificar uma lista de uma ou mais propriedades classificáveis e a ordem de classificação.

Atualmente, só há suporte para a classificação de resultados nos seguintes tipos de SharePoint e OneDrive: [driveItem](driveitem.md), [listItem](listitem.md), [list](list.md) e [site](site.md).

As propriedades nas quais a cláusula de classificação é aplicada devem ser classificáveis no [esquema de pesquisa](/sharepoint/manage-search-schema) do SharePoint. Se a propriedade especificada na solicitação não for classificável ou não existir, a resposta retornará um erro, `HTTP 400 Bad Request`. Observe que você não pode especificar a classificação de documentos por relevância usando [sortProperty](sortproperty.md).

Ao especificar o **nome** de um objeto [sortProperty](sortproperty.md), você pode usar o nome da propriedade do tipo Microsoft Graph (por exemplo, em [driveItem](driveitem.md)) ou o nome da propriedade gerenciada no índice de pesquisa.

Confira [classificar resultados de pesquisa](/graph/search-concept-sort) para obter exemplos que mostram como classificar resultados.

## <a name="refine-results-using-aggregations"></a>Refinar os resultados usando agregações

As agregações (também conhecidas como refinadores no SharePoint) são uma maneira muito popular de melhorar a experiência de pesquisa. Além dos resultados, eles fornecem algum nível de informações agregadas no conjunto de resultados de pesquisa. Por exemplo, você pode fornecer informações sobre os autores mais representados dos documentos correspondentes à consulta, ou os tipos de arquivo mais representados, etc.

Na[searchRequest](./searchrequest.md), especifique as agregações que devem ser retornadas além dos resultados da pesquisa. A descrição de cada agregação é definida na[aggregationOption](./aggregationoption.md), que especifica a propriedade na qual a agregação deve ser calculada, e o número de [searchBucket](searchBucket.md) a ser retornado na resposta.

As propriedades nas quais a agregação é solicitada devem ser refináveis no [esquema de pesquisa](/sharepoint/manage-search-schema) do SharePoint. Se a propriedade especificada não for refinável ou não existir, a resposta retornará `HTTP 400 Bad Request`.

Uma vez que a resposta é retornada contendo a coleção de objetos [searchBucket](searchBucket.md), é possível refinar a solicitação de pesquisa somente aos elementos correspondentes contidos em uma [searchBucket](searchBucket.md). Isso é conseguido passando o valor **aggregationsFilterToken** na propriedade **aggregationsFilters** na posterior [searchRequest](./searchrequest.md).

As agregações atualmente têm suporte para qualquer propriedade refinável nos seguintes tipos do SharePoint e OneDrive: [driveItem](driveitem.md), [listItem](listitem.md), [list](list.md), [site](site.md) e nos conectores do Microsoft Graph [externalItem](externalconnectors-externalitem.md).

Confira [refinar os resultados da pesquisa](/graph/search-concept-aggregation) para obter exemplos que mostram como usar a agregação para melhorar e restringir os resultados da pesquisa.

## <a name="error-handling"></a>Tratamento de erros

A API de pesquisa retorna respostas de erro conforme estipulado pela [definição de objeto de erro OData](http://docs.oasis-open.org/odata/odata-json-format/v4.01/cs01/odata-json-format-v4.01-cs01.html#sec_ErrorResponse). Cada uma delas é um objeto JSON que contém um código e uma mensagem.

<!---TODOSEARCHAPI Describe the know errors: bad requests.--->

## <a name="known-limitations"></a>Limitações conhecidas

A API de pesquisa tem as seguintes limitações:

- O método **query** é definido para permitir a passagem de um conjunto de uma ou mais instâncias de **searchRequest** de uma só vez. No entanto, atualmente o serviço dá suporte apenas a um único [searchRequest](./searchrequest.md) por vez.

- O recurso [searchRequest](./searchrequest.md) dá suporte à passagem de vários tipos de entidades por vez. No entanto, no momento, a única combinação com suporte é para os entityTypes do SharePoint e o OneDrive: **driveItem**, **drive**, **site**, **list**, **listItem**.
As combinações envolvendo **mensagem**, **evento**, tipos do SharePoint e do OneDrive ou **externalItem** não têm suporte no momento.  

- A propriedade **contentSource**, que define a conexão a ser usada, só será aplicável quando **entityType** for especificada como `externalItem`.

- A API de pesquisa não dá suporte à classificação personalizada para **mensagem**, **evento** ou  **externalItem**.

- A API de pesquisa não dá suporte a agregações para **mensagem**, **evento**, **site** ou **unidade**.

- As personalizações na pesquisa do SharePoint, como um esquema de pesquisa personalizado ou fontes de resultados, podem interferir na operação da API de Pesquisa da Microsoft.

## <a name="see-also"></a>Confira também

- Saiba mais sobre alguns dos principais casos de uso:
  - [Pesquisar mensagens do Outlook](/graph/search-concept-messages)
  - [Pesquisar eventos do calendário](/graph/search-concept-events)
  - [Pesquisar conteúdo no OneDrive e Microsoft Office SharePoint Online](/graph/search-concept-files)
  - [Classificar resultados de pesquisa](/graph/search-concept-sort)
  - [Refinar resultados de pesquisa](/graph/search-concept-aggregation)

- Explore as APIs no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
- Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.
