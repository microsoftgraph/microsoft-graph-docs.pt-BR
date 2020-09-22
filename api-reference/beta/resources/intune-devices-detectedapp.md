---
title: Tipo de recurso detectedApp
description: Um aplicativo gerenciado ou não gerenciado que está instalado em um dispositivo gerenciado. Aplicativos não gerenciados só aparecerão para dispositivos marcados como controlados pela empresa.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0039c7a19778ecda2f905672f4d73f53c0a6a999
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060570"
---
# <a name="detectedapp-resource-type"></a><span data-ttu-id="fbc14-104">Tipo de recurso detectedApp</span><span class="sxs-lookup"><span data-stu-id="fbc14-104">detectedApp resource type</span></span>

<span data-ttu-id="fbc14-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fbc14-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fbc14-106">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fbc14-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fbc14-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fbc14-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbc14-108">Um aplicativo gerenciado ou não gerenciado que está instalado em um dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="fbc14-108">A managed or unmanaged app that is installed on a managed device.</span></span> <span data-ttu-id="fbc14-109">Aplicativos não gerenciados só aparecerão para dispositivos marcados como controlados pela empresa.</span><span class="sxs-lookup"><span data-stu-id="fbc14-109">Unmanaged apps will only appear for devices marked as corporate owned.</span></span>

## <a name="methods"></a><span data-ttu-id="fbc14-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="fbc14-110">Methods</span></span>
|<span data-ttu-id="fbc14-111">Método</span><span class="sxs-lookup"><span data-stu-id="fbc14-111">Method</span></span>|<span data-ttu-id="fbc14-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fbc14-112">Return Type</span></span>|<span data-ttu-id="fbc14-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbc14-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fbc14-114">Listar detectedApps</span><span class="sxs-lookup"><span data-stu-id="fbc14-114">List detectedApps</span></span>](../api/intune-devices-detectedapp-list.md)|<span data-ttu-id="fbc14-115">Coleção [detectedApp](../resources/intune-devices-detectedapp.md)</span><span class="sxs-lookup"><span data-stu-id="fbc14-115">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="fbc14-116">Lista propriedades e relações dos objetos [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbc14-116">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>|
|[<span data-ttu-id="fbc14-117">Obter detectedApp</span><span class="sxs-lookup"><span data-stu-id="fbc14-117">Get detectedApp</span></span>](../api/intune-devices-detectedapp-get.md)|[<span data-ttu-id="fbc14-118">detectedApp</span><span class="sxs-lookup"><span data-stu-id="fbc14-118">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="fbc14-119">Propriedades de leitura e relações do objeto [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbc14-119">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="fbc14-120">Criar detectedApp</span><span class="sxs-lookup"><span data-stu-id="fbc14-120">Create detectedApp</span></span>](../api/intune-devices-detectedapp-create.md)|[<span data-ttu-id="fbc14-121">detectedApp</span><span class="sxs-lookup"><span data-stu-id="fbc14-121">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="fbc14-122">Cria um novo objeto [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbc14-122">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="fbc14-123">Excluir detectedApp</span><span class="sxs-lookup"><span data-stu-id="fbc14-123">Delete detectedApp</span></span>](../api/intune-devices-detectedapp-delete.md)|<span data-ttu-id="fbc14-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fbc14-124">None</span></span>|<span data-ttu-id="fbc14-125">Exclui um [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbc14-125">Deletes a [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>|
|[<span data-ttu-id="fbc14-126">Atualizar detectedApp</span><span class="sxs-lookup"><span data-stu-id="fbc14-126">Update detectedApp</span></span>](../api/intune-devices-detectedapp-update.md)|[<span data-ttu-id="fbc14-127">detectedApp</span><span class="sxs-lookup"><span data-stu-id="fbc14-127">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="fbc14-128">Atualiza as propriedades de um objeto [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="fbc14-128">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fbc14-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fbc14-129">Properties</span></span>
|<span data-ttu-id="fbc14-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fbc14-130">Property</span></span>|<span data-ttu-id="fbc14-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbc14-131">Type</span></span>|<span data-ttu-id="fbc14-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbc14-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbc14-133">id</span><span class="sxs-lookup"><span data-stu-id="fbc14-133">id</span></span>|<span data-ttu-id="fbc14-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbc14-134">String</span></span>|<span data-ttu-id="fbc14-135">O identificador exclusivo do aplicativo detectado.</span><span class="sxs-lookup"><span data-stu-id="fbc14-135">The unique Identifier for the detected application.</span></span> <span data-ttu-id="fbc14-136">Ele é gerado automaticamente pelo Intune no momento em que o aplicativo é criado.</span><span class="sxs-lookup"><span data-stu-id="fbc14-136">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="fbc14-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="fbc14-137">Read-only.</span></span>|
|<span data-ttu-id="fbc14-138">displayName</span><span class="sxs-lookup"><span data-stu-id="fbc14-138">displayName</span></span>|<span data-ttu-id="fbc14-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbc14-139">String</span></span>|<span data-ttu-id="fbc14-140">Nome do aplicativo descoberto.</span><span class="sxs-lookup"><span data-stu-id="fbc14-140">Name of the discovered application.</span></span> <span data-ttu-id="fbc14-141">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="fbc14-141">Read-only</span></span>|
|<span data-ttu-id="fbc14-142">version</span><span class="sxs-lookup"><span data-stu-id="fbc14-142">version</span></span>|<span data-ttu-id="fbc14-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fbc14-143">String</span></span>|<span data-ttu-id="fbc14-144">Versão do aplicativo descoberto.</span><span class="sxs-lookup"><span data-stu-id="fbc14-144">Version of the discovered application.</span></span> <span data-ttu-id="fbc14-145">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="fbc14-145">Read-only</span></span>|
|<span data-ttu-id="fbc14-146">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="fbc14-146">sizeInByte</span></span>|<span data-ttu-id="fbc14-147">Int64</span><span class="sxs-lookup"><span data-stu-id="fbc14-147">Int64</span></span>|<span data-ttu-id="fbc14-148">Tamanho do aplicativo descoberto, em bytes.</span><span class="sxs-lookup"><span data-stu-id="fbc14-148">Discovered application size in bytes.</span></span> <span data-ttu-id="fbc14-149">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="fbc14-149">Read-only</span></span>|
|<span data-ttu-id="fbc14-150">deviceCount</span><span class="sxs-lookup"><span data-stu-id="fbc14-150">deviceCount</span></span>|<span data-ttu-id="fbc14-151">Int32</span><span class="sxs-lookup"><span data-stu-id="fbc14-151">Int32</span></span>|<span data-ttu-id="fbc14-152">O número de dispositivos que instalaram esse aplicativo</span><span class="sxs-lookup"><span data-stu-id="fbc14-152">The number of devices that have installed this application</span></span>|

## <a name="relationships"></a><span data-ttu-id="fbc14-153">Relações</span><span class="sxs-lookup"><span data-stu-id="fbc14-153">Relationships</span></span>
|<span data-ttu-id="fbc14-154">Relação</span><span class="sxs-lookup"><span data-stu-id="fbc14-154">Relationship</span></span>|<span data-ttu-id="fbc14-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbc14-155">Type</span></span>|<span data-ttu-id="fbc14-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbc14-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbc14-157">managedDevices</span><span class="sxs-lookup"><span data-stu-id="fbc14-157">managedDevices</span></span>|<span data-ttu-id="fbc14-158">Coleção [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="fbc14-158">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="fbc14-159">Os dispositivos que descobriram o aplicativo instalado</span><span class="sxs-lookup"><span data-stu-id="fbc14-159">The devices that have the discovered application installed</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fbc14-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fbc14-160">JSON Representation</span></span>
<span data-ttu-id="fbc14-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fbc14-161">Here is a JSON representation of the resource.</span></span>
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






