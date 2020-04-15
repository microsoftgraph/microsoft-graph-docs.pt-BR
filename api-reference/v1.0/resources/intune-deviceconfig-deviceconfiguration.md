---
title: Tipo de recurso deviceConfiguration
description: Configuração do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d1927b4af889fb98e2e9c33561b9ff63042df5b6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465738"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="1a6b5-103">Tipo de recurso deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="1a6b5-103">deviceConfiguration resource type</span></span>

<span data-ttu-id="1a6b5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a6b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a6b5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1a6b5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a6b5-106">Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1a6b5-106">Device Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="1a6b5-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="1a6b5-107">Methods</span></span>
|<span data-ttu-id="1a6b5-108">Método</span><span class="sxs-lookup"><span data-stu-id="1a6b5-108">Method</span></span>|<span data-ttu-id="1a6b5-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1a6b5-109">Return Type</span></span>|<span data-ttu-id="1a6b5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a6b5-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1a6b5-111">Listar deviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="1a6b5-111">List deviceConfigurations</span></span>](../api/intune-deviceconfig-deviceconfiguration-list.md)|<span data-ttu-id="1a6b5-112">Conjunto [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1a6b5-112">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="1a6b5-113">Listar propriedades e relações de objetos de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a6b5-113">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="1a6b5-114">Obter deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="1a6b5-114">Get deviceConfiguration</span></span>](../api/intune-deviceconfig-deviceconfiguration-get.md)|[<span data-ttu-id="1a6b5-115">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="1a6b5-115">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="1a6b5-116">Ler propriedades e relações de objetos de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="1a6b5-116">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="1a6b5-117">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="1a6b5-117">assign action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assign.md)|<span data-ttu-id="1a6b5-118">Conjunto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1a6b5-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="1a6b5-119">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1a6b5-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="1a6b5-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1a6b5-120">Properties</span></span>
|<span data-ttu-id="1a6b5-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1a6b5-121">Property</span></span>|<span data-ttu-id="1a6b5-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a6b5-122">Type</span></span>|<span data-ttu-id="1a6b5-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a6b5-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a6b5-124">id</span><span class="sxs-lookup"><span data-stu-id="1a6b5-124">id</span></span>|<span data-ttu-id="1a6b5-125">String</span><span class="sxs-lookup"><span data-stu-id="1a6b5-125">String</span></span>|<span data-ttu-id="1a6b5-126">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1a6b5-126">Key of the entity.</span></span>|
|<span data-ttu-id="1a6b5-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a6b5-127">lastModifiedDateTime</span></span>|<span data-ttu-id="1a6b5-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a6b5-128">DateTimeOffset</span></span>|<span data-ttu-id="1a6b5-129">Última modificação de DateTime do objeto.</span><span class="sxs-lookup"><span data-stu-id="1a6b5-129">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="1a6b5-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1a6b5-130">createdDateTime</span></span>|<span data-ttu-id="1a6b5-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a6b5-131">DateTimeOffset</span></span>|<span data-ttu-id="1a6b5-132">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="1a6b5-132">DateTime the object was created.</span></span>|
|<span data-ttu-id="1a6b5-133">description</span><span class="sxs-lookup"><span data-stu-id="1a6b5-133">description</span></span>|<span data-ttu-id="1a6b5-134">String</span><span class="sxs-lookup"><span data-stu-id="1a6b5-134">String</span></span>|<span data-ttu-id="1a6b5-135">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1a6b5-135">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="1a6b5-136">displayName</span><span class="sxs-lookup"><span data-stu-id="1a6b5-136">displayName</span></span>|<span data-ttu-id="1a6b5-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a6b5-137">String</span></span>|<span data-ttu-id="1a6b5-138">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1a6b5-138">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="1a6b5-139">versão</span><span class="sxs-lookup"><span data-stu-id="1a6b5-139">version</span></span>|<span data-ttu-id="1a6b5-140">Int32</span><span class="sxs-lookup"><span data-stu-id="1a6b5-140">Int32</span></span>|<span data-ttu-id="1a6b5-141">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1a6b5-141">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a6b5-142">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="1a6b5-142">Relationships</span></span>
|<span data-ttu-id="1a6b5-143">Relação</span><span class="sxs-lookup"><span data-stu-id="1a6b5-143">Relationship</span></span>|<span data-ttu-id="1a6b5-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a6b5-144">Type</span></span>|<span data-ttu-id="1a6b5-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a6b5-145">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a6b5-146">assignments</span><span class="sxs-lookup"><span data-stu-id="1a6b5-146">assignments</span></span>|<span data-ttu-id="1a6b5-147">Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1a6b5-147">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="1a6b5-148">A lista de atribuições para o perfil de configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1a6b5-148">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="1a6b5-149">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="1a6b5-149">deviceStatuses</span></span>|<span data-ttu-id="1a6b5-150">Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="1a6b5-150">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="1a6b5-151">Status de instalação da configuração de dispositivo por dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1a6b5-151">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="1a6b5-152">userStatuses</span><span class="sxs-lookup"><span data-stu-id="1a6b5-152">userStatuses</span></span>|<span data-ttu-id="1a6b5-153">Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="1a6b5-153">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="1a6b5-154">Status de instalação da configuração do dispositivo por usuário.</span><span class="sxs-lookup"><span data-stu-id="1a6b5-154">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="1a6b5-155">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="1a6b5-155">deviceStatusOverview</span></span>|[<span data-ttu-id="1a6b5-156">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="1a6b5-156">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="1a6b5-157">Visão geral do status dos dispositivos da configuração de dispositivos</span><span class="sxs-lookup"><span data-stu-id="1a6b5-157">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="1a6b5-158">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="1a6b5-158">userStatusOverview</span></span>|[<span data-ttu-id="1a6b5-159">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="1a6b5-159">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="1a6b5-160">Visão geral do status dos usuários da configuração de dispositivos</span><span class="sxs-lookup"><span data-stu-id="1a6b5-160">Device Configuration users status overview</span></span>|
|<span data-ttu-id="1a6b5-161">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="1a6b5-161">deviceSettingStateSummaries</span></span>|<span data-ttu-id="1a6b5-162">Conjunto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="1a6b5-162">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="1a6b5-163">Resumo do dispositivo do estado de definição de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="1a6b5-163">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1a6b5-164">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1a6b5-164">JSON Representation</span></span>
<span data-ttu-id="1a6b5-165">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1a6b5-165">Here is a JSON representation of the resource.</span></span>
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







