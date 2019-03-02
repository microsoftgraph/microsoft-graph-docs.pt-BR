---
title: tipo de recurso de dimensões
description: Uma dimensão no Dynamics 365 Business central.
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 92ba48a7ad55b6a7dff28ccc1547769c149e378b
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365567"
---
# <a name="dimensions-resource-type"></a><span data-ttu-id="f6de1-103">Tipo de recurso de dimensões</span><span class="sxs-lookup"><span data-stu-id="f6de1-103">Dimensions resource type</span></span>
<span data-ttu-id="f6de1-104">Representa uma dimensão no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="f6de1-104">Represents a dimension in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="f6de1-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="f6de1-105">Methods</span></span>
| <span data-ttu-id="f6de1-106">Método</span><span class="sxs-lookup"><span data-stu-id="f6de1-106">Method</span></span>       | <span data-ttu-id="f6de1-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f6de1-107">Return Type</span></span>  |<span data-ttu-id="f6de1-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6de1-108">Description</span></span>|
|:-------------|:-------------|:----------|
|[<span data-ttu-id="f6de1-109">Obter dimensões</span><span class="sxs-lookup"><span data-stu-id="f6de1-109">Get dimensions</span></span>](../api/dynamics-dimension-get.md)|<span data-ttu-id="f6de1-110">expressão</span><span class="sxs-lookup"><span data-stu-id="f6de1-110">dimension</span></span>|<span data-ttu-id="f6de1-111">Obtém uma dimensão.</span><span class="sxs-lookup"><span data-stu-id="f6de1-111">Gets a dimension.</span></span>|


## <a name="properties"></a><span data-ttu-id="f6de1-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f6de1-112">Properties</span></span>
| <span data-ttu-id="f6de1-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f6de1-113">Property</span></span>           | <span data-ttu-id="f6de1-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6de1-114">Type</span></span>                  |<span data-ttu-id="f6de1-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6de1-115">Description</span></span>               |
|:-------------------|:----------------------|:-------------------------|
|<span data-ttu-id="f6de1-116">id</span><span class="sxs-lookup"><span data-stu-id="f6de1-116">id</span></span>                  |<span data-ttu-id="f6de1-117">GUID</span><span class="sxs-lookup"><span data-stu-id="f6de1-117">GUID</span></span>                   |<span data-ttu-id="f6de1-118">A ID exclusiva do item.</span><span class="sxs-lookup"><span data-stu-id="f6de1-118">The unique ID of the item.</span></span>|
|<span data-ttu-id="f6de1-119">código</span><span class="sxs-lookup"><span data-stu-id="f6de1-119">code</span></span>                |<span data-ttu-id="f6de1-120">Cadeia de caracteres, tamanho máximo 20</span><span class="sxs-lookup"><span data-stu-id="f6de1-120">string, maximum size 20</span></span>|<span data-ttu-id="f6de1-121">O código de dimensão.</span><span class="sxs-lookup"><span data-stu-id="f6de1-121">The dimension code.</span></span>       |
|<span data-ttu-id="f6de1-122">displayName</span><span class="sxs-lookup"><span data-stu-id="f6de1-122">displayName</span></span>         |<span data-ttu-id="f6de1-123">string</span><span class="sxs-lookup"><span data-stu-id="f6de1-123">string</span></span>                 |<span data-ttu-id="f6de1-124">Especifica o nome da dimensão.</span><span class="sxs-lookup"><span data-stu-id="f6de1-124">Specifies the dimension's name.</span></span> <span data-ttu-id="f6de1-125">Esse nome aparecerá onde a dimensão é usada.</span><span class="sxs-lookup"><span data-stu-id="f6de1-125">This name will appear where the dimension is used.</span></span>|
|<span data-ttu-id="f6de1-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f6de1-126">lastModifiedDateTime</span></span>|<span data-ttu-id="f6de1-127">DateTime</span><span class="sxs-lookup"><span data-stu-id="f6de1-127">datetime</span></span>               |<span data-ttu-id="f6de1-128">O último DateTime que a dimensão foi modificada.</span><span class="sxs-lookup"><span data-stu-id="f6de1-128">The last datetime the dimension was modified.</span></span>|  


## <a name="json-representation"></a><span data-ttu-id="f6de1-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f6de1-129">JSON representation</span></span>

<span data-ttu-id="f6de1-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f6de1-130">Here is a JSON representation of the resource.</span></span>


```json
{

    "id": "GUID",
    "code": "string",
    "displayName": "string",
    "lastModifiedDateTime": "datetime"
}
```

