---
title: tipo de recurso Print
description: Quando acompanhada por uma assinatura de impressão universal, o recurso de impressão permite o gerenciamento de impressoras e a descoberta de ServiceEndpoints que podem ser usados para gerenciar impressoras e trabalhos de impressão dentro do universal Print.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: b32ebb749b3b13ee1d468de69b0724fe281e6793
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091498"
---
# <a name="print-resource-type"></a><span data-ttu-id="c0f84-103">tipo de recurso Print</span><span class="sxs-lookup"><span data-stu-id="c0f84-103">print resource type</span></span>

<span data-ttu-id="c0f84-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0f84-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c0f84-105">Quando acompanhada por uma assinatura de impressão universal, o recurso de impressão permite o gerenciamento de impressoras e a descoberta de [ServiceEndpoints](printserviceendpoint.md) que podem ser usados para gerenciar impressoras e trabalhos de impressão dentro do universal Print.</span><span class="sxs-lookup"><span data-stu-id="c0f84-105">When accompanied by a Universal Print subscription, the Print feature enables management of printers and discovery of [printServiceEndpoints](printserviceendpoint.md) that can be used to manage printers and print jobs within Universal Print.</span></span>

## <a name="methods"></a><span data-ttu-id="c0f84-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="c0f84-106">Methods</span></span>
| <span data-ttu-id="c0f84-107">Método</span><span class="sxs-lookup"><span data-stu-id="c0f84-107">Method</span></span>       | <span data-ttu-id="c0f84-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c0f84-108">Return Type</span></span> | <span data-ttu-id="c0f84-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0f84-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="c0f84-110">Conectores de lista</span><span class="sxs-lookup"><span data-stu-id="c0f84-110">List connectors</span></span>](../api/print-list-connectors.md) | <span data-ttu-id="c0f84-111">coleção [Multiconnector](printconnector.md)</span><span class="sxs-lookup"><span data-stu-id="c0f84-111">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="c0f84-112">Obtenha uma lista de conectores de impressão.</span><span class="sxs-lookup"><span data-stu-id="c0f84-112">Get a list of print connectors.</span></span> |
| [<span data-ttu-id="c0f84-113">Listar impressoras</span><span class="sxs-lookup"><span data-stu-id="c0f84-113">List printers</span></span>](../api/print-list-printers.md) | <span data-ttu-id="c0f84-114">coleção de [impressoras](printer.md)</span><span class="sxs-lookup"><span data-stu-id="c0f84-114">[printer](printer.md) collection</span></span> | <span data-ttu-id="c0f84-115">Obter uma lista de impressoras.</span><span class="sxs-lookup"><span data-stu-id="c0f84-115">Get a list of printers.</span></span> |
| [<span data-ttu-id="c0f84-116">Lista de compartilhamentos</span><span class="sxs-lookup"><span data-stu-id="c0f84-116">List shares</span></span>](../api/print-list-shares.md) | <span data-ttu-id="c0f84-117">coleção [printerShare](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="c0f84-117">[printerShare](printershare.md) collection</span></span> | <span data-ttu-id="c0f84-118">Obter uma lista de compartilhamentos de impressora.</span><span class="sxs-lookup"><span data-stu-id="c0f84-118">Get a list of printer shares.</span></span> |
| [<span data-ttu-id="c0f84-119">Listar serviços</span><span class="sxs-lookup"><span data-stu-id="c0f84-119">List services</span></span>](../api/print-list-services.md) | <span data-ttu-id="c0f84-120">coleção de [serviços de multiserviço](printservice.md)</span><span class="sxs-lookup"><span data-stu-id="c0f84-120">[printService](printservice.md) collection</span></span> | <span data-ttu-id="c0f84-121">Obtenha uma lista de serviços.</span><span class="sxs-lookup"><span data-stu-id="c0f84-121">Get a list of services.</span></span> |
| [<span data-ttu-id="c0f84-122">Criar printerShare</span><span class="sxs-lookup"><span data-stu-id="c0f84-122">Create printerShare</span></span>](../api/print-post-shares.md) | [<span data-ttu-id="c0f84-123">printerShare</span><span class="sxs-lookup"><span data-stu-id="c0f84-123">printerShare</span></span>](printershare.md) | <span data-ttu-id="c0f84-124">Crie um novo compartilhamento de impressora postando na coleção de **compartilhamentos** .</span><span class="sxs-lookup"><span data-stu-id="c0f84-124">Create a new printer share by posting to the **shares** collection.</span></span> |
| [<span data-ttu-id="c0f84-125">Criar impressora</span><span class="sxs-lookup"><span data-stu-id="c0f84-125">Create printer</span></span>](../api/printer-create.md) | [<span data-ttu-id="c0f84-126">printerCreateOperation</span><span class="sxs-lookup"><span data-stu-id="c0f84-126">printerCreateOperation</span></span>](printerCreateOperation.md) | <span data-ttu-id="c0f84-127">Criar (registrar) uma nova impressora com impressão universal.</span><span class="sxs-lookup"><span data-stu-id="c0f84-127">Create (register) a new printer with Universal Print.</span></span> |
| [<span data-ttu-id="c0f84-128">Atualizar configurações</span><span class="sxs-lookup"><span data-stu-id="c0f84-128">Update settings</span></span>](../api/print-update-settings.md) |  [<span data-ttu-id="c0f84-129">printSettings</span><span class="sxs-lookup"><span data-stu-id="c0f84-129">printSettings</span></span>](printsettings.md) | <span data-ttu-id="c0f84-130">Atualiza as configurações de todos os locatários para o serviço de impressão universal.</span><span class="sxs-lookup"><span data-stu-id="c0f84-130">Updates tenant-wide settings for the Universal Print service.</span></span> |
| [<span data-ttu-id="c0f84-131">Listar taskDefinitions</span><span class="sxs-lookup"><span data-stu-id="c0f84-131">List taskDefinitions</span></span>](../api/print-list-taskdefinitions.md) | <span data-ttu-id="c0f84-132">coleção [printTaskDefinition](printtaskdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c0f84-132">[printTaskDefinition](printtaskdefinition.md) collection</span></span> | <span data-ttu-id="c0f84-133">Obter uma lista de todos os locatários de printTaskDefinitions criados dentro da impressão universal.</span><span class="sxs-lookup"><span data-stu-id="c0f84-133">Get a tenant-wide list of printTaskDefinitions created within Universal Print.</span></span> |
| [<span data-ttu-id="c0f84-134">Criar taskDefinition</span><span class="sxs-lookup"><span data-stu-id="c0f84-134">Create taskDefinition</span></span>](../api/print-post-taskdefinitions.md) | [<span data-ttu-id="c0f84-135">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="c0f84-135">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="c0f84-136">Criar um novo printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="c0f84-136">Create a new printTaskDefinition.</span></span> |
| [<span data-ttu-id="c0f84-137">Atualizar taskDefinition</span><span class="sxs-lookup"><span data-stu-id="c0f84-137">Update taskDefinition</span></span>](../api/print-update-taskdefinition.md) | [<span data-ttu-id="c0f84-138">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="c0f84-138">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="c0f84-139">Atualizar um printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="c0f84-139">Update a printTaskDefinition.</span></span> |
| [<span data-ttu-id="c0f84-140">Excluir taskDefinition</span><span class="sxs-lookup"><span data-stu-id="c0f84-140">Delete taskDefinition</span></span>](../api/print-delete-taskdefinition.md) | <span data-ttu-id="c0f84-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c0f84-141">None</span></span> | <span data-ttu-id="c0f84-142">Excluir um printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="c0f84-142">Delete a printTaskDefinition.</span></span> |

## <a name="properties"></a><span data-ttu-id="c0f84-143">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c0f84-143">Properties</span></span>
| <span data-ttu-id="c0f84-144">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c0f84-144">Property</span></span>     | <span data-ttu-id="c0f84-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0f84-145">Type</span></span>        | <span data-ttu-id="c0f84-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0f84-146">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c0f84-147">configurações</span><span class="sxs-lookup"><span data-stu-id="c0f84-147">settings</span></span>|[<span data-ttu-id="c0f84-148">printSettings</span><span class="sxs-lookup"><span data-stu-id="c0f84-148">printSettings</span></span>](printsettings.md)|<span data-ttu-id="c0f84-149">Configurações de todo o locatário para o serviço de impressão universal.</span><span class="sxs-lookup"><span data-stu-id="c0f84-149">Tenant-wide settings for the Universal Print service.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0f84-150">Relações</span><span class="sxs-lookup"><span data-stu-id="c0f84-150">Relationships</span></span>
| <span data-ttu-id="c0f84-151">Relação</span><span class="sxs-lookup"><span data-stu-id="c0f84-151">Relationship</span></span> | <span data-ttu-id="c0f84-152">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0f84-152">Type</span></span>        | <span data-ttu-id="c0f84-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0f84-153">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c0f84-154">serviço</span><span class="sxs-lookup"><span data-stu-id="c0f84-154">services</span></span>|<span data-ttu-id="c0f84-155">coleção de [serviços de multiserviço](printservice.md)</span><span class="sxs-lookup"><span data-stu-id="c0f84-155">[printService](printservice.md) collection</span></span>|<span data-ttu-id="c0f84-156">A lista de pontos de extremidade do serviço de impressão Universal disponível.</span><span class="sxs-lookup"><span data-stu-id="c0f84-156">The list of available Universal Print service endpoints.</span></span>|
|<span data-ttu-id="c0f84-157">impressoras</span><span class="sxs-lookup"><span data-stu-id="c0f84-157">printers</span></span>|<span data-ttu-id="c0f84-158">coleção de [impressoras](printer.md)</span><span class="sxs-lookup"><span data-stu-id="c0f84-158">[printer](printer.md) collection</span></span>|<span data-ttu-id="c0f84-159">A lista de impressoras registradas no locatário.</span><span class="sxs-lookup"><span data-stu-id="c0f84-159">The list of printers registered in the tenant.</span></span>|
|<span data-ttu-id="c0f84-160">shares</span><span class="sxs-lookup"><span data-stu-id="c0f84-160">shares</span></span>|<span data-ttu-id="c0f84-161">coleção [printerShare](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="c0f84-161">[printerShare](printershare.md) collection</span></span>|<span data-ttu-id="c0f84-162">A lista de compartilhamentos de impressora registrados no locatário.</span><span class="sxs-lookup"><span data-stu-id="c0f84-162">The list of printer shares registered in the tenant.</span></span>|
|<span data-ttu-id="c0f84-163">conectores</span><span class="sxs-lookup"><span data-stu-id="c0f84-163">connectors</span></span>|<span data-ttu-id="c0f84-164">coleção [Multiconnector](printconnector.md)</span><span class="sxs-lookup"><span data-stu-id="c0f84-164">[printConnector](printconnector.md) collection</span></span>|<span data-ttu-id="c0f84-165">A lista de conectores de impressão disponíveis.</span><span class="sxs-lookup"><span data-stu-id="c0f84-165">The list of available print connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c0f84-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c0f84-166">JSON representation</span></span>

<span data-ttu-id="c0f84-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c0f84-167">The following is a JSON representation of the resource.</span></span>

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
