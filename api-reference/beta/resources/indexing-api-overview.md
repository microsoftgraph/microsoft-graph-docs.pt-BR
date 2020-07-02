---
title: Usar a API de Pesquisa da Microsoft para indexar dados
description: Use o Microsoft Graph para indexar itens personalizados no serviço de Pesquisa da Microsoft.
localization_priority: Priority
author: snlraju-msft
ms.prod: search
doc_type: conceptualPageType
ms.openlocfilehash: 641b1f8b6288073a6079d2777bd30f8277467bed
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "44989811"
---
# <a name="use-the-microsoft-search-api-to-index-data"></a><span data-ttu-id="86662-103">Usar a API de Pesquisa da Microsoft para indexar dados</span><span class="sxs-lookup"><span data-stu-id="86662-103">Use the Microsoft Search API to index data</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86662-104">Você pode usar o Microsoft Graph para adicionar itens personalizados aos resultados da pesquisa na experiência de [Pesquisa da Microsoft](/microsoftsearch/overview-microsoft-search).</span><span class="sxs-lookup"><span data-stu-id="86662-104">You can use Microsoft Graph to add custom items to search results in the [Microsoft Search](/microsoftsearch/overview-microsoft-search) experience.</span></span>

<span data-ttu-id="86662-105">As solicitações de indexação de dados são realizadas em nome de um aplicativo sem a presença de um usuário conectado, identificado usando um [token de acesso com permissão de aplicativo](/graph/auth-v2-service).</span><span class="sxs-lookup"><span data-stu-id="86662-105">Requests to index data are performed on behalf of an application without the presence of a signed-in user, identified using an [access token with application permission](/graph/auth-v2-service).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="common-use-cases"></a><span data-ttu-id="86662-106">Casos de uso comuns</span><span class="sxs-lookup"><span data-stu-id="86662-106">Common use cases</span></span>

<span data-ttu-id="86662-107">Os casos de uso das APIs nesta seção tratam da criação de [conectores do Microsoft Graph](/microsoftsearch/connectors-overview), o que envolve as principais etapas para:</span><span class="sxs-lookup"><span data-stu-id="86662-107">The use cases for the APIs in this section involve building [Microsoft Graph connectors](/microsoftsearch/connectors-overview), which involves the following primary steps:</span></span>

1. <span data-ttu-id="86662-108">[Criar uma conexão](../api/external-post-connections.md) para uma fonte de dados externa.</span><span class="sxs-lookup"><span data-stu-id="86662-108">[Create a connection](../api/external-post-connections.md) to an external data source.</span></span>
2. <span data-ttu-id="86662-109">[Criar e registrar um esquema](../api/externalconnection-post-schema.md) que descreve o tipo e como indexar os dados externos.</span><span class="sxs-lookup"><span data-stu-id="86662-109">[Create and register a schema](../api/externalconnection-post-schema.md) that describes the type and how to index the external data.</span></span>
3. <span data-ttu-id="86662-110">[Indexar os dados](../api/externalconnection-put-items.md) como um item externo.</span><span class="sxs-lookup"><span data-stu-id="86662-110">[Index the data](../api/externalconnection-put-items.md) as an external item.</span></span>

| <span data-ttu-id="86662-111">Casos de uso</span><span class="sxs-lookup"><span data-stu-id="86662-111">Use cases</span></span>                                        | <span data-ttu-id="86662-112">Recursos REST</span><span class="sxs-lookup"><span data-stu-id="86662-112">REST resources</span></span>                              | <span data-ttu-id="86662-113">Confira também</span><span class="sxs-lookup"><span data-stu-id="86662-113">See also</span></span> |
|:-------------------------------------------------|:--------------------------------------------|:--|
| <span data-ttu-id="86662-114">**Ações de configuração**</span><span class="sxs-lookup"><span data-stu-id="86662-114">**Configuration actions**</span></span>                        |                                             |   |
| <span data-ttu-id="86662-115">Criar, atualizar ou excluir uma conexão</span><span class="sxs-lookup"><span data-stu-id="86662-115">Create, update, or delete a connection</span></span>           | [<span data-ttu-id="86662-116">externalConnection</span><span class="sxs-lookup"><span data-stu-id="86662-116">externalConnection</span></span>](externalconnection.md) | [<span data-ttu-id="86662-117">Métodos de externalConnection</span><span class="sxs-lookup"><span data-stu-id="86662-117">externalConnection methods</span></span>](externalconnection.md#methods) |
| <span data-ttu-id="86662-118">Registrar um esquema para os dados externos</span><span class="sxs-lookup"><span data-stu-id="86662-118">Register a schema for the external data</span></span>          | [<span data-ttu-id="86662-119">schema</span><span class="sxs-lookup"><span data-stu-id="86662-119">schema</span></span>](schema.md)                         | [<span data-ttu-id="86662-120">métodos de esquema</span><span class="sxs-lookup"><span data-stu-id="86662-120">schema methods</span></span>](schema.md#methods) |
| <span data-ttu-id="86662-121">**Ações de indexação**</span><span class="sxs-lookup"><span data-stu-id="86662-121">**Indexing actions**</span></span>                             |                                             |   |
| <span data-ttu-id="86662-122">Adicionar, atualizar ou excluir um item personalizado no índice</span><span class="sxs-lookup"><span data-stu-id="86662-122">Add, update or delete a custom item in the index</span></span> | [<span data-ttu-id="86662-123">externalItem</span><span class="sxs-lookup"><span data-stu-id="86662-123">externalItem</span></span>](externalitem.md)             | [<span data-ttu-id="86662-124">métodos de externalItem</span><span class="sxs-lookup"><span data-stu-id="86662-124">externalItem methods</span></span>](externalItem.md#methods) |

## <a name="known-limitations"></a><span data-ttu-id="86662-125">Limitações conhecidas</span><span class="sxs-lookup"><span data-stu-id="86662-125">Known limitations</span></span>

<span data-ttu-id="86662-126">Os seguintes são limitações conhecidas atuais:</span><span class="sxs-lookup"><span data-stu-id="86662-126">The following are current knownlimitations:</span></span>

- <span data-ttu-id="86662-127">As organizações estão limitadas a um máximo de 10 conexões.</span><span class="sxs-lookup"><span data-stu-id="86662-127">Organizations are limited to a maximum of 10 connections.</span></span>
- <span data-ttu-id="86662-128">Somente as identidades do Azure Active Directory são compatíveis.</span><span class="sxs-lookup"><span data-stu-id="86662-128">Only Azure Active Directory identities are supported.</span></span>
- <span data-ttu-id="86662-129">Você só pode criar quatro itens de recursos `externalItem` por segundo.</span><span class="sxs-lookup"><span data-stu-id="86662-129">You can create only four `externalItem` resources items per second.</span></span>
- <span data-ttu-id="86662-130">Um aplicativo está limitado a quatro operações simultâneas em uma conexão.</span><span class="sxs-lookup"><span data-stu-id="86662-130">An application is limited to four concurrent operations on a connection.</span></span>
- <span data-ttu-id="86662-131">As conexões têm um limite de capacidade de 700 mil itens ou aproximadamente 70 GB de dados.</span><span class="sxs-lookup"><span data-stu-id="86662-131">Connections have a capacity limit of 700,000 items or ~70 GB of data.</span></span>
- <span data-ttu-id="86662-132">O tamanho máximo de uma entidade `externalItem` é 4 MB.</span><span class="sxs-lookup"><span data-stu-id="86662-132">Maximum size of an `externalItem` entity is 4 MB.</span></span>
- <span data-ttu-id="86662-133">Não há suporte para a classificação de resultados.</span><span class="sxs-lookup"><span data-stu-id="86662-133">Sorting results is not supported.</span></span>
- <span data-ttu-id="86662-134">A classificação de resultados é pelo melhor esforço.</span><span class="sxs-lookup"><span data-stu-id="86662-134">Result ranking is best effort.</span></span>

## <a name="whats-new"></a><span data-ttu-id="86662-135">Novidades</span><span class="sxs-lookup"><span data-stu-id="86662-135">What's new</span></span>
<span data-ttu-id="86662-136">Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.</span><span class="sxs-lookup"><span data-stu-id="86662-136">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>

## <a name="next-steps"></a><span data-ttu-id="86662-137">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="86662-137">Next steps</span></span>

- <span data-ttu-id="86662-138">Confira a [Visão geral da API de Pesquisa da Microsoft](/graph/search-concept-overview).</span><span class="sxs-lookup"><span data-stu-id="86662-138">See the [Microsoft Search API overview](/graph/search-concept-overview).</span></span>
- <span data-ttu-id="86662-139">Faça uma busca detalhada sobre os métodos, propriedades e relações dos recursos [externalConnection](externalconnection.md), [schema](schema.md)e [externalItem](externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="86662-139">Drill down on the methods, properties, and relationships of the [externalConnection](externalconnection.md), [schema](schema.md), and [externalItem](externalitem.md) resources.</span></span>
- <span data-ttu-id="86662-140">Confira o [exemplo de conector de pesquisa](https://github.com/microsoftgraph/msgraph-search-connector-sample) no GitHub.</span><span class="sxs-lookup"><span data-stu-id="86662-140">Check out the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub.</span></span>
