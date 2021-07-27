---
title: Usar a API de Pesquisa da Microsoft para indexar dados
description: Use o Microsoft Graph para indexar itens personalizados no serviço de Pesquisa da Microsoft.
localization_priority: Priority
author: snlraju-msft
ms.prod: search
doc_type: conceptualPageType
ms.openlocfilehash: 5f829c767584366b3f291bf186073b40ace6ce41
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467224"
---
# <a name="use-the-microsoft-search-api-to-index-data"></a>Usar a API de Pesquisa da Microsoft para indexar dados

Você pode usar o Microsoft Graph para adicionar itens personalizados aos resultados da pesquisa na experiência de [Pesquisa da Microsoft](/microsoftsearch/overview-microsoft-search).

As solicitações de indexação de dados são realizadas em nome de um aplicativo sem a presença de um usuário conectado, identificado usando um [token de acesso com permissão de aplicativo](/graph/auth-v2-service).

## <a name="common-use-cases"></a>Casos de uso comuns

Os casos de uso das APIs nesta seção tratam da criação de [conectores do Microsoft Graph](/microsoftsearch/connectors-overview), o que envolve as principais etapas para:

1. [Criar uma conexão](../api/externalconnectors-external-post-connections.md) para uma fonte de dados externa.
2. [Criar e registrar um esquema](../api/externalconnectors-schema-create.md) que descreve o tipo e como indexar os dados externos.
3. [Indexar os dados](../api/externalconnectors-externalitem-create.md) como um item externo.

| Casos de uso                                        | Recursos REST                              | Confira também |
|:-------------------------------------------------|:--------------------------------------------|:--|
| **Ações de configuração**                        |                                             |   |
| Criar, atualizar ou excluir uma conexão           | [externalConnection](externalconnectors-externalconnection.md) | [Métodos de externalConnection](externalconnectors-externalconnection.md#methods) |
| Registrar um esquema para os dados externos          | [schema](externalconnectors-schema.md)                         | [métodos de esquema](externalconnectors-schema.md#methods) |
| **Ações de indexação**                             |                                             |   |
| Adicionar, atualizar ou excluir um item personalizado no índice | [externalItem](externalconnectors-externalitem.md)             | [métodos de externalItem](externalconnectors-externalitem.md#methods) |

## <a name="known-limitations"></a>Limitações conhecidas

A seguir estão as limitações conhecidas atuais:

- As organizações estão limitadas a um máximo de 10 conexões.
- Você só pode criar quatro itens de recursos `externalItem` por segundo.
- Um aplicativo está limitado a quatro operações simultâneas em uma conexão.
- As conexões têm um limite de capacidade de 700 mil itens ou aproximadamente 70 GB de dados.
- O tamanho máximo de uma entidade `externalItem` é 4 MB.
- A classificação de resultados não é compatível.

## <a name="whats-new"></a>Novidades
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.

## <a name="next-steps"></a>Próximas etapas

- Confira a [Visão geral da API de Pesquisa da Microsoft](/graph/search-concept-overview).
- Faça uma busca detalhada sobre os métodos, propriedades e relações dos recursos [externalConnection](externalconnectors-externalconnection.md), [schema](externalconnectors-schema.md)e [externalItem](externalconnectors-externalitem.md).
- Confira a [coleção Microsoft Graph postman](https://www.postman.com/microsoftgraph/workspace/microsoft-graph/folder/455214-66cbb476-ad94-448e-ba5a-ef58e1da7a90?ctx=documentation) ([saiba mais](https://developer.microsoft.com/pt-BR/graph/blogs/postman-collections))
- Confira o [exemplo de conector de pesquisa](https://github.com/microsoftgraph/msgraph-search-connector-sample) no GitHub.


