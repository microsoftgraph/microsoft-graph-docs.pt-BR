---
title: Tipo de recurso deviceCompliancePolicy
description: 'Esta é a classe base para a política de Conformidade. Políticas de conformidade são específicas de plataformas, e políticas de conformidade individuais por plataforma herdam a partir daqui. '
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7b6d74a558a09f22f3d01dbfb771c00311c4a2fd
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359632"
---
# <a name="devicecompliancepolicy-resource-type"></a><span data-ttu-id="76892-104">Tipo de recurso deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="76892-104">deviceCompliancePolicy resource type</span></span>

> <span data-ttu-id="76892-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="76892-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76892-106">Esta é a classe base para a política de Conformidade.</span><span class="sxs-lookup"><span data-stu-id="76892-106">This is the base class for Compliance policy.</span></span> <span data-ttu-id="76892-107">Políticas de conformidade são específicas de plataformas, e políticas de conformidade individuais por plataforma herdam a partir daqui.</span><span class="sxs-lookup"><span data-stu-id="76892-107">Compliance policies are platform specific and individual per-platform compliance policies inherit from here.</span></span> 

## <a name="methods"></a><span data-ttu-id="76892-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="76892-108">Methods</span></span>
|<span data-ttu-id="76892-109">Método</span><span class="sxs-lookup"><span data-stu-id="76892-109">Method</span></span>|<span data-ttu-id="76892-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="76892-110">Return Type</span></span>|<span data-ttu-id="76892-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="76892-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="76892-112">Listar deviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="76892-112">List deviceCompliancePolicies</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-list.md)|<span data-ttu-id="76892-113">Coleção [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="76892-113">[deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) collection</span></span>|<span data-ttu-id="76892-114">Lista propriedades e relações dos objetos [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="76892-114">List properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) objects.</span></span>|
|[<span data-ttu-id="76892-115">Obter deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="76892-115">Get deviceCompliancePolicy</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-get.md)|[<span data-ttu-id="76892-116">deviceCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="76892-116">deviceCompliancePolicy</span></span>](../resources/intune-deviceconfig-devicecompliancepolicy.md)|<span data-ttu-id="76892-117">Propriedades de leitura e relações do objeto [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="76892-117">Read properties and relationships of the [deviceCompliancePolicy](../resources/intune-deviceconfig-devicecompliancepolicy.md) object.</span></span>|
|[<span data-ttu-id="76892-118">ação assign</span><span class="sxs-lookup"><span data-stu-id="76892-118">assign action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-assign.md)|<span data-ttu-id="76892-119">Coleção [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="76892-119">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="76892-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="76892-120">Not yet documented</span></span>|
|[<span data-ttu-id="76892-121">ação scheduleActionsForRules</span><span class="sxs-lookup"><span data-stu-id="76892-121">scheduleActionsForRules action</span></span>](../api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules.md)|<span data-ttu-id="76892-122">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="76892-122">None</span></span>|<span data-ttu-id="76892-123">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="76892-123">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="76892-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="76892-124">Properties</span></span>
|<span data-ttu-id="76892-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="76892-125">Property</span></span>|<span data-ttu-id="76892-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="76892-126">Type</span></span>|<span data-ttu-id="76892-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="76892-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76892-128">id</span><span class="sxs-lookup"><span data-stu-id="76892-128">id</span></span>|<span data-ttu-id="76892-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="76892-129">String</span></span>|<span data-ttu-id="76892-130">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="76892-130">Key of the entity.</span></span>|
|<span data-ttu-id="76892-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="76892-131">createdDateTime</span></span>|<span data-ttu-id="76892-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76892-132">DateTimeOffset</span></span>|<span data-ttu-id="76892-133">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="76892-133">DateTime the object was created.</span></span>|
|<span data-ttu-id="76892-134">descrição</span><span class="sxs-lookup"><span data-stu-id="76892-134">description</span></span>|<span data-ttu-id="76892-135">String</span><span class="sxs-lookup"><span data-stu-id="76892-135">String</span></span>|<span data-ttu-id="76892-136">Descrição fornecida pelo administrador da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="76892-136">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="76892-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="76892-137">lastModifiedDateTime</span></span>|<span data-ttu-id="76892-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76892-138">DateTimeOffset</span></span>|<span data-ttu-id="76892-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="76892-139">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="76892-140">displayName</span><span class="sxs-lookup"><span data-stu-id="76892-140">displayName</span></span>|<span data-ttu-id="76892-141">String</span><span class="sxs-lookup"><span data-stu-id="76892-141">String</span></span>|<span data-ttu-id="76892-142">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="76892-142">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="76892-143">versão</span><span class="sxs-lookup"><span data-stu-id="76892-143">version</span></span>|<span data-ttu-id="76892-144">Int32</span><span class="sxs-lookup"><span data-stu-id="76892-144">Int32</span></span>|<span data-ttu-id="76892-145">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="76892-145">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="76892-146">Relações</span><span class="sxs-lookup"><span data-stu-id="76892-146">Relationships</span></span>
|<span data-ttu-id="76892-147">Relação</span><span class="sxs-lookup"><span data-stu-id="76892-147">Relationship</span></span>|<span data-ttu-id="76892-148">Tipo</span><span class="sxs-lookup"><span data-stu-id="76892-148">Type</span></span>|<span data-ttu-id="76892-149">Descrição</span><span class="sxs-lookup"><span data-stu-id="76892-149">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76892-150">scheduledActionsForRule</span><span class="sxs-lookup"><span data-stu-id="76892-150">scheduledActionsForRule</span></span>|<span data-ttu-id="76892-151">Coleção [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md)</span><span class="sxs-lookup"><span data-stu-id="76892-151">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="76892-152">A lista de ações agendadas para essa regra</span><span class="sxs-lookup"><span data-stu-id="76892-152">The list of scheduled action for this rule</span></span>|
|<span data-ttu-id="76892-153">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="76892-153">deviceStatuses</span></span>|<span data-ttu-id="76892-154">Coleção [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="76892-154">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) collection</span></span>|<span data-ttu-id="76892-155">Lista de DeviceComplianceDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="76892-155">List of DeviceComplianceDeviceStatus.</span></span>|
|<span data-ttu-id="76892-156">userStatuses</span><span class="sxs-lookup"><span data-stu-id="76892-156">userStatuses</span></span>|<span data-ttu-id="76892-157">Coleção [deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="76892-157">[deviceComplianceUserStatus](../resources/intune-deviceconfig-devicecomplianceuserstatus.md) collection</span></span>|<span data-ttu-id="76892-158">Lista de DeviceComplianceUserStatus.</span><span class="sxs-lookup"><span data-stu-id="76892-158">List of DeviceComplianceUserStatus.</span></span>|
|<span data-ttu-id="76892-159">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="76892-159">deviceStatusOverview</span></span>|[<span data-ttu-id="76892-160">deviceComplianceDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="76892-160">deviceComplianceDeviceOverview</span></span>](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|<span data-ttu-id="76892-161">Visão geral de status de dispositivos para conformidade de dispositivos</span><span class="sxs-lookup"><span data-stu-id="76892-161">Device compliance devices status overview</span></span>|
|<span data-ttu-id="76892-162">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="76892-162">userStatusOverview</span></span>|[<span data-ttu-id="76892-163">deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="76892-163">deviceComplianceUserOverview</span></span>](../resources/intune-deviceconfig-devicecomplianceuseroverview.md)|<span data-ttu-id="76892-164">Visão geral de status de usuários para conformidade de dispositivos</span><span class="sxs-lookup"><span data-stu-id="76892-164">Device compliance users status overview</span></span>|
|<span data-ttu-id="76892-165">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="76892-165">deviceSettingStateSummaries</span></span>|<span data-ttu-id="76892-166">Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)</span><span class="sxs-lookup"><span data-stu-id="76892-166">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="76892-167">Resumo do dispositivo para estado de configuração de conformidade</span><span class="sxs-lookup"><span data-stu-id="76892-167">Compliance Setting State Device Summary</span></span>|
|<span data-ttu-id="76892-168">assignments</span><span class="sxs-lookup"><span data-stu-id="76892-168">assignments</span></span>|<span data-ttu-id="76892-169">Coleção [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="76892-169">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="76892-170">A coleção de atribuições para essa política de conformidade.</span><span class="sxs-lookup"><span data-stu-id="76892-170">The collection of assignments for this compliance policy.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="76892-171">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="76892-171">JSON Representation</span></span>
<span data-ttu-id="76892-172">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="76892-172">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicy",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```




