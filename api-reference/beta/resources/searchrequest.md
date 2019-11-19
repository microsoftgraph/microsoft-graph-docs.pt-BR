---
title: tipo de recurso searchRequest
description: A solicitação de pesquisa a ser enviada para o ponto de extremidade da consulta. Ele contém o tipo de entidades esperadas na resposta, as fontes subjacentes, os parâmetros de paginação, a solicitação de campos e a consulta de pesquisa real.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 7f19b9a14e1f6f4016e53a4a0ff1f62ae27e1cfd
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703753"
---
# <a name="searchrequest-resource-type"></a><span data-ttu-id="dfa29-104">tipo de recurso searchRequest</span><span class="sxs-lookup"><span data-stu-id="dfa29-104">searchRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfa29-105">A solicitação de pesquisa a ser enviada para o ponto de extremidade da consulta.</span><span class="sxs-lookup"><span data-stu-id="dfa29-105">The search request to be sent to the query endpoint.</span></span> <span data-ttu-id="dfa29-106">Ele contém o tipo de entidades esperadas na resposta, as fontes subjacentes, os parâmetros de paginação, a solicitação de campos e a consulta de pesquisa real.</span><span class="sxs-lookup"><span data-stu-id="dfa29-106">It contains the type of entities expected in the response, the underlying sources, the paging parameters, the fields request and the actual search query.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="dfa29-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dfa29-107">Properties</span></span>

| <span data-ttu-id="dfa29-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dfa29-108">Property</span></span>     | <span data-ttu-id="dfa29-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="dfa29-109">Type</span></span>        | <span data-ttu-id="dfa29-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="dfa29-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dfa29-111">stored_fields</span><span class="sxs-lookup"><span data-stu-id="dfa29-111">stored_fields</span></span>|<span data-ttu-id="dfa29-112">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="dfa29-112">String collection</span></span> |<span data-ttu-id="dfa29-113">Contém os campos a serem retornados para earch _so objeto urces.</span><span class="sxs-lookup"><span data-stu-id="dfa29-113">Contains the fields to be returned for earch _so urces object.</span></span> <span data-ttu-id="dfa29-114">Observação isso só é aplicável quando entityType =`externalItem` é especificado na resposta.</span><span class="sxs-lookup"><span data-stu-id="dfa29-114">Note this is only applicable when entityType=`externalItem` is specified in the response.</span></span>|
|<span data-ttu-id="dfa29-115">contentSources</span><span class="sxs-lookup"><span data-stu-id="dfa29-115">contentSources</span></span>|<span data-ttu-id="dfa29-116">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="dfa29-116">String collection</span></span>|<span data-ttu-id="dfa29-117">Contém a conexão a ser direcionada.</span><span class="sxs-lookup"><span data-stu-id="dfa29-117">Contains the connection to be targeted.</span></span> <br><span data-ttu-id="dfa29-118">Respeite o seguinte formato: `/external/connections/connectionid` onde `connectionid` é a ConnectionID definida na administração de conectores</span><span class="sxs-lookup"><span data-stu-id="dfa29-118">Respect the following format : `/external/connections/connectionid` where `connectionid` is the ConnectionId been defined in the Connectors Administration</span></span> <br> <span data-ttu-id="dfa29-119">Observação contentSource só é aplicável quando entityType =`externalItem`.</span><span class="sxs-lookup"><span data-stu-id="dfa29-119">Note contentSource is only applicable when entityType=`externalItem`.</span></span> |
|<span data-ttu-id="dfa29-120">enableTopResults</span><span class="sxs-lookup"><span data-stu-id="dfa29-120">enableTopResults</span></span>|<span data-ttu-id="dfa29-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="dfa29-121">Boolean</span></span>|<span data-ttu-id="dfa29-122">Isso dispara a classificação híbrida para mensagens: as primeiras 3 mensagens são as mais relevantes</span><span class="sxs-lookup"><span data-stu-id="dfa29-122">This triggers hybrid sort for messages : the first 3 messages are the most relevant</span></span><br> <span data-ttu-id="dfa29-123">Isso só se aplica a entityType =`message`.</span><span class="sxs-lookup"><span data-stu-id="dfa29-123">This is only applicable for entityType=`message`.</span></span>|
|<span data-ttu-id="dfa29-124">entityTypes</span><span class="sxs-lookup"><span data-stu-id="dfa29-124">entityTypes</span></span>|<span data-ttu-id="dfa29-125">coleção `entityType`</span><span class="sxs-lookup"><span data-stu-id="dfa29-125">`entityType` collection</span></span>| <span data-ttu-id="dfa29-126">Os valores possíveis são: `event`, `message`, `driveItem`, `externalFile`, `externalItem`.</span><span class="sxs-lookup"><span data-stu-id="dfa29-126">Possible values are: `event`, `message`, `driveItem`, `externalFile`, `externalItem`.</span></span>|
|<span data-ttu-id="dfa29-127">from</span><span class="sxs-lookup"><span data-stu-id="dfa29-127">from</span></span>|<span data-ttu-id="dfa29-128">Int32</span><span class="sxs-lookup"><span data-stu-id="dfa29-128">Int32</span></span>|<span data-ttu-id="dfa29-129">Especifica o deslocamento dos resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="dfa29-129">Specifies the offset for the search results.</span></span> <span data-ttu-id="dfa29-130">Offset 0 retorna o primeiro resultado.</span><span class="sxs-lookup"><span data-stu-id="dfa29-130">Offset 0 returns the very first result.</span></span>|
|<span data-ttu-id="dfa29-131">consulta</span><span class="sxs-lookup"><span data-stu-id="dfa29-131">query</span></span>|[<span data-ttu-id="dfa29-132">searchQuery</span><span class="sxs-lookup"><span data-stu-id="dfa29-132">searchQuery</span></span>](searchquery.md)|<span data-ttu-id="dfa29-133">Contém os termos da consulta.</span><span class="sxs-lookup"><span data-stu-id="dfa29-133">Contains the query terms.</span></span>|
|<span data-ttu-id="dfa29-134">size</span><span class="sxs-lookup"><span data-stu-id="dfa29-134">size</span></span>|<span data-ttu-id="dfa29-135">Int32</span><span class="sxs-lookup"><span data-stu-id="dfa29-135">Int32</span></span>|<span data-ttu-id="dfa29-136">O tamanho da página a ser recuperada.</span><span class="sxs-lookup"><span data-stu-id="dfa29-136">The size of the page to be retrieved.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dfa29-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dfa29-137">JSON representation</span></span>

<span data-ttu-id="dfa29-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dfa29-138">The following is a JSON representation of the resource.</span></span>

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
