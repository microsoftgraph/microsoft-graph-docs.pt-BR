---
title: Fazer chamadas de API usando os SDKs do Microsoft Graph
description: Fornece instruções para criar solicitações HTTP do Microsoft Graph usando SDKs.
localization_priority: Normal
author: DarrelMiller
ms.openlocfilehash: d4fdd5fc6c9a5b2fb0e8acd6d5484176ef179333
ms.sourcegitcommit: d189830649794365464e37539e02239f883011da
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/24/2019
ms.locfileid: "37653514"
---
# <a name="make-api-calls-using-the-microsoft-graph-sdks"></a><span data-ttu-id="453c4-103">Fazer chamadas de API usando os SDKs do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="453c4-103">Make API calls using the Microsoft Graph SDKs</span></span>

<span data-ttu-id="453c4-104">As bibliotecas de serviço SDK do Microsoft Graph fornecem uma classe de cliente que você pode usar como o ponto de partida para a criação de todas as solicitações de API.</span><span class="sxs-lookup"><span data-stu-id="453c4-104">The Microsoft Graph SDK service libraries provide a client class that you can use as the starting point for creating all API requests.</span></span> <span data-ttu-id="453c4-105">Há dois estilos de classe de cliente: um usa uma interface fluente para criar a solicitação (por exemplo, `client.Me.Manager`) e o outro aceita uma cadeia de caracteres de caminho ( `api("/me/manager")`por exemplo,).</span><span class="sxs-lookup"><span data-stu-id="453c4-105">There are two styles of client class: one uses a fluent interface to create the request (for example, `client.Me.Manager`) and the other  accepts a path string (for example, `api("/me/manager")`).</span></span> <span data-ttu-id="453c4-106">Quando você tem um objeto Request, é possível especificar uma variedade de opções, como filtragem e classificação, e, por fim, você seleciona o tipo de operação que deseja executar.</span><span class="sxs-lookup"><span data-stu-id="453c4-106">When you have a request object, you can specify a variety of options such as filtering and sorting, and finally, you select the type of operation you want to perform.</span></span>

## <a name="read-information-from-microsoft-graph"></a><span data-ttu-id="453c4-107">Ler informações do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="453c4-107">Read information from Microsoft Graph</span></span>

<span data-ttu-id="453c4-108">Para ler informações do Microsoft Graph, você precisa primeiro criar um objeto Request e, em seguida, `GET` executar o método na solicitação.</span><span class="sxs-lookup"><span data-stu-id="453c4-108">To read information from Microsoft Graph, you first need to create a request object and then run the `GET` method on the request.</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="453c4-109">C#</span><span class="sxs-lookup"><span data-stu-id="453c4-109">C#</span></span>](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-read.md)]
# <a name="typescripttabtypescript"></a>[<span data-ttu-id="453c4-110">TypeScript</span><span class="sxs-lookup"><span data-stu-id="453c4-110">TypeScript</span></span>](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-read.md)]
---

## <a name="use-select-to-control-the-properties-returned"></a><span data-ttu-id="453c4-111">Use $select para controlar as propriedades retornadas</span><span class="sxs-lookup"><span data-stu-id="453c4-111">Use $select to control the properties returned</span></span>

<span data-ttu-id="453c4-112">Ao recuperar uma entidade, nem todas as propriedades são recuperadas automaticamente; às vezes, eles precisam ser explicitamente selecionados.</span><span class="sxs-lookup"><span data-stu-id="453c4-112">When retrieving an entity, not all properties are automatically retrieved; sometimes they need to be explicitly selected.</span></span> <span data-ttu-id="453c4-113">Além disso, em alguns cenários, não é necessário retornar o conjunto de propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="453c4-113">Also, in some scenarios it isn't necessary to return the default set of properties.</span></span> <span data-ttu-id="453c4-114">Selecionar apenas as propriedades necessárias pode melhorar o desempenho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="453c4-114">Selecting just the required properties can improve the performance of the request.</span></span> <span data-ttu-id="453c4-115">Você pode personalizar o objeto *Request* para emitir o `$select` parâmetro de consulta com uma lista de propriedades.</span><span class="sxs-lookup"><span data-stu-id="453c4-115">You can customize the *request* object to emit the `$select` query parameter with a list of properties.</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="453c4-116">C#</span><span class="sxs-lookup"><span data-stu-id="453c4-116">C#</span></span>](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-select.md)]
# <a name="typescripttabtypescript"></a>[<span data-ttu-id="453c4-117">TypeScript</span><span class="sxs-lookup"><span data-stu-id="453c4-117">TypeScript</span></span>](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-select.md)]
---


## <a name="retrieve-a-list-of-entities"></a><span data-ttu-id="453c4-118">Recuperar uma lista de entidades</span><span class="sxs-lookup"><span data-stu-id="453c4-118">Retrieve a list of entities</span></span>

<span data-ttu-id="453c4-119">A recuperação de uma lista de entidades é semelhante à recuperação de uma única entidade, exceto por várias outras opções de configuração da solicitação.</span><span class="sxs-lookup"><span data-stu-id="453c4-119">Retrieving a list of entities is similar to retrieving a single entity except there a number of other options for configuring the request.</span></span> <span data-ttu-id="453c4-120">O `$filter` parâmetro de consulta pode ser usado para reduzir o conjunto de resultados apenas às linhas que correspondem à condição fornecida.</span><span class="sxs-lookup"><span data-stu-id="453c4-120">The `$filter` query parameter can be used to reduce the result set to only those rows that match the provided condition.</span></span>  <span data-ttu-id="453c4-121">O `$orderBy` parâmetro de consulta solicitará que o servidor forneça a lista de entidades classificadas pelas propriedades especificadas.</span><span class="sxs-lookup"><span data-stu-id="453c4-121">The `$orderBy` query parameter will request that the server provide the list of entities sorted by the specified properties.</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="453c4-122">C#</span><span class="sxs-lookup"><span data-stu-id="453c4-122">C#</span></span>](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-list.md)]
# <a name="typescripttabtypescript"></a>[<span data-ttu-id="453c4-123">TypeScript</span><span class="sxs-lookup"><span data-stu-id="453c4-123">TypeScript</span></span>](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-list.md)]
---

<span data-ttu-id="453c4-124">O objeto retornado ao recuperar uma lista de entidades provavelmente será uma coleção paginável.</span><span class="sxs-lookup"><span data-stu-id="453c4-124">The object returned when retrieving a list of entities is likely to be a paged collection.</span></span> <span data-ttu-id="453c4-125">Para obter detalhes sobre como obter a lista completa de entidades, consulte [paginação por meio de uma coleção](../paging.md).</span><span class="sxs-lookup"><span data-stu-id="453c4-125">For details about how to get the complete list of entities, see [paging through a collection](../paging.md).</span></span>

## <a name="access-an-item-of-a-collection"></a><span data-ttu-id="453c4-126">Acessar um item de uma coleção</span><span class="sxs-lookup"><span data-stu-id="453c4-126">Access an item of a collection</span></span>

<span data-ttu-id="453c4-127">Para SDKs que oferecem suporte a um estilo fluente, as coleções de entidades podem ser acessadas usando um índice de matriz.</span><span class="sxs-lookup"><span data-stu-id="453c4-127">For SDKs that support a fluent style, collections of entities can be accessed using an array index.</span></span> <span data-ttu-id="453c4-128">Para SDKs baseados em modelo, é suficiente incorporar o identificador de item no segmento de caminho após a coleção.</span><span class="sxs-lookup"><span data-stu-id="453c4-128">For template-based SDKs, it is sufficient to embed the item identifier in the path segment following the collection.</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="453c4-129">C#</span><span class="sxs-lookup"><span data-stu-id="453c4-129">C#</span></span>](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-index.md)]
# <a name="typescripttabtypescript"></a>[<span data-ttu-id="453c4-130">TypeScript</span><span class="sxs-lookup"><span data-stu-id="453c4-130">TypeScript</span></span>](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-index.md)]
---

## <a name="use-expand-to-access-related-entities"></a><span data-ttu-id="453c4-131">Use $expand para acessar entidades relacionadas</span><span class="sxs-lookup"><span data-stu-id="453c4-131">Use $expand to access related entities</span></span>

<span data-ttu-id="453c4-132">Você pode usar o `$expand` filtro para solicitar uma entidade relacionada, ou uma coleção de entidades, ao mesmo que você solicite a entidade principal.</span><span class="sxs-lookup"><span data-stu-id="453c4-132">You can use the `$expand` filter to request a related entity, or collection of entities, at the same that you request the main entity.</span></span>  <span data-ttu-id="453c4-133">A `Expand()` função no objeto *Request* adiciona o parâmetro de consulta necessário.</span><span class="sxs-lookup"><span data-stu-id="453c4-133">The `Expand()` function on the *request* object adds the necessary query parameter.</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="453c4-134">C#</span><span class="sxs-lookup"><span data-stu-id="453c4-134">C#</span></span>](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-expand.md)]
# <a name="typescripttabtypescript"></a>[<span data-ttu-id="453c4-135">TypeScript</span><span class="sxs-lookup"><span data-stu-id="453c4-135">TypeScript</span></span>](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-expand.md)]
---


## <a name="delete-an-entity"></a><span data-ttu-id="453c4-136">Excluir uma entidade</span><span class="sxs-lookup"><span data-stu-id="453c4-136">Delete an entity</span></span>

<span data-ttu-id="453c4-137">Para excluir uma entidade, construa a *solicitação* da mesma maneira que você faz para recuperar uma entidade.</span><span class="sxs-lookup"><span data-stu-id="453c4-137">To delete an entity, construct the *request* in the same way that you do to retrieve an entity.</span></span> <span data-ttu-id="453c4-138">O método *delete* no objeto *Request* indica o desejo de excluir a entidade.</span><span class="sxs-lookup"><span data-stu-id="453c4-138">The *delete* method on the *request* object indicates the desire to delete the entity.</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="453c4-139">C#</span><span class="sxs-lookup"><span data-stu-id="453c4-139">C#</span></span>](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-delete.md)]
# <a name="typescripttabtypescript"></a>[<span data-ttu-id="453c4-140">TypeScript</span><span class="sxs-lookup"><span data-stu-id="453c4-140">TypeScript</span></span>](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-delete.md)]
---

## <a name="make-a-post-request-to-create-a-new-entity"></a><span data-ttu-id="453c4-141">Fazer uma solicitação POST para criar uma nova entidade</span><span class="sxs-lookup"><span data-stu-id="453c4-141">Make a POST request to create a new entity</span></span>

<span data-ttu-id="453c4-142">Para criar uma nova entidade em uma coleção, chame um `add` método `post` or e passe um objeto que contém as informações a serem usadas para criar a nova entidade.</span><span class="sxs-lookup"><span data-stu-id="453c4-142">To create a new entity in a collection, call an `add` or `post` method and pass in an object that contains the information to be used to create the new entity.</span></span> <span data-ttu-id="453c4-143">Uma versão atualizada da entidade criada normalmente é retornada da chamada.</span><span class="sxs-lookup"><span data-stu-id="453c4-143">An updated version of the created entity is usually returned from the call.</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="453c4-144">C#</span><span class="sxs-lookup"><span data-stu-id="453c4-144">C#</span></span>](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-create.md)]
# <a name="typescripttabtypescript"></a>[<span data-ttu-id="453c4-145">TypeScript</span><span class="sxs-lookup"><span data-stu-id="453c4-145">TypeScript</span></span>](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-create.md)]
---

## <a name="updating-an-existing-entity-with-patch"></a><span data-ttu-id="453c4-146">Atualizando uma entidade existente com PATCH</span><span class="sxs-lookup"><span data-stu-id="453c4-146">Updating an existing entity with PATCH</span></span>

<span data-ttu-id="453c4-147">A maioria das atualizações no Microsoft Graph é realizada `PATCH` usando um método e, portanto, só é necessário incluir as propriedades que você deseja alterar no objeto aprovado.</span><span class="sxs-lookup"><span data-stu-id="453c4-147">Most updates in Microsoft Graph are performed using a `PATCH` method and therefore it is only necessary to include the properties that you want to change in the object you pass.</span></span>  

# <a name="ctabcs"></a>[<span data-ttu-id="453c4-148">C#</span><span class="sxs-lookup"><span data-stu-id="453c4-148">C#</span></span>](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-update.md)]
# <a name="typescripttabtypescript"></a>[<span data-ttu-id="453c4-149">TypeScript</span><span class="sxs-lookup"><span data-stu-id="453c4-149">TypeScript</span></span>](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-update.md)]
---


## <a name="use-http-headers-to-control-request-behavior"></a><span data-ttu-id="453c4-150">Usar cabeçalhos HTTP para controlar o comportamento da solicitação</span><span class="sxs-lookup"><span data-stu-id="453c4-150">Use HTTP headers to control request behavior</span></span>

<span data-ttu-id="453c4-151">Você pode usar uma `header()` função para anexar cabeçalhos personalizados a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="453c4-151">You can use a `header()` function to attach custom headers to a request.</span></span> <span data-ttu-id="453c4-152">Vários cenários do Microsoft Graph usam cabeçalhos personalizados para ajustar o comportamento da solicitação.</span><span class="sxs-lookup"><span data-stu-id="453c4-152">A number of Microsoft Graph scenarios use custom headers to adjust the behavior of the request.</span></span>
 
# <a name="ctabcs"></a>[<span data-ttu-id="453c4-153">C#</span><span class="sxs-lookup"><span data-stu-id="453c4-153">C#</span></span>](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-headers.md)]
# <a name="typescripttabtypescript"></a>[<span data-ttu-id="453c4-154">TypeScript</span><span class="sxs-lookup"><span data-stu-id="453c4-154">TypeScript</span></span>](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-headers.md)]
---

## <a name="provide-custom-query-parameters"></a><span data-ttu-id="453c4-155">Fornecer parâmetros de consulta personalizados</span><span class="sxs-lookup"><span data-stu-id="453c4-155">Provide custom query parameters</span></span>

<span data-ttu-id="453c4-156">Em situações em que uma chamada de API permite parâmetros de consulta personalizados, você pode fornecer esses valores de parâmetro usando `QueryOptions` uma lista de objetos.</span><span class="sxs-lookup"><span data-stu-id="453c4-156">In situations where an API call allows custom query parameters, you can provide those parameter values by using a list of `QueryOptions` objects.</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="453c4-157">C#</span><span class="sxs-lookup"><span data-stu-id="453c4-157">C#</span></span>](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-queryparams.md)]
# <a name="typescripttabtypescript"></a>[<span data-ttu-id="453c4-158">TypeScript</span><span class="sxs-lookup"><span data-stu-id="453c4-158">TypeScript</span></span>](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-queryparams.md)]
---
