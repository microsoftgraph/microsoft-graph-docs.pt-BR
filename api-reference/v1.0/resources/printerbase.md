---
title: Tipo de recurso printerBase
description: Representa o tipo base para o compartilhamento de impressora e impressora
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 515c14bb4de7352a8c17cffdacbd7a4c9091fc70
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516820"
---
# <a name="printerbase-resource-type"></a><span data-ttu-id="1b1c3-103">Tipo de recurso printerBase</span><span class="sxs-lookup"><span data-stu-id="1b1c3-103">printerBase resource type</span></span>

<span data-ttu-id="1b1c3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b1c3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="1b1c3-105">Representa um tipo de base para [tipos de](printer.md) entidade printer e [printerShare.](printerShare.md)</span><span class="sxs-lookup"><span data-stu-id="1b1c3-105">Represents a base type for [printer](printer.md) and [printerShare](printerShare.md) entity types.</span></span>

## <a name="properties"></a><span data-ttu-id="1b1c3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1b1c3-106">Properties</span></span>
|<span data-ttu-id="1b1c3-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b1c3-107">Property</span></span>|<span data-ttu-id="1b1c3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b1c3-108">Type</span></span>|<span data-ttu-id="1b1c3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b1c3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b1c3-110">capabilities</span><span class="sxs-lookup"><span data-stu-id="1b1c3-110">capabilities</span></span>|[<span data-ttu-id="1b1c3-111">printerCapabilities</span><span class="sxs-lookup"><span data-stu-id="1b1c3-111">printerCapabilities</span></span>](printercapabilities.md)|<span data-ttu-id="1b1c3-112">Os recursos da impressora/printerShare.</span><span class="sxs-lookup"><span data-stu-id="1b1c3-112">The capabilities of the printer/printerShare.</span></span>|
|<span data-ttu-id="1b1c3-113">defaults</span><span class="sxs-lookup"><span data-stu-id="1b1c3-113">defaults</span></span>|[<span data-ttu-id="1b1c3-114">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="1b1c3-114">printerDefaults</span></span>](printerdefaults.md)|<span data-ttu-id="1b1c3-115">As configurações de impressão padrão de printer/printerShare.</span><span class="sxs-lookup"><span data-stu-id="1b1c3-115">The default print settings of printer/printerShare.</span></span>|
|<span data-ttu-id="1b1c3-116">displayName</span><span class="sxs-lookup"><span data-stu-id="1b1c3-116">displayName</span></span>|<span data-ttu-id="1b1c3-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b1c3-117">String</span></span>|<span data-ttu-id="1b1c3-118">O nome da impressora/printerShare.</span><span class="sxs-lookup"><span data-stu-id="1b1c3-118">The name of the printer/printerShare.</span></span>|
|<span data-ttu-id="1b1c3-119">id</span><span class="sxs-lookup"><span data-stu-id="1b1c3-119">id</span></span>|<span data-ttu-id="1b1c3-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b1c3-120">String</span></span>|<span data-ttu-id="1b1c3-121">O identificador.</span><span class="sxs-lookup"><span data-stu-id="1b1c3-121">The identifier.</span></span>|
|<span data-ttu-id="1b1c3-122">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="1b1c3-122">isAcceptingJobs</span></span>|<span data-ttu-id="1b1c3-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="1b1c3-123">Boolean</span></span>|<span data-ttu-id="1b1c3-124">Se a impressora/printerShare está aceitando novos trabalhos de impressão no momento.</span><span class="sxs-lookup"><span data-stu-id="1b1c3-124">Whether the printer/printerShare is currently accepting new print jobs.</span></span>|
|<span data-ttu-id="1b1c3-125">location</span><span class="sxs-lookup"><span data-stu-id="1b1c3-125">location</span></span>|[<span data-ttu-id="1b1c3-126">printerLocation</span><span class="sxs-lookup"><span data-stu-id="1b1c3-126">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="1b1c3-127">O local físico e/ou organizacional da impressora/printerShare.</span><span class="sxs-lookup"><span data-stu-id="1b1c3-127">The physical and/or organizational location of the printer/printerShare.</span></span>|
|<span data-ttu-id="1b1c3-128">fabricante</span><span class="sxs-lookup"><span data-stu-id="1b1c3-128">manufacturer</span></span>|<span data-ttu-id="1b1c3-129">String</span><span class="sxs-lookup"><span data-stu-id="1b1c3-129">String</span></span>|<span data-ttu-id="1b1c3-130">O fabricante da impressora/printerShare.</span><span class="sxs-lookup"><span data-stu-id="1b1c3-130">The manufacturer of the printer/printerShare.</span></span>|
|<span data-ttu-id="1b1c3-131">modelo</span><span class="sxs-lookup"><span data-stu-id="1b1c3-131">model</span></span>|<span data-ttu-id="1b1c3-132">String</span><span class="sxs-lookup"><span data-stu-id="1b1c3-132">String</span></span>|<span data-ttu-id="1b1c3-133">O nome do modelo da impressora/printerShare.</span><span class="sxs-lookup"><span data-stu-id="1b1c3-133">The model name of the printer/printerShare.</span></span>|
|<span data-ttu-id="1b1c3-134">status</span><span class="sxs-lookup"><span data-stu-id="1b1c3-134">status</span></span>|[<span data-ttu-id="1b1c3-135">printerStatus</span><span class="sxs-lookup"><span data-stu-id="1b1c3-135">printerStatus</span></span>](printerstatus.md)|<span data-ttu-id="1b1c3-136">O status de processamento da impressora/printerShare, incluindo quaisquer erros.</span><span class="sxs-lookup"><span data-stu-id="1b1c3-136">The processing status of the printer/printerShare, including any errors.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b1c3-137">Relações</span><span class="sxs-lookup"><span data-stu-id="1b1c3-137">Relationships</span></span>
|<span data-ttu-id="1b1c3-138">Relação</span><span class="sxs-lookup"><span data-stu-id="1b1c3-138">Relationship</span></span>|<span data-ttu-id="1b1c3-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b1c3-139">Type</span></span>|<span data-ttu-id="1b1c3-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b1c3-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b1c3-141">jobs</span><span class="sxs-lookup"><span data-stu-id="1b1c3-141">jobs</span></span>|<span data-ttu-id="1b1c3-142">[Coleção printJob](printjob.md)</span><span class="sxs-lookup"><span data-stu-id="1b1c3-142">[printJob](printjob.md) collection</span></span>|<span data-ttu-id="1b1c3-143">A lista de trabalhos que estão na fila para impressão pela impressora/printerShare.</span><span class="sxs-lookup"><span data-stu-id="1b1c3-143">The list of jobs that are queued for printing by the printer/printerShare.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1b1c3-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1b1c3-144">JSON representation</span></span>
<span data-ttu-id="1b1c3-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1b1c3-145">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printerBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerBase",
  "id": "String (identifier)",
  "displayName": "String",
  "manufacturer": "String",
  "model": "String",
  "isAcceptingJobs": "Boolean",
  "defaults": {
    "@odata.type": "microsoft.graph.printerDefaults"
  },
  "location": {
    "@odata.type": "microsoft.graph.printerLocation"
  },
  "capabilities": {
    "@odata.type": "microsoft.graph.printerCapabilities"
  },
  "status": {
    "@odata.type": "microsoft.graph.printerStatus"
  }
}
```

