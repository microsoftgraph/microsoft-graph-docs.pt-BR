---
title: tipo de recurso Print
description: Quando acompanhada por uma assinatura de impressão universal, o recurso de impressão permite o gerenciamento de impressoras e a descoberta de ServiceEndpoints que podem ser usados para gerenciar impressoras e trabalhos de impressão dentro do universal Print.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 551fa42736d6fa275a8f998274a6fccf55ac00b7
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006972"
---
# <a name="print-resource-type"></a><span data-ttu-id="9f421-103">tipo de recurso Print</span><span class="sxs-lookup"><span data-stu-id="9f421-103">print resource type</span></span>

<span data-ttu-id="9f421-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f421-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f421-105">Quando acompanhada por uma assinatura de impressão universal, o recurso de impressão permite o gerenciamento de impressoras e a descoberta de [ServiceEndpoints](printserviceendpoint.md) que podem ser usados para gerenciar impressoras e trabalhos de impressão dentro do universal Print.</span><span class="sxs-lookup"><span data-stu-id="9f421-105">When accompanied by a Universal Print subscription, the Print feature enables management of printers and discovery of [printServiceEndpoints](printserviceendpoint.md) that can be used to manage printers and print jobs within Universal Print.</span></span>

## <a name="methods"></a><span data-ttu-id="9f421-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="9f421-106">Methods</span></span>
| <span data-ttu-id="9f421-107">Método</span><span class="sxs-lookup"><span data-stu-id="9f421-107">Method</span></span>       | <span data-ttu-id="9f421-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9f421-108">Return Type</span></span> | <span data-ttu-id="9f421-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f421-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9f421-110">Conectores de lista</span><span class="sxs-lookup"><span data-stu-id="9f421-110">List connectors</span></span>](../api/print-list-connectors.md) | <span data-ttu-id="9f421-111">coleção [Multiconnector](printconnector.md)</span><span class="sxs-lookup"><span data-stu-id="9f421-111">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="9f421-112">Obtenha uma lista de conectores de impressão.</span><span class="sxs-lookup"><span data-stu-id="9f421-112">Get a list of print connectors.</span></span> |
| [<span data-ttu-id="9f421-113">Listar impressoras</span><span class="sxs-lookup"><span data-stu-id="9f421-113">List printers</span></span>](../api/print-list-printers.md) | <span data-ttu-id="9f421-114">coleção de [impressoras](printer.md)</span><span class="sxs-lookup"><span data-stu-id="9f421-114">[printer](printer.md) collection</span></span> | <span data-ttu-id="9f421-115">Obter uma lista de impressoras.</span><span class="sxs-lookup"><span data-stu-id="9f421-115">Get a list of printers.</span></span> |
| [<span data-ttu-id="9f421-116">Lista de compartilhamentos</span><span class="sxs-lookup"><span data-stu-id="9f421-116">List shares</span></span>](../api/print-list-shares.md) | <span data-ttu-id="9f421-117">coleção [printerShare](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="9f421-117">[printerShare](printershare.md) collection</span></span> | <span data-ttu-id="9f421-118">Obter uma lista de compartilhamentos de impressora.</span><span class="sxs-lookup"><span data-stu-id="9f421-118">Get a list of printer shares.</span></span> |
| [<span data-ttu-id="9f421-119">Listar serviços</span><span class="sxs-lookup"><span data-stu-id="9f421-119">List services</span></span>](../api/print-list-services.md) | <span data-ttu-id="9f421-120">coleção de [serviços de multiserviço](printservice.md)</span><span class="sxs-lookup"><span data-stu-id="9f421-120">[printService](printservice.md) collection</span></span> | <span data-ttu-id="9f421-121">Obtenha uma lista de serviços.</span><span class="sxs-lookup"><span data-stu-id="9f421-121">Get a list of services.</span></span> |
| [<span data-ttu-id="9f421-122">Criar printerShare</span><span class="sxs-lookup"><span data-stu-id="9f421-122">Create printerShare</span></span>](../api/print-post-shares.md) | [<span data-ttu-id="9f421-123">printerShare</span><span class="sxs-lookup"><span data-stu-id="9f421-123">printerShare</span></span>](printershare.md) | <span data-ttu-id="9f421-124">Crie um novo compartilhamento de impressora postando na coleção de **compartilhamentos** .</span><span class="sxs-lookup"><span data-stu-id="9f421-124">Create a new printer share by posting to the **shares** collection.</span></span> |
| [<span data-ttu-id="9f421-125">Criar impressora</span><span class="sxs-lookup"><span data-stu-id="9f421-125">Create printer</span></span>](../api/printer-create.md) | [<span data-ttu-id="9f421-126">printerCreateOperation</span><span class="sxs-lookup"><span data-stu-id="9f421-126">printerCreateOperation</span></span>](printerCreateOperation.md) | <span data-ttu-id="9f421-127">Criar (registrar) uma nova impressora com impressão universal.</span><span class="sxs-lookup"><span data-stu-id="9f421-127">Create (register) a new printer with Universal Print.</span></span> |
| [<span data-ttu-id="9f421-128">Atualizar configurações</span><span class="sxs-lookup"><span data-stu-id="9f421-128">Update settings</span></span>](../api/print-update-settings.md) |  [<span data-ttu-id="9f421-129">printSettings</span><span class="sxs-lookup"><span data-stu-id="9f421-129">printSettings</span></span>](printsettings.md) | <span data-ttu-id="9f421-130">Atualiza as configurações de todos os locatários para o serviço de impressão universal.</span><span class="sxs-lookup"><span data-stu-id="9f421-130">Updates tenant-wide settings for the Universal Print service.</span></span> |

## <a name="properties"></a><span data-ttu-id="9f421-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9f421-131">Properties</span></span>
| <span data-ttu-id="9f421-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9f421-132">Property</span></span>     | <span data-ttu-id="9f421-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f421-133">Type</span></span>        | <span data-ttu-id="9f421-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f421-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9f421-135">configurações</span><span class="sxs-lookup"><span data-stu-id="9f421-135">settings</span></span>|[<span data-ttu-id="9f421-136">printSettings</span><span class="sxs-lookup"><span data-stu-id="9f421-136">printSettings</span></span>](printsettings.md)|<span data-ttu-id="9f421-137">Configurações de todo o locatário para o serviço de impressão universal.</span><span class="sxs-lookup"><span data-stu-id="9f421-137">Tenant-wide settings for the Universal Print service.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f421-138">Relações</span><span class="sxs-lookup"><span data-stu-id="9f421-138">Relationships</span></span>
| <span data-ttu-id="9f421-139">Relação</span><span class="sxs-lookup"><span data-stu-id="9f421-139">Relationship</span></span> | <span data-ttu-id="9f421-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f421-140">Type</span></span>        | <span data-ttu-id="9f421-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f421-141">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9f421-142">serviço</span><span class="sxs-lookup"><span data-stu-id="9f421-142">services</span></span>|<span data-ttu-id="9f421-143">coleção de [serviços de multiserviço](printservice.md)</span><span class="sxs-lookup"><span data-stu-id="9f421-143">[printService](printservice.md) collection</span></span>|<span data-ttu-id="9f421-144">A lista de pontos de extremidade do serviço de impressão Universal disponível.</span><span class="sxs-lookup"><span data-stu-id="9f421-144">The list of available Universal Print service endpoints.</span></span>|
|<span data-ttu-id="9f421-145">impressoras</span><span class="sxs-lookup"><span data-stu-id="9f421-145">printers</span></span>|<span data-ttu-id="9f421-146">coleção de [impressoras](printer.md)</span><span class="sxs-lookup"><span data-stu-id="9f421-146">[printer](printer.md) collection</span></span>|<span data-ttu-id="9f421-147">A lista de impressoras registradas no locatário.</span><span class="sxs-lookup"><span data-stu-id="9f421-147">The list of printers registered in the tenant.</span></span>|
|<span data-ttu-id="9f421-148">shares</span><span class="sxs-lookup"><span data-stu-id="9f421-148">shares</span></span>|<span data-ttu-id="9f421-149">coleção [printerShare](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="9f421-149">[printerShare](printershare.md) collection</span></span>|<span data-ttu-id="9f421-150">A lista de compartilhamentos de impressora registrados no locatário.</span><span class="sxs-lookup"><span data-stu-id="9f421-150">The list of printer shares registered in the tenant.</span></span>|
|<span data-ttu-id="9f421-151">conectores</span><span class="sxs-lookup"><span data-stu-id="9f421-151">connectors</span></span>|<span data-ttu-id="9f421-152">coleção [Multiconnector](printconnector.md)</span><span class="sxs-lookup"><span data-stu-id="9f421-152">[printConnector](printconnector.md) collection</span></span>|<span data-ttu-id="9f421-153">A lista de conectores de impressão disponíveis.</span><span class="sxs-lookup"><span data-stu-id="9f421-153">The list of available print connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9f421-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9f421-154">JSON representation</span></span>

<span data-ttu-id="9f421-155">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9f421-155">The following is a JSON representation of the resource.</span></span>

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
