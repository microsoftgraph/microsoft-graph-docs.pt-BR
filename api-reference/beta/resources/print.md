---
title: tipo de recurso Print
description: Quando acompanhada por uma assinatura de impressão universal, o recurso de impressão permite o gerenciamento de impressoras e a descoberta de ServiceEndpoints que podem ser usados para gerenciar impressoras e trabalhos de impressão dentro do universal Print.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 3ef5c05be520bb407f17d0af14bbd4355e736c62
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895510"
---
# <a name="print-resource-type"></a><span data-ttu-id="a2a2d-103">tipo de recurso Print</span><span class="sxs-lookup"><span data-stu-id="a2a2d-103">print resource type</span></span>

<span data-ttu-id="a2a2d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2a2d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2a2d-105">Quando acompanhada por uma assinatura de impressão universal, o recurso de impressão permite o gerenciamento de impressoras e a descoberta de [ServiceEndpoints](printserviceendpoint.md) que podem ser usados para gerenciar impressoras e trabalhos de impressão dentro do universal Print.</span><span class="sxs-lookup"><span data-stu-id="a2a2d-105">When accompanied by a Universal Print subscription, the Print feature enables management of printers and discovery of [printServiceEndpoints](printserviceendpoint.md) that can be used to manage printers and print jobs within Universal Print.</span></span>

## <a name="methods"></a><span data-ttu-id="a2a2d-106">Methods</span><span class="sxs-lookup"><span data-stu-id="a2a2d-106">Methods</span></span>
| <span data-ttu-id="a2a2d-107">Método</span><span class="sxs-lookup"><span data-stu-id="a2a2d-107">Method</span></span>       | <span data-ttu-id="a2a2d-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a2a2d-108">Return Type</span></span> | <span data-ttu-id="a2a2d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2a2d-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a2a2d-110">Conectores de lista</span><span class="sxs-lookup"><span data-stu-id="a2a2d-110">List connectors</span></span>](../api/print-list-connectors.md) | <span data-ttu-id="a2a2d-111">coleção [Multiconnector](printconnector.md)</span><span class="sxs-lookup"><span data-stu-id="a2a2d-111">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="a2a2d-112">Obtenha uma lista de conectores de impressão.</span><span class="sxs-lookup"><span data-stu-id="a2a2d-112">Get a list of print connectors.</span></span> |
| [<span data-ttu-id="a2a2d-113">Listar impressoras</span><span class="sxs-lookup"><span data-stu-id="a2a2d-113">List printers</span></span>](../api/print-list-printers.md) | <span data-ttu-id="a2a2d-114">coleção de [impressoras](printer.md)</span><span class="sxs-lookup"><span data-stu-id="a2a2d-114">[printer](printer.md) collection</span></span> | <span data-ttu-id="a2a2d-115">Obter uma lista de impressoras.</span><span class="sxs-lookup"><span data-stu-id="a2a2d-115">Get a list of printers.</span></span> |
| [<span data-ttu-id="a2a2d-116">Listar printerShares</span><span class="sxs-lookup"><span data-stu-id="a2a2d-116">List printerShares</span></span>](../api/print-list-printershares.md) | <span data-ttu-id="a2a2d-117">coleção [printerShare](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="a2a2d-117">[printerShare](printershare.md) collection</span></span> | <span data-ttu-id="a2a2d-118">Obter uma lista de compartilhamentos de impressora.</span><span class="sxs-lookup"><span data-stu-id="a2a2d-118">Get a list of printer shares.</span></span> |
| [<span data-ttu-id="a2a2d-119">Listar serviços</span><span class="sxs-lookup"><span data-stu-id="a2a2d-119">List services</span></span>](../api/print-list-services.md) | <span data-ttu-id="a2a2d-120">coleção de [serviços de multiserviço](printservice.md)</span><span class="sxs-lookup"><span data-stu-id="a2a2d-120">[printService](printservice.md) collection</span></span> | <span data-ttu-id="a2a2d-121">Obtenha uma lista de serviços.</span><span class="sxs-lookup"><span data-stu-id="a2a2d-121">Get a list of services.</span></span> |
| [<span data-ttu-id="a2a2d-122">Criar printerShare</span><span class="sxs-lookup"><span data-stu-id="a2a2d-122">Create printerShare</span></span>](../api/print-post-printershares.md) | [<span data-ttu-id="a2a2d-123">printerShare</span><span class="sxs-lookup"><span data-stu-id="a2a2d-123">printerShare</span></span>](printershare.md) | <span data-ttu-id="a2a2d-124">Crie um novo compartilhamento de impressora postando na coleção **printerShares** .</span><span class="sxs-lookup"><span data-stu-id="a2a2d-124">Create a new printer share by posting to the **printerShares** collection.</span></span> |
| [<span data-ttu-id="a2a2d-125">Atualizar configurações</span><span class="sxs-lookup"><span data-stu-id="a2a2d-125">Update settings</span></span>](../api/print-update-settings.md) |  [<span data-ttu-id="a2a2d-126">printSettings</span><span class="sxs-lookup"><span data-stu-id="a2a2d-126">printSettings</span></span>](printsettings.md) | <span data-ttu-id="a2a2d-127">Atualiza as configurações de todos os locatários para o serviço de impressão universal.</span><span class="sxs-lookup"><span data-stu-id="a2a2d-127">Updates tenant-wide settings for the Universal Print service.</span></span> |

## <a name="properties"></a><span data-ttu-id="a2a2d-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a2a2d-128">Properties</span></span>
| <span data-ttu-id="a2a2d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a2a2d-129">Property</span></span>     | <span data-ttu-id="a2a2d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2a2d-130">Type</span></span>        | <span data-ttu-id="a2a2d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2a2d-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a2a2d-132">configurações</span><span class="sxs-lookup"><span data-stu-id="a2a2d-132">settings</span></span>|[<span data-ttu-id="a2a2d-133">printSettings</span><span class="sxs-lookup"><span data-stu-id="a2a2d-133">printSettings</span></span>](printsettings.md)|<span data-ttu-id="a2a2d-134">Configurações de todo o locatário para o serviço de impressão universal.</span><span class="sxs-lookup"><span data-stu-id="a2a2d-134">Tenant-wide settings for the Universal Print service.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2a2d-135">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="a2a2d-135">Relationships</span></span>
| <span data-ttu-id="a2a2d-136">Relação</span><span class="sxs-lookup"><span data-stu-id="a2a2d-136">Relationship</span></span> | <span data-ttu-id="a2a2d-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2a2d-137">Type</span></span>        | <span data-ttu-id="a2a2d-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2a2d-138">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a2a2d-139">serviço</span><span class="sxs-lookup"><span data-stu-id="a2a2d-139">services</span></span>|<span data-ttu-id="a2a2d-140">coleção de [serviços de multiserviço](printservice.md)</span><span class="sxs-lookup"><span data-stu-id="a2a2d-140">[printService](printservice.md) collection</span></span>|<span data-ttu-id="a2a2d-141">A lista de pontos de extremidade do serviço de impressão Universal disponível.</span><span class="sxs-lookup"><span data-stu-id="a2a2d-141">The list of available Universal Print service endpoints.</span></span>|
|<span data-ttu-id="a2a2d-142">impressoras</span><span class="sxs-lookup"><span data-stu-id="a2a2d-142">printers</span></span>|<span data-ttu-id="a2a2d-143">coleção de [impressoras](printer.md)</span><span class="sxs-lookup"><span data-stu-id="a2a2d-143">[printer](printer.md) collection</span></span>|<span data-ttu-id="a2a2d-144">A lista de impressoras registradas no locatário.</span><span class="sxs-lookup"><span data-stu-id="a2a2d-144">The list of printers registered in the tenant.</span></span>|
|<span data-ttu-id="a2a2d-145">printerShares</span><span class="sxs-lookup"><span data-stu-id="a2a2d-145">printerShares</span></span>|<span data-ttu-id="a2a2d-146">coleção de coleção [printerShare](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="a2a2d-146">[printerShare](printershare.md) collection collection</span></span>|<span data-ttu-id="a2a2d-147">A lista de compartilhamentos de impressora registrados no locatário.</span><span class="sxs-lookup"><span data-stu-id="a2a2d-147">The list of printer shares registered in the tenant.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a2a2d-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a2a2d-148">JSON representation</span></span>

<span data-ttu-id="a2a2d-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a2a2d-149">The following is a JSON representation of the resource.</span></span>

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