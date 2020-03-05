---
title: tipo de recurso dimensionValues
description: Um valor de dimensão no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 368fc28f7bd46d8d5385b6e6041cd82255e0271f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42504136"
---
# <a name="dimensionvalues-resource-type"></a><span data-ttu-id="2c948-103">tipo de recurso dimensionValues</span><span class="sxs-lookup"><span data-stu-id="2c948-103">dimensionValues resource type</span></span>

<span data-ttu-id="2c948-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2c948-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c948-105">Representa um valor de dimensão no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="2c948-105">Represents a dimension value in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="2c948-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="2c948-106">Methods</span></span>

| <span data-ttu-id="2c948-107">Método</span><span class="sxs-lookup"><span data-stu-id="2c948-107">Method</span></span>       | <span data-ttu-id="2c948-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2c948-108">Return Type</span></span>  |<span data-ttu-id="2c948-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c948-109">Description</span></span>                   |
|:-------------|:-------------|:-----------------------------|
|[<span data-ttu-id="2c948-110">Obter dimensionValues</span><span class="sxs-lookup"><span data-stu-id="2c948-110">Get dimensionValues</span></span>](../api/dynamics-dimensionvalue-get.md)|<span data-ttu-id="2c948-111">dimensionValues</span><span class="sxs-lookup"><span data-stu-id="2c948-111">dimensionValues</span></span>|<span data-ttu-id="2c948-112">Obtém um objeto de valor de dimensão.</span><span class="sxs-lookup"><span data-stu-id="2c948-112">Gets a dimension value object.</span></span>|


## <a name="properties"></a><span data-ttu-id="2c948-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2c948-113">Properties</span></span>
| <span data-ttu-id="2c948-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2c948-114">Property</span></span>           | <span data-ttu-id="2c948-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c948-115">Type</span></span>                  |<span data-ttu-id="2c948-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c948-116">Description</span></span>                                        |
|:-------------------|:----------------------|:--------------------------------------------------|
|<span data-ttu-id="2c948-117">id</span><span class="sxs-lookup"><span data-stu-id="2c948-117">id</span></span>                  |<span data-ttu-id="2c948-118">GUID</span><span class="sxs-lookup"><span data-stu-id="2c948-118">GUID</span></span>                   |<span data-ttu-id="2c948-119">A ID exclusiva do item.</span><span class="sxs-lookup"><span data-stu-id="2c948-119">The unique ID of the item.</span></span>                         |
|<span data-ttu-id="2c948-120">código</span><span class="sxs-lookup"><span data-stu-id="2c948-120">code</span></span>                |<span data-ttu-id="2c948-121">Cadeia de caracteres, tamanho máximo 20</span><span class="sxs-lookup"><span data-stu-id="2c948-121">string, maximum size 20</span></span>|<span data-ttu-id="2c948-122">O código do valor da dimensão.</span><span class="sxs-lookup"><span data-stu-id="2c948-122">The dimension value code.</span></span>                          |
|<span data-ttu-id="2c948-123">displayName</span><span class="sxs-lookup"><span data-stu-id="2c948-123">displayName</span></span>         |<span data-ttu-id="2c948-124">string</span><span class="sxs-lookup"><span data-stu-id="2c948-124">string</span></span>                 |<span data-ttu-id="2c948-125">Especifica o nome do valor da dimensão.</span><span class="sxs-lookup"><span data-stu-id="2c948-125">Specifies the dimension value's name.</span></span> <span data-ttu-id="2c948-126">Esse nome aparecerá onde o valor de dimensão é usado.</span><span class="sxs-lookup"><span data-stu-id="2c948-126">This name will appear where the dimension value is used.</span></span>|
|<span data-ttu-id="2c948-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2c948-127">lastModifiedDateTime</span></span>|<span data-ttu-id="2c948-128">datetime</span><span class="sxs-lookup"><span data-stu-id="2c948-128">datetime</span></span>               |<span data-ttu-id="2c948-129">A última data/hora em que o valor de dimensão foi modificado.</span><span class="sxs-lookup"><span data-stu-id="2c948-129">The last datetime the dimension value was modified.</span></span>|  


## <a name="json-representation"></a><span data-ttu-id="2c948-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2c948-130">JSON representation</span></span>

<span data-ttu-id="2c948-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2c948-131">Here is a JSON representation of the resource.</span></span>


```json
{

    "id": "GUID",
    "code": "string",
    "displayName": "string",
    "lastModifiedDateTime": "datetime"
}
```


