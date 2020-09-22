---
title: Tipo de recurso deviceConfiguration
description: Configuração do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ffcd58ee7dc23554908749d7c257fa8acccffe94
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075025"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="51cf3-103">Tipo de recurso deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="51cf3-103">deviceConfiguration resource type</span></span>

<span data-ttu-id="51cf3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51cf3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="51cf3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="51cf3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51cf3-106">Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="51cf3-106">Device Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="51cf3-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="51cf3-107">Methods</span></span>
|<span data-ttu-id="51cf3-108">Método</span><span class="sxs-lookup"><span data-stu-id="51cf3-108">Method</span></span>|<span data-ttu-id="51cf3-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="51cf3-109">Return Type</span></span>|<span data-ttu-id="51cf3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="51cf3-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="51cf3-111">Listar deviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="51cf3-111">List deviceConfigurations</span></span>](../api/intune-deviceconfig-deviceconfiguration-list.md)|<span data-ttu-id="51cf3-112">Conjunto [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="51cf3-112">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="51cf3-113">Listar propriedades e relações de objetos de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51cf3-113">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="51cf3-114">Obter deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="51cf3-114">Get deviceConfiguration</span></span>](../api/intune-deviceconfig-deviceconfiguration-get.md)|[<span data-ttu-id="51cf3-115">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="51cf3-115">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="51cf3-116">Ler propriedades e relações de objetos de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51cf3-116">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="51cf3-117">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="51cf3-117">assign action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assign.md)|<span data-ttu-id="51cf3-118">Conjunto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="51cf3-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="51cf3-119">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="51cf3-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="51cf3-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="51cf3-120">Properties</span></span>
|<span data-ttu-id="51cf3-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="51cf3-121">Property</span></span>|<span data-ttu-id="51cf3-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="51cf3-122">Type</span></span>|<span data-ttu-id="51cf3-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="51cf3-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51cf3-124">id</span><span class="sxs-lookup"><span data-stu-id="51cf3-124">id</span></span>|<span data-ttu-id="51cf3-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51cf3-125">String</span></span>|<span data-ttu-id="51cf3-126">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="51cf3-126">Key of the entity.</span></span>|
|<span data-ttu-id="51cf3-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="51cf3-127">lastModifiedDateTime</span></span>|<span data-ttu-id="51cf3-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51cf3-128">DateTimeOffset</span></span>|<span data-ttu-id="51cf3-129">Última modificação de DateTime do objeto.</span><span class="sxs-lookup"><span data-stu-id="51cf3-129">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="51cf3-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="51cf3-130">createdDateTime</span></span>|<span data-ttu-id="51cf3-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51cf3-131">DateTimeOffset</span></span>|<span data-ttu-id="51cf3-132">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="51cf3-132">DateTime the object was created.</span></span>|
|<span data-ttu-id="51cf3-133">description</span><span class="sxs-lookup"><span data-stu-id="51cf3-133">description</span></span>|<span data-ttu-id="51cf3-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51cf3-134">String</span></span>|<span data-ttu-id="51cf3-135">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="51cf3-135">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="51cf3-136">displayName</span><span class="sxs-lookup"><span data-stu-id="51cf3-136">displayName</span></span>|<span data-ttu-id="51cf3-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51cf3-137">String</span></span>|<span data-ttu-id="51cf3-138">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="51cf3-138">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="51cf3-139">versão</span><span class="sxs-lookup"><span data-stu-id="51cf3-139">version</span></span>|<span data-ttu-id="51cf3-140">Int32</span><span class="sxs-lookup"><span data-stu-id="51cf3-140">Int32</span></span>|<span data-ttu-id="51cf3-141">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="51cf3-141">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="51cf3-142">Relações</span><span class="sxs-lookup"><span data-stu-id="51cf3-142">Relationships</span></span>
|<span data-ttu-id="51cf3-143">Relação</span><span class="sxs-lookup"><span data-stu-id="51cf3-143">Relationship</span></span>|<span data-ttu-id="51cf3-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="51cf3-144">Type</span></span>|<span data-ttu-id="51cf3-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="51cf3-145">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51cf3-146">assignments</span><span class="sxs-lookup"><span data-stu-id="51cf3-146">assignments</span></span>|<span data-ttu-id="51cf3-147">Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="51cf3-147">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="51cf3-148">A lista de atribuições para o perfil de configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="51cf3-148">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="51cf3-149">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="51cf3-149">deviceStatuses</span></span>|<span data-ttu-id="51cf3-150">Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="51cf3-150">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="51cf3-151">Status de instalação da configuração de dispositivo por dispositivo.</span><span class="sxs-lookup"><span data-stu-id="51cf3-151">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="51cf3-152">userStatuses</span><span class="sxs-lookup"><span data-stu-id="51cf3-152">userStatuses</span></span>|<span data-ttu-id="51cf3-153">Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="51cf3-153">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="51cf3-154">Status de instalação da configuração do dispositivo por usuário.</span><span class="sxs-lookup"><span data-stu-id="51cf3-154">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="51cf3-155">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="51cf3-155">deviceStatusOverview</span></span>|[<span data-ttu-id="51cf3-156">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="51cf3-156">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="51cf3-157">Visão geral do status dos dispositivos da configuração de dispositivos</span><span class="sxs-lookup"><span data-stu-id="51cf3-157">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="51cf3-158">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="51cf3-158">userStatusOverview</span></span>|[<span data-ttu-id="51cf3-159">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="51cf3-159">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="51cf3-160">Visão geral do status dos usuários da configuração de dispositivos</span><span class="sxs-lookup"><span data-stu-id="51cf3-160">Device Configuration users status overview</span></span>|
|<span data-ttu-id="51cf3-161">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="51cf3-161">deviceSettingStateSummaries</span></span>|<span data-ttu-id="51cf3-162">Conjunto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="51cf3-162">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="51cf3-163">Resumo do dispositivo do estado de definição de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="51cf3-163">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="51cf3-164">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="51cf3-164">JSON Representation</span></span>
<span data-ttu-id="51cf3-165">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="51cf3-165">Here is a JSON representation of the resource.</span></span>
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









