---
title: tipo de recurso de dimensões
description: Uma dimensão no Dynamics 365 Business central.
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: ed7c7a389778e651af8d2c11c53277a27e022ce1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42504535"
---
# <a name="dimensions-resource-type"></a><span data-ttu-id="74f19-103">Tipo de recurso de dimensões</span><span class="sxs-lookup"><span data-stu-id="74f19-103">Dimensions resource type</span></span>

<span data-ttu-id="74f19-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="74f19-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74f19-105">Representa uma dimensão no Dynamics 365 Business central.</span><span class="sxs-lookup"><span data-stu-id="74f19-105">Represents a dimension in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="74f19-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="74f19-106">Methods</span></span>
| <span data-ttu-id="74f19-107">Método</span><span class="sxs-lookup"><span data-stu-id="74f19-107">Method</span></span>       | <span data-ttu-id="74f19-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="74f19-108">Return Type</span></span>  |<span data-ttu-id="74f19-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="74f19-109">Description</span></span>|
|:-------------|:-------------|:----------|
|[<span data-ttu-id="74f19-110">Obter dimensões</span><span class="sxs-lookup"><span data-stu-id="74f19-110">Get dimensions</span></span>](../api/dynamics-dimension-get.md)|<span data-ttu-id="74f19-111">expressão</span><span class="sxs-lookup"><span data-stu-id="74f19-111">dimension</span></span>|<span data-ttu-id="74f19-112">Obtém uma dimensão.</span><span class="sxs-lookup"><span data-stu-id="74f19-112">Gets a dimension.</span></span>|


## <a name="properties"></a><span data-ttu-id="74f19-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="74f19-113">Properties</span></span>
| <span data-ttu-id="74f19-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="74f19-114">Property</span></span>           | <span data-ttu-id="74f19-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="74f19-115">Type</span></span>                  |<span data-ttu-id="74f19-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="74f19-116">Description</span></span>               |
|:-------------------|:----------------------|:-------------------------|
|<span data-ttu-id="74f19-117">id</span><span class="sxs-lookup"><span data-stu-id="74f19-117">id</span></span>                  |<span data-ttu-id="74f19-118">GUID</span><span class="sxs-lookup"><span data-stu-id="74f19-118">GUID</span></span>                   |<span data-ttu-id="74f19-119">A ID exclusiva do item.</span><span class="sxs-lookup"><span data-stu-id="74f19-119">The unique ID of the item.</span></span>|
|<span data-ttu-id="74f19-120">código</span><span class="sxs-lookup"><span data-stu-id="74f19-120">code</span></span>                |<span data-ttu-id="74f19-121">Cadeia de caracteres, tamanho máximo 20</span><span class="sxs-lookup"><span data-stu-id="74f19-121">string, maximum size 20</span></span>|<span data-ttu-id="74f19-122">O código de dimensão.</span><span class="sxs-lookup"><span data-stu-id="74f19-122">The dimension code.</span></span>       |
|<span data-ttu-id="74f19-123">displayName</span><span class="sxs-lookup"><span data-stu-id="74f19-123">displayName</span></span>         |<span data-ttu-id="74f19-124">string</span><span class="sxs-lookup"><span data-stu-id="74f19-124">string</span></span>                 |<span data-ttu-id="74f19-125">Especifica o nome da dimensão.</span><span class="sxs-lookup"><span data-stu-id="74f19-125">Specifies the dimension's name.</span></span> <span data-ttu-id="74f19-126">Esse nome aparecerá onde a dimensão é usada.</span><span class="sxs-lookup"><span data-stu-id="74f19-126">This name will appear where the dimension is used.</span></span>|
|<span data-ttu-id="74f19-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="74f19-127">lastModifiedDateTime</span></span>|<span data-ttu-id="74f19-128">datetime</span><span class="sxs-lookup"><span data-stu-id="74f19-128">datetime</span></span>               |<span data-ttu-id="74f19-129">O último DateTime que a dimensão foi modificada.</span><span class="sxs-lookup"><span data-stu-id="74f19-129">The last datetime the dimension was modified.</span></span>|  


## <a name="json-representation"></a><span data-ttu-id="74f19-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="74f19-130">JSON representation</span></span>

<span data-ttu-id="74f19-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="74f19-131">Here is a JSON representation of the resource.</span></span>


```json
{

    "id": "GUID",
    "code": "string",
    "displayName": "string",
    "lastModifiedDateTime": "datetime"
}
```

