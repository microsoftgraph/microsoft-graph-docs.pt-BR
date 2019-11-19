---
title: Criar, atualizar e excluir itens adicionados por seu aplicativo no índice do serviço da Pesquisa da Microsoft
description: Aprenda a usar o Microsoft Graph para gerenciar itens adicionados pelo seu aplicativo ao serviço da Pesquisa da Microsoft
localization_priority: Priority
author: snlraju-msft
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: c5017943f966792e0246d3764a1c3e373718c63c
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704333"
---
# <a name="create-update-and-delete-items-added-by-your-application-in-the-microsoft-search-service-index"></a><span data-ttu-id="6166c-103">Criar, atualizar e excluir itens adicionados por seu aplicativo no índice do serviço da Pesquisa da Microsoft</span><span class="sxs-lookup"><span data-stu-id="6166c-103">Create, update, and delete items added by your application in the Microsoft Search service index</span></span>

<span data-ttu-id="6166c-104">Os itens adicionados pelo seu aplicativo ao serviço da Pesquisa da Microsoft são representados pelos recursos [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) e [externalFile](/graph/api/resources/externalfile?view=graph-rest-beta) no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6166c-104">Items added by your application to the Microsoft Search service are represented by the [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) and [externalFile](/graph/api/resources/externalfile?view=graph-rest-beta) resources in Microsoft Graph.</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

<span data-ttu-id="6166c-105">O recurso **externalItem** representa um tipo personalizado.</span><span class="sxs-lookup"><span data-stu-id="6166c-105">The **externalItem** resource represents a custom type.</span></span> <span data-ttu-id="6166c-106">Ele deve ser usado quando os itens que você adiciona ao índice usam um esquema personalizado não representado pelo recurso **externalFile**.</span><span class="sxs-lookup"><span data-stu-id="6166c-106">It should be used when the items you add to the index use a custom schema not represented by the **externalFile** resource.</span></span> <span data-ttu-id="6166c-107">Por exemplo, tíquetes de assistência técnica ou lista de produtos.</span><span class="sxs-lookup"><span data-stu-id="6166c-107">For example, helpdesk tickets or product listings.</span></span>

<span data-ttu-id="6166c-108">O recurso **externalFile** representa um arquivo em um sistema externo.</span><span class="sxs-lookup"><span data-stu-id="6166c-108">The **externalFile** resource represents a file in an external system.</span></span>

> [!NOTE]
> <span data-ttu-id="6166c-109">O esquema para **externalFile** não pode ser estendido.</span><span class="sxs-lookup"><span data-stu-id="6166c-109">The schema for **externalFile** cannot be extended.</span></span>

## <a name="add-an-item-or-file"></a><span data-ttu-id="6166c-110">Adicionar um item ou arquivo</span><span class="sxs-lookup"><span data-stu-id="6166c-110">Add an item or file</span></span>

<span data-ttu-id="6166c-111">Você pode adicionar um item ou arquivo ao índice [criando um externalItem](/graph/api/externalconnection-put-items?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="6166c-111">You can add an item or file to the index by [creating an externalItem](/graph/api/externalconnection-put-items?view=graph-rest-beta).</span></span> <span data-ttu-id="6166c-112">Ao criar um item, você atribui um identificador exclusivo na URL.</span><span class="sxs-lookup"><span data-stu-id="6166c-112">When you create an item, you assign a unique identifier in the URL.</span></span>

<span data-ttu-id="6166c-113">Por exemplo, seu aplicativo pode indexar tíquetes de assistência técnica usando o número do tíquete.</span><span class="sxs-lookup"><span data-stu-id="6166c-113">For example, your application may index helpdesk tickets using the ticket number.</span></span> <span data-ttu-id="6166c-114">Se um tíquete tiver o número do tíquete `SR00145`, a solicitação poderá ser semelhante à seguinte.</span><span class="sxs-lookup"><span data-stu-id="6166c-114">If a ticket has the ticket number `SR00145`, the request may look like the following.</span></span>

```http
PUT /external/connections/contosohelpdesk/items/SR00145
Content-Type: application/json

{
  "title": "WiFi outage in Conference Room A",
  "status": "New",
  "assignee": "meganb@contoso.com"
}
```

## <a name="update-an-item-or-file"></a><span data-ttu-id="6166c-115">Atualizar um item ou arquivo</span><span class="sxs-lookup"><span data-stu-id="6166c-115">Update an item or file</span></span>

<span data-ttu-id="6166c-116">Quando um item ou arquivo é atualizado no serviço externo (o tíquete da assistência técnica é reatribuído ou a descrição do produto é atualizada), você pode atualizar sua entrada no índice [atualizando o externalItem](/graph/api/externalitem-update?view=graph-rest-beta), usando o identificador exclusivo atribuído ao item quando você o criou.</span><span class="sxs-lookup"><span data-stu-id="6166c-116">When an item or file is updated in the external service (helpdesk ticket is reassigned, or a product description is updated), you can update its entry in the index by [updating the externalItem](/graph/api/externalitem-update?view=graph-rest-beta), using the unique identifier assigned to the item when you created it.</span></span>

```http
PATCH /external/connections/contosohelpdesk/items/SR00145
Content-Type: application/json

{
  "assignee": "alexw@contoso.com"
}
```

## <a name="delete-an-item-or-file"></a><span data-ttu-id="6166c-117">Excluir um item ou arquivo</span><span class="sxs-lookup"><span data-stu-id="6166c-117">Delete an item or file</span></span>

<span data-ttu-id="6166c-118">Você pode remover itens ou arquivos do índice [excluindo o externalItem](/graph/api/externalitem-delete?view=graph-rest-beta), usando o identificador exclusivo atribuído ao item quando você o criou.</span><span class="sxs-lookup"><span data-stu-id="6166c-118">You can remove items or files from the index by [deleting the externalItem](/graph/api/externalitem-delete?view=graph-rest-beta), using the unique identifier assigned to the item when you created it.</span></span>

```http
DELETE /external/connections/contosohelpdesk/items/SR00145
```

## <a name="next-steps"></a><span data-ttu-id="6166c-119">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="6166c-119">Next steps</span></span>

- [<span data-ttu-id="6166c-120">Por que usar a API de Pesquisa da Microsoft?</span><span class="sxs-lookup"><span data-stu-id="6166c-120">Why use the Microsoft Search API?</span></span>](search-concept-overview.md#why-use-the-microsoft-search-api)
- [<span data-ttu-id="6166c-121">Usar a API de Pesquisa da Microsoft para indexar dados</span><span class="sxs-lookup"><span data-stu-id="6166c-121">Use the Microsoft Search API to index data</span></span>](/graph/api/resources/indexing-api-overview?view=graph-rest-beta)
- [<span data-ttu-id="6166c-122">Pesquisar tipos personalizados (externalItem)</span><span class="sxs-lookup"><span data-stu-id="6166c-122">Search custom types (externalItem)</span></span>](search-concept-custom-types.md)
- [<span data-ttu-id="6166c-123">Pesquisar arquivos (incluindo externalFile)</span><span class="sxs-lookup"><span data-stu-id="6166c-123">Search files (including externalFile)</span></span>](search-concept-files.md)
- <span data-ttu-id="6166c-124">Baixe o [exemplo de conector de pesquisa](https://github.com/microsoftgraph/msgraph-search-connector-sample) no GitHub</span><span class="sxs-lookup"><span data-stu-id="6166c-124">Download the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub</span></span>
