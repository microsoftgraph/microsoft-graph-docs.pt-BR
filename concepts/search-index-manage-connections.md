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
# <a name="create-update-and-delete-connections-to-the-microsoft-search-service"></a><span data-ttu-id="0140e-103">Criar, atualizar e excluir conexões com o serviço da Pesquisa da Microsoft</span><span class="sxs-lookup"><span data-stu-id="0140e-103">Create, update, and delete connections to the Microsoft Search service</span></span>

<span data-ttu-id="0140e-104">As conexões de serviços externos com o serviço da Pesquisa da Microsoft são representadas pelo recurso [externalConnection](/graph/api/resources/externalconnection?view=graph-rest-beta) no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="0140e-104">Connections from external services to the Microsoft Search service are represented by the [externalConnection](/graph/api/resources/externalconnection?view=graph-rest-beta) resource in Microsoft Graph.</span></span>

<span data-ttu-id="0140e-105">Uma conexão permite que seu aplicativo [defina um esquema](/graph/api/externalconnection-post-schema?view=graph-rest-beta) para os itens que serão indexados e forneça um ponto de extremidade para o seu serviço [adicionar, atualizar ou excluir itens do índice](search-index-manage-items.md).</span><span class="sxs-lookup"><span data-stu-id="0140e-105">A connection allows your application to [define a schema](/graph/api/externalconnection-post-schema?view=graph-rest-beta) for items that will be indexed, and provides an endpoint for your service to [add, update, or delete items from the index](search-index-manage-items.md).</span></span> <span data-ttu-id="0140e-106">Criar uma conexão é a primeira etapa para um aplicativo para adicionar itens ao índice de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="0140e-106">Creating a connection is the first step for an application to add items to the search index.</span></span>

## <a name="create-a-connection"></a><span data-ttu-id="0140e-107">Criar uma conexão</span><span class="sxs-lookup"><span data-stu-id="0140e-107">Create a connection</span></span>

<span data-ttu-id="0140e-108">Antes que um aplicativo possa adicionar itens ao índice de pesquisa, ele deve criar e configurar uma conexão usando as etapas a seguir.</span><span class="sxs-lookup"><span data-stu-id="0140e-108">Before an application can add items to the search index, it must create and configure a connection using the following steps.</span></span>

- <span data-ttu-id="0140e-109">[Criar uma conexão](/graph/api/external-post-connections?view=graph-rest-beta) com ID exclusiva, nome de exibição e descrição.</span><span class="sxs-lookup"><span data-stu-id="0140e-109">[Create a connection](/graph/api/external-post-connections?view=graph-rest-beta) with a unique ID, display name, and description.</span></span>
- <span data-ttu-id="0140e-110">[Registrar um esquema](/graph/api/externalconnection-post-schema?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="0140e-110">[Registering a schema](/graph/api/externalconnection-post-schema?view=graph-rest-beta).</span></span>
  - <span data-ttu-id="0140e-111">Para itens personalizados (como tíquetes de assistência técnica ou entradas de banco de dados de inventário etc.), defina os campos que serão incluídos no índice.</span><span class="sxs-lookup"><span data-stu-id="0140e-111">For custom items (such as heldesk tickets or inventory database entries, etc.), define the fields that will be included in the index.</span></span>
  - <span data-ttu-id="0140e-112">Para arquivos externos, especifique o tipo `microsoft.graph.externalFile`.</span><span class="sxs-lookup"><span data-stu-id="0140e-112">For external files, specify the `microsoft.graph.externalFile` type.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="0140e-113">Depois que um esquema é registrado, ele não pode ser alterado para uma conexão existente.</span><span class="sxs-lookup"><span data-stu-id="0140e-113">Once a schema has been registered, it cannot be changed for an existing connection.</span></span>

## <a name="update-a-connection"></a><span data-ttu-id="0140e-114">Atualizar uma conexão</span><span class="sxs-lookup"><span data-stu-id="0140e-114">Update a connection</span></span>

<span data-ttu-id="0140e-115">Você pode alterar o nome de exibição ou a descrição de uma conexão existente [atualizando a conexão](/graph/api/externalconnection-update?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="0140e-115">You can change the display name or description of an existing connection by [updating the connection](/graph/api/externalconnection-update?view=graph-rest-beta).</span></span>

## <a name="delete-a-connection"></a><span data-ttu-id="0140e-116">Excluir uma conexão</span><span class="sxs-lookup"><span data-stu-id="0140e-116">Delete a connection</span></span>

<span data-ttu-id="0140e-117">Você pode [excluir uma conexão](/graph/api/externalconnection-delete?view=graph-rest-beta) e remover todos os itens que foram indexados por meio da conexão.</span><span class="sxs-lookup"><span data-stu-id="0140e-117">You can [delete a connection](/graph/api/externalconnection-delete?view=graph-rest-beta), and remove all items that were indexed via that connection.</span></span>

## <a name="next-steps"></a><span data-ttu-id="0140e-118">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="0140e-118">Next steps</span></span>

- [<span data-ttu-id="0140e-119">Por que usar a API de Pesquisa da Microsoft?</span><span class="sxs-lookup"><span data-stu-id="0140e-119">Why use the Microsoft Graph Security API?</span></span>](search-concept-overview.md#why-use-the-microsoft-search-api)
- [<span data-ttu-id="0140e-120">Usar a API de Pesquisa da Microsoft para indexar dados</span><span class="sxs-lookup"><span data-stu-id="0140e-120">Use the Microsoft Search API to index data</span></span>](/graph/api/resources/indexing-api-overview?view=graph-rest-beta)
- [<span data-ttu-id="0140e-121">Visão geral dos conectores do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0140e-121">Overview for Microsoft Graph Connectors</span></span>](/microsoftsearch/connectors-overview)
- <span data-ttu-id="0140e-122">Baixe o [exemplo de conector de pesquisa](https://github.com/microsoftgraph/msgraph-search-connector-sample) no GitHub</span><span class="sxs-lookup"><span data-stu-id="0140e-122">Download the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub</span></span>
