---
title: Tipo de recurso detectedApp
description: Um aplicativo gerenciado ou não gerenciado que está instalado em um dispositivo gerenciado. Aplicativos não gerenciados só aparecerão para dispositivos marcados como controlados pela empresa.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8b28965cb506075c8caf7d983ddf41eafcdda78d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27881421"
---
# <a name="detectedapp-resource-type"></a><span data-ttu-id="2ba4e-104">Tipo de recurso detectedApp</span><span class="sxs-lookup"><span data-stu-id="2ba4e-104">detectedApp resource type</span></span>

> <span data-ttu-id="2ba4e-105">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2ba4e-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2ba4e-106">Um aplicativo gerenciado ou não gerenciado que está instalado em um dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="2ba4e-106">A managed or unmanaged app that is installed on a managed device.</span></span> <span data-ttu-id="2ba4e-107">Aplicativos não gerenciados só aparecerão para dispositivos marcados como controlados pela empresa.</span><span class="sxs-lookup"><span data-stu-id="2ba4e-107">Unmanaged apps will only appear for devices marked as corporate owned.</span></span>
## <a name="methods"></a><span data-ttu-id="2ba4e-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="2ba4e-108">Methods</span></span>
|<span data-ttu-id="2ba4e-109">Método</span><span class="sxs-lookup"><span data-stu-id="2ba4e-109">Method</span></span>|<span data-ttu-id="2ba4e-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2ba4e-110">Return Type</span></span>|<span data-ttu-id="2ba4e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ba4e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2ba4e-112">Listar detectedApps</span><span class="sxs-lookup"><span data-stu-id="2ba4e-112">List detectedApps</span></span>](../api/intune-devices-detectedapp-list.md)|<span data-ttu-id="2ba4e-113">Coleção [detectedApp](../resources/intune-devices-detectedapp.md)</span><span class="sxs-lookup"><span data-stu-id="2ba4e-113">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="2ba4e-114">Lista propriedades e relações dos objetos [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ba4e-114">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>|
|[<span data-ttu-id="2ba4e-115">Obter detectedApp</span><span class="sxs-lookup"><span data-stu-id="2ba4e-115">Get detectedApp</span></span>](../api/intune-devices-detectedapp-get.md)|[<span data-ttu-id="2ba4e-116">detectedApp</span><span class="sxs-lookup"><span data-stu-id="2ba4e-116">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="2ba4e-117">Propriedades de leitura e relações do objeto [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ba4e-117">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="2ba4e-118">Criar detectedApp</span><span class="sxs-lookup"><span data-stu-id="2ba4e-118">Create detectedApp</span></span>](../api/intune-devices-detectedapp-create.md)|[<span data-ttu-id="2ba4e-119">detectedApp</span><span class="sxs-lookup"><span data-stu-id="2ba4e-119">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="2ba4e-120">Cria um novo objeto [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ba4e-120">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="2ba4e-121">Excluir detectedApp</span><span class="sxs-lookup"><span data-stu-id="2ba4e-121">Delete detectedApp</span></span>](../api/intune-devices-detectedapp-delete.md)|<span data-ttu-id="2ba4e-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2ba4e-122">None</span></span>|<span data-ttu-id="2ba4e-123">Exclui um [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ba4e-123">Deletes a [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>|
|[<span data-ttu-id="2ba4e-124">Atualizar detectedApp</span><span class="sxs-lookup"><span data-stu-id="2ba4e-124">Update detectedApp</span></span>](../api/intune-devices-detectedapp-update.md)|[<span data-ttu-id="2ba4e-125">detectedApp</span><span class="sxs-lookup"><span data-stu-id="2ba4e-125">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="2ba4e-126">Atualiza as propriedades de um objeto [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="2ba4e-126">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2ba4e-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2ba4e-127">Properties</span></span>
|<span data-ttu-id="2ba4e-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ba4e-128">Property</span></span>|<span data-ttu-id="2ba4e-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ba4e-129">Type</span></span>|<span data-ttu-id="2ba4e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ba4e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ba4e-131">id</span><span class="sxs-lookup"><span data-stu-id="2ba4e-131">id</span></span>|<span data-ttu-id="2ba4e-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ba4e-132">String</span></span>|<span data-ttu-id="2ba4e-133">O identificador exclusivo do aplicativo detectado.</span><span class="sxs-lookup"><span data-stu-id="2ba4e-133">The unique Identifier for the detected application.</span></span> <span data-ttu-id="2ba4e-134">Ele é gerado automaticamente pelo Intune no momento em que o aplicativo é criado.</span><span class="sxs-lookup"><span data-stu-id="2ba4e-134">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="2ba4e-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2ba4e-135">Read-only.</span></span>|
|<span data-ttu-id="2ba4e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="2ba4e-136">displayName</span></span>|<span data-ttu-id="2ba4e-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ba4e-137">String</span></span>|<span data-ttu-id="2ba4e-138">Nome do aplicativo descoberto.</span><span class="sxs-lookup"><span data-stu-id="2ba4e-138">Name of the discovered application.</span></span> <span data-ttu-id="2ba4e-139">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="2ba4e-139">Read-only</span></span>|
|<span data-ttu-id="2ba4e-140">version</span><span class="sxs-lookup"><span data-stu-id="2ba4e-140">version</span></span>|<span data-ttu-id="2ba4e-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ba4e-141">String</span></span>|<span data-ttu-id="2ba4e-142">Versão do aplicativo descoberto.</span><span class="sxs-lookup"><span data-stu-id="2ba4e-142">Version of the discovered application.</span></span> <span data-ttu-id="2ba4e-143">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="2ba4e-143">Read-only</span></span>|
|<span data-ttu-id="2ba4e-144">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="2ba4e-144">sizeInByte</span></span>|<span data-ttu-id="2ba4e-145">Int64</span><span class="sxs-lookup"><span data-stu-id="2ba4e-145">Int64</span></span>|<span data-ttu-id="2ba4e-146">Tamanho do aplicativo descoberto, em bytes.</span><span class="sxs-lookup"><span data-stu-id="2ba4e-146">Discovered application size in bytes.</span></span> <span data-ttu-id="2ba4e-147">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="2ba4e-147">Read-only</span></span>|
|<span data-ttu-id="2ba4e-148">deviceCount</span><span class="sxs-lookup"><span data-stu-id="2ba4e-148">deviceCount</span></span>|<span data-ttu-id="2ba4e-149">Int32</span><span class="sxs-lookup"><span data-stu-id="2ba4e-149">Int32</span></span>|<span data-ttu-id="2ba4e-150">O número de dispositivos que instalaram esse aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ba4e-150">The number of devices that have installed this application</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ba4e-151">Relações</span><span class="sxs-lookup"><span data-stu-id="2ba4e-151">Relationships</span></span>
|<span data-ttu-id="2ba4e-152">Relação</span><span class="sxs-lookup"><span data-stu-id="2ba4e-152">Relationship</span></span>|<span data-ttu-id="2ba4e-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ba4e-153">Type</span></span>|<span data-ttu-id="2ba4e-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ba4e-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ba4e-155">managedDevices</span><span class="sxs-lookup"><span data-stu-id="2ba4e-155">managedDevices</span></span>|<span data-ttu-id="2ba4e-156">Coleção [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="2ba4e-156">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="2ba4e-157">Os dispositivos que descobriram o aplicativo instalado</span><span class="sxs-lookup"><span data-stu-id="2ba4e-157">The devices that have the discovered application installed</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2ba4e-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2ba4e-158">JSON Representation</span></span>
<span data-ttu-id="2ba4e-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2ba4e-159">Here is a JSON representation of the resource.</span></span>
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



