---
title: tipo de recurso dimensionValues
description: Um valor de dimensão no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: da3935b8e784b05551af123c1832d5dc84a2c81c
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365315"
---
# <a name="dimensionvalues-resource-type"></a><span data-ttu-id="2b5d5-103">tipo de recurso dimensionValues</span><span class="sxs-lookup"><span data-stu-id="2b5d5-103">dimensionValues resource type</span></span>
<span data-ttu-id="2b5d5-104">Representa um valor de dimensão no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="2b5d5-104">Represents a dimension value in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="2b5d5-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="2b5d5-105">Methods</span></span>

| <span data-ttu-id="2b5d5-106">Método</span><span class="sxs-lookup"><span data-stu-id="2b5d5-106">Method</span></span>       | <span data-ttu-id="2b5d5-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2b5d5-107">Return Type</span></span>  |<span data-ttu-id="2b5d5-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b5d5-108">Description</span></span>                   |
|:-------------|:-------------|:-----------------------------|
|[<span data-ttu-id="2b5d5-109">Obter dimensionValues</span><span class="sxs-lookup"><span data-stu-id="2b5d5-109">Get dimensionValues</span></span>](../api/dynamics-dimensionvalue-get.md)|<span data-ttu-id="2b5d5-110">dimensionValues</span><span class="sxs-lookup"><span data-stu-id="2b5d5-110">dimensionValues</span></span>|<span data-ttu-id="2b5d5-111">Obtém um objeto de valor de dimensão.</span><span class="sxs-lookup"><span data-stu-id="2b5d5-111">Gets a dimension value object.</span></span>|


## <a name="properties"></a><span data-ttu-id="2b5d5-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2b5d5-112">Properties</span></span>
| <span data-ttu-id="2b5d5-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2b5d5-113">Property</span></span>           | <span data-ttu-id="2b5d5-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b5d5-114">Type</span></span>                  |<span data-ttu-id="2b5d5-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b5d5-115">Description</span></span>                                        |
|:-------------------|:----------------------|:--------------------------------------------------|
|<span data-ttu-id="2b5d5-116">id</span><span class="sxs-lookup"><span data-stu-id="2b5d5-116">id</span></span>                  |<span data-ttu-id="2b5d5-117">GUID</span><span class="sxs-lookup"><span data-stu-id="2b5d5-117">GUID</span></span>                   |<span data-ttu-id="2b5d5-118">A ID exclusiva do item.</span><span class="sxs-lookup"><span data-stu-id="2b5d5-118">The unique ID of the item.</span></span>                         |
|<span data-ttu-id="2b5d5-119">código</span><span class="sxs-lookup"><span data-stu-id="2b5d5-119">code</span></span>                |<span data-ttu-id="2b5d5-120">Cadeia de caracteres, tamanho máximo 20</span><span class="sxs-lookup"><span data-stu-id="2b5d5-120">string, maximum size 20</span></span>|<span data-ttu-id="2b5d5-121">O código do valor da dimensão.</span><span class="sxs-lookup"><span data-stu-id="2b5d5-121">The dimension value code.</span></span>                          |
|<span data-ttu-id="2b5d5-122">displayName</span><span class="sxs-lookup"><span data-stu-id="2b5d5-122">displayName</span></span>         |<span data-ttu-id="2b5d5-123">string</span><span class="sxs-lookup"><span data-stu-id="2b5d5-123">string</span></span>                 |<span data-ttu-id="2b5d5-124">Especifica o nome do valor da dimensão.</span><span class="sxs-lookup"><span data-stu-id="2b5d5-124">Specifies the dimension value's name.</span></span> <span data-ttu-id="2b5d5-125">Esse nome aparecerá onde o valor de dimensão é usado.</span><span class="sxs-lookup"><span data-stu-id="2b5d5-125">This name will appear where the dimension value is used.</span></span>|
|<span data-ttu-id="2b5d5-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2b5d5-126">lastModifiedDateTime</span></span>|<span data-ttu-id="2b5d5-127">DateTime</span><span class="sxs-lookup"><span data-stu-id="2b5d5-127">datetime</span></span>               |<span data-ttu-id="2b5d5-128">A última data/hora em que o valor de dimensão foi modificado.</span><span class="sxs-lookup"><span data-stu-id="2b5d5-128">The last datetime the dimension value was modified.</span></span>|  


## <a name="json-representation"></a><span data-ttu-id="2b5d5-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2b5d5-129">JSON representation</span></span>

<span data-ttu-id="2b5d5-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2b5d5-130">Here is a JSON representation of the resource.</span></span>


```json
{

    "id": "GUID",
    "code": "string",
    "displayName": "string",
    "lastModifiedDateTime": "datetime"
}
```


