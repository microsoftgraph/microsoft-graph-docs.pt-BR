---
title: Limites de API de conector do Microsoft Graph
description: Limites de API de conector do Microsoft Graph
author: mecampos
localization_priority: Priority
doc_type: conceptualPageType
ms.prod: search
ms.openlocfilehash: 6ab757d16a10f2291ad9bac5034e9fe7357a7188
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645672"
---
# <a name="microsoft-graph-connector-api-limits"></a><span data-ttu-id="4f2ab-103">Limites de API de conector do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="4f2ab-103">Microsoft Graph connector API limits</span></span>

<span data-ttu-id="4f2ab-104">Este tópico descreve os limites operacionais e de implementação dos conectores do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4f2ab-104">This topic describes implementation and operational limits for Microsoft Graph connectors.</span></span> <span data-ttu-id="4f2ab-105">Lembre-se desses limites ao criar conectores.</span><span class="sxs-lookup"><span data-stu-id="4f2ab-105">Keep these limits in mind when designing connectors.</span></span>

## <a name="connection-limits"></a><span data-ttu-id="4f2ab-106">Limites de conexão</span><span class="sxs-lookup"><span data-stu-id="4f2ab-106">Connection limits</span></span>

| <span data-ttu-id="4f2ab-107">**Limite**</span><span class="sxs-lookup"><span data-stu-id="4f2ab-107">**Limit**</span></span> | <span data-ttu-id="4f2ab-108">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4f2ab-108">**Description**</span></span> |
| --- | --- |
| <span data-ttu-id="4f2ab-109">**10 conexões**</span><span class="sxs-lookup"><span data-stu-id="4f2ab-109">**10 connections**</span></span> | <span data-ttu-id="4f2ab-110">O número máximo de recursos de [conexão](/graph/api/resources/externalconnection?view=graph-rest-beta&preserve-view=true) por locatário do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="4f2ab-110">The maximum number of [connection](/graph/api/resources/externalconnection?view=graph-rest-beta&preserve-view=true) resources per Microsoft 365 tenant.</span></span> |
| <span data-ttu-id="4f2ab-111">**700.000 itens**</span><span class="sxs-lookup"><span data-stu-id="4f2ab-111">**700,000 items**</span></span> | <span data-ttu-id="4f2ab-112">O número máximo de [itens](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) por conexão.</span><span class="sxs-lookup"><span data-stu-id="4f2ab-112">The maximum number of [items](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) per connection.</span></span> |
| <span data-ttu-id="4f2ab-113">**70 GB**</span><span class="sxs-lookup"><span data-stu-id="4f2ab-113">**70 GB**</span></span> | <span data-ttu-id="4f2ab-114">O tamanho máximo de byte de uma conexão.</span><span class="sxs-lookup"><span data-stu-id="4f2ab-114">The maximum byte size of a connection.</span></span> |

## <a name="schema-limits"></a><span data-ttu-id="4f2ab-115">Limites do esquema</span><span class="sxs-lookup"><span data-stu-id="4f2ab-115">Schema limits</span></span>

| <span data-ttu-id="4f2ab-116">**Limite**</span><span class="sxs-lookup"><span data-stu-id="4f2ab-116">**Limit**</span></span> | <span data-ttu-id="4f2ab-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4f2ab-117">**Description**</span></span> |
| --- | --- |
| <span data-ttu-id="4f2ab-118">**128 propriedades**</span><span class="sxs-lookup"><span data-stu-id="4f2ab-118">**128 properties**</span></span> | <span data-ttu-id="4f2ab-119">O número máximo de propriedades que podem ser definidas em um [esquema](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true), caracterizando o uso dos dados por meio de uma conexão.</span><span class="sxs-lookup"><span data-stu-id="4f2ab-119">The maximum number of properties that can be defined in a [schema](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true), characterizing the data ingested through a connection.</span></span> |

## <a name="group-limits"></a><span data-ttu-id="4f2ab-120">Limites de grupo</span><span class="sxs-lookup"><span data-stu-id="4f2ab-120">Group limits</span></span>

| <span data-ttu-id="4f2ab-121">**Limite**</span><span class="sxs-lookup"><span data-stu-id="4f2ab-121">**Limit**</span></span> | <span data-ttu-id="4f2ab-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4f2ab-122">**Description**</span></span> |
| --- | --- |
| <span data-ttu-id="4f2ab-123">100.000</span><span class="sxs-lookup"><span data-stu-id="4f2ab-123">100,000</span></span> | <span data-ttu-id="4f2ab-124">O número máximo de [grupos externos](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true) por locatário do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="4f2ab-124">The maximum number of [external groups](/graph/api/resources/externalgroup?view=graph-rest-beta&preserve-view=true) per Microsoft 365 tenant.</span></span> |
| <span data-ttu-id="4f2ab-125">**Mil solicitações/seg.**</span><span class="sxs-lookup"><span data-stu-id="4f2ab-125">**1000 requests/sec**</span></span> | <span data-ttu-id="4f2ab-126">O número máximo de solicitações permitidas por segundo na [limitação](#throttling) da administração de grupo.</span><span class="sxs-lookup"><span data-stu-id="4f2ab-126">The maximum number of requests allowed per second in the group administration [throttling](#throttling) threshold.</span></span> |

## <a name="item-ingestion"></a><span data-ttu-id="4f2ab-127">Ingestão de item</span><span class="sxs-lookup"><span data-stu-id="4f2ab-127">Item ingestion</span></span>

| <span data-ttu-id="4f2ab-128">**Limite**</span><span class="sxs-lookup"><span data-stu-id="4f2ab-128">**Limit**</span></span> | <span data-ttu-id="4f2ab-129">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4f2ab-129">**Description**</span></span> |
| --- | --- |
| <span data-ttu-id="4f2ab-130">**4 itens/seg (250 MB/hora)**</span><span class="sxs-lookup"><span data-stu-id="4f2ab-130">**4 items/sec (250 MB/hour)**</span></span> | <span data-ttu-id="4f2ab-131">O limite de produtividade para ingerir itens por meio de uma conexão.</span><span class="sxs-lookup"><span data-stu-id="4f2ab-131">The throughput limit to ingest items through a connection.</span></span> |
| <span data-ttu-id="4f2ab-132">**4 MB**</span><span class="sxs-lookup"><span data-stu-id="4f2ab-132">**4 MB**</span></span> | <span data-ttu-id="4f2ab-133">O tamanho máximo de um item; esse limite se aplica ao corpo da solicitação quando [como ingerir e indexar um item](/graph/api/externalconnection-put-items?view=graph-rest-beta&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="4f2ab-133">The maximum size of an item; this limit applies to the request body when [ingesting and indexing an item](/graph/api/externalconnection-put-items?view=graph-rest-beta&preserve-view=true).</span></span> |
| <span data-ttu-id="4f2ab-134">**N/D**</span><span class="sxs-lookup"><span data-stu-id="4f2ab-134">**N/A**</span></span> | <span data-ttu-id="4f2ab-135">O tamanho máximo de uma propriedade.</span><span class="sxs-lookup"><span data-stu-id="4f2ab-135">The maximum size of a property.</span></span> |

## <a name="throttling"></a><span data-ttu-id="4f2ab-136">Limitação</span><span class="sxs-lookup"><span data-stu-id="4f2ab-136">Throttling</span></span>

<span data-ttu-id="4f2ab-p102">Quando a restrição do [limite](throttling.md) for excedida, o Microsoft Graph limita quaisquer outras solicitações desse cliente por um período. Quando a limitação acontece, o Microsoft Graph retorna o código de status HTTP 429 (solicitações demais) e as solicitações falham. Um tempo de espera sugerido é retornado no cabeçalho da resposta da solicitação com falha. O comportamento de limitação pode depender do tipo e do número de solicitações. Por exemplo, se você tiver um grande volume de solicitações, todos os tipos de solicitação são limitados. Os limites de controle variam com base no tipo de solicitação. Portanto, você pode encontrar um cenário onde as gravações são limitadas, mas leituras ainda são permitidas.</span><span class="sxs-lookup"><span data-stu-id="4f2ab-p102">When a [throttling](throttling.md) threshold is exceeded, Microsoft Graph limits any further requests from that client for a period of time. When throttling occurs, Microsoft Graph returns HTTP status code 429 (Too many requests), and the requests fail. A suggested wait time is returned in the response header of the failed request. Throttling behavior can depend on the type and number of requests. For example, if you have a high volume of requests, all requests types are throttled. Threshold limits vary based on the request type. Therefore, you could encounter a scenario where writes are throttled but reads are still permitted.</span></span>
