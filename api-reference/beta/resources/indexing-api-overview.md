---
title: Usar a API de Pesquisa da Microsoft para indexar dados
description: Use o Microsoft Graph para indexar itens personalizados no serviço de Pesquisa da Microsoft.
localization_priority: Priority
author: snlraju-msft
ms.prod: search
doc_type: conceptualPageType
ms.openlocfilehash: 69a1c99af429b93d7fbddbea4e76523b281541d7
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366959"
---
# <a name="use-the-microsoft-search-api-to-index-data"></a>Usar a API de Pesquisa da Microsoft para indexar dados

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode usar o Microsoft Graph para adicionar itens personalizados aos resultados da pesquisa na experiência de [Pesquisa da Microsoft](/microsoftsearch/overview-microsoft-search).

As solicitações de indexação de dados são realizadas em nome de um aplicativo sem a presença de um usuário conectado, identificado usando um [token de acesso com permissão de aplicativo](/graph/auth-v2-service).

## <a name="common-use-cases"></a>Casos de uso comuns

Os casos de uso das APIs nesta seção tratam da criação de [conectores do Microsoft Graph](/microsoftsearch/connectors-overview), o que envolve as principais etapas para:

1. [Criar uma conexão](../api/external-post-connections.md) para uma fonte de dados externa.
2. [Criar e registrar um esquema](../api/externalconnection-post-schema.md) que descreve o tipo e como indexar os dados externos.
3. [Indexar os dados](../api/externalconnection-put-items.md) como um item externo.

| Casos de uso                                        | Recursos REST                              | Confira também |
|:-------------------------------------------------|:--------------------------------------------|:--|
| **Ações de configuração**                        |                                             |   |
| Criar, atualizar ou excluir uma conexão           | [externalConnection](externalconnection.md) | [Métodos de externalConnection](externalconnection.md#methods) |
| Registrar um esquema para os dados externos          | [schema](schema.md)                         | [métodos de esquema](schema.md#methods) |
| **Ações de indexação**                             |                                             |   |
| Adicionar, atualizar ou excluir um item personalizado no índice | [externalItem](externalitem.md)             | [métodos de externalItem](externalItem.md#methods) |

## <a name="known-limitations"></a>Limitações conhecidas

A seguir estão as limitações conhecidas atuais:

- As organizações estão limitadas a um máximo de 10 conexões.
- Somente as identidades do Azure Active Directory são compatíveis.
- Você só pode criar quatro itens de recursos `externalItem` por segundo.
- Um aplicativo está limitado a quatro operações simultâneas em uma conexão.
- As conexões têm um limite de capacidade de 700 mil itens ou aproximadamente 70 GB de dados.
- O tamanho máximo de uma entidade `externalItem` é 4 MB.
- A classificação de resultados não é compatível.
- A classificação de resultados é pelo melhor esforço.

## <a name="whats-new"></a>O que há de novo
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.

## <a name="next-steps"></a>Próximas etapas

- Confira a [Visão geral da API de Pesquisa da Microsoft](/graph/search-concept-overview).
- Faça uma busca detalhada sobre os métodos, propriedades e relações dos recursos [externalConnection](externalconnection.md), [schema](schema.md)e [externalItem](externalitem.md).
- Confira o [exemplo de conector de pesquisa](https://github.com/microsoftgraph/msgraph-search-connector-sample) no GitHub.


