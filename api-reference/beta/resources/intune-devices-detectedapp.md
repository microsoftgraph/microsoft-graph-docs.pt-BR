---
title: Tipo de recurso detectedApp
description: Um aplicativo gerenciado ou não gerenciado que está instalado em um dispositivo gerenciado. Aplicativos não gerenciados só aparecerão para dispositivos marcados como controlados pela empresa.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 01233111e74da95f84d0cbeb81e4675a5c6e049d
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31773193"
---
# <a name="detectedapp-resource-type"></a><span data-ttu-id="a60ff-104">Tipo de recurso detectedApp</span><span class="sxs-lookup"><span data-stu-id="a60ff-104">detectedApp resource type</span></span>

> <span data-ttu-id="a60ff-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a60ff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a60ff-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a60ff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a60ff-107">Um aplicativo gerenciado ou não gerenciado que está instalado em um dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="a60ff-107">A managed or unmanaged app that is installed on a managed device.</span></span> <span data-ttu-id="a60ff-108">Aplicativos não gerenciados só aparecerão para dispositivos marcados como controlados pela empresa.</span><span class="sxs-lookup"><span data-stu-id="a60ff-108">Unmanaged apps will only appear for devices marked as corporate owned.</span></span>

## <a name="methods"></a><span data-ttu-id="a60ff-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="a60ff-109">Methods</span></span>
|<span data-ttu-id="a60ff-110">Método</span><span class="sxs-lookup"><span data-stu-id="a60ff-110">Method</span></span>|<span data-ttu-id="a60ff-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a60ff-111">Return Type</span></span>|<span data-ttu-id="a60ff-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="a60ff-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a60ff-113">Listar detectedApps</span><span class="sxs-lookup"><span data-stu-id="a60ff-113">List detectedApps</span></span>](../api/intune-devices-detectedapp-list.md)|<span data-ttu-id="a60ff-114">Coleção [detectedApp](../resources/intune-devices-detectedapp.md)</span><span class="sxs-lookup"><span data-stu-id="a60ff-114">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="a60ff-115">Lista propriedades e relações dos objetos [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="a60ff-115">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>|
|[<span data-ttu-id="a60ff-116">Get detectedApp</span><span class="sxs-lookup"><span data-stu-id="a60ff-116">Get detectedApp</span></span>](../api/intune-devices-detectedapp-get.md)|[<span data-ttu-id="a60ff-117">detectedApp</span><span class="sxs-lookup"><span data-stu-id="a60ff-117">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="a60ff-118">Ler propriedades e relações do objeto [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="a60ff-118">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="a60ff-119">Criar detectedApp</span><span class="sxs-lookup"><span data-stu-id="a60ff-119">Create detectedApp</span></span>](../api/intune-devices-detectedapp-create.md)|[<span data-ttu-id="a60ff-120">detectedApp</span><span class="sxs-lookup"><span data-stu-id="a60ff-120">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="a60ff-121">Criar um novo objeto [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="a60ff-121">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="a60ff-122">Excluir detectedApp</span><span class="sxs-lookup"><span data-stu-id="a60ff-122">Delete detectedApp</span></span>](../api/intune-devices-detectedapp-delete.md)|<span data-ttu-id="a60ff-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a60ff-123">None</span></span>|<span data-ttu-id="a60ff-124">Exclui um [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="a60ff-124">Deletes a [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>|
|[<span data-ttu-id="a60ff-125">Atualizar detectedApp</span><span class="sxs-lookup"><span data-stu-id="a60ff-125">Update detectedApp</span></span>](../api/intune-devices-detectedapp-update.md)|[<span data-ttu-id="a60ff-126">detectedApp</span><span class="sxs-lookup"><span data-stu-id="a60ff-126">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="a60ff-127">Atualiza as propriedades de um objeto [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="a60ff-127">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a60ff-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a60ff-128">Properties</span></span>
|<span data-ttu-id="a60ff-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a60ff-129">Property</span></span>|<span data-ttu-id="a60ff-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a60ff-130">Type</span></span>|<span data-ttu-id="a60ff-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a60ff-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a60ff-132">id</span><span class="sxs-lookup"><span data-stu-id="a60ff-132">id</span></span>|<span data-ttu-id="a60ff-133">String</span><span class="sxs-lookup"><span data-stu-id="a60ff-133">String</span></span>|<span data-ttu-id="a60ff-134">O identificador exclusivo do aplicativo detectado.</span><span class="sxs-lookup"><span data-stu-id="a60ff-134">The unique Identifier for the detected application.</span></span> <span data-ttu-id="a60ff-135">Ele é gerado automaticamente pelo Intune no momento em que o aplicativo é criado.</span><span class="sxs-lookup"><span data-stu-id="a60ff-135">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="a60ff-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a60ff-136">Read-only.</span></span>|
|<span data-ttu-id="a60ff-137">displayName</span><span class="sxs-lookup"><span data-stu-id="a60ff-137">displayName</span></span>|<span data-ttu-id="a60ff-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a60ff-138">String</span></span>|<span data-ttu-id="a60ff-139">Nome do aplicativo descoberto.</span><span class="sxs-lookup"><span data-stu-id="a60ff-139">Name of the discovered application.</span></span> <span data-ttu-id="a60ff-140">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="a60ff-140">Read-only</span></span>|
|<span data-ttu-id="a60ff-141">version</span><span class="sxs-lookup"><span data-stu-id="a60ff-141">version</span></span>|<span data-ttu-id="a60ff-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a60ff-142">String</span></span>|<span data-ttu-id="a60ff-143">Versão do aplicativo descoberto.</span><span class="sxs-lookup"><span data-stu-id="a60ff-143">Version of the discovered application.</span></span> <span data-ttu-id="a60ff-144">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="a60ff-144">Read-only</span></span>|
|<span data-ttu-id="a60ff-145">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="a60ff-145">sizeInByte</span></span>|<span data-ttu-id="a60ff-146">Int64</span><span class="sxs-lookup"><span data-stu-id="a60ff-146">Int64</span></span>|<span data-ttu-id="a60ff-147">Tamanho do aplicativo descoberto, em bytes.</span><span class="sxs-lookup"><span data-stu-id="a60ff-147">Discovered application size in bytes.</span></span> <span data-ttu-id="a60ff-148">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="a60ff-148">Read-only</span></span>|
|<span data-ttu-id="a60ff-149">deviceCount</span><span class="sxs-lookup"><span data-stu-id="a60ff-149">deviceCount</span></span>|<span data-ttu-id="a60ff-150">Int32</span><span class="sxs-lookup"><span data-stu-id="a60ff-150">Int32</span></span>|<span data-ttu-id="a60ff-151">O número de dispositivos que instalaram esse aplicativo</span><span class="sxs-lookup"><span data-stu-id="a60ff-151">The number of devices that have installed this application</span></span>|

## <a name="relationships"></a><span data-ttu-id="a60ff-152">Relações</span><span class="sxs-lookup"><span data-stu-id="a60ff-152">Relationships</span></span>
|<span data-ttu-id="a60ff-153">Relação</span><span class="sxs-lookup"><span data-stu-id="a60ff-153">Relationship</span></span>|<span data-ttu-id="a60ff-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="a60ff-154">Type</span></span>|<span data-ttu-id="a60ff-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="a60ff-155">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a60ff-156">managedDevices</span><span class="sxs-lookup"><span data-stu-id="a60ff-156">managedDevices</span></span>|<span data-ttu-id="a60ff-157">Coleção [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="a60ff-157">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="a60ff-158">Os dispositivos que descobriram o aplicativo instalado</span><span class="sxs-lookup"><span data-stu-id="a60ff-158">The devices that have the discovered application installed</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a60ff-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a60ff-159">JSON Representation</span></span>
<span data-ttu-id="a60ff-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a60ff-160">Here is a JSON representation of the resource.</span></span>
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





