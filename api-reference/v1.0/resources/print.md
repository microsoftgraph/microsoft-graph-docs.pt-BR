---
title: tipo de recurso de impressão
description: Quando acompanhado por uma assinatura de Impressão Universal, o recurso Imprimir permite o gerenciamento de impressoras e a descoberta de printServiceEndpoints que podem ser usados para gerenciar impressoras e trabalhos de impressão no Universal Print.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: db532fed1bcdeeec749d59c8297fc36d836aed78
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516917"
---
# <a name="print-resource-type"></a><span data-ttu-id="778c8-103">tipo de recurso de impressão</span><span class="sxs-lookup"><span data-stu-id="778c8-103">print resource type</span></span>

<span data-ttu-id="778c8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="778c8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="778c8-105">Quando acompanhado por uma assinatura de Impressão Universal, o recurso Imprimir permite o gerenciamento de impressoras e a descoberta de [printServiceEndpoints](printserviceendpoint.md) que podem ser usados para gerenciar impressoras e trabalhos de impressão no Universal Print.</span><span class="sxs-lookup"><span data-stu-id="778c8-105">When accompanied by a Universal Print subscription, the Print feature enables management of printers and discovery of [printServiceEndpoints](printserviceendpoint.md) that can be used to manage printers and print jobs within Universal Print.</span></span>

## <a name="methods"></a><span data-ttu-id="778c8-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="778c8-106">Methods</span></span>
|<span data-ttu-id="778c8-107">Método</span><span class="sxs-lookup"><span data-stu-id="778c8-107">Method</span></span>|<span data-ttu-id="778c8-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="778c8-108">Return type</span></span>|<span data-ttu-id="778c8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="778c8-109">Description</span></span>|
|:---|:---|:---|
| [<span data-ttu-id="778c8-110">Listar conectores</span><span class="sxs-lookup"><span data-stu-id="778c8-110">List connectors</span></span>](../api/print-list-connectors.md) | <span data-ttu-id="778c8-111">[Coleção printConnector](printconnector.md)</span><span class="sxs-lookup"><span data-stu-id="778c8-111">[printConnector](printconnector.md) collection</span></span> | <span data-ttu-id="778c8-112">Obter uma lista de conectores de impressão.</span><span class="sxs-lookup"><span data-stu-id="778c8-112">Get a list of print connectors.</span></span> |
| [<span data-ttu-id="778c8-113">Lista de impressoras</span><span class="sxs-lookup"><span data-stu-id="778c8-113">List printers</span></span>](../api/print-list-printers.md) | <span data-ttu-id="778c8-114">[coleção printer](printer.md)</span><span class="sxs-lookup"><span data-stu-id="778c8-114">[printer](printer.md) collection</span></span> | <span data-ttu-id="778c8-115">Obter uma lista de impressoras.</span><span class="sxs-lookup"><span data-stu-id="778c8-115">Get a list of printers.</span></span> |
| [<span data-ttu-id="778c8-116">Listar shares</span><span class="sxs-lookup"><span data-stu-id="778c8-116">List shares</span></span>](../api/print-list-shares.md) | <span data-ttu-id="778c8-117">[Coleção printerShare](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="778c8-117">[printerShare](printershare.md) collection</span></span> | <span data-ttu-id="778c8-118">Obter uma lista de compartilhamentos de impressora.</span><span class="sxs-lookup"><span data-stu-id="778c8-118">Get a list of printer shares.</span></span> |
| [<span data-ttu-id="778c8-119">Listar serviços</span><span class="sxs-lookup"><span data-stu-id="778c8-119">List services</span></span>](../api/print-list-services.md) | <span data-ttu-id="778c8-120">[Coleção printService](printservice.md)</span><span class="sxs-lookup"><span data-stu-id="778c8-120">[printService](printservice.md) collection</span></span> | <span data-ttu-id="778c8-121">Obter uma lista de serviços.</span><span class="sxs-lookup"><span data-stu-id="778c8-121">Get a list of services.</span></span> |
| [<span data-ttu-id="778c8-122">Criar printerShare</span><span class="sxs-lookup"><span data-stu-id="778c8-122">Create printerShare</span></span>](../api/print-post-shares.md) | [<span data-ttu-id="778c8-123">printerShare</span><span class="sxs-lookup"><span data-stu-id="778c8-123">printerShare</span></span>](printershare.md) | <span data-ttu-id="778c8-124">Crie um novo compartilhamento de impressora postando na coleção **de compartilhamentos.**</span><span class="sxs-lookup"><span data-stu-id="778c8-124">Create a new printer share by posting to the **shares** collection.</span></span> |
| [<span data-ttu-id="778c8-125">Criar impressora</span><span class="sxs-lookup"><span data-stu-id="778c8-125">Create printer</span></span>](../api/printer-create.md) | [<span data-ttu-id="778c8-126">printerCreateOperation</span><span class="sxs-lookup"><span data-stu-id="778c8-126">printerCreateOperation</span></span>](printerCreateOperation.md) | <span data-ttu-id="778c8-127">Criar (registrar) uma nova impressora com Impressão Universal.</span><span class="sxs-lookup"><span data-stu-id="778c8-127">Create (register) a new printer with Universal Print.</span></span> |
| [<span data-ttu-id="778c8-128">Atualizar configurações</span><span class="sxs-lookup"><span data-stu-id="778c8-128">Update settings</span></span>](../api/print-update-settings.md) |  [<span data-ttu-id="778c8-129">printSettings</span><span class="sxs-lookup"><span data-stu-id="778c8-129">printSettings</span></span>](printsettings.md) | <span data-ttu-id="778c8-130">Atualiza as configurações de todo o locatário para o serviço de Impressão Universal.</span><span class="sxs-lookup"><span data-stu-id="778c8-130">Updates tenant-wide settings for the Universal Print service.</span></span> |
| [<span data-ttu-id="778c8-131">Listar taskDefinitions</span><span class="sxs-lookup"><span data-stu-id="778c8-131">List taskDefinitions</span></span>](../api/print-list-taskdefinitions.md) | <span data-ttu-id="778c8-132">[Coleção printTaskDefinition](printtaskdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="778c8-132">[printTaskDefinition](printtaskdefinition.md) collection</span></span> | <span data-ttu-id="778c8-133">Obter uma lista em todo o locatário de printTaskDefinitions criada em Impressão Universal.</span><span class="sxs-lookup"><span data-stu-id="778c8-133">Get a tenant-wide list of printTaskDefinitions created within Universal Print.</span></span> |
| [<span data-ttu-id="778c8-134">Criar taskDefinition</span><span class="sxs-lookup"><span data-stu-id="778c8-134">Create taskDefinition</span></span>](../api/print-post-taskdefinitions.md) | [<span data-ttu-id="778c8-135">printTaskDefinition</span><span class="sxs-lookup"><span data-stu-id="778c8-135">printTaskDefinition</span></span>](printtaskdefinition.md) | <span data-ttu-id="778c8-136">Crie uma nova printTaskDefinition.</span><span class="sxs-lookup"><span data-stu-id="778c8-136">Create a new printTaskDefinition.</span></span> |

## <a name="properties"></a><span data-ttu-id="778c8-137">Propriedades</span><span class="sxs-lookup"><span data-stu-id="778c8-137">Properties</span></span>
|<span data-ttu-id="778c8-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="778c8-138">Property</span></span>|<span data-ttu-id="778c8-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="778c8-139">Type</span></span>|<span data-ttu-id="778c8-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="778c8-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="778c8-141">settings</span><span class="sxs-lookup"><span data-stu-id="778c8-141">settings</span></span>|[<span data-ttu-id="778c8-142">printSettings</span><span class="sxs-lookup"><span data-stu-id="778c8-142">printSettings</span></span>](../resources/printsettings.md)|<span data-ttu-id="778c8-143">Configurações em todo o locatário para o serviço de Impressão Universal.</span><span class="sxs-lookup"><span data-stu-id="778c8-143">Tenant-wide settings for the Universal Print service.</span></span>|

## <a name="relationships"></a><span data-ttu-id="778c8-144">Relações</span><span class="sxs-lookup"><span data-stu-id="778c8-144">Relationships</span></span>
|<span data-ttu-id="778c8-145">Relação</span><span class="sxs-lookup"><span data-stu-id="778c8-145">Relationship</span></span>|<span data-ttu-id="778c8-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="778c8-146">Type</span></span>|<span data-ttu-id="778c8-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="778c8-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="778c8-148">services</span><span class="sxs-lookup"><span data-stu-id="778c8-148">services</span></span>|<span data-ttu-id="778c8-149">[Coleção printService](printservice.md)</span><span class="sxs-lookup"><span data-stu-id="778c8-149">[printService](printservice.md) collection</span></span>|<span data-ttu-id="778c8-150">A lista de pontos de extremidade de serviço de Impressão Universal disponíveis.</span><span class="sxs-lookup"><span data-stu-id="778c8-150">The list of available Universal Print service endpoints.</span></span>|
|<span data-ttu-id="778c8-151">impressoras</span><span class="sxs-lookup"><span data-stu-id="778c8-151">printers</span></span>|<span data-ttu-id="778c8-152">[coleção printer](printer.md)</span><span class="sxs-lookup"><span data-stu-id="778c8-152">[printer](printer.md) collection</span></span>|<span data-ttu-id="778c8-153">A lista de impressoras registradas no locatário.</span><span class="sxs-lookup"><span data-stu-id="778c8-153">The list of printers registered in the tenant.</span></span>|
|<span data-ttu-id="778c8-154">shares</span><span class="sxs-lookup"><span data-stu-id="778c8-154">shares</span></span>|<span data-ttu-id="778c8-155">[Coleção printerShare](printershare.md)</span><span class="sxs-lookup"><span data-stu-id="778c8-155">[printerShare](printershare.md) collection</span></span>|<span data-ttu-id="778c8-156">A lista de compartilhamentos de impressora registrados no locatário.</span><span class="sxs-lookup"><span data-stu-id="778c8-156">The list of printer shares registered in the tenant.</span></span>|
|<span data-ttu-id="778c8-157">conectores</span><span class="sxs-lookup"><span data-stu-id="778c8-157">connectors</span></span>|<span data-ttu-id="778c8-158">[Coleção printConnector](printconnector.md)</span><span class="sxs-lookup"><span data-stu-id="778c8-158">[printConnector](printconnector.md) collection</span></span>|<span data-ttu-id="778c8-159">A lista de conectores de impressão disponíveis.</span><span class="sxs-lookup"><span data-stu-id="778c8-159">The list of available print connectors.</span></span>|
|<span data-ttu-id="778c8-160">operations</span><span class="sxs-lookup"><span data-stu-id="778c8-160">operations</span></span>|<span data-ttu-id="778c8-161">[Coleção printOperation](../resources/printoperation.md)</span><span class="sxs-lookup"><span data-stu-id="778c8-161">[printOperation](../resources/printoperation.md) collection</span></span>|<span data-ttu-id="778c8-162">A lista de operações de longa execução de impressão.</span><span class="sxs-lookup"><span data-stu-id="778c8-162">The list of print long running operations.</span></span>|
|<span data-ttu-id="778c8-163">services</span><span class="sxs-lookup"><span data-stu-id="778c8-163">services</span></span>|<span data-ttu-id="778c8-164">[Coleção printService](../resources/printservice.md)</span><span class="sxs-lookup"><span data-stu-id="778c8-164">[printService](../resources/printservice.md) collection</span></span>|<span data-ttu-id="778c8-165">A lista de instâncias de serviço de impressão para vários componentes da infraestrutura de impressão.</span><span class="sxs-lookup"><span data-stu-id="778c8-165">The list of print service instances for various components of the printing infrastructure.</span></span>|
|<span data-ttu-id="778c8-166">taskDefinitions</span><span class="sxs-lookup"><span data-stu-id="778c8-166">taskDefinitions</span></span>|<span data-ttu-id="778c8-167">[Coleção printTaskDefinition](../resources/printtaskdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="778c8-167">[printTaskDefinition](../resources/printtaskdefinition.md) collection</span></span>|<span data-ttu-id="778c8-168">Lista de definição abstrata para uma tarefa que pode ser disparada quando vários eventos ocorrem em Impressão Universal.</span><span class="sxs-lookup"><span data-stu-id="778c8-168">List of abstract definition for a task that can be triggered when various events occur within Universal Print.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="778c8-169">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="778c8-169">JSON representation</span></span>
<span data-ttu-id="778c8-170">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="778c8-170">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.print",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.print",
  "settings": {
    "@odata.type": "microsoft.graph.printSettings"
  }
}
```

