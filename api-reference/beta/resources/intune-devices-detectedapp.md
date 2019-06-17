---
title: Tipo de recurso detectedApp
description: Um aplicativo gerenciado ou não gerenciado que está instalado em um dispositivo gerenciado. Aplicativos não gerenciados só aparecerão para dispositivos marcados como controlados pela empresa.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 098ad481c854514e988037e755cefd3dbecd8165
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983152"
---
# <a name="detectedapp-resource-type"></a><span data-ttu-id="b6d0a-104">Tipo de recurso detectedApp</span><span class="sxs-lookup"><span data-stu-id="b6d0a-104">detectedApp resource type</span></span>

> <span data-ttu-id="b6d0a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b6d0a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6d0a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b6d0a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6d0a-107">Um aplicativo gerenciado ou não gerenciado que está instalado em um dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="b6d0a-107">A managed or unmanaged app that is installed on a managed device.</span></span> <span data-ttu-id="b6d0a-108">Aplicativos não gerenciados só aparecerão para dispositivos marcados como controlados pela empresa.</span><span class="sxs-lookup"><span data-stu-id="b6d0a-108">Unmanaged apps will only appear for devices marked as corporate owned.</span></span>

## <a name="methods"></a><span data-ttu-id="b6d0a-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="b6d0a-109">Methods</span></span>
|<span data-ttu-id="b6d0a-110">Método</span><span class="sxs-lookup"><span data-stu-id="b6d0a-110">Method</span></span>|<span data-ttu-id="b6d0a-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b6d0a-111">Return Type</span></span>|<span data-ttu-id="b6d0a-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6d0a-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b6d0a-113">Listar detectedApps</span><span class="sxs-lookup"><span data-stu-id="b6d0a-113">List detectedApps</span></span>](../api/intune-devices-detectedapp-list.md)|<span data-ttu-id="b6d0a-114">Coleção [detectedApp](../resources/intune-devices-detectedapp.md)</span><span class="sxs-lookup"><span data-stu-id="b6d0a-114">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="b6d0a-115">Lista propriedades e relações dos objetos [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="b6d0a-115">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>|
|[<span data-ttu-id="b6d0a-116">Obter detectedApp</span><span class="sxs-lookup"><span data-stu-id="b6d0a-116">Get detectedApp</span></span>](../api/intune-devices-detectedapp-get.md)|[<span data-ttu-id="b6d0a-117">detectedApp</span><span class="sxs-lookup"><span data-stu-id="b6d0a-117">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="b6d0a-118">Propriedades de leitura e relações do objeto [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="b6d0a-118">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="b6d0a-119">Criar detectedApp</span><span class="sxs-lookup"><span data-stu-id="b6d0a-119">Create detectedApp</span></span>](../api/intune-devices-detectedapp-create.md)|[<span data-ttu-id="b6d0a-120">detectedApp</span><span class="sxs-lookup"><span data-stu-id="b6d0a-120">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="b6d0a-121">Cria um novo objeto [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="b6d0a-121">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="b6d0a-122">Excluir detectedApp</span><span class="sxs-lookup"><span data-stu-id="b6d0a-122">Delete detectedApp</span></span>](../api/intune-devices-detectedapp-delete.md)|<span data-ttu-id="b6d0a-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b6d0a-123">None</span></span>|<span data-ttu-id="b6d0a-124">Exclui um [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="b6d0a-124">Deletes a [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>|
|[<span data-ttu-id="b6d0a-125">Atualizar detectedApp</span><span class="sxs-lookup"><span data-stu-id="b6d0a-125">Update detectedApp</span></span>](../api/intune-devices-detectedapp-update.md)|[<span data-ttu-id="b6d0a-126">detectedApp</span><span class="sxs-lookup"><span data-stu-id="b6d0a-126">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="b6d0a-127">Atualiza as propriedades de um objeto [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="b6d0a-127">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b6d0a-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b6d0a-128">Properties</span></span>
|<span data-ttu-id="b6d0a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6d0a-129">Property</span></span>|<span data-ttu-id="b6d0a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6d0a-130">Type</span></span>|<span data-ttu-id="b6d0a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6d0a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6d0a-132">id</span><span class="sxs-lookup"><span data-stu-id="b6d0a-132">id</span></span>|<span data-ttu-id="b6d0a-133">String</span><span class="sxs-lookup"><span data-stu-id="b6d0a-133">String</span></span>|<span data-ttu-id="b6d0a-134">O identificador exclusivo do aplicativo detectado.</span><span class="sxs-lookup"><span data-stu-id="b6d0a-134">The unique Identifier for the detected application.</span></span> <span data-ttu-id="b6d0a-135">Ele é gerado automaticamente pelo Intune no momento em que o aplicativo é criado.</span><span class="sxs-lookup"><span data-stu-id="b6d0a-135">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="b6d0a-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b6d0a-136">Read-only.</span></span>|
|<span data-ttu-id="b6d0a-137">displayName</span><span class="sxs-lookup"><span data-stu-id="b6d0a-137">displayName</span></span>|<span data-ttu-id="b6d0a-138">String</span><span class="sxs-lookup"><span data-stu-id="b6d0a-138">String</span></span>|<span data-ttu-id="b6d0a-139">Nome do aplicativo descoberto.</span><span class="sxs-lookup"><span data-stu-id="b6d0a-139">Name of the discovered application.</span></span> <span data-ttu-id="b6d0a-140">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="b6d0a-140">Read-only</span></span>|
|<span data-ttu-id="b6d0a-141">version</span><span class="sxs-lookup"><span data-stu-id="b6d0a-141">version</span></span>|<span data-ttu-id="b6d0a-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6d0a-142">String</span></span>|<span data-ttu-id="b6d0a-143">Versão do aplicativo descoberto.</span><span class="sxs-lookup"><span data-stu-id="b6d0a-143">Version of the discovered application.</span></span> <span data-ttu-id="b6d0a-144">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="b6d0a-144">Read-only</span></span>|
|<span data-ttu-id="b6d0a-145">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="b6d0a-145">sizeInByte</span></span>|<span data-ttu-id="b6d0a-146">Int64</span><span class="sxs-lookup"><span data-stu-id="b6d0a-146">Int64</span></span>|<span data-ttu-id="b6d0a-147">Tamanho do aplicativo descoberto, em bytes.</span><span class="sxs-lookup"><span data-stu-id="b6d0a-147">Discovered application size in bytes.</span></span> <span data-ttu-id="b6d0a-148">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="b6d0a-148">Read-only</span></span>|
|<span data-ttu-id="b6d0a-149">deviceCount</span><span class="sxs-lookup"><span data-stu-id="b6d0a-149">deviceCount</span></span>|<span data-ttu-id="b6d0a-150">Int32</span><span class="sxs-lookup"><span data-stu-id="b6d0a-150">Int32</span></span>|<span data-ttu-id="b6d0a-151">O número de dispositivos que instalaram esse aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6d0a-151">The number of devices that have installed this application</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6d0a-152">Relações</span><span class="sxs-lookup"><span data-stu-id="b6d0a-152">Relationships</span></span>
|<span data-ttu-id="b6d0a-153">Relação</span><span class="sxs-lookup"><span data-stu-id="b6d0a-153">Relationship</span></span>|<span data-ttu-id="b6d0a-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6d0a-154">Type</span></span>|<span data-ttu-id="b6d0a-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6d0a-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6d0a-156">managedDevices</span><span class="sxs-lookup"><span data-stu-id="b6d0a-156">managedDevices</span></span>|<span data-ttu-id="b6d0a-157">Coleção [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="b6d0a-157">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="b6d0a-158">Os dispositivos que descobriram o aplicativo instalado</span><span class="sxs-lookup"><span data-stu-id="b6d0a-158">The devices that have the discovered application installed</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b6d0a-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b6d0a-159">JSON Representation</span></span>
<span data-ttu-id="b6d0a-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b6d0a-160">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.detectedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.detectedApp",
  "id": "String (identifier)",
  "displayName": "String",
  "version": "String",
  "sizeInByte": 1024,
  "deviceCount": 1024
}
```





