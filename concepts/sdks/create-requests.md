---
title: Fazer chamadas de API usando os SDKs do Microsoft Graph
description: Fornece instruções para criar solicitações HTTP do Microsoft Graph usando SDKs.
localization_priority: Normal
author: DarrelMiller
ms.openlocfilehash: 1338cbe7411a3643eaa5c1e1e58cf8d5b9b47c0a
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288282"
---
# <a name="make-api-calls-using-the-microsoft-graph-sdks"></a><span data-ttu-id="a1912-103">Fazer chamadas de API usando os SDKs do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a1912-103">Make API calls using the Microsoft Graph SDKs</span></span>

<span data-ttu-id="a1912-104">As bibliotecas de serviço SDK do Microsoft Graph fornecem uma classe de cliente que você pode usar como o ponto de partida para a criação de todas as solicitações de API.</span><span class="sxs-lookup"><span data-stu-id="a1912-104">The Microsoft Graph SDK service libraries provide a client class that you can use as the starting point for creating all API requests.</span></span> <span data-ttu-id="a1912-105">Há dois estilos de classe de cliente: um usa uma interface fluente para criar a solicitação (por exemplo, `client.Users["user-id"].Manager` ) e o outro aceita uma cadeia de caracteres de caminho (por exemplo, `api("/users/user-id/manager")` ).</span><span class="sxs-lookup"><span data-stu-id="a1912-105">There are two styles of client class: one uses a fluent interface to create the request (for example, `client.Users["user-id"].Manager`) and the other accepts a path string (for example, `api("/users/user-id/manager")`).</span></span> <span data-ttu-id="a1912-106">Quando você tem um objeto Request, é possível especificar uma variedade de opções, como filtragem e classificação, e, por fim, você seleciona o tipo de operação que deseja executar.</span><span class="sxs-lookup"><span data-stu-id="a1912-106">When you have a request object, you can specify a variety of options such as filtering and sorting, and finally, you select the type of operation you want to perform.</span></span>

<span data-ttu-id="a1912-107">Há também o [SDK do Microsoft Graph PowerShell](../powershell/get-started.md), que não tem nenhuma classe de cliente.</span><span class="sxs-lookup"><span data-stu-id="a1912-107">There is also the [Microsoft Graph PowerShell SDK](../powershell/get-started.md), which has no client class at all.</span></span> <span data-ttu-id="a1912-108">Em vez disso, todas as solicitações são representadas como comandos do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a1912-108">Instead, all requests are represented as PowerShell commands.</span></span> <span data-ttu-id="a1912-109">Por exemplo, para obter o gerente de um usuário, o comando é `Get-MgUserManager` .</span><span class="sxs-lookup"><span data-stu-id="a1912-109">For example, to get a user's manager, the command is `Get-MgUserManager`.</span></span> <span data-ttu-id="a1912-110">Para obter mais informações sobre como localizar comandos para chamadas de API, consulte [navegação no Microsoft Graph PowerShell SDK](../powershell/navigating.md).</span><span class="sxs-lookup"><span data-stu-id="a1912-110">For more information on finding commands for API calls, see [Navigating the Microsoft Graph PowerShell SDK](../powershell/navigating.md).</span></span>

## <a name="read-information-from-microsoft-graph"></a><span data-ttu-id="a1912-111">Ler informações do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a1912-111">Read information from Microsoft Graph</span></span>

<span data-ttu-id="a1912-112">Para ler informações do Microsoft Graph, você precisa primeiro criar um objeto Request e, em seguida, executar o `GET` método na solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1912-112">To read information from Microsoft Graph, you first need to create a request object and then run the `GET` method on the request.</span></span>

# <a name="c"></a>[<span data-ttu-id="a1912-113">C#</span><span class="sxs-lookup"><span data-stu-id="a1912-113">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-read.md)]

# <a name="typescript"></a>[<span data-ttu-id="a1912-114">TypeScript</span><span class="sxs-lookup"><span data-stu-id="a1912-114">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-read.md)]

# <a name="java"></a>[<span data-ttu-id="a1912-115">Java</span><span class="sxs-lookup"><span data-stu-id="a1912-115">Java</span></span>](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-read.md)]

# <a name="powershell"></a>[<span data-ttu-id="a1912-116">PowerShell</span><span class="sxs-lookup"><span data-stu-id="a1912-116">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-read.md)]

---

## <a name="use-select-to-control-the-properties-returned"></a><span data-ttu-id="a1912-117">Use $select para controlar as propriedades retornadas</span><span class="sxs-lookup"><span data-stu-id="a1912-117">Use $select to control the properties returned</span></span>

<span data-ttu-id="a1912-118">Ao recuperar uma entidade, nem todas as propriedades são recuperadas automaticamente; às vezes, eles precisam ser explicitamente selecionados.</span><span class="sxs-lookup"><span data-stu-id="a1912-118">When retrieving an entity, not all properties are automatically retrieved; sometimes they need to be explicitly selected.</span></span> <span data-ttu-id="a1912-119">Além disso, em alguns cenários, não é necessário retornar o conjunto de propriedades padrão.</span><span class="sxs-lookup"><span data-stu-id="a1912-119">Also, in some scenarios it isn't necessary to return the default set of properties.</span></span> <span data-ttu-id="a1912-120">Selecionar apenas as propriedades necessárias pode melhorar o desempenho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1912-120">Selecting just the required properties can improve the performance of the request.</span></span> <span data-ttu-id="a1912-121">Você pode personalizar a solicitação para incluir o `$select` parâmetro de consulta com uma lista de propriedades.</span><span class="sxs-lookup"><span data-stu-id="a1912-121">You can customize the request to include the `$select` query parameter with a list of properties.</span></span>

<!-- markdownlint-disable MD024 -->
# <a name="c"></a>[<span data-ttu-id="a1912-122">C#</span><span class="sxs-lookup"><span data-stu-id="a1912-122">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-select.md)]

# <a name="typescript"></a>[<span data-ttu-id="a1912-123">TypeScript</span><span class="sxs-lookup"><span data-stu-id="a1912-123">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-select.md)]

# <a name="java"></a>[<span data-ttu-id="a1912-124">Java</span><span class="sxs-lookup"><span data-stu-id="a1912-124">Java</span></span>](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-select.md)]

# <a name="powershell"></a>[<span data-ttu-id="a1912-125">PowerShell</span><span class="sxs-lookup"><span data-stu-id="a1912-125">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-select.md)]

---

## <a name="retrieve-a-list-of-entities"></a><span data-ttu-id="a1912-126">Recuperar uma lista de entidades</span><span class="sxs-lookup"><span data-stu-id="a1912-126">Retrieve a list of entities</span></span>

<span data-ttu-id="a1912-127">A recuperação de uma lista de entidades é semelhante à recuperação de uma única entidade, exceto por várias outras opções de configuração da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1912-127">Retrieving a list of entities is similar to retrieving a single entity except there a number of other options for configuring the request.</span></span> <span data-ttu-id="a1912-128">O `$filter` parâmetro de consulta pode ser usado para reduzir o conjunto de resultados apenas às linhas que correspondem à condição fornecida.</span><span class="sxs-lookup"><span data-stu-id="a1912-128">The `$filter` query parameter can be used to reduce the result set to only those rows that match the provided condition.</span></span>  <span data-ttu-id="a1912-129">O `$orderBy` parâmetro de consulta solicitará que o servidor forneça a lista de entidades classificadas pelas propriedades especificadas.</span><span class="sxs-lookup"><span data-stu-id="a1912-129">The `$orderBy` query parameter will request that the server provide the list of entities sorted by the specified properties.</span></span>

# <a name="c"></a>[<span data-ttu-id="a1912-130">C#</span><span class="sxs-lookup"><span data-stu-id="a1912-130">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-list.md)]

# <a name="typescript"></a>[<span data-ttu-id="a1912-131">TypeScript</span><span class="sxs-lookup"><span data-stu-id="a1912-131">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-list.md)]

# <a name="java"></a>[<span data-ttu-id="a1912-132">Java</span><span class="sxs-lookup"><span data-stu-id="a1912-132">Java</span></span>](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-list.md)]

# <a name="powershell"></a>[<span data-ttu-id="a1912-133">PowerShell</span><span class="sxs-lookup"><span data-stu-id="a1912-133">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-list.md)]

---

<span data-ttu-id="a1912-134">O objeto retornado ao recuperar uma lista de entidades provavelmente será uma coleção paginável.</span><span class="sxs-lookup"><span data-stu-id="a1912-134">The object returned when retrieving a list of entities is likely to be a paged collection.</span></span> <span data-ttu-id="a1912-135">Para obter detalhes sobre como obter a lista completa de entidades, consulte [paginação por meio de uma coleção](../paging.md).</span><span class="sxs-lookup"><span data-stu-id="a1912-135">For details about how to get the complete list of entities, see [paging through a collection](../paging.md).</span></span>

## <a name="access-an-item-of-a-collection"></a><span data-ttu-id="a1912-136">Acessar um item de uma coleção</span><span class="sxs-lookup"><span data-stu-id="a1912-136">Access an item of a collection</span></span>

<span data-ttu-id="a1912-137">Para SDKs que oferecem suporte a um estilo fluente, as coleções de entidades podem ser acessadas usando um índice de matriz.</span><span class="sxs-lookup"><span data-stu-id="a1912-137">For SDKs that support a fluent style, collections of entities can be accessed using an array index.</span></span> <span data-ttu-id="a1912-138">Para SDKs baseados em modelo, é suficiente incorporar o identificador de item no segmento de caminho após a coleção.</span><span class="sxs-lookup"><span data-stu-id="a1912-138">For template-based SDKs, it is sufficient to embed the item identifier in the path segment following the collection.</span></span> <span data-ttu-id="a1912-139">Para o PowerShell, os identificadores são passados como parâmetros.</span><span class="sxs-lookup"><span data-stu-id="a1912-139">For PowerShell, identifiers are passed as parameters.</span></span>

# <a name="c"></a>[<span data-ttu-id="a1912-140">C#</span><span class="sxs-lookup"><span data-stu-id="a1912-140">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-index.md)]

# <a name="typescript"></a>[<span data-ttu-id="a1912-141">TypeScript</span><span class="sxs-lookup"><span data-stu-id="a1912-141">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-index.md)]

# <a name="java"></a>[<span data-ttu-id="a1912-142">Java</span><span class="sxs-lookup"><span data-stu-id="a1912-142">Java</span></span>](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-index.md)]

# <a name="powershell"></a>[<span data-ttu-id="a1912-143">PowerShell</span><span class="sxs-lookup"><span data-stu-id="a1912-143">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-index.md)]

---

## <a name="use-expand-to-access-related-entities"></a><span data-ttu-id="a1912-144">Use $expand para acessar entidades relacionadas</span><span class="sxs-lookup"><span data-stu-id="a1912-144">Use $expand to access related entities</span></span>

<span data-ttu-id="a1912-145">Você pode usar o `$expand` filtro para solicitar uma entidade relacionada, ou uma coleção de entidades, ao mesmo que você solicite a entidade principal.</span><span class="sxs-lookup"><span data-stu-id="a1912-145">You can use the `$expand` filter to request a related entity, or collection of entities, at the same that you request the main entity.</span></span>

# <a name="c"></a>[<span data-ttu-id="a1912-146">C#</span><span class="sxs-lookup"><span data-stu-id="a1912-146">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-expand.md)]

# <a name="typescript"></a>[<span data-ttu-id="a1912-147">TypeScript</span><span class="sxs-lookup"><span data-stu-id="a1912-147">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-expand.md)]

# <a name="java"></a>[<span data-ttu-id="a1912-148">Java</span><span class="sxs-lookup"><span data-stu-id="a1912-148">Java</span></span>](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-expand.md)]

# <a name="powershell"></a>[<span data-ttu-id="a1912-149">PowerShell</span><span class="sxs-lookup"><span data-stu-id="a1912-149">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-expand.md)]

---

## <a name="delete-an-entity"></a><span data-ttu-id="a1912-150">Excluir uma entidade</span><span class="sxs-lookup"><span data-stu-id="a1912-150">Delete an entity</span></span>

<span data-ttu-id="a1912-151">As solicitações Delete são criadas da mesma maneira que as solicitações para recuperar uma entidade, mas usam uma `DELETE` solicitação em vez de um `GET` .</span><span class="sxs-lookup"><span data-stu-id="a1912-151">Delete requests are constructed in the same way as requests to retrieve an entity, but use a `DELETE` request instead of a `GET`.</span></span>

# <a name="c"></a>[<span data-ttu-id="a1912-152">C#</span><span class="sxs-lookup"><span data-stu-id="a1912-152">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-delete.md)]

# <a name="typescript"></a>[<span data-ttu-id="a1912-153">TypeScript</span><span class="sxs-lookup"><span data-stu-id="a1912-153">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-delete.md)]

# <a name="java"></a>[<span data-ttu-id="a1912-154">Java</span><span class="sxs-lookup"><span data-stu-id="a1912-154">Java</span></span>](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-delete.md)]

# <a name="powershell"></a>[<span data-ttu-id="a1912-155">PowerShell</span><span class="sxs-lookup"><span data-stu-id="a1912-155">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-delete.md)]

---

## <a name="make-a-post-request-to-create-a-new-entity"></a><span data-ttu-id="a1912-156">Fazer uma solicitação POST para criar uma nova entidade</span><span class="sxs-lookup"><span data-stu-id="a1912-156">Make a POST request to create a new entity</span></span>

<span data-ttu-id="a1912-157">Para SDKs que oferecem suporte a um estilo fluente, novos itens podem ser adicionados às coleções com um `Add` método.</span><span class="sxs-lookup"><span data-stu-id="a1912-157">For SDKs that support a fluent style, new items can be added to collections with an `Add` method.</span></span> <span data-ttu-id="a1912-158">Para SDKs baseados em modelo, o objeto Request expõe um `post` método.</span><span class="sxs-lookup"><span data-stu-id="a1912-158">For template-based SDKs, the request object exposes a `post` method.</span></span> <span data-ttu-id="a1912-159">Para o PowerShell, um `New-*` comando disponível que aceita parâmetros que mapeiam a entidade a ser adicionada.</span><span class="sxs-lookup"><span data-stu-id="a1912-159">For PowerShell, a `New-*` command is available that accepts parameters that map to the entity to add.</span></span> <span data-ttu-id="a1912-160">A entidade criada é normalmente retornada da chamada.</span><span class="sxs-lookup"><span data-stu-id="a1912-160">The created entity is usually returned from the call.</span></span>

# <a name="c"></a>[<span data-ttu-id="a1912-161">C#</span><span class="sxs-lookup"><span data-stu-id="a1912-161">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-create.md)]

# <a name="typescript"></a>[<span data-ttu-id="a1912-162">TypeScript</span><span class="sxs-lookup"><span data-stu-id="a1912-162">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-create.md)]

# <a name="java"></a>[<span data-ttu-id="a1912-163">Java</span><span class="sxs-lookup"><span data-stu-id="a1912-163">Java</span></span>](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-create.md)]

# <a name="powershell"></a>[<span data-ttu-id="a1912-164">PowerShell</span><span class="sxs-lookup"><span data-stu-id="a1912-164">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-create.md)]

---

## <a name="updating-an-existing-entity-with-patch"></a><span data-ttu-id="a1912-165">Atualizando uma entidade existente com PATCH</span><span class="sxs-lookup"><span data-stu-id="a1912-165">Updating an existing entity with PATCH</span></span>

<span data-ttu-id="a1912-166">A maioria das atualizações no Microsoft Graph é realizada usando um `PATCH` método e, portanto, só é necessário incluir as propriedades que você deseja alterar no objeto aprovado.</span><span class="sxs-lookup"><span data-stu-id="a1912-166">Most updates in Microsoft Graph are performed using a `PATCH` method and therefore it is only necessary to include the properties that you want to change in the object you pass.</span></span>

# <a name="c"></a>[<span data-ttu-id="a1912-167">C#</span><span class="sxs-lookup"><span data-stu-id="a1912-167">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-update.md)]

# <a name="typescript"></a>[<span data-ttu-id="a1912-168">TypeScript</span><span class="sxs-lookup"><span data-stu-id="a1912-168">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-update.md)]

# <a name="java"></a>[<span data-ttu-id="a1912-169">Java</span><span class="sxs-lookup"><span data-stu-id="a1912-169">Java</span></span>](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-update.md)]

# <a name="powershell"></a>[<span data-ttu-id="a1912-170">PowerShell</span><span class="sxs-lookup"><span data-stu-id="a1912-170">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-update.md)]

---

## <a name="use-http-headers-to-control-request-behavior"></a><span data-ttu-id="a1912-171">Usar cabeçalhos HTTP para controlar o comportamento da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1912-171">Use HTTP headers to control request behavior</span></span>

<span data-ttu-id="a1912-172">Você pode usar uma `Header()` função para anexar cabeçalhos personalizados a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1912-172">You can use a `Header()` function to attach custom headers to a request.</span></span> <span data-ttu-id="a1912-173">Para o PowerShell, a adição de cabeçalhos só é possível com o `Invoke-GraphRequest` método.</span><span class="sxs-lookup"><span data-stu-id="a1912-173">For PowerShell, adding headers is only possible with the `Invoke-GraphRequest` method.</span></span> <span data-ttu-id="a1912-174">Vários cenários do Microsoft Graph usam cabeçalhos personalizados para ajustar o comportamento da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1912-174">A number of Microsoft Graph scenarios use custom headers to adjust the behavior of the request.</span></span>

# <a name="c"></a>[<span data-ttu-id="a1912-175">C#</span><span class="sxs-lookup"><span data-stu-id="a1912-175">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-headers.md)]

# <a name="typescript"></a>[<span data-ttu-id="a1912-176">TypeScript</span><span class="sxs-lookup"><span data-stu-id="a1912-176">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-headers.md)]

# <a name="java"></a>[<span data-ttu-id="a1912-177">Java</span><span class="sxs-lookup"><span data-stu-id="a1912-177">Java</span></span>](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-headers.md)]

# <a name="powershell"></a>[<span data-ttu-id="a1912-178">PowerShell</span><span class="sxs-lookup"><span data-stu-id="a1912-178">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-headers.md)]

---

## <a name="provide-custom-query-parameters"></a><span data-ttu-id="a1912-179">Fornecer parâmetros de consulta personalizados</span><span class="sxs-lookup"><span data-stu-id="a1912-179">Provide custom query parameters</span></span>

<span data-ttu-id="a1912-180">Para SDKs que oferecem suporte a um estilo fluente, você pode fornecer valores de parâmetro de consulta personalizados usando uma lista de `QueryOptions` objetos.</span><span class="sxs-lookup"><span data-stu-id="a1912-180">For SDKs that support a fluent style, you can provide custom query parameter values by using a list of `QueryOptions` objects.</span></span> <span data-ttu-id="a1912-181">Para SDKs baseados em modelo, os parâmetros são codificados por URL e adicionados à URI de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1912-181">For template-based SDKs, the parameters are URL-encoded and added to the request URI.</span></span> <span data-ttu-id="a1912-182">Para o PowerShell, os parâmetros de consulta definidos para uma determinada API são expostos como parâmetros para o comando correspondente.</span><span class="sxs-lookup"><span data-stu-id="a1912-182">For PowerShell, defined query parameters for a given API are exposed as parameters to the corresponding command.</span></span>

# <a name="c"></a>[<span data-ttu-id="a1912-183">C#</span><span class="sxs-lookup"><span data-stu-id="a1912-183">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-queryparams.md)]

# <a name="typescript"></a>[<span data-ttu-id="a1912-184">TypeScript</span><span class="sxs-lookup"><span data-stu-id="a1912-184">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-queryparams.md)]

# <a name="java"></a>[<span data-ttu-id="a1912-185">Java</span><span class="sxs-lookup"><span data-stu-id="a1912-185">Java</span></span>](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-queryparams.md)]

# <a name="powershell"></a>[<span data-ttu-id="a1912-186">PowerShell</span><span class="sxs-lookup"><span data-stu-id="a1912-186">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-queryparams.md)]

---
