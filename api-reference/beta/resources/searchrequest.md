---
title: tipo de recurso searchRequest
description: A solicitação de pesquisa a ser enviada para o ponto de extremidade da consulta. Ele contém o tipo de entidades esperadas na resposta, as fontes subjacentes, os parâmetros de paginação, a solicitação de campos e a consulta de pesquisa real.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: fac759f190f193fb2fe37e769feedc1164fc3f95
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973731"
---
# <a name="searchrequest-resource-type"></a><span data-ttu-id="929f3-104">tipo de recurso searchRequest</span><span class="sxs-lookup"><span data-stu-id="929f3-104">searchRequest resource type</span></span>

<span data-ttu-id="929f3-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="929f3-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="929f3-106">A solicitação de pesquisa a ser enviada para o ponto de extremidade da consulta.</span><span class="sxs-lookup"><span data-stu-id="929f3-106">The search request to be sent to the query endpoint.</span></span> <span data-ttu-id="929f3-107">Ele contém o tipo de entidades esperadas na resposta, as fontes subjacentes, os parâmetros de paginação, a solicitação de campos e a consulta de pesquisa real.</span><span class="sxs-lookup"><span data-stu-id="929f3-107">It contains the type of entities expected in the response, the underlying sources, the paging parameters, the fields request and the actual search query.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="929f3-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="929f3-108">Properties</span></span>

| <span data-ttu-id="929f3-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="929f3-109">Property</span></span>     | <span data-ttu-id="929f3-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="929f3-110">Type</span></span>        | <span data-ttu-id="929f3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="929f3-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="929f3-112">stored_fields</span><span class="sxs-lookup"><span data-stu-id="929f3-112">stored_fields</span></span>|<span data-ttu-id="929f3-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="929f3-113">String collection</span></span> |<span data-ttu-id="929f3-114">Contém os campos a serem retornados para earch _so objeto urces.</span><span class="sxs-lookup"><span data-stu-id="929f3-114">Contains the fields to be returned for earch _so urces object.</span></span> <span data-ttu-id="929f3-115">Observação isso só é aplicável quando entityType = `externalItem` é especificado na resposta.</span><span class="sxs-lookup"><span data-stu-id="929f3-115">Note this is only applicable when entityType=`externalItem` is specified in the response.</span></span>|
|<span data-ttu-id="929f3-116">contentSources</span><span class="sxs-lookup"><span data-stu-id="929f3-116">contentSources</span></span>|<span data-ttu-id="929f3-117">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="929f3-117">String collection</span></span>|<span data-ttu-id="929f3-118">Contém a conexão a ser direcionada.</span><span class="sxs-lookup"><span data-stu-id="929f3-118">Contains the connection to be targeted.</span></span> <br><span data-ttu-id="929f3-119">Respeite o seguinte formato: `/external/connections/connectionid` onde `connectionid` é a ConnectionID definida na administração de conectores</span><span class="sxs-lookup"><span data-stu-id="929f3-119">Respect the following format : `/external/connections/connectionid` where `connectionid` is the ConnectionId been defined in the Connectors Administration</span></span> <br> <span data-ttu-id="929f3-120">Observação contentSource só é aplicável quando entityType = `externalItem` .</span><span class="sxs-lookup"><span data-stu-id="929f3-120">Note contentSource is only applicable when entityType=`externalItem`.</span></span> |
|<span data-ttu-id="929f3-121">enableTopResults</span><span class="sxs-lookup"><span data-stu-id="929f3-121">enableTopResults</span></span>|<span data-ttu-id="929f3-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="929f3-122">Boolean</span></span>|<span data-ttu-id="929f3-123">Isso dispara a classificação híbrida para mensagens: as primeiras 3 mensagens são as mais relevantes</span><span class="sxs-lookup"><span data-stu-id="929f3-123">This triggers hybrid sort for messages : the first 3 messages are the most relevant</span></span><br> <span data-ttu-id="929f3-124">Isso só se aplica a entityType = `message` .</span><span class="sxs-lookup"><span data-stu-id="929f3-124">This is only applicable for entityType=`message`.</span></span>|
|<span data-ttu-id="929f3-125">entityTypes</span><span class="sxs-lookup"><span data-stu-id="929f3-125">entityTypes</span></span>|<span data-ttu-id="929f3-126">coleção `entityType`</span><span class="sxs-lookup"><span data-stu-id="929f3-126">`entityType` collection</span></span>| <span data-ttu-id="929f3-127">Os valores possíveis são: `event`, `message`, `driveItem`, `externalItem`.</span><span class="sxs-lookup"><span data-stu-id="929f3-127">Possible values are: `event`, `message`, `driveItem`, `externalItem`.</span></span>|
|<span data-ttu-id="929f3-128">from</span><span class="sxs-lookup"><span data-stu-id="929f3-128">from</span></span>|<span data-ttu-id="929f3-129">Int32</span><span class="sxs-lookup"><span data-stu-id="929f3-129">Int32</span></span>|<span data-ttu-id="929f3-130">Especifica o deslocamento dos resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="929f3-130">Specifies the offset for the search results.</span></span> <span data-ttu-id="929f3-131">Offset 0 retorna o primeiro resultado.</span><span class="sxs-lookup"><span data-stu-id="929f3-131">Offset 0 returns the very first result.</span></span>|
|<span data-ttu-id="929f3-132">consulta</span><span class="sxs-lookup"><span data-stu-id="929f3-132">query</span></span>|[<span data-ttu-id="929f3-133">searchQuery</span><span class="sxs-lookup"><span data-stu-id="929f3-133">searchQuery</span></span>](searchquery.md)|<span data-ttu-id="929f3-134">Contém os termos da consulta.</span><span class="sxs-lookup"><span data-stu-id="929f3-134">Contains the query terms.</span></span>|
|<span data-ttu-id="929f3-135">size</span><span class="sxs-lookup"><span data-stu-id="929f3-135">size</span></span>|<span data-ttu-id="929f3-136">Int32</span><span class="sxs-lookup"><span data-stu-id="929f3-136">Int32</span></span>|<span data-ttu-id="929f3-137">O tamanho da página a ser recuperada.</span><span class="sxs-lookup"><span data-stu-id="929f3-137">The size of the page to be retrieved.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="929f3-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="929f3-138">JSON representation</span></span>

<span data-ttu-id="929f3-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="929f3-139">The following is a JSON representation of the resource.</span></span>

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


