---
title: Tipo de recurso deviceConfiguration
description: Configuração do dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b054e2472965f59d8350a52fe22134ab98e00fdf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028423"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="ea4ad-103">Tipo de recurso deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="ea4ad-103">deviceConfiguration resource type</span></span>

> <span data-ttu-id="ea4ad-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ea4ad-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea4ad-105">Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ea4ad-105">Device Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="ea4ad-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="ea4ad-106">Methods</span></span>
|<span data-ttu-id="ea4ad-107">Método</span><span class="sxs-lookup"><span data-stu-id="ea4ad-107">Method</span></span>|<span data-ttu-id="ea4ad-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ea4ad-108">Return Type</span></span>|<span data-ttu-id="ea4ad-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea4ad-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ea4ad-110">Listar deviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="ea4ad-110">List deviceConfigurations</span></span>](../api/intune-deviceconfig-deviceconfiguration-list.md)|<span data-ttu-id="ea4ad-111">Conjunto [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ea4ad-111">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="ea4ad-112">Listar propriedades e relações de objetos de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea4ad-112">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="ea4ad-113">Obter deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="ea4ad-113">Get deviceConfiguration</span></span>](../api/intune-deviceconfig-deviceconfiguration-get.md)|[<span data-ttu-id="ea4ad-114">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="ea4ad-114">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="ea4ad-115">Ler propriedades e relações de objetos de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="ea4ad-115">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="ea4ad-116">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="ea4ad-116">assign action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assign.md)|<span data-ttu-id="ea4ad-117">Conjunto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="ea4ad-117">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="ea4ad-118">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ea4ad-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="ea4ad-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ea4ad-119">Properties</span></span>
|<span data-ttu-id="ea4ad-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea4ad-120">Property</span></span>|<span data-ttu-id="ea4ad-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea4ad-121">Type</span></span>|<span data-ttu-id="ea4ad-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea4ad-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea4ad-123">id</span><span class="sxs-lookup"><span data-stu-id="ea4ad-123">id</span></span>|<span data-ttu-id="ea4ad-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ea4ad-124">String</span></span>|<span data-ttu-id="ea4ad-125">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ea4ad-125">Key of the entity.</span></span>|
|<span data-ttu-id="ea4ad-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ea4ad-126">lastModifiedDateTime</span></span>|<span data-ttu-id="ea4ad-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea4ad-127">DateTimeOffset</span></span>|<span data-ttu-id="ea4ad-128">Última modificação de DateTime do objeto.</span><span class="sxs-lookup"><span data-stu-id="ea4ad-128">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="ea4ad-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ea4ad-129">createdDateTime</span></span>|<span data-ttu-id="ea4ad-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea4ad-130">DateTimeOffset</span></span>|<span data-ttu-id="ea4ad-131">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ea4ad-131">DateTime the object was created.</span></span>|
|<span data-ttu-id="ea4ad-132">descrição</span><span class="sxs-lookup"><span data-stu-id="ea4ad-132">description</span></span>|<span data-ttu-id="ea4ad-133">String</span><span class="sxs-lookup"><span data-stu-id="ea4ad-133">String</span></span>|<span data-ttu-id="ea4ad-134">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ea4ad-134">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="ea4ad-135">displayName</span><span class="sxs-lookup"><span data-stu-id="ea4ad-135">displayName</span></span>|<span data-ttu-id="ea4ad-136">String</span><span class="sxs-lookup"><span data-stu-id="ea4ad-136">String</span></span>|<span data-ttu-id="ea4ad-137">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ea4ad-137">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="ea4ad-138">versão</span><span class="sxs-lookup"><span data-stu-id="ea4ad-138">version</span></span>|<span data-ttu-id="ea4ad-139">Int32</span><span class="sxs-lookup"><span data-stu-id="ea4ad-139">Int32</span></span>|<span data-ttu-id="ea4ad-140">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ea4ad-140">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea4ad-141">Relações</span><span class="sxs-lookup"><span data-stu-id="ea4ad-141">Relationships</span></span>
|<span data-ttu-id="ea4ad-142">Relação</span><span class="sxs-lookup"><span data-stu-id="ea4ad-142">Relationship</span></span>|<span data-ttu-id="ea4ad-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea4ad-143">Type</span></span>|<span data-ttu-id="ea4ad-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea4ad-144">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea4ad-145">assignments</span><span class="sxs-lookup"><span data-stu-id="ea4ad-145">assignments</span></span>|<span data-ttu-id="ea4ad-146">Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="ea4ad-146">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="ea4ad-147">A lista de atribuições para o perfil de configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ea4ad-147">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="ea4ad-148">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="ea4ad-148">deviceStatuses</span></span>|<span data-ttu-id="ea4ad-149">Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="ea4ad-149">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="ea4ad-150">Status de instalação da configuração de dispositivo por dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ea4ad-150">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="ea4ad-151">userStatuses</span><span class="sxs-lookup"><span data-stu-id="ea4ad-151">userStatuses</span></span>|<span data-ttu-id="ea4ad-152">Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="ea4ad-152">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="ea4ad-153">Status de instalação da configuração do dispositivo por usuário.</span><span class="sxs-lookup"><span data-stu-id="ea4ad-153">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="ea4ad-154">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="ea4ad-154">deviceStatusOverview</span></span>|[<span data-ttu-id="ea4ad-155">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="ea4ad-155">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="ea4ad-156">Visão geral do status dos dispositivos da configuração de dispositivos</span><span class="sxs-lookup"><span data-stu-id="ea4ad-156">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="ea4ad-157">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="ea4ad-157">userStatusOverview</span></span>|[<span data-ttu-id="ea4ad-158">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="ea4ad-158">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="ea4ad-159">Visão geral do status dos usuários da configuração de dispositivos</span><span class="sxs-lookup"><span data-stu-id="ea4ad-159">Device Configuration users status overview</span></span>|
|<span data-ttu-id="ea4ad-160">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="ea4ad-160">deviceSettingStateSummaries</span></span>|<span data-ttu-id="ea4ad-161">Conjunto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="ea4ad-161">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="ea4ad-162">Resumo do dispositivo do estado de definição de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="ea4ad-162">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ea4ad-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ea4ad-163">JSON Representation</span></span>
<span data-ttu-id="ea4ad-164">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ea4ad-164">Here is a JSON representation of the resource.</span></span>
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



