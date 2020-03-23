---
title: Criar, atualizar e excluir itens adicionados por seu aplicativo no índice do serviço da Pesquisa da Microsoft
description: Aprenda a usar o Microsoft Graph para gerenciar itens adicionados pelo seu aplicativo ao serviço da Pesquisa da Microsoft
localization_priority: Priority
author: snlraju-msft
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: 5b969bd058b8c1e2790b0039a4369623287f641d
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42892783"
---
# <a name="create-update-and-delete-items-added-by-your-application-in-the-microsoft-search-service-index"></a><span data-ttu-id="1961c-103">Criar, atualizar e excluir itens adicionados por seu aplicativo no índice do serviço da Pesquisa da Microsoft</span><span class="sxs-lookup"><span data-stu-id="1961c-103">Create, update, and delete items added by your application in the Microsoft Search service index</span></span>

<span data-ttu-id="1961c-104">Os itens adicionados por seu aplicativo ao serviço de Pesquisa da Microsoft são representados pelo recurso [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1961c-104">Items added by your application to the Microsoft Search service are represented by the [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) resource in Microsoft Graph.</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

## <a name="add-an-item"></a><span data-ttu-id="1961c-105">Adicionar um item</span><span class="sxs-lookup"><span data-stu-id="1961c-105">Add an item</span></span>

<span data-ttu-id="1961c-106">Você pode adicionar um item ao índice [criando um externalItem](/graph/api/externalconnection-put-items?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="1961c-106">You can add an item to the index by [creating an externalItem](/graph/api/externalconnection-put-items?view=graph-rest-beta).</span></span> <span data-ttu-id="1961c-107">Ao criar um item, você atribui um identificador exclusivo na URL.</span><span class="sxs-lookup"><span data-stu-id="1961c-107">When you create an item, you assign a unique identifier in the URL.</span></span>

<span data-ttu-id="1961c-108">Por exemplo, seu aplicativo pode indexar tíquetes de assistência técnica usando o número do tíquete.</span><span class="sxs-lookup"><span data-stu-id="1961c-108">For example, your application may index helpdesk tickets using the ticket number.</span></span> <span data-ttu-id="1961c-109">Se um tíquete tiver o número do tíquete `SR00145`, a solicitação poderá ser semelhante à seguinte.</span><span class="sxs-lookup"><span data-stu-id="1961c-109">If a ticket has the ticket number `SR00145`, the request may look like the following.</span></span>

```http
PUT /external/connections/contosohelpdesk/items/SR00145
Content-Type: application/json

{
  "title": "WiFi outage in Conference Room A",
  "status": "New",
  "assignee": "meganb@contoso.com"
}
```

> <span data-ttu-id="1961c-110">![OBSERVAÇÃO] Antes que os itens indexados possam ser encontrados na IU da Pesquisa da Microsoft, um administrador deve [personalizar a página de resultados de pesquisa](/MicrosoftSearch/configure-connector#next-steps-customize-the-search-results-page) para a conexão correspondente.</span><span class="sxs-lookup"><span data-stu-id="1961c-110">![NOTE] Before indexed items can be found in the Microsoft Search UI, an administrator must [customize the search results page](/MicrosoftSearch/configure-connector#next-steps-customize-the-search-results-page) for the corresponding connection.</span></span>

## <a name="update-an-item"></a><span data-ttu-id="1961c-111">Atualizar um item</span><span class="sxs-lookup"><span data-stu-id="1961c-111">Update an item</span></span>

<span data-ttu-id="1961c-112">Quando um item é atualizado no serviço externo (o tíquete de assistência técnica é reatribuído ou uma descrição de produto é atualizada), você pode atualizar a respectiva entrada no índice [atualizando o externalItem](/graph/api/externalitem-update?view=graph-rest-beta), usando o identificador exclusivo atribuído ao item quando ele foi criado.</span><span class="sxs-lookup"><span data-stu-id="1961c-112">When an item is updated in the external service (helpdesk ticket is reassigned, or a product description is updated), you can update its entry in the index by [updating the externalItem](/graph/api/externalitem-update?view=graph-rest-beta), using the unique identifier assigned to the item when you created it.</span></span>

```http
PATCH /external/connections/contosohelpdesk/items/SR00145
Content-Type: application/json

{
  "assignee": "alexw@contoso.com"
}
```

## <a name="delete-an-item"></a><span data-ttu-id="1961c-113">Excluir um item</span><span class="sxs-lookup"><span data-stu-id="1961c-113">Delete an item</span></span>

<span data-ttu-id="1961c-114">Você pode remover os itens do índice [excluindo o externalItem](/graph/api/externalitem-delete?view=graph-rest-beta), usando o identificador exclusivo atribuído ao item quando ele foi criado.</span><span class="sxs-lookup"><span data-stu-id="1961c-114">You can remove items from the index by [deleting the externalItem](/graph/api/externalitem-delete?view=graph-rest-beta), using the unique identifier assigned to the item when you created it.</span></span>

```http
DELETE /external/connections/contosohelpdesk/items/SR00145
```

## <a name="next-steps"></a><span data-ttu-id="1961c-115">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="1961c-115">Next steps</span></span>

- [<span data-ttu-id="1961c-116">Por que usar a API de Pesquisa da Microsoft?</span><span class="sxs-lookup"><span data-stu-id="1961c-116">Why use the Microsoft Search API?</span></span>](search-concept-overview.md#why-use-the-microsoft-search-api)
- [<span data-ttu-id="1961c-117">Ler a referência da API de Indexação</span><span class="sxs-lookup"><span data-stu-id="1961c-117">Review the Indexing API reference</span></span>](/graph/api/resources/indexing-api-overview?view=graph-rest-beta)
- [<span data-ttu-id="1961c-118">Personalizar a página de resultados da pesquisa da Microsoft</span><span class="sxs-lookup"><span data-stu-id="1961c-118">Customize Microsoft Search results page</span></span>](/MicrosoftSearch/configure-connector#next-steps-customize-the-search-results-page)
- [<span data-ttu-id="1961c-119">Pesquisar tipos personalizados (externalItem)</span><span class="sxs-lookup"><span data-stu-id="1961c-119">Search custom types (externalItem)</span></span>](search-concept-custom-types.md)
- <span data-ttu-id="1961c-120">Baixe o [exemplo de conector de pesquisa](https://github.com/microsoftgraph/msgraph-search-connector-sample) no GitHub</span><span class="sxs-lookup"><span data-stu-id="1961c-120">Download the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub</span></span>
