---
title: tipo de recurso de dimensões
description: Uma dimensão no Dynamics 365 Business central.
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 92ba48a7ad55b6a7dff28ccc1547769c149e378b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543085"
---
# <a name="dimensions-resource-type"></a><span data-ttu-id="c954a-103">Tipo de recurso de dimensões</span><span class="sxs-lookup"><span data-stu-id="c954a-103">Dimensions resource type</span></span>
<span data-ttu-id="c954a-104">Representa uma dimensão no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="c954a-104">Represents a dimension in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="c954a-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="c954a-105">Methods</span></span>
| <span data-ttu-id="c954a-106">Método</span><span class="sxs-lookup"><span data-stu-id="c954a-106">Method</span></span>       | <span data-ttu-id="c954a-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c954a-107">Return Type</span></span>  |<span data-ttu-id="c954a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c954a-108">Description</span></span>|
|:-------------|:-------------|:----------|
|[<span data-ttu-id="c954a-109">Obter dimensões</span><span class="sxs-lookup"><span data-stu-id="c954a-109">Get dimensions</span></span>](../api/dynamics-dimension-get.md)|<span data-ttu-id="c954a-110">expressão</span><span class="sxs-lookup"><span data-stu-id="c954a-110">dimension</span></span>|<span data-ttu-id="c954a-111">Obtém uma dimensão.</span><span class="sxs-lookup"><span data-stu-id="c954a-111">Gets a dimension.</span></span>|


## <a name="properties"></a><span data-ttu-id="c954a-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c954a-112">Properties</span></span>
| <span data-ttu-id="c954a-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c954a-113">Property</span></span>           | <span data-ttu-id="c954a-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="c954a-114">Type</span></span>                  |<span data-ttu-id="c954a-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="c954a-115">Description</span></span>               |
|:-------------------|:----------------------|:-------------------------|
|<span data-ttu-id="c954a-116">id</span><span class="sxs-lookup"><span data-stu-id="c954a-116">id</span></span>                  |<span data-ttu-id="c954a-117">GUID</span><span class="sxs-lookup"><span data-stu-id="c954a-117">GUID</span></span>                   |<span data-ttu-id="c954a-118">A ID exclusiva do item.</span><span class="sxs-lookup"><span data-stu-id="c954a-118">The unique ID of the item.</span></span>|
|<span data-ttu-id="c954a-119">código</span><span class="sxs-lookup"><span data-stu-id="c954a-119">code</span></span>                |<span data-ttu-id="c954a-120">Cadeia de caracteres, tamanho máximo 20</span><span class="sxs-lookup"><span data-stu-id="c954a-120">string, maximum size 20</span></span>|<span data-ttu-id="c954a-121">O código de dimensão.</span><span class="sxs-lookup"><span data-stu-id="c954a-121">The dimension code.</span></span>       |
|<span data-ttu-id="c954a-122">displayName</span><span class="sxs-lookup"><span data-stu-id="c954a-122">displayName</span></span>         |<span data-ttu-id="c954a-123">string</span><span class="sxs-lookup"><span data-stu-id="c954a-123">string</span></span>                 |<span data-ttu-id="c954a-124">Especifica o nome da dimensão.</span><span class="sxs-lookup"><span data-stu-id="c954a-124">Specifies the dimension's name.</span></span> <span data-ttu-id="c954a-125">Esse nome aparecerá onde a dimensão é usada.</span><span class="sxs-lookup"><span data-stu-id="c954a-125">This name will appear where the dimension is used.</span></span>|
|<span data-ttu-id="c954a-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c954a-126">lastModifiedDateTime</span></span>|<span data-ttu-id="c954a-127">DateTime</span><span class="sxs-lookup"><span data-stu-id="c954a-127">datetime</span></span>               |<span data-ttu-id="c954a-128">O último DateTime que a dimensão foi modificada.</span><span class="sxs-lookup"><span data-stu-id="c954a-128">The last datetime the dimension was modified.</span></span>|  


## <a name="json-representation"></a><span data-ttu-id="c954a-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c954a-129">JSON representation</span></span>

<span data-ttu-id="c954a-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c954a-130">Here is a JSON representation of the resource.</span></span>


```json
{

    "id": "GUID",
    "code": "string",
    "displayName": "string",
    "lastModifiedDateTime": "datetime"
}
```

