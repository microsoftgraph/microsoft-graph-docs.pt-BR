---
title: Tipo de recurso deviceConfiguration
description: Configuração do dispositivo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bf0f541fff8cdf238dc2883efcf82def89fd1ac0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532588"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="aac63-103">Tipo de recurso deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="aac63-103">deviceConfiguration resource type</span></span>

<span data-ttu-id="aac63-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aac63-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aac63-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aac63-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aac63-106">Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aac63-106">Device Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="aac63-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="aac63-107">Methods</span></span>
|<span data-ttu-id="aac63-108">Método</span><span class="sxs-lookup"><span data-stu-id="aac63-108">Method</span></span>|<span data-ttu-id="aac63-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="aac63-109">Return Type</span></span>|<span data-ttu-id="aac63-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="aac63-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="aac63-111">Listar deviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="aac63-111">List deviceConfigurations</span></span>](../api/intune-deviceconfig-deviceconfiguration-list.md)|<span data-ttu-id="aac63-112">Conjunto [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aac63-112">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="aac63-113">Listar propriedades e relações de objetos de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aac63-113">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="aac63-114">Obter deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="aac63-114">Get deviceConfiguration</span></span>](../api/intune-deviceconfig-deviceconfiguration-get.md)|[<span data-ttu-id="aac63-115">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="aac63-115">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="aac63-116">Ler propriedades e relações de objetos de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aac63-116">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="aac63-117">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="aac63-117">assign action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assign.md)|<span data-ttu-id="aac63-118">Conjunto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="aac63-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="aac63-119">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="aac63-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="aac63-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aac63-120">Properties</span></span>
|<span data-ttu-id="aac63-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aac63-121">Property</span></span>|<span data-ttu-id="aac63-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="aac63-122">Type</span></span>|<span data-ttu-id="aac63-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="aac63-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aac63-124">id</span><span class="sxs-lookup"><span data-stu-id="aac63-124">id</span></span>|<span data-ttu-id="aac63-125">String</span><span class="sxs-lookup"><span data-stu-id="aac63-125">String</span></span>|<span data-ttu-id="aac63-126">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="aac63-126">Key of the entity.</span></span>|
|<span data-ttu-id="aac63-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aac63-127">lastModifiedDateTime</span></span>|<span data-ttu-id="aac63-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aac63-128">DateTimeOffset</span></span>|<span data-ttu-id="aac63-129">Última modificação de DateTime do objeto.</span><span class="sxs-lookup"><span data-stu-id="aac63-129">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="aac63-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aac63-130">createdDateTime</span></span>|<span data-ttu-id="aac63-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aac63-131">DateTimeOffset</span></span>|<span data-ttu-id="aac63-132">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="aac63-132">DateTime the object was created.</span></span>|
|<span data-ttu-id="aac63-133">description</span><span class="sxs-lookup"><span data-stu-id="aac63-133">description</span></span>|<span data-ttu-id="aac63-134">String</span><span class="sxs-lookup"><span data-stu-id="aac63-134">String</span></span>|<span data-ttu-id="aac63-135">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aac63-135">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="aac63-136">displayName</span><span class="sxs-lookup"><span data-stu-id="aac63-136">displayName</span></span>|<span data-ttu-id="aac63-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aac63-137">String</span></span>|<span data-ttu-id="aac63-138">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aac63-138">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="aac63-139">versão</span><span class="sxs-lookup"><span data-stu-id="aac63-139">version</span></span>|<span data-ttu-id="aac63-140">Int32</span><span class="sxs-lookup"><span data-stu-id="aac63-140">Int32</span></span>|<span data-ttu-id="aac63-141">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aac63-141">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aac63-142">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="aac63-142">Relationships</span></span>
|<span data-ttu-id="aac63-143">Relação</span><span class="sxs-lookup"><span data-stu-id="aac63-143">Relationship</span></span>|<span data-ttu-id="aac63-144">Tipo</span><span class="sxs-lookup"><span data-stu-id="aac63-144">Type</span></span>|<span data-ttu-id="aac63-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="aac63-145">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aac63-146">assignments</span><span class="sxs-lookup"><span data-stu-id="aac63-146">assignments</span></span>|<span data-ttu-id="aac63-147">Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="aac63-147">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="aac63-148">A lista de atribuições para o perfil de configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aac63-148">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="aac63-149">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="aac63-149">deviceStatuses</span></span>|<span data-ttu-id="aac63-150">Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="aac63-150">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="aac63-151">Status de instalação da configuração de dispositivo por dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aac63-151">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="aac63-152">userStatuses</span><span class="sxs-lookup"><span data-stu-id="aac63-152">userStatuses</span></span>|<span data-ttu-id="aac63-153">Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="aac63-153">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="aac63-154">Status de instalação da configuração do dispositivo por usuário.</span><span class="sxs-lookup"><span data-stu-id="aac63-154">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="aac63-155">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="aac63-155">deviceStatusOverview</span></span>|[<span data-ttu-id="aac63-156">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="aac63-156">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="aac63-157">Visão geral do status dos dispositivos da configuração de dispositivos</span><span class="sxs-lookup"><span data-stu-id="aac63-157">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="aac63-158">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="aac63-158">userStatusOverview</span></span>|[<span data-ttu-id="aac63-159">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="aac63-159">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="aac63-160">Visão geral do status dos usuários da configuração de dispositivos</span><span class="sxs-lookup"><span data-stu-id="aac63-160">Device Configuration users status overview</span></span>|
|<span data-ttu-id="aac63-161">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="aac63-161">deviceSettingStateSummaries</span></span>|<span data-ttu-id="aac63-162">Conjunto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="aac63-162">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="aac63-163">Resumo do dispositivo do estado de definição de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="aac63-163">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aac63-164">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="aac63-164">JSON Representation</span></span>
<span data-ttu-id="aac63-165">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="aac63-165">Here is a JSON representation of the resource.</span></span>
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




