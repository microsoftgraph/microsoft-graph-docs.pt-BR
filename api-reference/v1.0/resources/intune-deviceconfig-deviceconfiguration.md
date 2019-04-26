---
title: Tipo de recurso deviceConfiguration
description: Configuração do dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2a3d0ecc27fc0fe29ed2ed3ca4080e3fea70d264
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32560785"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="f799c-103">Tipo de recurso deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="f799c-103">deviceConfiguration resource type</span></span>

> <span data-ttu-id="f799c-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f799c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f799c-105">Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f799c-105">Device Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="f799c-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="f799c-106">Methods</span></span>
|<span data-ttu-id="f799c-107">Método</span><span class="sxs-lookup"><span data-stu-id="f799c-107">Method</span></span>|<span data-ttu-id="f799c-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f799c-108">Return Type</span></span>|<span data-ttu-id="f799c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f799c-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f799c-110">Listar deviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="f799c-110">List deviceConfigurations</span></span>](../api/intune-deviceconfig-deviceconfiguration-list.md)|<span data-ttu-id="f799c-111">Conjunto [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f799c-111">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="f799c-112">Listar propriedades e relações de objetos de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f799c-112">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="f799c-113">Obter deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="f799c-113">Get deviceConfiguration</span></span>](../api/intune-deviceconfig-deviceconfiguration-get.md)|[<span data-ttu-id="f799c-114">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="f799c-114">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="f799c-115">Ler propriedades e relações de objetos de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f799c-115">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="f799c-116">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="f799c-116">assign action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assign.md)|<span data-ttu-id="f799c-117">Conjunto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f799c-117">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="f799c-118">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f799c-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="f799c-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f799c-119">Properties</span></span>
|<span data-ttu-id="f799c-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f799c-120">Property</span></span>|<span data-ttu-id="f799c-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="f799c-121">Type</span></span>|<span data-ttu-id="f799c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f799c-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f799c-123">id</span><span class="sxs-lookup"><span data-stu-id="f799c-123">id</span></span>|<span data-ttu-id="f799c-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f799c-124">String</span></span>|<span data-ttu-id="f799c-125">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f799c-125">Key of the entity.</span></span>|
|<span data-ttu-id="f799c-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f799c-126">lastModifiedDateTime</span></span>|<span data-ttu-id="f799c-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f799c-127">DateTimeOffset</span></span>|<span data-ttu-id="f799c-128">Última modificação de DateTime do objeto.</span><span class="sxs-lookup"><span data-stu-id="f799c-128">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="f799c-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f799c-129">createdDateTime</span></span>|<span data-ttu-id="f799c-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f799c-130">DateTimeOffset</span></span>|<span data-ttu-id="f799c-131">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f799c-131">DateTime the object was created.</span></span>|
|<span data-ttu-id="f799c-132">description</span><span class="sxs-lookup"><span data-stu-id="f799c-132">description</span></span>|<span data-ttu-id="f799c-133">String</span><span class="sxs-lookup"><span data-stu-id="f799c-133">String</span></span>|<span data-ttu-id="f799c-134">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f799c-134">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="f799c-135">displayName</span><span class="sxs-lookup"><span data-stu-id="f799c-135">displayName</span></span>|<span data-ttu-id="f799c-136">String</span><span class="sxs-lookup"><span data-stu-id="f799c-136">String</span></span>|<span data-ttu-id="f799c-137">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f799c-137">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="f799c-138">versão</span><span class="sxs-lookup"><span data-stu-id="f799c-138">version</span></span>|<span data-ttu-id="f799c-139">Int32</span><span class="sxs-lookup"><span data-stu-id="f799c-139">Int32</span></span>|<span data-ttu-id="f799c-140">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f799c-140">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f799c-141">Relações</span><span class="sxs-lookup"><span data-stu-id="f799c-141">Relationships</span></span>
|<span data-ttu-id="f799c-142">Relação</span><span class="sxs-lookup"><span data-stu-id="f799c-142">Relationship</span></span>|<span data-ttu-id="f799c-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="f799c-143">Type</span></span>|<span data-ttu-id="f799c-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="f799c-144">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f799c-145">assignments</span><span class="sxs-lookup"><span data-stu-id="f799c-145">assignments</span></span>|<span data-ttu-id="f799c-146">Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f799c-146">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="f799c-147">A lista de atribuições para o perfil de configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f799c-147">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="f799c-148">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="f799c-148">deviceStatuses</span></span>|<span data-ttu-id="f799c-149">Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="f799c-149">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="f799c-150">Status de instalação da configuração de dispositivo por dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f799c-150">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="f799c-151">userStatuses</span><span class="sxs-lookup"><span data-stu-id="f799c-151">userStatuses</span></span>|<span data-ttu-id="f799c-152">Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="f799c-152">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="f799c-153">Status de instalação da configuração do dispositivo por usuário.</span><span class="sxs-lookup"><span data-stu-id="f799c-153">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="f799c-154">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="f799c-154">deviceStatusOverview</span></span>|[<span data-ttu-id="f799c-155">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="f799c-155">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="f799c-156">Visão geral do status dos dispositivos da configuração de dispositivos</span><span class="sxs-lookup"><span data-stu-id="f799c-156">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="f799c-157">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="f799c-157">userStatusOverview</span></span>|[<span data-ttu-id="f799c-158">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="f799c-158">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="f799c-159">Visão geral do status dos usuários da configuração de dispositivos</span><span class="sxs-lookup"><span data-stu-id="f799c-159">Device Configuration users status overview</span></span>|
|<span data-ttu-id="f799c-160">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="f799c-160">deviceSettingStateSummaries</span></span>|<span data-ttu-id="f799c-161">Conjunto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="f799c-161">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="f799c-162">Resumo do dispositivo do estado de definição de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="f799c-162">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f799c-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f799c-163">JSON Representation</span></span>
<span data-ttu-id="f799c-164">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f799c-164">Here is a JSON representation of the resource.</span></span>
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



