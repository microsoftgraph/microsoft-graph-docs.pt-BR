---
title: Usar a API de Pesquisa da Microsoft para indexar dados
description: O Microsoft Graph permite que o índice do aplicativo tenha itens personalizados ou arquivos externos no serviço da Pesquisa da Microsoft.
localization_priority: Priority
author: snlraju-msft
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: cac6d8e9d399e13554e9a9ef44fe8d869c0ad70d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938945"
---
# <a name="use-the-microsoft-search-api-to-index-data"></a>Usar a API de Pesquisa da Microsoft para indexar dados

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O Microsoft Graph permite que o seu aplicativo adicione itens personalizados ou arquivos externos aos resultados da pesquisa na experiência da [Pesquisa da Microsoft](/microsoftsearch/overview-microsoft-search).

As solicitações de indexação de dados são realizadas em nome de um aplicativo sem a presença de um usuário conectado, identificado usando um [token de acesso com permissão de aplicativo](/graph/auth-v2-service).

## <a name="common-use-cases"></a>Casos de uso comuns

Os casos de uso das APIs nesta seção se concentram na criação de [conectores do Microsoft Graph](/microsoftsearch/connectors-overview), o que envolve as principais etapas para:

1. [Criar uma conexão](../api/external-post-connections.md) com uma fonte de dados externa
2. [Criar e registrar um esquema](../api/externalconnection-post-schema.md) que descreve o tipo e como indexar os dados externos
3. [Indexar dados](../api/externalconnection-put-items.md) como um item externo ou um arquivo externo

| Casos de uso                                        | Recursos REST                              | Confira também |
|:-------------------------------------------------|:--------------------------------------------|:--|
| **Ações de configuração**                        |                                             |   |
| Criar, atualizar ou excluir uma conexão           | [externalConnection](externalconnection.md) | [Métodos de externalConnection](externalconnection.md#methods) |
| Registrar um esquema para os dados externos          | [schema](schema.md)                         | [Métodos de schema](schema.md#methods) |
| **Ações de indexação**                             |                                             |   |
| Adicionar, atualizar ou excluir um item personalizado no índice | [externalItem](externalitem.md)             | [Métodos de externalItem](externalItem.md#methods) |
| Adicionar, atualizar ou excluir um arquivo no índice        | [externalFile](externalfile.md)             | [Métodos de externalFile](externalfile.md#methods) |

## <a name="known-limitations"></a>Limitações conhecidas

Observe as seguintes limitações durante a visualização.

- As organizações estão limitadas a um máximo de 10 conexões.
- Não há suporte para propriedades personalizadas ao indexar arquivos usando o recurso `externalFile`.
- Somente as identidades do Azure Active Directory são compatíveis.
- A criação de recursos `externalItem` ou `externalFile` está limitada a quatro itens por segundo.
- Um aplicativo está limitado a quatro operações simultâneas em uma conexão.
- As conexões têm um limite de capacidade de 700 mil itens ou aproximadamente 70 GB de dados.
- O tamanho máximo de uma entidade `externalItem` ou `externalFile` é 4 MB.
- Não há suporte para refinar e classificar os resultados.
- A classificação de resultados é pelo melhor esforço.

## <a name="next-steps"></a>Próximas etapas

- [Visão geral da API de Pesquisa da Microsoft](/graph/search-concept-overview)
- Faça uma busca detalhada sobre os métodos, as propriedades e as relações dos recursos [externalConnection](externalconnection.md), [schema](schema.md), [externalItem](externalitem.md) e [externalFile](externalfile.md).
- Confira o [exemplo de conector de pesquisa](https://github.com/microsoftgraph/msgraph-search-connector-sample) no GitHub.
