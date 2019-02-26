---
title: Tipo de recurso deviceConfiguration
description: Configuração do dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2a3d0ecc27fc0fe29ed2ed3ca4080e3fea70d264
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250492"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="66315-103">Tipo de recurso deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="66315-103">deviceConfiguration resource type</span></span>

> <span data-ttu-id="66315-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="66315-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66315-105">Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66315-105">Device Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="66315-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="66315-106">Methods</span></span>
|<span data-ttu-id="66315-107">Método</span><span class="sxs-lookup"><span data-stu-id="66315-107">Method</span></span>|<span data-ttu-id="66315-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="66315-108">Return Type</span></span>|<span data-ttu-id="66315-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="66315-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="66315-110">Listar deviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="66315-110">List deviceConfigurations</span></span>](../api/intune-deviceconfig-deviceconfiguration-list.md)|<span data-ttu-id="66315-111">Conjunto [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="66315-111">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="66315-112">Listar propriedades e relações de objetos de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="66315-112">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="66315-113">Obter deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="66315-113">Get deviceConfiguration</span></span>](../api/intune-deviceconfig-deviceconfiguration-get.md)|[<span data-ttu-id="66315-114">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="66315-114">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="66315-115">Ler propriedades e relações de objetos de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="66315-115">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="66315-116">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="66315-116">assign action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assign.md)|<span data-ttu-id="66315-117">Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="66315-117">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="66315-118">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="66315-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="66315-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="66315-119">Properties</span></span>
|<span data-ttu-id="66315-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="66315-120">Property</span></span>|<span data-ttu-id="66315-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="66315-121">Type</span></span>|<span data-ttu-id="66315-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="66315-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66315-123">id</span><span class="sxs-lookup"><span data-stu-id="66315-123">id</span></span>|<span data-ttu-id="66315-124">String</span><span class="sxs-lookup"><span data-stu-id="66315-124">String</span></span>|<span data-ttu-id="66315-125">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="66315-125">Key of the entity.</span></span>|
|<span data-ttu-id="66315-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="66315-126">lastModifiedDateTime</span></span>|<span data-ttu-id="66315-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66315-127">DateTimeOffset</span></span>|<span data-ttu-id="66315-128">Última modificação de DateTime do objeto.</span><span class="sxs-lookup"><span data-stu-id="66315-128">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="66315-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="66315-129">createdDateTime</span></span>|<span data-ttu-id="66315-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66315-130">DateTimeOffset</span></span>|<span data-ttu-id="66315-131">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="66315-131">DateTime the object was created.</span></span>|
|<span data-ttu-id="66315-132">description</span><span class="sxs-lookup"><span data-stu-id="66315-132">description</span></span>|<span data-ttu-id="66315-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="66315-133">String</span></span>|<span data-ttu-id="66315-134">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66315-134">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="66315-135">displayName</span><span class="sxs-lookup"><span data-stu-id="66315-135">displayName</span></span>|<span data-ttu-id="66315-136">String</span><span class="sxs-lookup"><span data-stu-id="66315-136">String</span></span>|<span data-ttu-id="66315-137">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66315-137">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="66315-138">version</span><span class="sxs-lookup"><span data-stu-id="66315-138">version</span></span>|<span data-ttu-id="66315-139">Int32</span><span class="sxs-lookup"><span data-stu-id="66315-139">Int32</span></span>|<span data-ttu-id="66315-140">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66315-140">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66315-141">Relações</span><span class="sxs-lookup"><span data-stu-id="66315-141">Relationships</span></span>
|<span data-ttu-id="66315-142">Relação</span><span class="sxs-lookup"><span data-stu-id="66315-142">Relationship</span></span>|<span data-ttu-id="66315-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="66315-143">Type</span></span>|<span data-ttu-id="66315-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="66315-144">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66315-145">assignments</span><span class="sxs-lookup"><span data-stu-id="66315-145">assignments</span></span>|<span data-ttu-id="66315-146">Conjunto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="66315-146">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="66315-147">A lista de atribuições para o perfil de configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66315-147">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="66315-148">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="66315-148">deviceStatuses</span></span>|<span data-ttu-id="66315-149">Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="66315-149">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="66315-150">Status de instalação da configuração de dispositivo por dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66315-150">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="66315-151">userStatuses</span><span class="sxs-lookup"><span data-stu-id="66315-151">userStatuses</span></span>|<span data-ttu-id="66315-152">Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="66315-152">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="66315-153">Status de instalação da configuração do dispositivo por usuário.</span><span class="sxs-lookup"><span data-stu-id="66315-153">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="66315-154">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="66315-154">deviceStatusOverview</span></span>|[<span data-ttu-id="66315-155">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="66315-155">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="66315-156">Visão geral do status dos dispositivos da configuração de dispositivos</span><span class="sxs-lookup"><span data-stu-id="66315-156">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="66315-157">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="66315-157">userStatusOverview</span></span>|[<span data-ttu-id="66315-158">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="66315-158">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="66315-159">Visão geral do status dos usuários da configuração de dispositivos</span><span class="sxs-lookup"><span data-stu-id="66315-159">Device Configuration users status overview</span></span>|
|<span data-ttu-id="66315-160">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="66315-160">deviceSettingStateSummaries</span></span>|<span data-ttu-id="66315-161">Conjunto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="66315-161">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="66315-162">Resumo do dispositivo do estado de definição de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="66315-162">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="66315-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="66315-163">JSON Representation</span></span>
<span data-ttu-id="66315-164">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="66315-164">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024
}
```



