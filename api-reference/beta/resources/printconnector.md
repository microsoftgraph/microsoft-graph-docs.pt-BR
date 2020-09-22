---
title: tipo de recurso de multiconnector
description: Representa um conector de impressão que foi registrado usando uma assinatura de impressão universal. O recurso Print Connector pode ser usado para exibir o status do conector e propriedades de atualização.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: d027344db67a26fc0af7ebffaaad63d3fe3c4971
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046805"
---
# <a name="printconnector-resource-type"></a><span data-ttu-id="e9e0f-104">tipo de recurso de multiconnector</span><span class="sxs-lookup"><span data-stu-id="e9e0f-104">printConnector resource type</span></span>

<span data-ttu-id="e9e0f-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9e0f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9e0f-106">Representa um conector de impressão que foi registrado usando uma assinatura de impressão universal.</span><span class="sxs-lookup"><span data-stu-id="e9e0f-106">Represents a print connector that has been registered by using a Universal Print subscription.</span></span> <span data-ttu-id="e9e0f-107">O recurso Print Connector pode ser usado para exibir o status do conector e propriedades de atualização.</span><span class="sxs-lookup"><span data-stu-id="e9e0f-107">The printConnector resource can be used to view connector status and update properties.</span></span>

## <a name="methods"></a><span data-ttu-id="e9e0f-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="e9e0f-108">Methods</span></span>

| <span data-ttu-id="e9e0f-109">Método</span><span class="sxs-lookup"><span data-stu-id="e9e0f-109">Method</span></span>       | <span data-ttu-id="e9e0f-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e9e0f-110">Return Type</span></span> | <span data-ttu-id="e9e0f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9e0f-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e9e0f-112">Obter conector</span><span class="sxs-lookup"><span data-stu-id="e9e0f-112">Get connector</span></span>](../api/printconnector-get.md) | [<span data-ttu-id="e9e0f-113">separador de Hiperligação</span><span class="sxs-lookup"><span data-stu-id="e9e0f-113">printConnector</span></span>](printconnector.md) | <span data-ttu-id="e9e0f-114">Leia as propriedades e as relações do objeto Connector.</span><span class="sxs-lookup"><span data-stu-id="e9e0f-114">Read the properties and relationships of the connector object.</span></span> |
| [<span data-ttu-id="e9e0f-115">Conector de atualização</span><span class="sxs-lookup"><span data-stu-id="e9e0f-115">Update connector</span></span>](../api/printconnector-update.md) | [<span data-ttu-id="e9e0f-116">separador de Hiperligação</span><span class="sxs-lookup"><span data-stu-id="e9e0f-116">printConnector</span></span>](printconnector.md) | <span data-ttu-id="e9e0f-117">Atualize o objeto Connector.</span><span class="sxs-lookup"><span data-stu-id="e9e0f-117">Update the connector object.</span></span> |
| [<span data-ttu-id="e9e0f-118">Excluir conector</span><span class="sxs-lookup"><span data-stu-id="e9e0f-118">Delete connector</span></span>](../api/printconnector-delete.md) | <span data-ttu-id="e9e0f-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e9e0f-119">None</span></span> | <span data-ttu-id="e9e0f-120">Cancele o registro do conector do serviço de impressão universal.</span><span class="sxs-lookup"><span data-stu-id="e9e0f-120">Unregister the connector from the Universal Print service.</span></span> |

## <a name="properties"></a><span data-ttu-id="e9e0f-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e9e0f-121">Properties</span></span>
| <span data-ttu-id="e9e0f-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e9e0f-122">Property</span></span>     | <span data-ttu-id="e9e0f-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="e9e0f-123">Type</span></span>        | <span data-ttu-id="e9e0f-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9e0f-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e9e0f-125">id</span><span class="sxs-lookup"><span data-stu-id="e9e0f-125">id</span></span>|<span data-ttu-id="e9e0f-126">String</span><span class="sxs-lookup"><span data-stu-id="e9e0f-126">String</span></span>| <span data-ttu-id="e9e0f-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e9e0f-127">Read-only.</span></span>|
|<span data-ttu-id="e9e0f-128">name</span><span class="sxs-lookup"><span data-stu-id="e9e0f-128">name</span></span>|<span data-ttu-id="e9e0f-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9e0f-129">String</span></span>|<span data-ttu-id="e9e0f-130">O nome do conector.</span><span class="sxs-lookup"><span data-stu-id="e9e0f-130">The name of the connector.</span></span>|
|<span data-ttu-id="e9e0f-131">Nomededomíniototalmentequalificado</span><span class="sxs-lookup"><span data-stu-id="e9e0f-131">fullyQualifiedDomainName</span></span>|<span data-ttu-id="e9e0f-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9e0f-132">String</span></span>|<span data-ttu-id="e9e0f-133">O nome de host do computador do conector.</span><span class="sxs-lookup"><span data-stu-id="e9e0f-133">The connector machine's hostname.</span></span>|
|<span data-ttu-id="e9e0f-134">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="e9e0f-134">operatingSystem</span></span>|<span data-ttu-id="e9e0f-135">String</span><span class="sxs-lookup"><span data-stu-id="e9e0f-135">String</span></span>|<span data-ttu-id="e9e0f-136">A versão do sistema operacional do computador do conector.</span><span class="sxs-lookup"><span data-stu-id="e9e0f-136">The connector machine's operating system version.</span></span>|
|<span data-ttu-id="e9e0f-137">appVersion</span><span class="sxs-lookup"><span data-stu-id="e9e0f-137">appVersion</span></span>|<span data-ttu-id="e9e0f-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e9e0f-138">String</span></span>|<span data-ttu-id="e9e0f-139">A versão do conector.</span><span class="sxs-lookup"><span data-stu-id="e9e0f-139">The connector's version.</span></span>|
|<span data-ttu-id="e9e0f-140">deviceHealth</span><span class="sxs-lookup"><span data-stu-id="e9e0f-140">deviceHealth</span></span>|[<span data-ttu-id="e9e0f-141">deviceHealth</span><span class="sxs-lookup"><span data-stu-id="e9e0f-141">deviceHealth</span></span>](devicehealth.md)|<span data-ttu-id="e9e0f-142">A integridade do dispositivo do conector.</span><span class="sxs-lookup"><span data-stu-id="e9e0f-142">The connector's device health.</span></span>|
|<span data-ttu-id="e9e0f-143">localização</span><span class="sxs-lookup"><span data-stu-id="e9e0f-143">location</span></span>|[<span data-ttu-id="e9e0f-144">printerLocation</span><span class="sxs-lookup"><span data-stu-id="e9e0f-144">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="e9e0f-145">O local físico e/ou organizacional do conector.</span><span class="sxs-lookup"><span data-stu-id="e9e0f-145">The physical and/or organizational location of the connector.</span></span>|
|<span data-ttu-id="e9e0f-146">registeredDateTime</span><span class="sxs-lookup"><span data-stu-id="e9e0f-146">registeredDateTime</span></span>|<span data-ttu-id="e9e0f-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9e0f-147">DateTimeOffset</span></span>|<span data-ttu-id="e9e0f-148">O DateTimeOffset quando o conector foi registrado.</span><span class="sxs-lookup"><span data-stu-id="e9e0f-148">The DateTimeOffset when the connector was registered.</span></span>|
|<span data-ttu-id="e9e0f-149">registeredBy</span><span class="sxs-lookup"><span data-stu-id="e9e0f-149">registeredBy</span></span>|[<span data-ttu-id="e9e0f-150">userIdentity</span><span class="sxs-lookup"><span data-stu-id="e9e0f-150">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="e9e0f-151">O usuário que registrou o conector.</span><span class="sxs-lookup"><span data-stu-id="e9e0f-151">The user who registered the connector.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e9e0f-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e9e0f-152">JSON representation</span></span>

<span data-ttu-id="e9e0f-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e9e0f-153">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printConnector"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "fullyQualifiedDomainName": "String",
  "operatingSystem": "String",
  "appVersion": "String",
  "deviceHealth": {"@odata.type": "microsoft.graph.deviceHealth"},
  "location": {"@odata.type": "microsoft.graph.printerLocation"},
  "registeredDateTime": "String (timestamp)",
  "registeredBy": {"@odata.type": "microsoft.graph.userIdentity"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printConnector resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


