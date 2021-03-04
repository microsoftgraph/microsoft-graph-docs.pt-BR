---
title: Tipo de recurso dataSource
description: A entidade dataSource é uma classe base abstrata usada para identificar fontes de conteúdo para Descoberta eDiscovery.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 2f945ba74a5576a35146ee1832f3740b537ed23b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445902"
---
# <a name="datasource-resource-type"></a><span data-ttu-id="17f02-103">Tipo de recurso dataSource</span><span class="sxs-lookup"><span data-stu-id="17f02-103">dataSource resource type</span></span>

<span data-ttu-id="17f02-104">Namespace: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="17f02-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17f02-105">A entidade dataSource é uma classe base abstrata usada para identificar fontes de conteúdo para Descoberta eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="17f02-105">The dataSource entity is an abstract base class used to identify sources of content for eDiscovery.</span></span>

## <a name="methods"></a><span data-ttu-id="17f02-106">Methods</span><span class="sxs-lookup"><span data-stu-id="17f02-106">Methods</span></span>

<span data-ttu-id="17f02-107">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="17f02-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="17f02-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="17f02-108">Properties</span></span>

|<span data-ttu-id="17f02-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="17f02-109">Property</span></span>|<span data-ttu-id="17f02-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="17f02-110">Type</span></span>|<span data-ttu-id="17f02-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="17f02-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17f02-112">createdBy</span><span class="sxs-lookup"><span data-stu-id="17f02-112">createdBy</span></span>|[<span data-ttu-id="17f02-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="17f02-113">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="17f02-114">O usuário que criou **o dataSource**.</span><span class="sxs-lookup"><span data-stu-id="17f02-114">The user who created the **dataSource**.</span></span>|
|<span data-ttu-id="17f02-115">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="17f02-115">createdDateTime</span></span>|<span data-ttu-id="17f02-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17f02-116">DateTimeOffset</span></span>|<span data-ttu-id="17f02-117">A data e a hora **em que dataSource** foi criado.</span><span class="sxs-lookup"><span data-stu-id="17f02-117">The date and time the **dataSource** was created.</span></span>|
|<span data-ttu-id="17f02-118">displayName</span><span class="sxs-lookup"><span data-stu-id="17f02-118">displayName</span></span>|<span data-ttu-id="17f02-119">String</span><span class="sxs-lookup"><span data-stu-id="17f02-119">String</span></span>|<span data-ttu-id="17f02-120">O nome de exibição **do dataSource**.</span><span class="sxs-lookup"><span data-stu-id="17f02-120">The display name of the **dataSource**.</span></span> <span data-ttu-id="17f02-121">Esse será o nome do site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="17f02-121">This will be the name of the SharePoint site.</span></span>|
|<span data-ttu-id="17f02-122">id</span><span class="sxs-lookup"><span data-stu-id="17f02-122">id</span></span>|<span data-ttu-id="17f02-123">String</span><span class="sxs-lookup"><span data-stu-id="17f02-123">String</span></span>| <span data-ttu-id="17f02-124">A ID do **dataSource**.</span><span class="sxs-lookup"><span data-stu-id="17f02-124">The ID of the **dataSource**.</span></span> <span data-ttu-id="17f02-125">Essa não é a ID do site real.</span><span class="sxs-lookup"><span data-stu-id="17f02-125">This is not the ID of the actual site.</span></span>|

## <a name="relationships"></a><span data-ttu-id="17f02-126">Relações</span><span class="sxs-lookup"><span data-stu-id="17f02-126">Relationships</span></span>

<span data-ttu-id="17f02-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="17f02-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="17f02-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="17f02-128">JSON representation</span></span>

<span data-ttu-id="17f02-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="17f02-129">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.dataSource",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.dataSource",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)"
}
```
