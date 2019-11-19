---
title: Usar a API de Pesquisa da Microsoft para indexar dados
description: O Microsoft Graph permite que o índice do aplicativo tenha itens personalizados ou arquivos externos no serviço da Pesquisa da Microsoft.
localization_priority: Priority
author: snlraju-msft
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: e6afa7be0f1bf7dbda0561f8bd0e89ce8b0a3e4d
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703781"
---
# <a name="use-the-microsoft-search-api-to-index-data"></a><span data-ttu-id="7b853-103">Usar a API de Pesquisa da Microsoft para indexar dados</span><span class="sxs-lookup"><span data-stu-id="7b853-103">Use the Microsoft Search API to index data</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b853-104">O Microsoft Graph permite que o seu aplicativo adicione itens personalizados ou arquivos externos aos resultados da pesquisa na experiência da [Pesquisa da Microsoft](/microsoftsearch/overview-microsoft-search).</span><span class="sxs-lookup"><span data-stu-id="7b853-104">Microsoft Graph lets your app add custom items or external files into search results in the [Microsoft Search](/microsoftsearch/overview-microsoft-search) experience.</span></span>

<span data-ttu-id="7b853-105">As solicitações de indexação de dados são realizadas em nome de um aplicativo sem a presença de um usuário conectado, identificado usando um [token de acesso com permissão de aplicativo](/graph/auth-v2-service).</span><span class="sxs-lookup"><span data-stu-id="7b853-105">Requests to index data are performed on behalf of an application without the presence of a signed-in user, identified using an [access token with application permission](/graph/auth-v2-service).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="common-use-cases"></a><span data-ttu-id="7b853-106">Casos de uso comuns</span><span class="sxs-lookup"><span data-stu-id="7b853-106">Common use cases</span></span>

<span data-ttu-id="7b853-107">Os casos de uso das APIs nesta seção se concentram na criação de [conectores do Microsoft Graph](/microsoftsearch/connectors-overview), o que envolve as principais etapas para:</span><span class="sxs-lookup"><span data-stu-id="7b853-107">The use cases for the APIs in this section center around building [Microsoft Graph connectors](/microsoftsearch/connectors-overview), which involves the main steps of:</span></span>

1. <span data-ttu-id="7b853-108">[Criar uma conexão](../api/external-post-connections.md) com uma fonte de dados externa</span><span class="sxs-lookup"><span data-stu-id="7b853-108">[Creating a connection](../api/external-post-connections.md) to an external data source</span></span>
2. <span data-ttu-id="7b853-109">[Criar e registrar um esquema](../api/externalconnection-post-schema.md) que descreve o tipo e como indexar os dados externos</span><span class="sxs-lookup"><span data-stu-id="7b853-109">[Creating and registering a schema](../api/externalconnection-post-schema.md) that describes the type and how to index the external data</span></span>
3. <span data-ttu-id="7b853-110">[Indexar dados](../api/externalconnection-put-items.md) como um item externo ou um arquivo externo</span><span class="sxs-lookup"><span data-stu-id="7b853-110">[Indexing the data](../api/externalconnection-put-items.md) as an external item or external file</span></span>

| <span data-ttu-id="7b853-111">Casos de uso</span><span class="sxs-lookup"><span data-stu-id="7b853-111">Use cases</span></span>                                        | <span data-ttu-id="7b853-112">Recursos REST</span><span class="sxs-lookup"><span data-stu-id="7b853-112">REST resources</span></span>                              | <span data-ttu-id="7b853-113">Confira também</span><span class="sxs-lookup"><span data-stu-id="7b853-113">See also</span></span> |
|:-------------------------------------------------|:--------------------------------------------|:--|
| <span data-ttu-id="7b853-114">**Ações de configuração**</span><span class="sxs-lookup"><span data-stu-id="7b853-114">**Configuration actions**</span></span>                        |                                             |   |
| <span data-ttu-id="7b853-115">Criar, atualizar ou excluir uma conexão</span><span class="sxs-lookup"><span data-stu-id="7b853-115">Create, update, or delete a connection</span></span>           | [<span data-ttu-id="7b853-116">externalConnection</span><span class="sxs-lookup"><span data-stu-id="7b853-116">externalConnection</span></span>](externalconnection.md) | [<span data-ttu-id="7b853-117">Métodos de externalConnection</span><span class="sxs-lookup"><span data-stu-id="7b853-117">Methods of externalConnection</span></span>](externalconnection.md#methods) |
| <span data-ttu-id="7b853-118">Registrar um esquema para os dados externos</span><span class="sxs-lookup"><span data-stu-id="7b853-118">Register a schema for the external data</span></span>          | [<span data-ttu-id="7b853-119">schema</span><span class="sxs-lookup"><span data-stu-id="7b853-119">schema</span></span>](schema.md)                         | [<span data-ttu-id="7b853-120">Métodos de schema</span><span class="sxs-lookup"><span data-stu-id="7b853-120">Methods of schema</span></span>](schema.md#methods) |
| <span data-ttu-id="7b853-121">**Ações de indexação**</span><span class="sxs-lookup"><span data-stu-id="7b853-121">**Indexing actions**</span></span>                             |                                             |   |
| <span data-ttu-id="7b853-122">Adicionar, atualizar ou excluir um item personalizado no índice</span><span class="sxs-lookup"><span data-stu-id="7b853-122">Add, update or delete a custom item in the index</span></span> | [<span data-ttu-id="7b853-123">externalItem</span><span class="sxs-lookup"><span data-stu-id="7b853-123">externalItem</span></span>](externalitem.md)             | [<span data-ttu-id="7b853-124">Métodos de externalItem</span><span class="sxs-lookup"><span data-stu-id="7b853-124">Methods of externalItem</span></span>](externalItem.md#methods) |
| <span data-ttu-id="7b853-125">Adicionar, atualizar ou excluir um arquivo no índice</span><span class="sxs-lookup"><span data-stu-id="7b853-125">Add, update or delete a file in the index</span></span>        | [<span data-ttu-id="7b853-126">externalFile</span><span class="sxs-lookup"><span data-stu-id="7b853-126">externalFile</span></span>](externalfile.md)             | [<span data-ttu-id="7b853-127">Métodos de externalFile</span><span class="sxs-lookup"><span data-stu-id="7b853-127">Methods of externalFile</span></span>](externalfile.md#methods) |

## <a name="known-limitations"></a><span data-ttu-id="7b853-128">Limitações conhecidas</span><span class="sxs-lookup"><span data-stu-id="7b853-128">Known limitations</span></span>

<span data-ttu-id="7b853-129">Observe as seguintes limitações durante a visualização.</span><span class="sxs-lookup"><span data-stu-id="7b853-129">Note the following limitations during preview.</span></span>

- <span data-ttu-id="7b853-130">As organizações estão limitadas a um máximo de 10 conexões.</span><span class="sxs-lookup"><span data-stu-id="7b853-130">Organizations are limited to a maximum of 10 connections.</span></span>
- <span data-ttu-id="7b853-131">Não há suporte para propriedades personalizadas ao indexar arquivos usando o recurso `externalFile`.</span><span class="sxs-lookup"><span data-stu-id="7b853-131">No support for custom properties when indexing files using the `externalFile` resource.</span></span>
- <span data-ttu-id="7b853-132">Somente as identidades do Azure Active Directory são compatíveis.</span><span class="sxs-lookup"><span data-stu-id="7b853-132">Only Azure Active Directory identities are supported.</span></span>
- <span data-ttu-id="7b853-133">A criação de recursos `externalItem` ou `externalFile` está limitada a quatro itens por segundo.</span><span class="sxs-lookup"><span data-stu-id="7b853-133">Creating `externalItem` or `externalFile` resources is limited to 4 items per second.</span></span>
- <span data-ttu-id="7b853-134">Um aplicativo está limitado a quatro operações simultâneas em uma conexão.</span><span class="sxs-lookup"><span data-stu-id="7b853-134">An application is limited to 4 concurrent operations on a connection.</span></span>
- <span data-ttu-id="7b853-135">As conexões têm um limite de capacidade de 700 mil itens ou aproximadamente 70 GB de dados.</span><span class="sxs-lookup"><span data-stu-id="7b853-135">Connections have a capacity limit of 700,000 items or ~70 GB of data.</span></span>
- <span data-ttu-id="7b853-136">O tamanho máximo de uma entidade `externalItem` ou `externalFile` é 4 MB.</span><span class="sxs-lookup"><span data-stu-id="7b853-136">Maximum size of an `externalItem` or `externalFile` entity is 4 MB.</span></span>
- <span data-ttu-id="7b853-137">Não há suporte para refinar e classificar os resultados.</span><span class="sxs-lookup"><span data-stu-id="7b853-137">No support for refining and sorting results.</span></span>
- <span data-ttu-id="7b853-138">A classificação de resultados é pelo melhor esforço.</span><span class="sxs-lookup"><span data-stu-id="7b853-138">Result ranking is best effort.</span></span>

## <a name="next-steps"></a><span data-ttu-id="7b853-139">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="7b853-139">Next steps</span></span>

- [<span data-ttu-id="7b853-140">Visão geral da API de Pesquisa da Microsoft</span><span class="sxs-lookup"><span data-stu-id="7b853-140">Microsoft Search API overview</span></span>](/graph/search-concept-overview)
- <span data-ttu-id="7b853-141">Faça uma busca detalhada sobre os métodos, as propriedades e as relações dos recursos [externalConnection](externalconnection.md), [schema](schema.md), [externalItem](externalitem.md) e [externalFile](externalfile.md).</span><span class="sxs-lookup"><span data-stu-id="7b853-141">Drill down on the methods, properties, and relationships of the [externalConnection](externalconnection.md), [schema](schema.md), [externalItem](externalitem.md), and [externalFile](externalfile.md) resources.</span></span>
- <span data-ttu-id="7b853-142">Confira o [exemplo de conector de pesquisa](https://github.com/microsoftgraph/msgraph-search-connector-sample) no GitHub.</span><span class="sxs-lookup"><span data-stu-id="7b853-142">Check out the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub.</span></span>
