---
title: tipo de recurso searchRequest
description: A solicitação de pesquisa a ser enviada para o ponto de extremidade da consulta. Ele contém o tipo de entidades esperadas na resposta, as fontes subjacentes, os parâmetros de paginação, a solicitação de campos e a consulta de pesquisa real.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: fe3117eae0e514bea979281220da12820574cb4a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520896"
---
# <a name="searchrequest-resource-type"></a><span data-ttu-id="150dc-104">tipo de recurso searchRequest</span><span class="sxs-lookup"><span data-stu-id="150dc-104">searchRequest resource type</span></span>

<span data-ttu-id="150dc-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="150dc-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="150dc-106">A solicitação de pesquisa a ser enviada para o ponto de extremidade da consulta.</span><span class="sxs-lookup"><span data-stu-id="150dc-106">The search request to be sent to the query endpoint.</span></span> <span data-ttu-id="150dc-107">Ele contém o tipo de entidades esperadas na resposta, as fontes subjacentes, os parâmetros de paginação, a solicitação de campos e a consulta de pesquisa real.</span><span class="sxs-lookup"><span data-stu-id="150dc-107">It contains the type of entities expected in the response, the underlying sources, the paging parameters, the fields request and the actual search query.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="150dc-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="150dc-108">Properties</span></span>

| <span data-ttu-id="150dc-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="150dc-109">Property</span></span>     | <span data-ttu-id="150dc-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="150dc-110">Type</span></span>        | <span data-ttu-id="150dc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="150dc-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="150dc-112">stored_fields</span><span class="sxs-lookup"><span data-stu-id="150dc-112">stored_fields</span></span>|<span data-ttu-id="150dc-113">String collection</span><span class="sxs-lookup"><span data-stu-id="150dc-113">String collection</span></span> |<span data-ttu-id="150dc-114">Contém os campos a serem retornados para earch _so objeto urces.</span><span class="sxs-lookup"><span data-stu-id="150dc-114">Contains the fields to be returned for earch _so urces object.</span></span> <span data-ttu-id="150dc-115">Observação isso só é aplicável quando entityType =`externalItem` é especificado na resposta.</span><span class="sxs-lookup"><span data-stu-id="150dc-115">Note this is only applicable when entityType=`externalItem` is specified in the response.</span></span>|
|<span data-ttu-id="150dc-116">contentSources</span><span class="sxs-lookup"><span data-stu-id="150dc-116">contentSources</span></span>|<span data-ttu-id="150dc-117">String collection</span><span class="sxs-lookup"><span data-stu-id="150dc-117">String collection</span></span>|<span data-ttu-id="150dc-118">Contém a conexão a ser direcionada.</span><span class="sxs-lookup"><span data-stu-id="150dc-118">Contains the connection to be targeted.</span></span> <br><span data-ttu-id="150dc-119">Respeite o seguinte formato: `/external/connections/connectionid` onde `connectionid` é a ConnectionID definida na administração de conectores</span><span class="sxs-lookup"><span data-stu-id="150dc-119">Respect the following format : `/external/connections/connectionid` where `connectionid` is the ConnectionId been defined in the Connectors Administration</span></span> <br> <span data-ttu-id="150dc-120">Observação contentSource só é aplicável quando entityType =`externalItem`.</span><span class="sxs-lookup"><span data-stu-id="150dc-120">Note contentSource is only applicable when entityType=`externalItem`.</span></span> |
|<span data-ttu-id="150dc-121">enableTopResults</span><span class="sxs-lookup"><span data-stu-id="150dc-121">enableTopResults</span></span>|<span data-ttu-id="150dc-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="150dc-122">Boolean</span></span>|<span data-ttu-id="150dc-123">Isso dispara a classificação híbrida para mensagens: as primeiras 3 mensagens são as mais relevantes</span><span class="sxs-lookup"><span data-stu-id="150dc-123">This triggers hybrid sort for messages : the first 3 messages are the most relevant</span></span><br> <span data-ttu-id="150dc-124">Isso só se aplica a entityType =`message`.</span><span class="sxs-lookup"><span data-stu-id="150dc-124">This is only applicable for entityType=`message`.</span></span>|
|<span data-ttu-id="150dc-125">entityTypes</span><span class="sxs-lookup"><span data-stu-id="150dc-125">entityTypes</span></span>|<span data-ttu-id="150dc-126">coleção `entityType`</span><span class="sxs-lookup"><span data-stu-id="150dc-126">`entityType` collection</span></span>| <span data-ttu-id="150dc-127">Os valores possíveis são: `event`, `message`, `driveItem`, `externalFile`, `externalItem`.</span><span class="sxs-lookup"><span data-stu-id="150dc-127">Possible values are: `event`, `message`, `driveItem`, `externalFile`, `externalItem`.</span></span>|
|<span data-ttu-id="150dc-128">from</span><span class="sxs-lookup"><span data-stu-id="150dc-128">from</span></span>|<span data-ttu-id="150dc-129">Int32</span><span class="sxs-lookup"><span data-stu-id="150dc-129">Int32</span></span>|<span data-ttu-id="150dc-130">Especifica o deslocamento dos resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="150dc-130">Specifies the offset for the search results.</span></span> <span data-ttu-id="150dc-131">Offset 0 retorna o primeiro resultado.</span><span class="sxs-lookup"><span data-stu-id="150dc-131">Offset 0 returns the very first result.</span></span>|
|<span data-ttu-id="150dc-132">consulta</span><span class="sxs-lookup"><span data-stu-id="150dc-132">query</span></span>|[<span data-ttu-id="150dc-133">searchQuery</span><span class="sxs-lookup"><span data-stu-id="150dc-133">searchQuery</span></span>](searchquery.md)|<span data-ttu-id="150dc-134">Contém os termos da consulta.</span><span class="sxs-lookup"><span data-stu-id="150dc-134">Contains the query terms.</span></span>|
|<span data-ttu-id="150dc-135">size</span><span class="sxs-lookup"><span data-stu-id="150dc-135">size</span></span>|<span data-ttu-id="150dc-136">Int32</span><span class="sxs-lookup"><span data-stu-id="150dc-136">Int32</span></span>|<span data-ttu-id="150dc-137">O tamanho da página a ser recuperada.</span><span class="sxs-lookup"><span data-stu-id="150dc-137">The size of the page to be retrieved.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="150dc-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="150dc-138">JSON representation</span></span>

<span data-ttu-id="150dc-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="150dc-139">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchRequest",
  "baseType": null
}-->

```json
{
  "stored_fields": ["String"],
  "contentSources": ["String"],
  "entityTypes": ["String"],
  "query": {"@odata.type": "microsoft.graph.searchQuery"},
  "from": 1024,
  "size": 1024,
  "enableTopResults": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
