---
title: Tipo de recurso deviceConfiguration
description: Configuração do dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 82f1de5e835ceba2a15559411a07638dee2602bd
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52742906"
---
# <a name="deviceconfiguration-resource-type"></a><span data-ttu-id="760f2-103">Tipo de recurso deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="760f2-103">deviceConfiguration resource type</span></span>

<span data-ttu-id="760f2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="760f2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="760f2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="760f2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="760f2-106">Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="760f2-106">Device Configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="760f2-107">Methods</span><span class="sxs-lookup"><span data-stu-id="760f2-107">Methods</span></span>
|<span data-ttu-id="760f2-108">Método</span><span class="sxs-lookup"><span data-stu-id="760f2-108">Method</span></span>|<span data-ttu-id="760f2-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="760f2-109">Return Type</span></span>|<span data-ttu-id="760f2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="760f2-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="760f2-111">Listar deviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="760f2-111">List deviceConfigurations</span></span>](../api/intune-deviceconfig-deviceconfiguration-list.md)|<span data-ttu-id="760f2-112">Conjunto [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="760f2-112">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) collection</span></span>|<span data-ttu-id="760f2-113">Listar propriedades e relações de objetos de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="760f2-113">List properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="760f2-114">Obter deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="760f2-114">Get deviceConfiguration</span></span>](../api/intune-deviceconfig-deviceconfiguration-get.md)|[<span data-ttu-id="760f2-115">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="760f2-115">deviceConfiguration</span></span>](../resources/intune-deviceconfig-deviceconfiguration.md)|<span data-ttu-id="760f2-116">Ler propriedades e relações de objetos de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="760f2-116">Read properties and relationships of the [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="760f2-117">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="760f2-117">assign action</span></span>](../api/intune-deviceconfig-deviceconfiguration-assign.md)|<span data-ttu-id="760f2-118">Conjunto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="760f2-118">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="760f2-119">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="760f2-119">Not yet documented</span></span>|
|[<span data-ttu-id="760f2-120">função getOmaSettingPlainTextValue</span><span class="sxs-lookup"><span data-stu-id="760f2-120">getOmaSettingPlainTextValue function</span></span>](../api/intune-deviceconfig-deviceconfiguration-getomasettingplaintextvalue.md)|<span data-ttu-id="760f2-121">String</span><span class="sxs-lookup"><span data-stu-id="760f2-121">String</span></span>|<span data-ttu-id="760f2-122">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="760f2-122">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="760f2-123">Propriedades</span><span class="sxs-lookup"><span data-stu-id="760f2-123">Properties</span></span>
|<span data-ttu-id="760f2-124">Propriedade</span><span class="sxs-lookup"><span data-stu-id="760f2-124">Property</span></span>|<span data-ttu-id="760f2-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="760f2-125">Type</span></span>|<span data-ttu-id="760f2-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="760f2-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="760f2-127">id</span><span class="sxs-lookup"><span data-stu-id="760f2-127">id</span></span>|<span data-ttu-id="760f2-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="760f2-128">String</span></span>|<span data-ttu-id="760f2-129">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="760f2-129">Key of the entity.</span></span>|
|<span data-ttu-id="760f2-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="760f2-130">lastModifiedDateTime</span></span>|<span data-ttu-id="760f2-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="760f2-131">DateTimeOffset</span></span>|<span data-ttu-id="760f2-132">Última modificação de DateTime do objeto.</span><span class="sxs-lookup"><span data-stu-id="760f2-132">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="760f2-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="760f2-133">createdDateTime</span></span>|<span data-ttu-id="760f2-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="760f2-134">DateTimeOffset</span></span>|<span data-ttu-id="760f2-135">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="760f2-135">DateTime the object was created.</span></span>|
|<span data-ttu-id="760f2-136">descrição</span><span class="sxs-lookup"><span data-stu-id="760f2-136">description</span></span>|<span data-ttu-id="760f2-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="760f2-137">String</span></span>|<span data-ttu-id="760f2-138">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="760f2-138">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="760f2-139">displayName</span><span class="sxs-lookup"><span data-stu-id="760f2-139">displayName</span></span>|<span data-ttu-id="760f2-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="760f2-140">String</span></span>|<span data-ttu-id="760f2-141">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="760f2-141">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="760f2-142">versão</span><span class="sxs-lookup"><span data-stu-id="760f2-142">version</span></span>|<span data-ttu-id="760f2-143">Int32</span><span class="sxs-lookup"><span data-stu-id="760f2-143">Int32</span></span>|<span data-ttu-id="760f2-144">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="760f2-144">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="760f2-145">Relações</span><span class="sxs-lookup"><span data-stu-id="760f2-145">Relationships</span></span>
|<span data-ttu-id="760f2-146">Relação</span><span class="sxs-lookup"><span data-stu-id="760f2-146">Relationship</span></span>|<span data-ttu-id="760f2-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="760f2-147">Type</span></span>|<span data-ttu-id="760f2-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="760f2-148">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="760f2-149">assignments</span><span class="sxs-lookup"><span data-stu-id="760f2-149">assignments</span></span>|<span data-ttu-id="760f2-150">Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="760f2-150">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="760f2-151">A lista de atribuições para o perfil de configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="760f2-151">The list of assignments for the device configuration profile.</span></span>|
|<span data-ttu-id="760f2-152">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="760f2-152">deviceStatuses</span></span>|<span data-ttu-id="760f2-153">Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="760f2-153">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="760f2-154">Status de instalação da configuração de dispositivo por dispositivo.</span><span class="sxs-lookup"><span data-stu-id="760f2-154">Device configuration installation status by device.</span></span>|
|<span data-ttu-id="760f2-155">userStatuses</span><span class="sxs-lookup"><span data-stu-id="760f2-155">userStatuses</span></span>|<span data-ttu-id="760f2-156">Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="760f2-156">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="760f2-157">Status da instalação de configuração do dispositivo pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="760f2-157">Device configuration installation status by user.</span></span>|
|<span data-ttu-id="760f2-158">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="760f2-158">deviceStatusOverview</span></span>|[<span data-ttu-id="760f2-159">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="760f2-159">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="760f2-160">Visão geral do status dos dispositivos da configuração de dispositivos</span><span class="sxs-lookup"><span data-stu-id="760f2-160">Device Configuration devices status overview</span></span>|
|<span data-ttu-id="760f2-161">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="760f2-161">userStatusOverview</span></span>|[<span data-ttu-id="760f2-162">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="760f2-162">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="760f2-163">Visão geral do status dos usuários da configuração de dispositivos</span><span class="sxs-lookup"><span data-stu-id="760f2-163">Device Configuration users status overview</span></span>|
|<span data-ttu-id="760f2-164">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="760f2-164">deviceSettingStateSummaries</span></span>|<span data-ttu-id="760f2-165">Conjunto [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="760f2-165">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="760f2-166">Resumo do dispositivo do estado de definição de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="760f2-166">Device Configuration Setting State Device Summary</span></span>|

## <a name="json-representation"></a><span data-ttu-id="760f2-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="760f2-167">JSON Representation</span></span>
<span data-ttu-id="760f2-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="760f2-168">Here is a JSON representation of the resource.</span></span>
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




