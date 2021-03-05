---
title: Práticas recomendadas para trabalhar com a API do OneNote no Microsoft Graph
description: Este artigo fornece recomendações para trabalhar com APIs do OneNote no Microsoft Graph. Essas recomendações se baseiam em respostas a perguntas comuns sobre o Microsoft Q&A e o Twitter.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 8ceb848e4d48954d9a08c8bc9f7b28e2521c9aed
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472801"
---
# <a name="best-practices-for-working-with-the-onenote-api-in-microsoft-graph"></a><span data-ttu-id="35e47-104">Práticas recomendadas para trabalhar com a API do OneNote no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="35e47-104">Best practices for working with the OneNote API in Microsoft Graph</span></span>

<span data-ttu-id="35e47-105">Este artigo fornece recomendações para trabalhar com APIs do OneNote no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="35e47-105">This article provides recommendations for working with the OneNote APIs in Microsoft Graph.</span></span> <span data-ttu-id="35e47-106">Essas recomendações se baseiam em respostas a perguntas comuns sobre [o Microsoft Q&A](https://docs.microsoft.com/answers/topics/microsoft-graph-notes.html)  e o Twitter.</span><span class="sxs-lookup"><span data-stu-id="35e47-106">These recommendations are based on answers to common questions on [Microsoft Q&A](https://docs.microsoft.com/answers/topics/microsoft-graph-notes.html)  and Twitter.</span></span>

## <a name="use-select-to-select-the-minimum-set-of-properties-you-need"></a><span data-ttu-id="35e47-107">Use $select para selecionar o conjunto mínimo de propriedades de que você precisa</span><span class="sxs-lookup"><span data-stu-id="35e47-107">Use $select to select the minimum set of properties you need</span></span>

<span data-ttu-id="35e47-108">Quando você consulta um recurso (por exemplo, seções em um bloco de anotações), faz uma solicitação semelhante à seguinte.</span><span class="sxs-lookup"><span data-stu-id="35e47-108">When you query for a resource (for example, sections inside a notebook), you make a request similar to the following.</span></span>

```http
GET ~/notebooks/{id}/sections
```

<span data-ttu-id="35e47-109">Isso recupera todas as propriedades das seções.</span><span class="sxs-lookup"><span data-stu-id="35e47-109">This retrieves all the properties of the sections.</span></span> <span data-ttu-id="35e47-110">No entanto, você pode não precisar de todas as propriedades.</span><span class="sxs-lookup"><span data-stu-id="35e47-110">However, you might not need all properties.</span></span> <span data-ttu-id="35e47-111">Você pode usar o parâmetro de consulta `$select` para retornar apenas as propriedades desejadas, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="35e47-111">You can use the `$select` query parameter to return just the properties that you want, as shown in the following example.</span></span>

```http
GET ~/notebooks/{id}/sections?$select=id,displayName
```

<span data-ttu-id="35e47-112">A mesma abordagem se aplica a outras APIs do OneNote.</span><span class="sxs-lookup"><span data-stu-id="35e47-112">The same approach applies to other OneNote APIs.</span></span>

## <a name="use-expand-instead-of-making-multiple-api-calls"></a><span data-ttu-id="35e47-113">Use $expand em vez de várias chamadas à API</span><span class="sxs-lookup"><span data-stu-id="35e47-113">Use $expand instead of making multiple API calls</span></span>

<span data-ttu-id="35e47-114">Suponha que você queira recuperar todos os blocos de anotações, seções e grupos de seções do usuário em uma exibição hierárquica.</span><span class="sxs-lookup"><span data-stu-id="35e47-114">Suppose you want to retrieve all of the user’s notebooks, sections, and section groups in a hierarchical view.</span></span> <span data-ttu-id="35e47-115">Você pode fazer isso seguindo este procedimento:</span><span class="sxs-lookup"><span data-stu-id="35e47-115">You might accomplish that by doing the following:</span></span>

* <span data-ttu-id="35e47-116">Chamar `GET ~/notebooks` para obter a lista de blocos de anotações.</span><span class="sxs-lookup"><span data-stu-id="35e47-116">Call `GET ~/notebooks` to get the list of notebooks.</span></span>

* <span data-ttu-id="35e47-117">Para cada bloco de anotações recuperado, chame `GET ~/notebooks/{notebookId}/sections` para recuperar a lista de seções.</span><span class="sxs-lookup"><span data-stu-id="35e47-117">For every retrieved notebook, call `GET ~/notebooks/{notebookId}/sections` to retrieve the list of sections.</span></span>

* <span data-ttu-id="35e47-118">Para cada bloco de anotações recuperado, chame `GET ~/notebooks/{notebookId}/sectionGroups` para recuperar a lista de grupos de seções.</span><span class="sxs-lookup"><span data-stu-id="35e47-118">For every retrieved notebook, call `GET ~/notebooks/{notebookId}/sectionGroups` to retrieve the list of section groups.</span></span>

* <span data-ttu-id="35e47-119">Opcionalmente, iterar de forma repetida em grupos de seções.</span><span class="sxs-lookup"><span data-stu-id="35e47-119">Optionally recursively iterate through section groups.</span></span>

<span data-ttu-id="35e47-120">Embora isso funcione (com algumas viagens de ida e volta sequenciais extra ao serviço), uma abordagem melhor é usar o parâmetro de consulta `$expand`.</span><span class="sxs-lookup"><span data-stu-id="35e47-120">While this will work (with a few extra sequential roundtrips to the service), a better approach is to use the `$expand` query parameter.</span></span> 

```http
GET ~/notebooks?$expand=sections,sectionGroups($expand=sections)
```

<span data-ttu-id="35e47-121">Isso produzirá os mesmos resultados de ida e volta na rede, com melhor desempenho.</span><span class="sxs-lookup"><span data-stu-id="35e47-121">This will yield the same results in one network roundtrip, with better performance.</span></span>

## <a name="when-getting-all-pages-for-a-user-do-so-for-each-section-separately"></a><span data-ttu-id="35e47-122">Ao obter todas as páginas de um usuário, faça isso para cada seção separadamente</span><span class="sxs-lookup"><span data-stu-id="35e47-122">When getting all pages for a user, do so for each section separately</span></span>

<span data-ttu-id="35e47-123">Embora o Microsoft Graph exponha um ponto de extremidade para recuperar todas as páginas, essa não é a melhor maneira de obter todas as páginas às quais o usuário tem acesso.</span><span class="sxs-lookup"><span data-stu-id="35e47-123">While Microsoft Graph exposes an endpoint to retrieve all pages, this isn't the best way to get all the pages the user has access to.</span></span> <span data-ttu-id="35e47-124">Quando o usuário tem muitas seções, isso pode causar tempos limite ou mau desempenho.</span><span class="sxs-lookup"><span data-stu-id="35e47-124">When the user has too many sections, this can lead to timeouts or bad performance.</span></span> <span data-ttu-id="35e47-125">É melhor iterar cada seção, obtendo páginas para cada uma separadamente.</span><span class="sxs-lookup"><span data-stu-id="35e47-125">It is better to iterate each section, getting pages for each one separately.</span></span>

<span data-ttu-id="35e47-126">Por exemplo, em vez de usar essa chamada (essa API é paginada; portanto, você não poderá buscar todas as páginas de uma só vez):</span><span class="sxs-lookup"><span data-stu-id="35e47-126">For example, instead of using this call (this API is paged, so you won't be able to fetch the pages all at once):</span></span>

```http
GET ~/pages
```

<span data-ttu-id="35e47-127">É melhor usar a seguinte chamada várias vezes (especialmente se você não precisar de todas as seções):</span><span class="sxs-lookup"><span data-stu-id="35e47-127">It is better to use the following call several times (especially if you don't need all sections):</span></span>

```http
GET ~/sections/{id}/pages
```

<span data-ttu-id="35e47-128">Ao obter metadados de página, substitua a ordenação padrão `lastModifiedDateTime`.</span><span class="sxs-lookup"><span data-stu-id="35e47-128">When getting page metadata, override the default `lastModifiedDateTime` ordering.</span></span> <span data-ttu-id="35e47-129">É mais rápido acessar páginas quando não é preciso classificá-las por `lastModifiedDateTime`.</span><span class="sxs-lookup"><span data-stu-id="35e47-129">It is faster to get pages when you don't have to sort them by `lastModifiedDateTime`.</span></span> <span data-ttu-id="35e47-130">Para fazer isso, você pode classificar por qualquer outra propriedade; por exemplo:</span><span class="sxs-lookup"><span data-stu-id="35e47-130">To do this, you can sort by any other property; for example:</span></span>

```http
GET ~/sections/{id}/pages?$select=id,title,createdDateTime&$orderby=createdDateTime
```
