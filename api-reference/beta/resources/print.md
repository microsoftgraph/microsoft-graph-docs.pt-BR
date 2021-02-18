---
title: tipo de recurso print
description: Quando acompanhado por uma assinatura de Impressão Universal, o recurso Imprimir permite o gerenciamento de impressoras e a descoberta de printServiceEndpoints que podem ser usados para gerenciar impressoras e trabalhos de impressão dentro da Impressão Universal.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 0604044824d153c9e6d39586c2ca58ee9ca893ea
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292249"
---
# <a name="print-resource-type"></a><span data-ttu-id="8d661-103">tipo de recurso print</span><span class="sxs-lookup"><span data-stu-id="8d661-103">print resource type</span></span>

<span data-ttu-id="8d661-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d661-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d661-105">Quando acompanhado por uma assinatura de Impressão Universal, o recurso Imprimir permite o gerenciamento de impressoras e a descoberta de [printServiceEndpoints](printserviceendpoint.md) que podem ser usados para gerenciar impressoras e trabalhos de impressão dentro da Impressão Universal.</span><span class="sxs-lookup"><span data-stu-id="8d661-105">When accompanied by a Universal Print subscription, the Print feature enables management of printers and discovery of [printServiceEndpoints](printserviceendpoint.md) that can be used to manage printers and print jobs within Universal Print.</span></span>

## <a name="methods"></a><span data-ttu-id="8d661-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="8d661-106">Methods</span></span>
| <span data-ttu-id="8d661-107">Método</span><span class="sxs-lookup"><span data-stu-id="8d661-107">Method</span></span>       | <span data-ttu-id="8d661-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8d661-108">Return Type</span></span> | <span data-ttu-id="8d661-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d661-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8d661-110">Listar conectores</span><span class="sxs-lookup"><span data-stu-id="8d661-110">List connectors</span></span>](../api/print-list-connectors.md) | <span data-ttu-id="8d661-111">[Coleção printConnector](printconnector.md)</span><span class="sxs-lookup"><span data-stu-id="8d661-111">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="8d661-112">Obter uma lista de conectores de impressão.</span><span class="sxs-lookup"><span data-stu-id="8d661-112">Get a list of print connectors.</span></span> |
| [<span data-ttu-id="8d661-113">Lista de impressoras</span><span class="sxs-lookup"><span data-stu-id="8d661-113">List printers</span></span>](../api/print-list-printers.md) | <span data-ttu-id="8d661-114">[coleção printer](printer.md)</span><span class="sxs-lookup"><span data-stu-id="8d661-114">[printer](printer.md) collection</span></span> | <span data-ttu-id="8d661-115">Obter uma lista de impressoras.</span><span class="sxs-lookup"><span data-stu-id="8d661-115">Get a list of printers.</span></span> |
| [<span data-ttu-id="8d661-116">Listar shares</span><span class="sxs-lookup"><span data-stu-id="8d661-116">List shares</span></span>](../api/print-list-shares.md) | <span data-ttu-id="8d661-117">[Coleção printerShare](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="8d661-117">[printerShare](printershare.md) collection</span></span> | <span data-ttu-id="8d661-118">Obter uma lista de compartilhamentos de impressora.</span><span class="sxs-lookup"><span data-stu-id="8d661-118">Get a list of printer shares.</span></span> |
| [<span data-ttu-id="8d661-119">Listar serviços</span><span class="sxs-lookup"><span data-stu-id="8d661-119">List services</span></span>](../api/print-list-services.md) | <span data-ttu-id="8d661-120">[Coleção printService](printservice.md)</span><span class="sxs-lookup"><span data-stu-id="8d661-120">[printService](printservice.md) collection</span></span> | <span data-ttu-id="8d661-121">Obter uma lista de serviços.</span><span class="sxs-lookup"><span data-stu-id="8d661-121">Get a list of services.</span></span> |
| [<span data-ttu-id="8d661-122">Criar printerShare</span><span class="sxs-lookup"><span data-stu-id="8d661-122">Create printerShare</span></span>](../api/print-post-shares.md) | [<span data-ttu-id="8d661-123">printerShare</span><span class="sxs-lookup"><span data-stu-id="8d661-123">printerShare</span></span>](printershare.md) | <span data-ttu-id="8d661-124">Crie um novo compartilhamento de impressora postando na coleção **shares.**</span><span class="sxs-lookup"><span data-stu-id="8d661-124">Create a new printer share by posting to the **shares** collection.</span></span> |
| [<span data-ttu-id="8d661-125">Criar impressora</span><span class="sxs-lookup"><span data-stu-id="8d661-125">Create printer</span></span>](../api/printer-create.md) | [<span data-ttu-id="8d661-126">printerCreateOperation</span><span class="sxs-lookup"><span data-stu-id="8d661-126">printerCreateOperation</span></span>](printerCreateOperation.md) | <span data-ttu-id="8d661-127">Crie (registre) uma nova impressora com Impressão Universal.</span><span class="sxs-lookup"><span data-stu-id="8d661-127">Create (register) a new printer with Universal Print.</span></span> |
| [<span data-ttu-id="8d661-128">Atualizar configurações</span><span class="sxs-lookup"><span data-stu-id="8d661-128">Update settings</span></span>](../api/print-update-settings.md) |  [<span data-ttu-id="8d661-129">printSettings</span><span class="sxs-lookup"><span data-stu-id="8d661-129">printSettings</span></span>](printsettings.md) | <span data-ttu-id="8d661-130">Atualiza as configurações de todo o locatário para o serviço de Impressão Universal.</span><span class="sxs-lookup"><span data-stu-id="8d661-130">Updates tenant-wide settings for the Universal Print service.</span></span> |
| [<span data-ttu-id="8d661-131">Listar taskDefinitions</span><span class="sxs-lookup"><span data-stu-id="8d661-131">List taskDefinitions</span></span>](../api/print-list-taskdefinitions.md) | <span data-ttu-id="8d661-132">[Coleção printTaskDefinition](printtaskdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="8d661-132">[printTaskDefinition](printtaskdefinition.md) collection</span></span> | <span data-ttu-id="8d661-133">Obter uma lista de todos os locatários de printTaskDefinitions criadas na Impressão Universal.</span><span class="sxs-lookup"><span data-stu-id="8d661-133">Get a tenant-wide list of printTaskDefinitions created within Universal Print.</span></span> |
| [<span data-ttu-id="8d661-134">Criar taskDefinition</span><span class="sxs-lookup"><span data-stu-id="8d661-134">Create taskDefinition</span></span>](../api/print-post-taskdefinitions.md) | [<span data-ttu-id="8d661-135">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="8d661-135">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="8d661-136">Crie uma nova printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="8d661-136">Create a new printTaskDefinition.</span></span> |
| [<span data-ttu-id="8d661-137">Atualizar taskDefinition</span><span class="sxs-lookup"><span data-stu-id="8d661-137">Update taskDefinition</span></span>](../api/print-update-taskdefinition.md) | [<span data-ttu-id="8d661-138">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="8d661-138">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="8d661-139">Atualize uma printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="8d661-139">Update a printTaskDefinition.</span></span> |
| [<span data-ttu-id="8d661-140">Excluir taskDefinition</span><span class="sxs-lookup"><span data-stu-id="8d661-140">Delete taskDefinition</span></span>](../api/print-delete-taskdefinition.md) | <span data-ttu-id="8d661-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8d661-141">None</span></span> | <span data-ttu-id="8d661-142">Exclua uma printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="8d661-142">Delete a printTaskDefinition.</span></span> |

## <a name="properties"></a><span data-ttu-id="8d661-143">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8d661-143">Properties</span></span>
| <span data-ttu-id="8d661-144">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8d661-144">Property</span></span>     | <span data-ttu-id="8d661-145">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d661-145">Type</span></span>        | <span data-ttu-id="8d661-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d661-146">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8d661-147">settings</span><span class="sxs-lookup"><span data-stu-id="8d661-147">settings</span></span>|[<span data-ttu-id="8d661-148">printSettings</span><span class="sxs-lookup"><span data-stu-id="8d661-148">printSettings</span></span>](printsettings.md)|<span data-ttu-id="8d661-149">Configurações para todo o locatário para o serviço de Impressão Universal.</span><span class="sxs-lookup"><span data-stu-id="8d661-149">Tenant-wide settings for the Universal Print service.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d661-150">Relações</span><span class="sxs-lookup"><span data-stu-id="8d661-150">Relationships</span></span>
| <span data-ttu-id="8d661-151">Relação</span><span class="sxs-lookup"><span data-stu-id="8d661-151">Relationship</span></span> | <span data-ttu-id="8d661-152">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d661-152">Type</span></span>        | <span data-ttu-id="8d661-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d661-153">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8d661-154">serviços</span><span class="sxs-lookup"><span data-stu-id="8d661-154">services</span></span>|<span data-ttu-id="8d661-155">[Coleção printService](printservice.md)</span><span class="sxs-lookup"><span data-stu-id="8d661-155">[printService](printservice.md) collection</span></span>|<span data-ttu-id="8d661-156">A lista de pontos de extremidade de serviço de Impressão Universal disponíveis.</span><span class="sxs-lookup"><span data-stu-id="8d661-156">The list of available Universal Print service endpoints.</span></span>|
|<span data-ttu-id="8d661-157">impressoras</span><span class="sxs-lookup"><span data-stu-id="8d661-157">printers</span></span>|<span data-ttu-id="8d661-158">[coleção printer](printer.md)</span><span class="sxs-lookup"><span data-stu-id="8d661-158">[printer](printer.md) collection</span></span>|<span data-ttu-id="8d661-159">A lista de impressoras registradas no locatário.</span><span class="sxs-lookup"><span data-stu-id="8d661-159">The list of printers registered in the tenant.</span></span>|
|<span data-ttu-id="8d661-160">shares</span><span class="sxs-lookup"><span data-stu-id="8d661-160">shares</span></span>|<span data-ttu-id="8d661-161">[Coleção printerShare](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="8d661-161">[printerShare](printershare.md) collection</span></span>|<span data-ttu-id="8d661-162">A lista de compartilhamentos de impressora registrados no locatário.</span><span class="sxs-lookup"><span data-stu-id="8d661-162">The list of printer shares registered in the tenant.</span></span>|
|<span data-ttu-id="8d661-163">conectores</span><span class="sxs-lookup"><span data-stu-id="8d661-163">connectors</span></span>|<span data-ttu-id="8d661-164">[Coleção printConnector](printconnector.md)</span><span class="sxs-lookup"><span data-stu-id="8d661-164">[printConnector](printconnector.md) collection</span></span>|<span data-ttu-id="8d661-165">A lista de conectores de impressão disponíveis.</span><span class="sxs-lookup"><span data-stu-id="8d661-165">The list of available print connectors.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8d661-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8d661-166">JSON representation</span></span>

<span data-ttu-id="8d661-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8d661-167">The following is a JSON representation of the resource.</span></span>

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
  ]
}-->


