---
title: Criar, atualizar e excluir conexões com o serviço da Pesquisa da Microsoft
description: Aprenda a usar o Microsoft Graph para gerenciar conexões com o serviço da Pesquisa da Microsoft
localization_priority: Priority
author: snlraju-msft
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: b1f599a4610ce4cb939c7733949eac4c0ddba371
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939527"
---
# <a name="create-update-and-delete-connections-to-the-microsoft-search-service"></a>Criar, atualizar e excluir conexões com o serviço da Pesquisa da Microsoft

As conexões de serviços externos com o serviço da Pesquisa da Microsoft são representadas pelo recurso [externalConnection](/graph/api/resources/externalconnection?view=graph-rest-beta) no Microsoft Graph.

Uma conexão permite que seu aplicativo [defina um esquema](/graph/api/externalconnection-post-schema?view=graph-rest-beta) para os itens que serão indexados e forneça um ponto de extremidade para o seu serviço [adicionar, atualizar ou excluir itens do índice](search-index-manage-items.md). Criar uma conexão é a primeira etapa para um aplicativo para adicionar itens ao índice de pesquisa.

## <a name="create-a-connection"></a>Criar uma conexão

Antes que um aplicativo possa adicionar itens ao índice de pesquisa, ele deve criar e configurar uma conexão usando as etapas a seguir.

- [Criar uma conexão](/graph/api/external-post-connections?view=graph-rest-beta) com ID exclusiva, nome de exibição e descrição.
- [Registrar um esquema](/graph/api/externalconnection-post-schema?view=graph-rest-beta).
  - Para itens personalizados (como tíquetes de assistência técnica ou entradas de banco de dados de inventário etc.), defina os campos que serão incluídos no índice.
  - Para arquivos externos, especifique o tipo `microsoft.graph.externalFile`.

> [!IMPORTANT]
> Depois que um esquema é registrado, ele não pode ser alterado para uma conexão existente.

## <a name="update-a-connection"></a>Atualizar uma conexão

Você pode alterar o nome de exibição ou a descrição de uma conexão existente [atualizando a conexão](/graph/api/externalconnection-update?view=graph-rest-beta).

## <a name="delete-a-connection"></a>Excluir uma conexão

Você pode [excluir uma conexão](/graph/api/externalconnection-delete?view=graph-rest-beta) e remover todos os itens que foram indexados por meio da conexão.

## <a name="next-steps"></a>Próximas etapas

- [Por que usar a API de Pesquisa da Microsoft?](search-concept-overview.md#why-use-the-microsoft-search-api)
- [Usar a API de Pesquisa da Microsoft para indexar dados](/graph/api/resources/indexing-api-overview?view=graph-rest-beta)
- [Visão geral dos conectores do Microsoft Graph](/microsoftsearch/connectors-overview)
- Baixe o [exemplo de conector de pesquisa](https://github.com/microsoftgraph/msgraph-search-connector-sample) no GitHub
