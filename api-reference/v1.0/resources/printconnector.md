---
title: Tipo de recurso printConnector
description: Representa um conector de impressão que foi registrado usando uma assinatura de Impressão Universal. O recurso printConnector pode ser usado para exibir o status do conector e atualizar as propriedades.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: e791ca755b695fc8e4704b65aff98a9db934d901
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516914"
---
# <a name="printconnector-resource-type"></a><span data-ttu-id="efccb-104">Tipo de recurso printConnector</span><span class="sxs-lookup"><span data-stu-id="efccb-104">printConnector resource type</span></span>

<span data-ttu-id="efccb-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efccb-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="efccb-106">Representa um conector de impressão que foi registrado usando uma assinatura de Impressão Universal.</span><span class="sxs-lookup"><span data-stu-id="efccb-106">Represents a print connector that has been registered by using a Universal Print subscription.</span></span> <span data-ttu-id="efccb-107">O recurso printConnector pode ser usado para exibir o status do conector e atualizar as propriedades.</span><span class="sxs-lookup"><span data-stu-id="efccb-107">The printConnector resource can be used to view connector status and update properties.</span></span>

## <a name="methods"></a><span data-ttu-id="efccb-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="efccb-108">Methods</span></span>
|<span data-ttu-id="efccb-109">Método</span><span class="sxs-lookup"><span data-stu-id="efccb-109">Method</span></span>|<span data-ttu-id="efccb-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="efccb-110">Return type</span></span>|<span data-ttu-id="efccb-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="efccb-111">Description</span></span>|
|:---|:---|:---|
| [<span data-ttu-id="efccb-112">Obter conector</span><span class="sxs-lookup"><span data-stu-id="efccb-112">Get connector</span></span>](../api/printconnector-get.md) | [<span data-ttu-id="efccb-113">printConnector</span><span class="sxs-lookup"><span data-stu-id="efccb-113">printConnector</span></span>](printconnector.md) | <span data-ttu-id="efccb-114">Leia as propriedades e as relações do objeto conector.</span><span class="sxs-lookup"><span data-stu-id="efccb-114">Read the properties and relationships of the connector object.</span></span> |
| [<span data-ttu-id="efccb-115">Conector de atualização</span><span class="sxs-lookup"><span data-stu-id="efccb-115">Update connector</span></span>](../api/printconnector-update.md) | [<span data-ttu-id="efccb-116">printConnector</span><span class="sxs-lookup"><span data-stu-id="efccb-116">printConnector</span></span>](printconnector.md) | <span data-ttu-id="efccb-117">Atualize o objeto connector.</span><span class="sxs-lookup"><span data-stu-id="efccb-117">Update the connector object.</span></span> |
| [<span data-ttu-id="efccb-118">Excluir conector</span><span class="sxs-lookup"><span data-stu-id="efccb-118">Delete connector</span></span>](../api/printconnector-delete.md) | <span data-ttu-id="efccb-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="efccb-119">None</span></span> | <span data-ttu-id="efccb-120">Desaconselhe o conector do serviço de Impressão Universal.</span><span class="sxs-lookup"><span data-stu-id="efccb-120">Unregister the connector from the Universal Print service.</span></span> |

## <a name="properties"></a><span data-ttu-id="efccb-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="efccb-121">Properties</span></span>
|<span data-ttu-id="efccb-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="efccb-122">Property</span></span>|<span data-ttu-id="efccb-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="efccb-123">Type</span></span>|<span data-ttu-id="efccb-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="efccb-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efccb-125">id</span><span class="sxs-lookup"><span data-stu-id="efccb-125">id</span></span>|<span data-ttu-id="efccb-126">String</span><span class="sxs-lookup"><span data-stu-id="efccb-126">String</span></span>| <span data-ttu-id="efccb-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="efccb-127">Read-only.</span></span>|
|<span data-ttu-id="efccb-128">displayName</span><span class="sxs-lookup"><span data-stu-id="efccb-128">displayName</span></span>|<span data-ttu-id="efccb-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="efccb-129">String</span></span>|<span data-ttu-id="efccb-130">O nome do conector.</span><span class="sxs-lookup"><span data-stu-id="efccb-130">The name of the connector.</span></span>|
|<span data-ttu-id="efccb-131">fullyQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="efccb-131">fullyQualifiedDomainName</span></span>|<span data-ttu-id="efccb-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="efccb-132">String</span></span>|<span data-ttu-id="efccb-133">O nome de host do computador do conector.</span><span class="sxs-lookup"><span data-stu-id="efccb-133">The connector machine's hostname.</span></span>|
|<span data-ttu-id="efccb-134">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="efccb-134">operatingSystem</span></span>|<span data-ttu-id="efccb-135">String</span><span class="sxs-lookup"><span data-stu-id="efccb-135">String</span></span>|<span data-ttu-id="efccb-136">A versão do sistema operacional do conector.</span><span class="sxs-lookup"><span data-stu-id="efccb-136">The connector machine's operating system version.</span></span>|
|<span data-ttu-id="efccb-137">appVersion</span><span class="sxs-lookup"><span data-stu-id="efccb-137">appVersion</span></span>|<span data-ttu-id="efccb-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="efccb-138">String</span></span>|<span data-ttu-id="efccb-139">A versão do conector.</span><span class="sxs-lookup"><span data-stu-id="efccb-139">The connector's version.</span></span>|
|<span data-ttu-id="efccb-140">location</span><span class="sxs-lookup"><span data-stu-id="efccb-140">location</span></span>|[<span data-ttu-id="efccb-141">printerLocation</span><span class="sxs-lookup"><span data-stu-id="efccb-141">printerLocation</span></span>](printerlocation.md)|<span data-ttu-id="efccb-142">O local físico e/ou organizacional do conector.</span><span class="sxs-lookup"><span data-stu-id="efccb-142">The physical and/or organizational location of the connector.</span></span>|
|<span data-ttu-id="efccb-143">registeredDateTime</span><span class="sxs-lookup"><span data-stu-id="efccb-143">registeredDateTime</span></span>|<span data-ttu-id="efccb-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="efccb-144">DateTimeOffset</span></span>|<span data-ttu-id="efccb-145">DateTimeOffset quando o conector foi registrado.</span><span class="sxs-lookup"><span data-stu-id="efccb-145">The DateTimeOffset when the connector was registered.</span></span>|
|<span data-ttu-id="efccb-146">registeredBy</span><span class="sxs-lookup"><span data-stu-id="efccb-146">registeredBy</span></span>|[<span data-ttu-id="efccb-147">userIdentity</span><span class="sxs-lookup"><span data-stu-id="efccb-147">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="efccb-148">O usuário que registrou o conector.</span><span class="sxs-lookup"><span data-stu-id="efccb-148">The user who registered the connector.</span></span>|

## <a name="relationships"></a><span data-ttu-id="efccb-149">Relações</span><span class="sxs-lookup"><span data-stu-id="efccb-149">Relationships</span></span>
<span data-ttu-id="efccb-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="efccb-150">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="efccb-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="efccb-151">JSON representation</span></span>
<span data-ttu-id="efccb-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="efccb-152">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printConnector",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printConnector",
  "id": "String (identifier)",
  "displayName": "String",
  "fullyQualifiedDomainName": "String",
  "operatingSystem": "String",
  "appVersion": "String",
  "location": {
    "@odata.type": "microsoft.graph.printerLocation"
  },
  "registeredDateTime": "String (timestamp)"
}
```