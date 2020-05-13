---
title: tipo de recurso Print
description: Quando acompanhada por uma assinatura de impressão universal, o recurso de impressão permite o gerenciamento de impressoras e a descoberta de ServiceEndpoints que podem ser usados para gerenciar impressoras e trabalhos de impressão dentro do universal Print.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: b0af3f7443b77920804f5868fe9ecc3f8b4cec41
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "44217084"
---
# <a name="print-resource-type"></a><span data-ttu-id="434e2-103">tipo de recurso Print</span><span class="sxs-lookup"><span data-stu-id="434e2-103">print resource type</span></span>

<span data-ttu-id="434e2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="434e2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="434e2-105">Quando acompanhada por uma assinatura de impressão universal, o recurso de impressão permite o gerenciamento de impressoras e a descoberta de [ServiceEndpoints](printserviceendpoint.md) que podem ser usados para gerenciar impressoras e trabalhos de impressão dentro do universal Print.</span><span class="sxs-lookup"><span data-stu-id="434e2-105">When accompanied by a Universal Print subscription, the Print feature enables management of printers and discovery of [printServiceEndpoints](printserviceendpoint.md) that can be used to manage printers and print jobs within Universal Print.</span></span>

## <a name="methods"></a><span data-ttu-id="434e2-106">Methods</span><span class="sxs-lookup"><span data-stu-id="434e2-106">Methods</span></span>
| <span data-ttu-id="434e2-107">Método</span><span class="sxs-lookup"><span data-stu-id="434e2-107">Method</span></span>       | <span data-ttu-id="434e2-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="434e2-108">Return Type</span></span> | <span data-ttu-id="434e2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="434e2-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="434e2-110">Conectores de lista</span><span class="sxs-lookup"><span data-stu-id="434e2-110">List connectors</span></span>](../api/print-list-connectors.md) | <span data-ttu-id="434e2-111">coleção [Multiconnector](printconnector.md)</span><span class="sxs-lookup"><span data-stu-id="434e2-111">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="434e2-112">Obtenha uma lista de conectores de impressão.</span><span class="sxs-lookup"><span data-stu-id="434e2-112">Get a list of print connectors.</span></span> |
| [<span data-ttu-id="434e2-113">Listar impressoras</span><span class="sxs-lookup"><span data-stu-id="434e2-113">List printers</span></span>](../api/print-list-printers.md) | <span data-ttu-id="434e2-114">coleção de [impressoras](printer.md)</span><span class="sxs-lookup"><span data-stu-id="434e2-114">[printer](printer.md) collection</span></span> | <span data-ttu-id="434e2-115">Obter uma lista de impressoras.</span><span class="sxs-lookup"><span data-stu-id="434e2-115">Get a list of printers.</span></span> |
| [<span data-ttu-id="434e2-116">Lista de compartilhamentos</span><span class="sxs-lookup"><span data-stu-id="434e2-116">List shares</span></span>](../api/print-list-shares.md) | <span data-ttu-id="434e2-117">coleção [printerShare](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="434e2-117">[printerShare](printershare.md) collection</span></span> | <span data-ttu-id="434e2-118">Obter uma lista de compartilhamentos de impressora.</span><span class="sxs-lookup"><span data-stu-id="434e2-118">Get a list of printer shares.</span></span> |
| [<span data-ttu-id="434e2-119">Listar serviços</span><span class="sxs-lookup"><span data-stu-id="434e2-119">List services</span></span>](../api/print-list-services.md) | <span data-ttu-id="434e2-120">coleção de [serviços de multiserviço](printservice.md)</span><span class="sxs-lookup"><span data-stu-id="434e2-120">[printService](printservice.md) collection</span></span> | <span data-ttu-id="434e2-121">Obtenha uma lista de serviços.</span><span class="sxs-lookup"><span data-stu-id="434e2-121">Get a list of services.</span></span> |
| [<span data-ttu-id="434e2-122">Criar printerShare</span><span class="sxs-lookup"><span data-stu-id="434e2-122">Create printerShare</span></span>](../api/print-post-shares.md) | [<span data-ttu-id="434e2-123">printerShare</span><span class="sxs-lookup"><span data-stu-id="434e2-123">printerShare</span></span>](printershare.md) | <span data-ttu-id="434e2-124">Crie um novo compartilhamento de impressora postando na coleção de **compartilhamentos** .</span><span class="sxs-lookup"><span data-stu-id="434e2-124">Create a new printer share by posting to the **shares** collection.</span></span> |
| [<span data-ttu-id="434e2-125">Atualizar configurações</span><span class="sxs-lookup"><span data-stu-id="434e2-125">Update settings</span></span>](../api/print-update-settings.md) |  [<span data-ttu-id="434e2-126">printSettings</span><span class="sxs-lookup"><span data-stu-id="434e2-126">printSettings</span></span>](printsettings.md) | <span data-ttu-id="434e2-127">Atualiza as configurações de todos os locatários para o serviço de impressão universal.</span><span class="sxs-lookup"><span data-stu-id="434e2-127">Updates tenant-wide settings for the Universal Print service.</span></span> |

## <a name="properties"></a><span data-ttu-id="434e2-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="434e2-128">Properties</span></span>
| <span data-ttu-id="434e2-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="434e2-129">Property</span></span>     | <span data-ttu-id="434e2-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="434e2-130">Type</span></span>        | <span data-ttu-id="434e2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="434e2-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="434e2-132">configurações</span><span class="sxs-lookup"><span data-stu-id="434e2-132">settings</span></span>|[<span data-ttu-id="434e2-133">printSettings</span><span class="sxs-lookup"><span data-stu-id="434e2-133">printSettings</span></span>](printsettings.md)|<span data-ttu-id="434e2-134">Configurações de todo o locatário para o serviço de impressão universal.</span><span class="sxs-lookup"><span data-stu-id="434e2-134">Tenant-wide settings for the Universal Print service.</span></span>|

## <a name="relationships"></a><span data-ttu-id="434e2-135">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="434e2-135">Relationships</span></span>
| <span data-ttu-id="434e2-136">Relação</span><span class="sxs-lookup"><span data-stu-id="434e2-136">Relationship</span></span> | <span data-ttu-id="434e2-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="434e2-137">Type</span></span>        | <span data-ttu-id="434e2-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="434e2-138">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="434e2-139">serviço</span><span class="sxs-lookup"><span data-stu-id="434e2-139">services</span></span>|<span data-ttu-id="434e2-140">coleção de [serviços de multiserviço](printservice.md)</span><span class="sxs-lookup"><span data-stu-id="434e2-140">[printService](printservice.md) collection</span></span>|<span data-ttu-id="434e2-141">A lista de pontos de extremidade do serviço de impressão Universal disponível.</span><span class="sxs-lookup"><span data-stu-id="434e2-141">The list of available Universal Print service endpoints.</span></span>|
|<span data-ttu-id="434e2-142">impressoras</span><span class="sxs-lookup"><span data-stu-id="434e2-142">printers</span></span>|<span data-ttu-id="434e2-143">coleção de [impressoras](printer.md)</span><span class="sxs-lookup"><span data-stu-id="434e2-143">[printer](printer.md) collection</span></span>|<span data-ttu-id="434e2-144">A lista de impressoras registradas no locatário.</span><span class="sxs-lookup"><span data-stu-id="434e2-144">The list of printers registered in the tenant.</span></span>|
|<span data-ttu-id="434e2-145">shares</span><span class="sxs-lookup"><span data-stu-id="434e2-145">shares</span></span>|<span data-ttu-id="434e2-146">coleção [printerShare](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="434e2-146">[printerShare](printershare.md) collection</span></span>|<span data-ttu-id="434e2-147">A lista de compartilhamentos de impressora registrados no locatário.</span><span class="sxs-lookup"><span data-stu-id="434e2-147">The list of printer shares registered in the tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="434e2-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="434e2-148">JSON representation</span></span>

<span data-ttu-id="434e2-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="434e2-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.print",
  "keyProperty": "settings"
}-->

```json
{
  "settings": {"@odata.type": "microsoft.graph.printSettings"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "print resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [ 
    "Error: Resource print has documented navigation properties, but we thought it was a complex type!",
    "Resource print has documented navigation properties, but we thought it was a complex type!"
}-->