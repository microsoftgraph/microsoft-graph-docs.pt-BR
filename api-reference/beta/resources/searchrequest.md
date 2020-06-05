---
title: tipo de recurso searchRequest
description: A solicitação de pesquisa a ser enviada para o ponto de extremidade da consulta. Ele contém o tipo de entidades esperadas na resposta, as fontes subjacentes, os parâmetros de paginação, a solicitação de campos e a consulta de pesquisa real.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 457009dc48fba07b7d66662aa1504395f5d906ef
ms.sourcegitcommit: 093d89c7583bb6880c8395e9498a1f33cdd938b4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44568800"
---
# <a name="searchrequest-resource-type"></a><span data-ttu-id="b96d8-104">tipo de recurso searchRequest</span><span class="sxs-lookup"><span data-stu-id="b96d8-104">searchRequest resource type</span></span>

<span data-ttu-id="b96d8-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b96d8-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b96d8-106">A solicitação de pesquisa a ser enviada para o ponto de extremidade da consulta.</span><span class="sxs-lookup"><span data-stu-id="b96d8-106">The search request to be sent to the query endpoint.</span></span> <span data-ttu-id="b96d8-107">Ele contém o tipo de entidades esperadas na resposta, as fontes subjacentes, os parâmetros de paginação, a solicitação de campos e a consulta de pesquisa real.</span><span class="sxs-lookup"><span data-stu-id="b96d8-107">It contains the type of entities expected in the response, the underlying sources, the paging parameters, the fields request and the actual search query.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="b96d8-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b96d8-108">Properties</span></span>

| <span data-ttu-id="b96d8-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b96d8-109">Property</span></span>     | <span data-ttu-id="b96d8-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b96d8-110">Type</span></span>        | <span data-ttu-id="b96d8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b96d8-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b96d8-112">stored_fields</span><span class="sxs-lookup"><span data-stu-id="b96d8-112">stored_fields</span></span>|<span data-ttu-id="b96d8-113">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b96d8-113">String collection</span></span> |<span data-ttu-id="b96d8-114">Contém os campos a serem retornados para earch _so objeto urces.</span><span class="sxs-lookup"><span data-stu-id="b96d8-114">Contains the fields to be returned for earch _so urces object.</span></span> <span data-ttu-id="b96d8-115">Observação isso só é aplicável quando entityType = `externalItem` é especificado na resposta.</span><span class="sxs-lookup"><span data-stu-id="b96d8-115">Note this is only applicable when entityType=`externalItem` is specified in the response.</span></span>|
|<span data-ttu-id="b96d8-116">contentSources</span><span class="sxs-lookup"><span data-stu-id="b96d8-116">contentSources</span></span>|<span data-ttu-id="b96d8-117">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b96d8-117">String collection</span></span>|<span data-ttu-id="b96d8-118">Contém a conexão a ser direcionada.</span><span class="sxs-lookup"><span data-stu-id="b96d8-118">Contains the connection to be targeted.</span></span> <br><span data-ttu-id="b96d8-119">Respeite o seguinte formato: `/external/connections/connectionid` onde `connectionid` é a ConnectionID definida na administração de conectores</span><span class="sxs-lookup"><span data-stu-id="b96d8-119">Respect the following format : `/external/connections/connectionid` where `connectionid` is the ConnectionId been defined in the Connectors Administration</span></span> <br> <span data-ttu-id="b96d8-120">Observação contentSource só é aplicável quando entityType = `externalItem` .</span><span class="sxs-lookup"><span data-stu-id="b96d8-120">Note contentSource is only applicable when entityType=`externalItem`.</span></span> |
|<span data-ttu-id="b96d8-121">enableTopResults</span><span class="sxs-lookup"><span data-stu-id="b96d8-121">enableTopResults</span></span>|<span data-ttu-id="b96d8-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="b96d8-122">Boolean</span></span>|<span data-ttu-id="b96d8-123">Isso dispara a classificação híbrida para mensagens: as primeiras 3 mensagens são as mais relevantes</span><span class="sxs-lookup"><span data-stu-id="b96d8-123">This triggers hybrid sort for messages : the first 3 messages are the most relevant</span></span><br> <span data-ttu-id="b96d8-124">Isso só se aplica a entityType = `message` .</span><span class="sxs-lookup"><span data-stu-id="b96d8-124">This is only applicable for entityType=`message`.</span></span>|
|<span data-ttu-id="b96d8-125">entityTypes</span><span class="sxs-lookup"><span data-stu-id="b96d8-125">entityTypes</span></span>|<span data-ttu-id="b96d8-126">coleção `entityType`</span><span class="sxs-lookup"><span data-stu-id="b96d8-126">`entityType` collection</span></span>| <span data-ttu-id="b96d8-127">Os valores possíveis são: `event`, `message`, `driveItem`, `externalItem`.</span><span class="sxs-lookup"><span data-stu-id="b96d8-127">Possible values are: `event`, `message`, `driveItem`, `externalItem`.</span></span>|
|<span data-ttu-id="b96d8-128">from</span><span class="sxs-lookup"><span data-stu-id="b96d8-128">from</span></span>|<span data-ttu-id="b96d8-129">Int32</span><span class="sxs-lookup"><span data-stu-id="b96d8-129">Int32</span></span>|<span data-ttu-id="b96d8-130">Especifica o deslocamento dos resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="b96d8-130">Specifies the offset for the search results.</span></span> <span data-ttu-id="b96d8-131">Offset 0 retorna o primeiro resultado.</span><span class="sxs-lookup"><span data-stu-id="b96d8-131">Offset 0 returns the very first result.</span></span>|
|<span data-ttu-id="b96d8-132">consulta</span><span class="sxs-lookup"><span data-stu-id="b96d8-132">query</span></span>|[<span data-ttu-id="b96d8-133">searchQuery</span><span class="sxs-lookup"><span data-stu-id="b96d8-133">searchQuery</span></span>](searchquery.md)|<span data-ttu-id="b96d8-134">Contém os termos da consulta.</span><span class="sxs-lookup"><span data-stu-id="b96d8-134">Contains the query terms.</span></span>|
|<span data-ttu-id="b96d8-135">size</span><span class="sxs-lookup"><span data-stu-id="b96d8-135">size</span></span>|<span data-ttu-id="b96d8-136">Int32</span><span class="sxs-lookup"><span data-stu-id="b96d8-136">Int32</span></span>|<span data-ttu-id="b96d8-137">O tamanho da página a ser recuperada.</span><span class="sxs-lookup"><span data-stu-id="b96d8-137">The size of the page to be retrieved.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b96d8-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b96d8-138">JSON representation</span></span>

<span data-ttu-id="b96d8-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b96d8-139">The following is a JSON representation of the resource.</span></span>

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
