---
title: Tipo de recurso deviceConfiguration
description: Configuração do dispositivo.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 255826460a81544d27620807d569ce3857e1034e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884039"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="bad90-103">Tipo de recurso deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="bad90-103">deviceConfiguration resource type</span></span>

> <span data-ttu-id="bad90-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bad90-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bad90-105">Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bad90-105">Device Configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="bad90-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="bad90-106">Methods</span></span>
|<span data-ttu-id="bad90-107">Método</span><span class="sxs-lookup"><span data-stu-id="bad90-107">Method</span></span>|<span data-ttu-id="bad90-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bad90-108">Return Type</span></span>|<span data-ttu-id="bad90-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="bad90-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bad90-110">Listar deviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="bad90-110">List deviceConfigurations</span></span>](../api/intune-deviceconfig-deviceconfiguration-list.md)|<span data-ttu-id="bad90-111">Conjunto [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bad90-111">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="bad90-112">Listar propriedades e relações de objetos de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bad90-112">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="bad90-113">Obter deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="bad90-113">Get deviceConfiguration</span></span>](../api/intune-deviceconfig-deviceconfiguration-get.md)|[<span data-ttu-id="bad90-114">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="bad90-114">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="bad90-115">Ler propriedades e relações de objetos de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bad90-115">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="bad90-116">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="bad90-116">assign action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assign.md)|<span data-ttu-id="bad90-117">Conjunto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="bad90-117">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="bad90-118">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="bad90-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="bad90-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bad90-119">Properties</span></span>
|<span data-ttu-id="bad90-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bad90-120">Property</span></span>|<span data-ttu-id="bad90-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="bad90-121">Type</span></span>|<span data-ttu-id="bad90-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="bad90-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bad90-123">id</span><span class="sxs-lookup"><span data-stu-id="bad90-123">id</span></span>|<span data-ttu-id="bad90-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bad90-124">String</span></span>|<span data-ttu-id="bad90-125">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bad90-125">Key of the entity.</span></span>|
|<span data-ttu-id="bad90-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bad90-126">lastModifiedDateTime</span></span>|<span data-ttu-id="bad90-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bad90-127">DateTimeOffset</span></span>|<span data-ttu-id="bad90-128">Última modificação de DateTime do objeto.</span><span class="sxs-lookup"><span data-stu-id="bad90-128">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="bad90-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bad90-129">createdDateTime</span></span>|<span data-ttu-id="bad90-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bad90-130">DateTimeOffset</span></span>|<span data-ttu-id="bad90-131">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="bad90-131">DateTime the object was created.</span></span>|
|<span data-ttu-id="bad90-132">description</span><span class="sxs-lookup"><span data-stu-id="bad90-132">description</span></span>|<span data-ttu-id="bad90-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bad90-133">String</span></span>|<span data-ttu-id="bad90-134">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bad90-134">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="bad90-135">displayName</span><span class="sxs-lookup"><span data-stu-id="bad90-135">displayName</span></span>|<span data-ttu-id="bad90-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bad90-136">String</span></span>|<span data-ttu-id="bad90-137">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bad90-137">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="bad90-138">version</span><span class="sxs-lookup"><span data-stu-id="bad90-138">version</span></span>|<span data-ttu-id="bad90-139">Int32</span><span class="sxs-lookup"><span data-stu-id="bad90-139">Int32</span></span>|<span data-ttu-id="bad90-140">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bad90-140">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bad90-141">Relações</span><span class="sxs-lookup"><span data-stu-id="bad90-141">Relationships</span></span>
|<span data-ttu-id="bad90-142">Relação</span><span class="sxs-lookup"><span data-stu-id="bad90-142">Relationship</span></span>|<span data-ttu-id="bad90-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="bad90-143">Type</span></span>|<span data-ttu-id="bad90-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="bad90-144">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bad90-145">assignments</span><span class="sxs-lookup"><span data-stu-id="bad90-145">assignments</span></span>|<span data-ttu-id="bad90-146">Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="bad90-146">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="bad90-147">A lista de atribuições para o perfil de configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bad90-147">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="bad90-148">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="bad90-148">deviceStatuses</span></span>|<span data-ttu-id="bad90-149">Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="bad90-149">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="bad90-150">Status de instalação da configuração de dispositivo por dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bad90-150">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="bad90-151">userStatuses</span><span class="sxs-lookup"><span data-stu-id="bad90-151">userStatuses</span></span>|<span data-ttu-id="bad90-152">Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="bad90-152">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="bad90-153">Status de instalação da configuração de dispositivo por usuário.</span><span class="sxs-lookup"><span data-stu-id="bad90-153">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="bad90-154">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="bad90-154">deviceStatusOverview</span></span>|[<span data-ttu-id="bad90-155">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="bad90-155">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="bad90-156">Visão geral do status dos dispositivos da configuração de dispositivos</span><span class="sxs-lookup"><span data-stu-id="bad90-156">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="bad90-157">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="bad90-157">userStatusOverview</span></span>|[<span data-ttu-id="bad90-158">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="bad90-158">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="bad90-159">Visão geral do status dos usuários da configuração de dispositivos</span><span class="sxs-lookup"><span data-stu-id="bad90-159">Device Configuration users status overview</span></span>|
|<span data-ttu-id="bad90-160">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="bad90-160">deviceSettingStateSummaries</span></span>|<span data-ttu-id="bad90-161">Conjunto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="bad90-161">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="bad90-162">Resumo do dispositivo do estado de definição de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="bad90-162">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bad90-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bad90-163">JSON Representation</span></span>
<span data-ttu-id="bad90-164">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bad90-164">Here is a JSON representation of the resource.</span></span>
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



