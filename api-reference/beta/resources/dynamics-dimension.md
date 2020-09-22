---
title: tipo de recurso de dimensões
description: Uma dimensão no Dynamics 365 Business central.
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 61666cdaf87e095707e90345128b5ad2cda47426
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071351"
---
# <a name="dimensions-resource-type"></a><span data-ttu-id="8e92f-103">Tipo de recurso de dimensões</span><span class="sxs-lookup"><span data-stu-id="8e92f-103">Dimensions resource type</span></span>

<span data-ttu-id="8e92f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e92f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e92f-105">Representa uma dimensão no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="8e92f-105">Represents a dimension in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="8e92f-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="8e92f-106">Methods</span></span>
| <span data-ttu-id="8e92f-107">Método</span><span class="sxs-lookup"><span data-stu-id="8e92f-107">Method</span></span>       | <span data-ttu-id="8e92f-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8e92f-108">Return Type</span></span>  |<span data-ttu-id="8e92f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e92f-109">Description</span></span>|
|:-------------|:-------------|:----------|
|[<span data-ttu-id="8e92f-110">Obter dimensões</span><span class="sxs-lookup"><span data-stu-id="8e92f-110">Get dimensions</span></span>](../api/dynamics-dimension-get.md)|<span data-ttu-id="8e92f-111">expressão</span><span class="sxs-lookup"><span data-stu-id="8e92f-111">dimension</span></span>|<span data-ttu-id="8e92f-112">Obtém uma dimensão.</span><span class="sxs-lookup"><span data-stu-id="8e92f-112">Gets a dimension.</span></span>|


## <a name="properties"></a><span data-ttu-id="8e92f-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8e92f-113">Properties</span></span>
| <span data-ttu-id="8e92f-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e92f-114">Property</span></span>           | <span data-ttu-id="8e92f-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e92f-115">Type</span></span>                  |<span data-ttu-id="8e92f-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e92f-116">Description</span></span>               |
|:-------------------|:----------------------|:-------------------------|
|<span data-ttu-id="8e92f-117">id</span><span class="sxs-lookup"><span data-stu-id="8e92f-117">id</span></span>                  |<span data-ttu-id="8e92f-118">GUID</span><span class="sxs-lookup"><span data-stu-id="8e92f-118">GUID</span></span>                   |<span data-ttu-id="8e92f-119">A ID exclusiva do item.</span><span class="sxs-lookup"><span data-stu-id="8e92f-119">The unique ID of the item.</span></span>|
|<span data-ttu-id="8e92f-120">código</span><span class="sxs-lookup"><span data-stu-id="8e92f-120">code</span></span>                |<span data-ttu-id="8e92f-121">Cadeia de caracteres, tamanho máximo 20</span><span class="sxs-lookup"><span data-stu-id="8e92f-121">string, maximum size 20</span></span>|<span data-ttu-id="8e92f-122">O código de dimensão.</span><span class="sxs-lookup"><span data-stu-id="8e92f-122">The dimension code.</span></span>       |
|<span data-ttu-id="8e92f-123">displayName</span><span class="sxs-lookup"><span data-stu-id="8e92f-123">displayName</span></span>         |<span data-ttu-id="8e92f-124">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e92f-124">string</span></span>                 |<span data-ttu-id="8e92f-125">Especifica o nome da dimensão.</span><span class="sxs-lookup"><span data-stu-id="8e92f-125">Specifies the dimension's name.</span></span> <span data-ttu-id="8e92f-126">Esse nome aparecerá onde a dimensão é usada.</span><span class="sxs-lookup"><span data-stu-id="8e92f-126">This name will appear where the dimension is used.</span></span>|
|<span data-ttu-id="8e92f-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8e92f-127">lastModifiedDateTime</span></span>|<span data-ttu-id="8e92f-128">datetime</span><span class="sxs-lookup"><span data-stu-id="8e92f-128">datetime</span></span>               |<span data-ttu-id="8e92f-129">O último DateTime que a dimensão foi modificada.</span><span class="sxs-lookup"><span data-stu-id="8e92f-129">The last datetime the dimension was modified.</span></span>|  


## <a name="json-representation"></a><span data-ttu-id="8e92f-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8e92f-130">JSON representation</span></span>

<span data-ttu-id="8e92f-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8e92f-131">Here is a JSON representation of the resource.</span></span>


```json
{

    "id": "GUID",
    "code": "string",
    "displayName": "string",
    "lastModifiedDateTime": "datetime"
}
```



