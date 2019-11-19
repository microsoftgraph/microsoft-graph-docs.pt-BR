---
title: Usar a API de Pesquisa da Microsoft para consultar dados
description: Usando a API de pesquisa, os aplicativos podem pesquisar dados do Office 365 no contexto do usuário autenticado
localization_priority: Priority
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: afbb9ba469dad7751422902ea4a9876b6ca6b904
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704126"
---
# <a name="use-the-microsoft-search-api-to-query-data"></a>Usar a API de Pesquisa da Microsoft para consultar dados

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usando a API de Pesquisa da Microsoft, os aplicativos podem consultar dados do Office 365.

As solicitações de pesquisa são executadas no contexto do usuário conectado, identificado usando um [token de acesso com permissões delegadas](/graph/auth-v2-user).

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="common-use-cases"></a>Casos de uso comuns

A API de pesquisa fornece um método [query](../api/search-query.md) para pesquisar os dados na Pesquisa da Microsoft. Esta seção lista os casos de uso comuns, com base nas propriedades definidas no corpo da solicitação **query**.

As solicitações de pesquisa são executadas em nome do usuário. Os resultados da pesquisa são cortados para impor o controle de acesso aplicado aos itens.  Por exemplo, no contexto de arquivos, as permissões em relação aos arquivos serão avaliadas na parte da solicitação de pesquisa. Os usuários não podem acessar mais itens na pesquisa do que poderiam na API de enumeração.

| Casos de uso | Propriedades a serem definidas no corpo da solicitação de consulta |
|:------------------|:---------|
|[Pesquisa de escopo com base em tipos de entidade](#scope-search-based-on-entity-types)| **entityTypes** |
|[Resultados da página](#page-search-results) | **from** e **size** |
|[Obter os emails mais relevantes](#get-the-most-relevant-emails) | **enableTopResults** |
|[Obter as propriedades selecionadas](#get-selected-properties) | **stored_fields** |
|[Usar KQL em termos de consulta](#keyword-query-language-kql-support) | **query** |
|[Pesquisar arquivos externos](/graph/search-concept-files)| **entityTypes** |
|[Pesquisar em um contentSource específico (API de indexação)](/graph/search-concept-custom-types)| **contentSources** |

### <a name="scope-search-based-on-entity-types"></a>Pesquisa de escopo com base em tipos de entidade

Defina o escopo da solicitação de pesquisa usando a propriedade **entityTypes** no conteúdo da solicitação **query**.
Estes são os tipos de entidade com suporte:

- [event](event.md)
- [message](message.md)
- [driveItem](driveitem.md)
- [externalFile](externalfile.md)
- [externalItem](externalitem.md)

### <a name="page-search-results"></a>Resultados da pesquisa de página

Para controlar a paginação dos resultados da pesquisa, especifique as duas seguintes propriedades no corpo da solicitação **query**:

- **from**, um número inteiro que indica o ponto de partida baseado em 0 para listar os resultados da pesquisa na página. O valor padrão é 0.

- **size**, um número inteiro que indica o número de resultados a serem retornados para uma página. O valor padrão é 25.

Observe os seguintes limites se você estiver pesquisando a entidade **event** ou **message**:

- **from** deve começar em zero na primeira solicitação de página. Caso contrário, a solicitação resultará em HTTP 400 `Bad request`.
- O máximo de resultados por página (**size**) é 200.
- O número máximo total de itens que podem ser retornados por meio de paginação é 1000.
- Se os limites forem excedidos, será retornada uma resposta de melhor esforço. A solicitação não resulta em HTTP 400.

Práticas recomendadas:

- Especifique uma primeira página menor na solicitação inicial. Por exemplo, especifique **from** como 0 e **size** como 25.
- Pagine as páginas subsequentes atualizando as propriedades **from** e **size**. Você pode aumentar o tamanho de página em cada solicitação subsequente. A tabela a seguir mostra um exemplo.

    | Página | from | size |
    |:-----|:-----|:-----|
    | 1    | 0 | 25 |
    | 2    | 25 | 50 |
    | 3    | 75 | 75 |
    | 4    | 150 | 100 |

### <a name="get-the-most-relevant-emails"></a>Obter os emails mais relevantes

Quando você pesquisa na entidade **message**, a especificação de **enableTopResults** como `true` retorna uma lista híbrida de mensagens: as três primeiras mensagens na resposta são classificadas por relevância, e as mensagens restantes são classificadas por data.

### <a name="get-selected-properties"></a>Obter as propriedades selecionadas

Ao pesquisar em uma entidade **externalItem**, use a propriedade **stored_fields** para especificar os campos a serem retornados na resposta.

Os nomes especificados em **stored_fields** devem ser a Propriedade Gerenciada recuperável. Esses nomes de propriedades foram configurados para a conexão na administração de locatários da Pesquisa da Microsoft.

### <a name="keyword-query-language-kql-support"></a>Suporte a KQL (Linguagem de Consulta de Palavra-chave)

Especifique palavras-chave de texto livre, operadores (como `AND`, `OR`) e restrições de propriedade na sintaxe KQL na cadeia de caracteres de consulta de pesquisa real (propriedade **query** do corpo da solicitação **query**). A sintaxe e o comando dependem dos tipos de entidade (na propriedade **entityTypes**) que você direciona no corpo da solicitação **query**.

Dependendo do tipo de entidade, as propriedades pesquisáveis variam:

- [propriedades de mensagem](/microsoft-365/compliance/keyword-queries-and-search-conditions#searchable-email-properties)
- [propriedades de driveItem](/microsoft-365/compliance/keyword-queries-and-search-conditions#searchable-site-properties)

## <a name="error-handling"></a>Tratamento de erro

A API de pesquisa retorna respostas de erro conforme estipulado pela [definição de objeto de erro OData](http://docs.oasis-open.org/odata/odata-json-format/v4.01/cs01/odata-json-format-v4.01-cs01.html#sec_ErrorResponse). Cada uma delas é um objeto JSON que contém um código e uma mensagem.

<!---TODO Describe the know errors : bad requests.--->

## <a name="known-limitations"></a>Limitações conhecidas

A API de pesquisa tem as seguintes limitações:

- O método **query** é definido para permitir a passagem de um conjunto de uma ou mais instâncias de **searchRequest** de uma só vez. No entanto, atualmente o serviço dá suporte apenas a um único [searchRequest](./searchrequest.md) por vez.

- O recurso [searchRequest](./searchrequest.md) dá suporte à passagem de vários tipos de entidades por vez. No entanto, atualmente a única combinação com suporte é **driveItem** e **externalfile**. Outras combinações são inválidas.

- A propriedade **contentSource**, que define a conexão a ser usada, só será aplicável quando **entityType** for especificada como `externalItem`.
<!--todo nmoreauteam Fix the link to ContentSource  pls provide the content source url--->

- A API de pesquisa não dá suporte à classificação personalizada e sempre classifica os resultados da seguinte maneira:

  - Classificar resultados dos tipos **message** ou **event** por data.

  - Classificar resultados dos tipos **driveItem**, **externalfile** ou **externalItem** por relevância.
