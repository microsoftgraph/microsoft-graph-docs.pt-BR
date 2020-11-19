---
title: Tipo de recurso detectedApp
description: Um aplicativo gerenciado ou não gerenciado que está instalado em um dispositivo gerenciado. Aplicativos não gerenciados só aparecerão para dispositivos marcados como controlados pela empresa.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bfd569086784964a7685ab6b5f174cefd906c2f7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49267758"
---
# <a name="detectedapp-resource-type"></a><span data-ttu-id="7056f-104">Tipo de recurso detectedApp</span><span class="sxs-lookup"><span data-stu-id="7056f-104">detectedApp resource type</span></span>

<span data-ttu-id="7056f-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7056f-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7056f-106">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7056f-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7056f-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7056f-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7056f-108">Um aplicativo gerenciado ou não gerenciado que está instalado em um dispositivo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="7056f-108">A managed or unmanaged app that is installed on a managed device.</span></span> <span data-ttu-id="7056f-109">Aplicativos não gerenciados só aparecerão para dispositivos marcados como controlados pela empresa.</span><span class="sxs-lookup"><span data-stu-id="7056f-109">Unmanaged apps will only appear for devices marked as corporate owned.</span></span>

## <a name="methods"></a><span data-ttu-id="7056f-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="7056f-110">Methods</span></span>
|<span data-ttu-id="7056f-111">Método</span><span class="sxs-lookup"><span data-stu-id="7056f-111">Method</span></span>|<span data-ttu-id="7056f-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7056f-112">Return Type</span></span>|<span data-ttu-id="7056f-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="7056f-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7056f-114">Listar detectedApps</span><span class="sxs-lookup"><span data-stu-id="7056f-114">List detectedApps</span></span>](../api/intune-devices-detectedapp-list.md)|<span data-ttu-id="7056f-115">Coleção [detectedApp](../resources/intune-devices-detectedapp.md)</span><span class="sxs-lookup"><span data-stu-id="7056f-115">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="7056f-116">Lista propriedades e relações dos objetos [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="7056f-116">List properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) objects.</span></span>|
|[<span data-ttu-id="7056f-117">Obter detectedApp</span><span class="sxs-lookup"><span data-stu-id="7056f-117">Get detectedApp</span></span>](../api/intune-devices-detectedapp-get.md)|[<span data-ttu-id="7056f-118">detectedApp</span><span class="sxs-lookup"><span data-stu-id="7056f-118">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="7056f-119">Propriedades de leitura e relações do objeto [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="7056f-119">Read properties and relationships of the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="7056f-120">Criar detectedApp</span><span class="sxs-lookup"><span data-stu-id="7056f-120">Create detectedApp</span></span>](../api/intune-devices-detectedapp-create.md)|[<span data-ttu-id="7056f-121">detectedApp</span><span class="sxs-lookup"><span data-stu-id="7056f-121">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="7056f-122">Cria um novo objeto [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="7056f-122">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|
|[<span data-ttu-id="7056f-123">Excluir detectedApp</span><span class="sxs-lookup"><span data-stu-id="7056f-123">Delete detectedApp</span></span>](../api/intune-devices-detectedapp-delete.md)|<span data-ttu-id="7056f-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7056f-124">None</span></span>|<span data-ttu-id="7056f-125">Exclui um [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="7056f-125">Deletes a [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>|
|[<span data-ttu-id="7056f-126">Atualizar detectedApp</span><span class="sxs-lookup"><span data-stu-id="7056f-126">Update detectedApp</span></span>](../api/intune-devices-detectedapp-update.md)|[<span data-ttu-id="7056f-127">detectedApp</span><span class="sxs-lookup"><span data-stu-id="7056f-127">detectedApp</span></span>](../resources/intune-devices-detectedapp.md)|<span data-ttu-id="7056f-128">Atualiza as propriedades de um objeto [detectedApp](../resources/intune-devices-detectedapp.md).</span><span class="sxs-lookup"><span data-stu-id="7056f-128">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7056f-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7056f-129">Properties</span></span>
|<span data-ttu-id="7056f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7056f-130">Property</span></span>|<span data-ttu-id="7056f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7056f-131">Type</span></span>|<span data-ttu-id="7056f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7056f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7056f-133">id</span><span class="sxs-lookup"><span data-stu-id="7056f-133">id</span></span>|<span data-ttu-id="7056f-134">String</span><span class="sxs-lookup"><span data-stu-id="7056f-134">String</span></span>|<span data-ttu-id="7056f-135">O identificador exclusivo do aplicativo detectado.</span><span class="sxs-lookup"><span data-stu-id="7056f-135">The unique Identifier for the detected application.</span></span> <span data-ttu-id="7056f-136">Ele é gerado automaticamente pelo Intune no momento em que o aplicativo é criado.</span><span class="sxs-lookup"><span data-stu-id="7056f-136">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="7056f-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7056f-137">Read-only.</span></span>|
|<span data-ttu-id="7056f-138">displayName</span><span class="sxs-lookup"><span data-stu-id="7056f-138">displayName</span></span>|<span data-ttu-id="7056f-139">String</span><span class="sxs-lookup"><span data-stu-id="7056f-139">String</span></span>|<span data-ttu-id="7056f-140">Nome do aplicativo descoberto.</span><span class="sxs-lookup"><span data-stu-id="7056f-140">Name of the discovered application.</span></span> <span data-ttu-id="7056f-141">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="7056f-141">Read-only</span></span>|
|<span data-ttu-id="7056f-142">version</span><span class="sxs-lookup"><span data-stu-id="7056f-142">version</span></span>|<span data-ttu-id="7056f-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7056f-143">String</span></span>|<span data-ttu-id="7056f-144">Versão do aplicativo descoberto.</span><span class="sxs-lookup"><span data-stu-id="7056f-144">Version of the discovered application.</span></span> <span data-ttu-id="7056f-145">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="7056f-145">Read-only</span></span>|
|<span data-ttu-id="7056f-146">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="7056f-146">sizeInByte</span></span>|<span data-ttu-id="7056f-147">Int64</span><span class="sxs-lookup"><span data-stu-id="7056f-147">Int64</span></span>|<span data-ttu-id="7056f-148">Tamanho do aplicativo descoberto, em bytes.</span><span class="sxs-lookup"><span data-stu-id="7056f-148">Discovered application size in bytes.</span></span> <span data-ttu-id="7056f-149">Somente leitura</span><span class="sxs-lookup"><span data-stu-id="7056f-149">Read-only</span></span>|
|<span data-ttu-id="7056f-150">deviceCount</span><span class="sxs-lookup"><span data-stu-id="7056f-150">deviceCount</span></span>|<span data-ttu-id="7056f-151">Int32</span><span class="sxs-lookup"><span data-stu-id="7056f-151">Int32</span></span>|<span data-ttu-id="7056f-152">O número de dispositivos que instalaram esse aplicativo</span><span class="sxs-lookup"><span data-stu-id="7056f-152">The number of devices that have installed this application</span></span>|

## <a name="relationships"></a><span data-ttu-id="7056f-153">Relações</span><span class="sxs-lookup"><span data-stu-id="7056f-153">Relationships</span></span>
|<span data-ttu-id="7056f-154">Relação</span><span class="sxs-lookup"><span data-stu-id="7056f-154">Relationship</span></span>|<span data-ttu-id="7056f-155">Tipo</span><span class="sxs-lookup"><span data-stu-id="7056f-155">Type</span></span>|<span data-ttu-id="7056f-156">Descrição</span><span class="sxs-lookup"><span data-stu-id="7056f-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7056f-157">managedDevices</span><span class="sxs-lookup"><span data-stu-id="7056f-157">managedDevices</span></span>|<span data-ttu-id="7056f-158">Coleção [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="7056f-158">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="7056f-159">Os dispositivos que descobriram o aplicativo instalado</span><span class="sxs-lookup"><span data-stu-id="7056f-159">The devices that have the discovered application installed</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7056f-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7056f-160">JSON Representation</span></span>
<span data-ttu-id="7056f-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7056f-161">Here is a JSON representation of the resource.</span></span>
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




