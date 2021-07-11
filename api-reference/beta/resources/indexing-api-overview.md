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
# <a name="use-the-microsoft-search-api-to-index-data"></a><span data-ttu-id="259cc-103">Usar a API de Pesquisa da Microsoft para indexar dados</span><span class="sxs-lookup"><span data-stu-id="259cc-103">Use the Microsoft Search API to index data</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="259cc-104">Você pode usar o Microsoft Graph para adicionar itens personalizados aos resultados da pesquisa na experiência de [Pesquisa da Microsoft](/microsoftsearch/overview-microsoft-search).</span><span class="sxs-lookup"><span data-stu-id="259cc-104">You can use Microsoft Graph to add custom items to search results in the [Microsoft Search](/microsoftsearch/overview-microsoft-search) experience.</span></span>

<span data-ttu-id="259cc-105">As solicitações de indexação de dados são realizadas em nome de um aplicativo sem a presença de um usuário conectado, identificado usando um [token de acesso com permissão de aplicativo](/graph/auth-v2-service).</span><span class="sxs-lookup"><span data-stu-id="259cc-105">Requests to index data are performed on behalf of an application without the presence of a signed-in user, identified using an [access token with application permission](/graph/auth-v2-service).</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="259cc-106">Casos de uso comuns</span><span class="sxs-lookup"><span data-stu-id="259cc-106">Common use cases</span></span>

<span data-ttu-id="259cc-107">Os casos de uso das APIs nesta seção tratam da criação de [conectores do Microsoft Graph](/microsoftsearch/connectors-overview), o que envolve as principais etapas para:</span><span class="sxs-lookup"><span data-stu-id="259cc-107">The use cases for the APIs in this section involve building [Microsoft Graph connectors](/microsoftsearch/connectors-overview), which involves the following primary steps:</span></span>

1. <span data-ttu-id="259cc-108">[Criar uma conexão](../api/external-post-connections.md) para uma fonte de dados externa.</span><span class="sxs-lookup"><span data-stu-id="259cc-108">[Create a connection](../api/external-post-connections.md) to an external data source.</span></span>
2. <span data-ttu-id="259cc-109">[Criar e registrar um esquema](../api/externalconnection-post-schema.md) que descreve o tipo e como indexar os dados externos.</span><span class="sxs-lookup"><span data-stu-id="259cc-109">[Create and register a schema](../api/externalconnection-post-schema.md) that describes the type and how to index the external data.</span></span>
3. <span data-ttu-id="259cc-110">[Indexar os dados](../api/externalconnection-put-items.md) como um item externo.</span><span class="sxs-lookup"><span data-stu-id="259cc-110">[Index the data](../api/externalconnection-put-items.md) as an external item.</span></span>

| <span data-ttu-id="259cc-111">Casos de uso</span><span class="sxs-lookup"><span data-stu-id="259cc-111">Use cases</span></span>                                        | <span data-ttu-id="259cc-112">Recursos REST</span><span class="sxs-lookup"><span data-stu-id="259cc-112">REST resources</span></span>                              | <span data-ttu-id="259cc-113">Confira também</span><span class="sxs-lookup"><span data-stu-id="259cc-113">See also</span></span> |
|:-------------------------------------------------|:--------------------------------------------|:--|
| <span data-ttu-id="259cc-114">**Ações de configuração**</span><span class="sxs-lookup"><span data-stu-id="259cc-114">**Configuration actions**</span></span>                        |                                             |   |
| <span data-ttu-id="259cc-115">Criar, atualizar ou excluir uma conexão</span><span class="sxs-lookup"><span data-stu-id="259cc-115">Create, update, or delete a connection</span></span>           | [<span data-ttu-id="259cc-116">externalConnection</span><span class="sxs-lookup"><span data-stu-id="259cc-116">externalConnection</span></span>](externalconnection.md) | [<span data-ttu-id="259cc-117">Métodos de externalConnection</span><span class="sxs-lookup"><span data-stu-id="259cc-117">externalConnection methods</span></span>](externalconnection.md#methods) |
| <span data-ttu-id="259cc-118">Registrar um esquema para os dados externos</span><span class="sxs-lookup"><span data-stu-id="259cc-118">Register a schema for the external data</span></span>          | [<span data-ttu-id="259cc-119">schema</span><span class="sxs-lookup"><span data-stu-id="259cc-119">schema</span></span>](schema.md)                         | [<span data-ttu-id="259cc-120">métodos de esquema</span><span class="sxs-lookup"><span data-stu-id="259cc-120">schema methods</span></span>](schema.md#methods) |
| <span data-ttu-id="259cc-121">**Ações de indexação**</span><span class="sxs-lookup"><span data-stu-id="259cc-121">**Indexing actions**</span></span>                             |                                             |   |
| <span data-ttu-id="259cc-122">Adicionar, atualizar ou excluir um item personalizado no índice</span><span class="sxs-lookup"><span data-stu-id="259cc-122">Add, update or delete a custom item in the index</span></span> | [<span data-ttu-id="259cc-123">externalItem</span><span class="sxs-lookup"><span data-stu-id="259cc-123">externalItem</span></span>](externalitem.md)             | [<span data-ttu-id="259cc-124">métodos de externalItem</span><span class="sxs-lookup"><span data-stu-id="259cc-124">externalItem methods</span></span>](externalItem.md#methods) |

## <a name="known-limitations"></a><span data-ttu-id="259cc-125">Limitações conhecidas</span><span class="sxs-lookup"><span data-stu-id="259cc-125">Known limitations</span></span>

<span data-ttu-id="259cc-126">A seguir estão as limitações conhecidas atuais:</span><span class="sxs-lookup"><span data-stu-id="259cc-126">The following are current known limitations:</span></span>

- <span data-ttu-id="259cc-127">As organizações estão limitadas a um máximo de 10 conexões.</span><span class="sxs-lookup"><span data-stu-id="259cc-127">Organizations are limited to a maximum of 10 connections.</span></span>
- <span data-ttu-id="259cc-128">Somente as identidades do Azure Active Directory são compatíveis.</span><span class="sxs-lookup"><span data-stu-id="259cc-128">Only Azure Active Directory identities are supported.</span></span>
- <span data-ttu-id="259cc-129">Você só pode criar quatro itens de recursos `externalItem` por segundo.</span><span class="sxs-lookup"><span data-stu-id="259cc-129">You can create only four `externalItem` resources items per second.</span></span>
- <span data-ttu-id="259cc-130">Um aplicativo está limitado a quatro operações simultâneas em uma conexão.</span><span class="sxs-lookup"><span data-stu-id="259cc-130">An application is limited to four concurrent operations on a connection.</span></span>
- <span data-ttu-id="259cc-131">As conexões têm um limite de capacidade de 700 mil itens ou aproximadamente 70 GB de dados.</span><span class="sxs-lookup"><span data-stu-id="259cc-131">Connections have a capacity limit of 700,000 items or ~70 GB of data.</span></span>
- <span data-ttu-id="259cc-132">O tamanho máximo de uma entidade `externalItem` é 4 MB.</span><span class="sxs-lookup"><span data-stu-id="259cc-132">Maximum size of an `externalItem` entity is 4 MB.</span></span>
- <span data-ttu-id="259cc-133">A classificação de resultados não é compatível.</span><span class="sxs-lookup"><span data-stu-id="259cc-133">Sorting results is not supported.</span></span>
- <span data-ttu-id="259cc-134">A classificação de resultados é pelo melhor esforço.</span><span class="sxs-lookup"><span data-stu-id="259cc-134">Result ranking is best effort.</span></span>

## <a name="whats-new"></a><span data-ttu-id="259cc-135">O que há de novo</span><span class="sxs-lookup"><span data-stu-id="259cc-135">What's new</span></span>
<span data-ttu-id="259cc-136">Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.</span><span class="sxs-lookup"><span data-stu-id="259cc-136">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>

## <a name="next-steps"></a><span data-ttu-id="259cc-137">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="259cc-137">Next steps</span></span>

- <span data-ttu-id="259cc-138">Confira a [Visão geral da API de Pesquisa da Microsoft](/graph/search-concept-overview).</span><span class="sxs-lookup"><span data-stu-id="259cc-138">See the [Microsoft Search API overview](/graph/search-concept-overview).</span></span>
- <span data-ttu-id="259cc-139">Faça uma busca detalhada sobre os métodos, propriedades e relações dos recursos [externalConnection](externalconnection.md), [schema](schema.md)e [externalItem](externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="259cc-139">Drill down on the methods, properties, and relationships of the [externalConnection](externalconnection.md), [schema](schema.md), and [externalItem](externalitem.md) resources.</span></span>
- <span data-ttu-id="259cc-140">Confira o [exemplo de conector de pesquisa](https://github.com/microsoftgraph/msgraph-search-connector-sample) no GitHub.</span><span class="sxs-lookup"><span data-stu-id="259cc-140">Check out the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub.</span></span>


