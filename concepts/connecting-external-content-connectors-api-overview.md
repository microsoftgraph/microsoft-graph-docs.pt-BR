---
title: Trabalhar com a API de conectores do Microsoft Graph
description: Use a API de conectores do Microsoft Graph para criar conectores personalizados que trazem dados externos para o Microsoft Graph aprimorar as experiências inteligentes do Microsoft 365.
author: mecampos
ms.localizationpriority: high
doc_type: conceptualPageType
ms.prod: search
ms.openlocfilehash: 4c2359f7e565b9d1ff00e623649e833363fc6231
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094414"
---
# <a name="work-with-the-microsoft-graph-connectors-api"></a>Trabalhar com a API de conectores do Microsoft Graph

Os conectores do Microsoft Graph trazem dados externos para o Microsoft Graph e aprimoram as experiências inteligentes do Microsoft 365. Você pode criar um conector personalizado para integração com serviços que não estão disponíveis como conectores desenvolvidos pela Microsoft. Para criar conectores personalizados, use as APIs REST de conectores do Microsoft Graph.

![Imagem mostrando os dados externos chegando através de diferentes tipos de conectores para o Microsoft Graph](./images/connectors-images/api-overview.png)

Você pode usar a API de conectores do Microsoft Graph para:

1. Criar e gerenciar conexões de dados externos.
2. Defina e registre o esquema dos tipos de dados externos.
3. Ingerir itens de dados externos no Microsoft Graph.
4. Sincronizar grupos externos.

## <a name="create-and-manage-external-data-connections"></a>Criar e gerenciar conexões de dados externos.

O recurso [externalConnection](/graph/api/resources/externalconnectors-externalconnection) (API de conexão externa) é um contêiner lógico para seus dados externos que você pode gerenciar como uma única unidade.

Para saber mais, consulte [Criar, atualizar e excluir conexões no Microsoft Graph](connecting-external-content-manage-connections.md).

## <a name="define-and-register-the-schema-of-the-external-data-types"></a>Definir e registrar o esquema dos tipos de dados externos

O [esquema](/graph/api/resources/externalconnectors-schema) de conexão (API de esquema) determina como seu conteúdo é usado em várias experiências do Microsoft 365. O esquema é uma lista simples de todas as propriedades que você planeja adicionar à conexão junto com seus atributos, rótulos e aliases. Você deve registrar o esquema antes de ingerir itens no Microsoft Graph.

Para saber mais, consulte [Registrar e atualizar o esquema para a conexão do Microsoft Graph](connecting-external-content-manage-schema.md).

## <a name="ingest-external-data-items-into-microsoft-graph"></a>Ingerir itens de dados externos no Microsoft Graph.

Os itens adicionados por seu aplicativo ao serviço Pesquisa da Microsoft são representados pelo recurso [externalItem](/graph/api/resources/externalconnectors-externalitem) (API de item externo) no Microsoft Graph.

Para saber mais, consulte [Criar, atualizar e excluir itens adicionados por seu aplicativo por meio de conectores do Microsoft Graph](connecting-external-content-manage-items.md).

## <a name="sync-external-groups"></a>Sincronizar grupos externos

Os itens no serviço externo podem ter acesso concedido ou negado por meio da ACL para diferentes tipos de grupos que não são do Azure Active Directory. Por exemplo, os itens do Salesforce podem ter conjuntos de permissões e perfis, enquanto os itens do ServiceNow podem ter grupos locais. Ao ingerir esses itens no Microsoft Graph, você precisará respeitar essas ACLs.

Você pode usar a API de grupo externo para definir permissões em itens externos ingeridos no Microsoft Graph. Um [externalGroup](/graph/api/resources/externalconnectors-externalgroup) representa um grupo não Azure Active Directory ou uma construção semelhante a um grupo (como unidades de negócios, equipes e assim por diante) e determina permissões no conteúdo em sua fonte de dados externa.

Para saber mais, consulte [Usar grupos externos para gerenciar permissões para fontes de dados de conectores do Microsoft Graph](connecting-external-content-external-groups.md).

## <a name="next-steps"></a>Próximas etapas

- [Criar um conector personalizado](/graph/connecting-external-content-build-quickstart)