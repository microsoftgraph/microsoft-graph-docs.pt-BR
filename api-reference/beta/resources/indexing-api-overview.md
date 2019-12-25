---
title: Usar a API de Pesquisa da Microsoft para indexar dados
description: Use o Microsoft Graph para indexar itens personalizados ou arquivos externos no serviço da Pesquisa da Microsoft.
localization_priority: Priority
author: snlraju-msft
ms.prod: search
doc_type: conceptualPageType
ms.openlocfilehash: f1a39a42f94a072c501c288b55a6b665af0fc640
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870226"
---
# <a name="use-the-microsoft-search-api-to-index-data"></a><span data-ttu-id="15beb-103">Usar a API de Pesquisa da Microsoft para indexar dados</span><span class="sxs-lookup"><span data-stu-id="15beb-103">Use the Microsoft Search API to index data</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15beb-104">Você pode usar o Microsoft Graph para adicionar itens personalizados ou arquivos externos aos resultados da pesquisa na experiência da [Pesquisa da Microsoft](/microsoftsearch/overview-microsoft-search).</span><span class="sxs-lookup"><span data-stu-id="15beb-104">Microsoft Graph lets your app add custom items or external files into search results in the [Microsoft Search](/microsoftsearch/overview-microsoft-search) experience.</span></span>

<span data-ttu-id="15beb-105">As solicitações de indexação de dados são realizadas em nome de um aplicativo sem a presença de um usuário conectado, identificado usando um [token de acesso com permissão de aplicativo](/graph/auth-v2-service).</span><span class="sxs-lookup"><span data-stu-id="15beb-105">Requests to index data are performed on behalf of an application without the presence of a signed-in user, identified using an [access token with application permission](/graph/auth-v2-service).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="common-use-cases"></a><span data-ttu-id="15beb-106">Casos de uso comuns</span><span class="sxs-lookup"><span data-stu-id="15beb-106">Common use cases</span></span>

<span data-ttu-id="15beb-107">Os casos de uso das APIs nesta seção tratam da criação de [conectores do Microsoft Graph](/microsoftsearch/connectors-overview), o que envolve as principais etapas para:</span><span class="sxs-lookup"><span data-stu-id="15beb-107">The use cases for the APIs in this section center around building [Microsoft Graph connectors](/microsoftsearch/connectors-overview), which involves the main steps of:</span></span>

1. <span data-ttu-id="15beb-108">[Criar uma conexão](../api/external-post-connections.md) para uma fonte de dados externa.</span><span class="sxs-lookup"><span data-stu-id="15beb-108">[Creating a connection](../api/external-post-connections.md) to an external data source</span></span>
2. <span data-ttu-id="15beb-109">[Criar e registrar um esquema](../api/externalconnection-post-schema.md) que descreve o tipo e como indexar os dados externos.</span><span class="sxs-lookup"><span data-stu-id="15beb-109">[Creating and registering a schema](../api/externalconnection-post-schema.md) that describes the type and how to index the external data</span></span>
3. <span data-ttu-id="15beb-110">[Indexar dados](../api/externalconnection-put-items.md) como um item ou arquivo externos.</span><span class="sxs-lookup"><span data-stu-id="15beb-110">[Indexing the data](../api/externalconnection-put-items.md) as an external item or external file</span></span>

| <span data-ttu-id="15beb-111">Casos de uso</span><span class="sxs-lookup"><span data-stu-id="15beb-111">Use cases</span></span>                                        | <span data-ttu-id="15beb-112">Recursos REST</span><span class="sxs-lookup"><span data-stu-id="15beb-112">REST resources</span></span>                              | <span data-ttu-id="15beb-113">Confira também</span><span class="sxs-lookup"><span data-stu-id="15beb-113">See also</span></span> |
|:-------------------------------------------------|:--------------------------------------------|:--|
| <span data-ttu-id="15beb-114">**Ações de configuração**</span><span class="sxs-lookup"><span data-stu-id="15beb-114">**Configuration actions**</span></span>                        |                                             |   |
| <span data-ttu-id="15beb-115">Criar, atualizar ou excluir uma conexão</span><span class="sxs-lookup"><span data-stu-id="15beb-115">Create, update, or delete a connection</span></span>           | [<span data-ttu-id="15beb-116">externalConnection</span><span class="sxs-lookup"><span data-stu-id="15beb-116">externalConnection</span></span>](externalconnection.md) | [<span data-ttu-id="15beb-117">Métodos de externalConnection</span><span class="sxs-lookup"><span data-stu-id="15beb-117">externalConnection methods</span></span>](externalconnection.md#methods) |
| <span data-ttu-id="15beb-118">Registrar um esquema para os dados externos</span><span class="sxs-lookup"><span data-stu-id="15beb-118">Register a schema for the external data</span></span>          | [<span data-ttu-id="15beb-119">schema</span><span class="sxs-lookup"><span data-stu-id="15beb-119">schema</span></span>](schema.md)                         | [<span data-ttu-id="15beb-120">métodos de esquema</span><span class="sxs-lookup"><span data-stu-id="15beb-120">schema methods</span></span>](schema.md#methods) |
| <span data-ttu-id="15beb-121">**Ações de indexação**</span><span class="sxs-lookup"><span data-stu-id="15beb-121">**Indexing actions**</span></span>                             |                                             |   |
| <span data-ttu-id="15beb-122">Adicionar, atualizar ou excluir um item personalizado no índice</span><span class="sxs-lookup"><span data-stu-id="15beb-122">Add, update or delete a custom item in the index</span></span> | [<span data-ttu-id="15beb-123">externalItem</span><span class="sxs-lookup"><span data-stu-id="15beb-123">externalItem</span></span>](externalitem.md)             | [<span data-ttu-id="15beb-124">métodos de externalItem</span><span class="sxs-lookup"><span data-stu-id="15beb-124">externalItem methods</span></span>](externalItem.md#methods) |
| <span data-ttu-id="15beb-125">Adicionar, atualizar ou excluir um arquivo no índice</span><span class="sxs-lookup"><span data-stu-id="15beb-125">Add, update or delete a file in the index</span></span>        | [<span data-ttu-id="15beb-126">externalFile</span><span class="sxs-lookup"><span data-stu-id="15beb-126">externalFile</span></span>](externalfile.md)             | [<span data-ttu-id="15beb-127">métodos de externalFile</span><span class="sxs-lookup"><span data-stu-id="15beb-127">externalFile methods</span></span>](externalfile.md#methods) |

## <a name="known-limitations"></a><span data-ttu-id="15beb-128">Limitações conhecidas</span><span class="sxs-lookup"><span data-stu-id="15beb-128">Known limitations</span></span>

<span data-ttu-id="15beb-129">Os seguintes são limitações conhecidas atuais:</span><span class="sxs-lookup"><span data-stu-id="15beb-129">The following are current knownlimitations:</span></span>

- <span data-ttu-id="15beb-130">As organizações estão limitadas a um máximo de 10 conexões.</span><span class="sxs-lookup"><span data-stu-id="15beb-130">Organizations are limited to a maximum of 10 connections.</span></span>
- <span data-ttu-id="15beb-131">Não há suporte para propriedades personalizadas ao indexar arquivos usando o recurso `externalFile`.</span><span class="sxs-lookup"><span data-stu-id="15beb-131">Custom properties are not supported when indexing files using the `externalFile` resource.</span></span>
- <span data-ttu-id="15beb-132">Somente as identidades do Azure Active Directory são compatíveis.</span><span class="sxs-lookup"><span data-stu-id="15beb-132">Only Azure Active Directory identities are supported.</span></span>
- <span data-ttu-id="15beb-133">Você pode criar apenas quatro itens de recursos `externalItem` ou `externalFile` por segundo.</span><span class="sxs-lookup"><span data-stu-id="15beb-133">You can create only four `externalItem` or `externalFile` resources items per second.</span></span>
- <span data-ttu-id="15beb-134">Um aplicativo está limitado a quatro operações simultâneas em uma conexão.</span><span class="sxs-lookup"><span data-stu-id="15beb-134">An application is limited to 4 concurrent operations on a connection.</span></span>
- <span data-ttu-id="15beb-135">As conexões têm um limite de capacidade de 700 mil itens ou aproximadamente 70 GB de dados.</span><span class="sxs-lookup"><span data-stu-id="15beb-135">Connections have a capacity limit of 700,000 items or ~70 GB of data.</span></span>
- <span data-ttu-id="15beb-136">O tamanho máximo de uma entidade `externalItem` ou `externalFile` é 4 MB.</span><span class="sxs-lookup"><span data-stu-id="15beb-136">Maximum size of an `externalItem` or `externalFile` entity is 4 MB.</span></span>
- <span data-ttu-id="15beb-137">Não há suporte para refinar e classificar os resultados.</span><span class="sxs-lookup"><span data-stu-id="15beb-137">Refining and sorting results is not supported.</span></span>
- <span data-ttu-id="15beb-138">A classificação de resultados é pelo melhor esforço.</span><span class="sxs-lookup"><span data-stu-id="15beb-138">Result ranking is best effort.</span></span>

## <a name="next-steps"></a><span data-ttu-id="15beb-139">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="15beb-139">Next steps</span></span>

- <span data-ttu-id="15beb-140">Confira a [Visão geral da API de Pesquisa da Microsoft](/graph/search-concept-overview).</span><span class="sxs-lookup"><span data-stu-id="15beb-140">See the [Microsoft Search API overview](/graph/search-concept-overview).</span></span>
- <span data-ttu-id="15beb-141">Faça uma busca detalhada sobre os métodos, as propriedades e as relações dos recursos [externalConnection](externalconnection.md), [schema](schema.md), [externalItem](externalitem.md) e [externalFile](externalfile.md).</span><span class="sxs-lookup"><span data-stu-id="15beb-141">Drill down on the methods, properties, and relationships of the [externalConnection](externalconnection.md), [schema](schema.md), [externalItem](externalitem.md), and [externalFile](externalfile.md) resources.</span></span>
- <span data-ttu-id="15beb-142">Confira o [exemplo de conector de pesquisa](https://github.com/microsoftgraph/msgraph-search-connector-sample) no GitHub.</span><span class="sxs-lookup"><span data-stu-id="15beb-142">Check out the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub.</span></span>
