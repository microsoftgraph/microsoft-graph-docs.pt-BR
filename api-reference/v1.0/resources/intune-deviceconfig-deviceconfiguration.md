---
title: Tipo de recurso deviceConfiguration
description: Configuração do dispositivo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f27d69a4cae2ee3a723ea14e4394bc18ba778a8c
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359534"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="3acc6-103">Tipo de recurso deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="3acc6-103">deviceConfiguration resource type</span></span>

> <span data-ttu-id="3acc6-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3acc6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3acc6-105">Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3acc6-105">Device Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="3acc6-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="3acc6-106">Methods</span></span>
|<span data-ttu-id="3acc6-107">Método</span><span class="sxs-lookup"><span data-stu-id="3acc6-107">Method</span></span>|<span data-ttu-id="3acc6-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3acc6-108">Return Type</span></span>|<span data-ttu-id="3acc6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3acc6-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3acc6-110">Listar deviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="3acc6-110">List deviceConfigurations</span></span>](../api/intune-deviceconfig-deviceconfiguration-list.md)|<span data-ttu-id="3acc6-111">Conjunto [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3acc6-111">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="3acc6-112">Listar propriedades e relações de objetos de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3acc6-112">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="3acc6-113">Obter deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="3acc6-113">Get deviceConfiguration</span></span>](../api/intune-deviceconfig-deviceconfiguration-get.md)|[<span data-ttu-id="3acc6-114">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="3acc6-114">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="3acc6-115">Ler propriedades e relações de objetos de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3acc6-115">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="3acc6-116">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="3acc6-116">assign action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assign.md)|<span data-ttu-id="3acc6-117">Conjunto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3acc6-117">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="3acc6-118">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3acc6-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="3acc6-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3acc6-119">Properties</span></span>
|<span data-ttu-id="3acc6-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3acc6-120">Property</span></span>|<span data-ttu-id="3acc6-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="3acc6-121">Type</span></span>|<span data-ttu-id="3acc6-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="3acc6-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3acc6-123">id</span><span class="sxs-lookup"><span data-stu-id="3acc6-123">id</span></span>|<span data-ttu-id="3acc6-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3acc6-124">String</span></span>|<span data-ttu-id="3acc6-125">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3acc6-125">Key of the entity.</span></span>|
|<span data-ttu-id="3acc6-126">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3acc6-126">lastModifiedDateTime</span></span>|<span data-ttu-id="3acc6-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3acc6-127">DateTimeOffset</span></span>|<span data-ttu-id="3acc6-128">Última modificação de DateTime do objeto.</span><span class="sxs-lookup"><span data-stu-id="3acc6-128">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="3acc6-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3acc6-129">createdDateTime</span></span>|<span data-ttu-id="3acc6-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3acc6-130">DateTimeOffset</span></span>|<span data-ttu-id="3acc6-131">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="3acc6-131">DateTime the object was created.</span></span>|
|<span data-ttu-id="3acc6-132">descrição</span><span class="sxs-lookup"><span data-stu-id="3acc6-132">description</span></span>|<span data-ttu-id="3acc6-133">String</span><span class="sxs-lookup"><span data-stu-id="3acc6-133">String</span></span>|<span data-ttu-id="3acc6-134">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3acc6-134">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="3acc6-135">displayName</span><span class="sxs-lookup"><span data-stu-id="3acc6-135">displayName</span></span>|<span data-ttu-id="3acc6-136">String</span><span class="sxs-lookup"><span data-stu-id="3acc6-136">String</span></span>|<span data-ttu-id="3acc6-137">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3acc6-137">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="3acc6-138">versão</span><span class="sxs-lookup"><span data-stu-id="3acc6-138">version</span></span>|<span data-ttu-id="3acc6-139">Int32</span><span class="sxs-lookup"><span data-stu-id="3acc6-139">Int32</span></span>|<span data-ttu-id="3acc6-140">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3acc6-140">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3acc6-141">Relações</span><span class="sxs-lookup"><span data-stu-id="3acc6-141">Relationships</span></span>
|<span data-ttu-id="3acc6-142">Relação</span><span class="sxs-lookup"><span data-stu-id="3acc6-142">Relationship</span></span>|<span data-ttu-id="3acc6-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="3acc6-143">Type</span></span>|<span data-ttu-id="3acc6-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="3acc6-144">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3acc6-145">assignments</span><span class="sxs-lookup"><span data-stu-id="3acc6-145">assignments</span></span>|<span data-ttu-id="3acc6-146">Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="3acc6-146">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="3acc6-147">A lista de atribuições para o perfil de configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3acc6-147">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="3acc6-148">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="3acc6-148">deviceStatuses</span></span>|<span data-ttu-id="3acc6-149">Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="3acc6-149">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="3acc6-150">Status de instalação da configuração de dispositivo por dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3acc6-150">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="3acc6-151">userStatuses</span><span class="sxs-lookup"><span data-stu-id="3acc6-151">userStatuses</span></span>|<span data-ttu-id="3acc6-152">Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="3acc6-152">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="3acc6-153">Status de instalação da configuração do dispositivo por usuário.</span><span class="sxs-lookup"><span data-stu-id="3acc6-153">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="3acc6-154">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="3acc6-154">deviceStatusOverview</span></span>|[<span data-ttu-id="3acc6-155">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="3acc6-155">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="3acc6-156">Visão geral do status dos dispositivos da configuração de dispositivos</span><span class="sxs-lookup"><span data-stu-id="3acc6-156">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="3acc6-157">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="3acc6-157">userStatusOverview</span></span>|[<span data-ttu-id="3acc6-158">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="3acc6-158">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="3acc6-159">Visão geral do status dos usuários da configuração de dispositivos</span><span class="sxs-lookup"><span data-stu-id="3acc6-159">Device Configuration users status overview</span></span>|
|<span data-ttu-id="3acc6-160">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="3acc6-160">deviceSettingStateSummaries</span></span>|<span data-ttu-id="3acc6-161">Conjunto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="3acc6-161">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="3acc6-162">Resumo do dispositivo do estado de definição de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="3acc6-162">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3acc6-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3acc6-163">JSON Representation</span></span>
<span data-ttu-id="3acc6-164">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3acc6-164">Here is a JSON representation of the resource.</span></span>
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




