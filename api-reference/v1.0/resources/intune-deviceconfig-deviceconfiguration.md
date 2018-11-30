---
title: Tipo de recurso deviceConfiguration
description: Configuração do dispositivo.
ms.openlocfilehash: 7cde579aa9d2e096380286d628a9964d4522f402
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007554"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="0c7c2-103">Tipo de recurso deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="0c7c2-103">deviceConfiguration resource type</span></span>

> <span data-ttu-id="0c7c2-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0c7c2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0c7c2-105">Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0c7c2-105">Device Configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="0c7c2-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="0c7c2-106">Methods</span></span>
|<span data-ttu-id="0c7c2-107">Método</span><span class="sxs-lookup"><span data-stu-id="0c7c2-107">Method</span></span>|<span data-ttu-id="0c7c2-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0c7c2-108">Return Type</span></span>|<span data-ttu-id="0c7c2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c7c2-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0c7c2-110">Listar deviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="0c7c2-110">List deviceConfigurations</span></span>](../api/intune-deviceconfig-deviceconfiguration-list.md)|<span data-ttu-id="0c7c2-111">Conjunto [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0c7c2-111">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="0c7c2-112">Listar propriedades e relações de objetos de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0c7c2-112">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="0c7c2-113">Obter deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="0c7c2-113">Get deviceConfiguration</span></span>](../api/intune-deviceconfig-deviceconfiguration-get.md)|[<span data-ttu-id="0c7c2-114">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="0c7c2-114">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="0c7c2-115">Ler propriedades e relações de objetos de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0c7c2-115">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="0c7c2-116">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="0c7c2-116">assign action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assign.md)|<span data-ttu-id="0c7c2-117">Conjunto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="0c7c2-117">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="0c7c2-118">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0c7c2-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="0c7c2-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0c7c2-119">Properties</span></span>
|<span data-ttu-id="0c7c2-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c7c2-120">Property</span></span>|<span data-ttu-id="0c7c2-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c7c2-121">Type</span></span>|<span data-ttu-id="0c7c2-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c7c2-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c7c2-123">id</span><span class="sxs-lookup"><span data-stu-id="0c7c2-123">id</span></span>|<span data-ttu-id="0c7c2-124">String</span><span class="sxs-lookup"><span data-stu-id="0c7c2-124">String</span></span>|<span data-ttu-id="0c7c2-125">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0c7c2-125">Key of the entity.</span></span>|
|<span data-ttu-id="0c7c2-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0c7c2-126">lastModifiedDateTime</span></span>|<span data-ttu-id="0c7c2-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c7c2-127">DateTimeOffset</span></span>|<span data-ttu-id="0c7c2-128">Última modificação de DateTime do objeto.</span><span class="sxs-lookup"><span data-stu-id="0c7c2-128">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="0c7c2-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0c7c2-129">createdDateTime</span></span>|<span data-ttu-id="0c7c2-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c7c2-130">DateTimeOffset</span></span>|<span data-ttu-id="0c7c2-131">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="0c7c2-131">DateTime the object was created.</span></span>|
|<span data-ttu-id="0c7c2-132">description</span><span class="sxs-lookup"><span data-stu-id="0c7c2-132">description</span></span>|<span data-ttu-id="0c7c2-133">String</span><span class="sxs-lookup"><span data-stu-id="0c7c2-133">String</span></span>|<span data-ttu-id="0c7c2-134">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0c7c2-134">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="0c7c2-135">displayName</span><span class="sxs-lookup"><span data-stu-id="0c7c2-135">displayName</span></span>|<span data-ttu-id="0c7c2-136">String</span><span class="sxs-lookup"><span data-stu-id="0c7c2-136">String</span></span>|<span data-ttu-id="0c7c2-137">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0c7c2-137">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="0c7c2-138">version</span><span class="sxs-lookup"><span data-stu-id="0c7c2-138">version</span></span>|<span data-ttu-id="0c7c2-139">Int32</span><span class="sxs-lookup"><span data-stu-id="0c7c2-139">Int32</span></span>|<span data-ttu-id="0c7c2-140">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0c7c2-140">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c7c2-141">Relações</span><span class="sxs-lookup"><span data-stu-id="0c7c2-141">Relationships</span></span>
|<span data-ttu-id="0c7c2-142">Relação</span><span class="sxs-lookup"><span data-stu-id="0c7c2-142">Relationship</span></span>|<span data-ttu-id="0c7c2-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c7c2-143">Type</span></span>|<span data-ttu-id="0c7c2-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c7c2-144">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c7c2-145">assignments</span><span class="sxs-lookup"><span data-stu-id="0c7c2-145">assignments</span></span>|<span data-ttu-id="0c7c2-146">Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="0c7c2-146">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="0c7c2-147">A lista de atribuições para o perfil de configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0c7c2-147">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="0c7c2-148">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="0c7c2-148">deviceStatuses</span></span>|<span data-ttu-id="0c7c2-149">Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="0c7c2-149">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="0c7c2-150">Status de instalação da configuração de dispositivo por dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0c7c2-150">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="0c7c2-151">userStatuses</span><span class="sxs-lookup"><span data-stu-id="0c7c2-151">userStatuses</span></span>|<span data-ttu-id="0c7c2-152">Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="0c7c2-152">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="0c7c2-153">Status de instalação da configuração de dispositivo por usuário.</span><span class="sxs-lookup"><span data-stu-id="0c7c2-153">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="0c7c2-154">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="0c7c2-154">deviceStatusOverview</span></span>|[<span data-ttu-id="0c7c2-155">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="0c7c2-155">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="0c7c2-156">Visão geral do status dos dispositivos da configuração de dispositivos</span><span class="sxs-lookup"><span data-stu-id="0c7c2-156">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="0c7c2-157">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="0c7c2-157">userStatusOverview</span></span>|[<span data-ttu-id="0c7c2-158">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="0c7c2-158">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="0c7c2-159">Visão geral do status dos usuários da configuração de dispositivos</span><span class="sxs-lookup"><span data-stu-id="0c7c2-159">Device Configuration users status overview</span></span>|
|<span data-ttu-id="0c7c2-160">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="0c7c2-160">deviceSettingStateSummaries</span></span>|<span data-ttu-id="0c7c2-161">Conjunto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="0c7c2-161">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="0c7c2-162">Resumo do dispositivo do estado de definição de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="0c7c2-162">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0c7c2-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0c7c2-163">JSON Representation</span></span>
<span data-ttu-id="0c7c2-164">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0c7c2-164">Here is a JSON representation of the resource.</span></span>
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



