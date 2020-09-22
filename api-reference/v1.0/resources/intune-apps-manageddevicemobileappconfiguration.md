---
title: Tipo de recurso managedDeviceMobileAppConfiguration
description: Uma classe abstrata para a configuração do Aplicativo móvel para dispositivos registrados.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4a8954b276ce297f3a304a0a408ec22063ee3634
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015411"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="c34a8-103">Tipo de recurso managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="c34a8-103">managedDeviceMobileAppConfiguration resource type</span></span>

<span data-ttu-id="c34a8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c34a8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c34a8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c34a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c34a8-106">Uma classe abstrata para a configuração do Aplicativo móvel para dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="c34a8-106">An abstract class for Mobile app configuration for enrolled devices.</span></span>

## <a name="methods"></a><span data-ttu-id="c34a8-107">Methods</span><span class="sxs-lookup"><span data-stu-id="c34a8-107">Methods</span></span>
|<span data-ttu-id="c34a8-108">Método</span><span class="sxs-lookup"><span data-stu-id="c34a8-108">Method</span></span>|<span data-ttu-id="c34a8-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c34a8-109">Return Type</span></span>|<span data-ttu-id="c34a8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c34a8-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c34a8-111">Listar managedDeviceMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="c34a8-111">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="c34a8-112">Coleção [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c34a8-112">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="c34a8-113">Lista propriedades e relações dos objetos [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c34a8-113">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="c34a8-114">Obter managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="c34a8-114">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="c34a8-115">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="c34a8-115">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="c34a8-116">Propriedades de leitura e relações do objeto [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c34a8-116">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="c34a8-117">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="c34a8-117">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="c34a8-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c34a8-118">None</span></span>|<span data-ttu-id="c34a8-119">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c34a8-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="c34a8-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c34a8-120">Properties</span></span>
|<span data-ttu-id="c34a8-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c34a8-121">Property</span></span>|<span data-ttu-id="c34a8-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="c34a8-122">Type</span></span>|<span data-ttu-id="c34a8-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c34a8-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c34a8-124">id</span><span class="sxs-lookup"><span data-stu-id="c34a8-124">id</span></span>|<span data-ttu-id="c34a8-125">String</span><span class="sxs-lookup"><span data-stu-id="c34a8-125">String</span></span>|<span data-ttu-id="c34a8-126">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c34a8-126">Key of the entity.</span></span>|
|<span data-ttu-id="c34a8-127">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="c34a8-127">targetedMobileApps</span></span>|<span data-ttu-id="c34a8-128">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c34a8-128">String collection</span></span>|<span data-ttu-id="c34a8-129">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="c34a8-129">the associated app.</span></span>|
|<span data-ttu-id="c34a8-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c34a8-130">createdDateTime</span></span>|<span data-ttu-id="c34a8-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c34a8-131">DateTimeOffset</span></span>|<span data-ttu-id="c34a8-132">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="c34a8-132">DateTime the object was created.</span></span>|
|<span data-ttu-id="c34a8-133">description</span><span class="sxs-lookup"><span data-stu-id="c34a8-133">description</span></span>|<span data-ttu-id="c34a8-134">String</span><span class="sxs-lookup"><span data-stu-id="c34a8-134">String</span></span>|<span data-ttu-id="c34a8-135">Descrição fornecida pelo administrador da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c34a8-135">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="c34a8-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c34a8-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c34a8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c34a8-137">DateTimeOffset</span></span>|<span data-ttu-id="c34a8-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="c34a8-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="c34a8-139">displayName</span><span class="sxs-lookup"><span data-stu-id="c34a8-139">displayName</span></span>|<span data-ttu-id="c34a8-140">String</span><span class="sxs-lookup"><span data-stu-id="c34a8-140">String</span></span>|<span data-ttu-id="c34a8-141">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c34a8-141">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="c34a8-142">versão</span><span class="sxs-lookup"><span data-stu-id="c34a8-142">version</span></span>|<span data-ttu-id="c34a8-143">Int32</span><span class="sxs-lookup"><span data-stu-id="c34a8-143">Int32</span></span>|<span data-ttu-id="c34a8-144">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c34a8-144">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c34a8-145">Relações</span><span class="sxs-lookup"><span data-stu-id="c34a8-145">Relationships</span></span>
|<span data-ttu-id="c34a8-146">Relação</span><span class="sxs-lookup"><span data-stu-id="c34a8-146">Relationship</span></span>|<span data-ttu-id="c34a8-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="c34a8-147">Type</span></span>|<span data-ttu-id="c34a8-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="c34a8-148">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c34a8-149">assignments</span><span class="sxs-lookup"><span data-stu-id="c34a8-149">assignments</span></span>|<span data-ttu-id="c34a8-150">Coleção [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="c34a8-150">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="c34a8-151">A lista de atribuições de grupo para configuração de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="c34a8-151">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="c34a8-152">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="c34a8-152">deviceStatuses</span></span>|<span data-ttu-id="c34a8-153">coleção [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="c34a8-153">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="c34a8-154">Lista de ManagedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="c34a8-154">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="c34a8-155">userStatuses</span><span class="sxs-lookup"><span data-stu-id="c34a8-155">userStatuses</span></span>|<span data-ttu-id="c34a8-156">Coleção [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="c34a8-156">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="c34a8-157">Lista de ManagedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="c34a8-157">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="c34a8-158">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="c34a8-158">deviceStatusSummary</span></span>|[<span data-ttu-id="c34a8-159">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="c34a8-159">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="c34a8-160">Resumo do status do dispositivo de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c34a8-160">App configuration device status summary.</span></span>|
|<span data-ttu-id="c34a8-161">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="c34a8-161">userStatusSummary</span></span>|[<span data-ttu-id="c34a8-162">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="c34a8-162">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="c34a8-163">Resumo do status do usuário de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c34a8-163">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c34a8-164">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c34a8-164">JSON Representation</span></span>
<span data-ttu-id="c34a8-165">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c34a8-165">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfiguration",
  "id": "String (identifier)",
  "targetedMobileApps": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```









