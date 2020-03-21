---
title: tipo de recurso de multiconnector
description: Representa um conector de impressão que foi registrado usando uma assinatura de impressão universal. O recurso Print Connector pode ser usado para exibir o status do conector e propriedades de atualização.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 7c66933c381e2f7563f4666ca788d06970b04490
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895506"
---
# <a name="printconnector-resource-type"></a><span data-ttu-id="99cc5-104">tipo de recurso de multiconnector</span><span class="sxs-lookup"><span data-stu-id="99cc5-104">printConnector resource type</span></span>

<span data-ttu-id="99cc5-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99cc5-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99cc5-106">Representa um conector de impressão que foi registrado usando uma assinatura de impressão universal.</span><span class="sxs-lookup"><span data-stu-id="99cc5-106">Represents a print connector that has been registered by using a Universal Print subscription.</span></span> <span data-ttu-id="99cc5-107">O recurso Print Connector pode ser usado para exibir o status do conector e propriedades de atualização.</span><span class="sxs-lookup"><span data-stu-id="99cc5-107">The printConnector resource can be used to view connector status and update properties.</span></span>

## <a name="methods"></a><span data-ttu-id="99cc5-108">Methods</span><span class="sxs-lookup"><span data-stu-id="99cc5-108">Methods</span></span>

| <span data-ttu-id="99cc5-109">Método</span><span class="sxs-lookup"><span data-stu-id="99cc5-109">Method</span></span>       | <span data-ttu-id="99cc5-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="99cc5-110">Return Type</span></span> | <span data-ttu-id="99cc5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="99cc5-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="99cc5-112">Obter conector</span><span class="sxs-lookup"><span data-stu-id="99cc5-112">Get connector</span></span>](../api/printconnector-get.md) | [<span data-ttu-id="99cc5-113">separador de Hiperligação</span><span class="sxs-lookup"><span data-stu-id="99cc5-113">printConnector</span></span>](printconnector.md) | <span data-ttu-id="99cc5-114">Leia as propriedades e as relações do objeto Connector.</span><span class="sxs-lookup"><span data-stu-id="99cc5-114">Read the properties and relationships of the connector object.</span></span> |
| [<span data-ttu-id="99cc5-115">Conector de atualização</span><span class="sxs-lookup"><span data-stu-id="99cc5-115">Update connector</span></span>](../api/printconnector-update.md) | [<span data-ttu-id="99cc5-116">separador de Hiperligação</span><span class="sxs-lookup"><span data-stu-id="99cc5-116">printConnector</span></span>](printconnector.md) | <span data-ttu-id="99cc5-117">Atualize o objeto Connector.</span><span class="sxs-lookup"><span data-stu-id="99cc5-117">Update the connector object.</span></span> |
| [<span data-ttu-id="99cc5-118">Excluir conector</span><span class="sxs-lookup"><span data-stu-id="99cc5-118">Delete connector</span></span>](../api/printconnector-delete.md) | <span data-ttu-id="99cc5-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="99cc5-119">None</span></span> | <span data-ttu-id="99cc5-120">Cancele o registro do conector do serviço de impressão universal.</span><span class="sxs-lookup"><span data-stu-id="99cc5-120">Unregister the connector from the Universal Print service.</span></span> |

## <a name="properties"></a><span data-ttu-id="99cc5-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="99cc5-121">Properties</span></span>
| <span data-ttu-id="99cc5-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="99cc5-122">Property</span></span>     | <span data-ttu-id="99cc5-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="99cc5-123">Type</span></span>        | <span data-ttu-id="99cc5-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="99cc5-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="99cc5-125">id</span><span class="sxs-lookup"><span data-stu-id="99cc5-125">id</span></span>|<span data-ttu-id="99cc5-126">String</span><span class="sxs-lookup"><span data-stu-id="99cc5-126">String</span></span>| <span data-ttu-id="99cc5-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="99cc5-127">Read-only.</span></span>|
|<span data-ttu-id="99cc5-128">name</span><span class="sxs-lookup"><span data-stu-id="99cc5-128">name</span></span>|<span data-ttu-id="99cc5-129">String</span><span class="sxs-lookup"><span data-stu-id="99cc5-129">String</span></span>|<span data-ttu-id="99cc5-130">O nome do conector.</span><span class="sxs-lookup"><span data-stu-id="99cc5-130">The name of the connector.</span></span>|
|<span data-ttu-id="99cc5-131">Nomededomíniototalmentequalificado</span><span class="sxs-lookup"><span data-stu-id="99cc5-131">fullyQualifiedDomainName</span></span>|<span data-ttu-id="99cc5-132">String</span><span class="sxs-lookup"><span data-stu-id="99cc5-132">String</span></span>|<span data-ttu-id="99cc5-133">O nome de host do computador do conector.</span><span class="sxs-lookup"><span data-stu-id="99cc5-133">The connector machine's hostname.</span></span>|
|<span data-ttu-id="99cc5-134">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="99cc5-134">operatingSystem</span></span>|<span data-ttu-id="99cc5-135">String</span><span class="sxs-lookup"><span data-stu-id="99cc5-135">String</span></span>|<span data-ttu-id="99cc5-136">A versão do sistema operacional do computador do conector.</span><span class="sxs-lookup"><span data-stu-id="99cc5-136">The connector machine's operating system version.</span></span>|
|<span data-ttu-id="99cc5-137">appVersion</span><span class="sxs-lookup"><span data-stu-id="99cc5-137">appVersion</span></span>|<span data-ttu-id="99cc5-138">String</span><span class="sxs-lookup"><span data-stu-id="99cc5-138">String</span></span>|<span data-ttu-id="99cc5-139">A versão do conector.</span><span class="sxs-lookup"><span data-stu-id="99cc5-139">The connector's version.</span></span>|
|<span data-ttu-id="99cc5-140">deviceHealth</span><span class="sxs-lookup"><span data-stu-id="99cc5-140">deviceHealth</span></span>|[<span data-ttu-id="99cc5-141">deviceHealth</span><span class="sxs-lookup"><span data-stu-id="99cc5-141">deviceHealth</span></span>](devicehealth.md)|<span data-ttu-id="99cc5-142">A integridade do dispositivo do conector.</span><span class="sxs-lookup"><span data-stu-id="99cc5-142">The connector's device health.</span></span>|
|<span data-ttu-id="99cc5-143">location</span><span class="sxs-lookup"><span data-stu-id="99cc5-143">location</span></span>|[<span data-ttu-id="99cc5-144">printerLocation</span><span class="sxs-lookup"><span data-stu-id="99cc5-144">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="99cc5-145">O local físico e/ou organizacional do conector.</span><span class="sxs-lookup"><span data-stu-id="99cc5-145">The physical and/or organizational location of the connector.</span></span>|
|<span data-ttu-id="99cc5-146">registeredDateTime</span><span class="sxs-lookup"><span data-stu-id="99cc5-146">registeredDateTime</span></span>|<span data-ttu-id="99cc5-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99cc5-147">DateTimeOffset</span></span>|<span data-ttu-id="99cc5-148">O DateTimeOffset quando o conector foi registrado.</span><span class="sxs-lookup"><span data-stu-id="99cc5-148">The DateTimeOffset when the connector was registered.</span></span>|
|<span data-ttu-id="99cc5-149">registeredBy</span><span class="sxs-lookup"><span data-stu-id="99cc5-149">registeredBy</span></span>|[<span data-ttu-id="99cc5-150">userIdentity</span><span class="sxs-lookup"><span data-stu-id="99cc5-150">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="99cc5-151">O usuário que registrou o conector.</span><span class="sxs-lookup"><span data-stu-id="99cc5-151">The user who registered the connector.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="99cc5-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="99cc5-152">JSON representation</span></span>

<span data-ttu-id="99cc5-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="99cc5-153">The following is a JSON representation of the resource.</span></span>

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