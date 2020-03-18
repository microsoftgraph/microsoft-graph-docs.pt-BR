---
title: Tipo de recurso managedDeviceMobileAppConfiguration
description: Uma classe abstrata para a configuração do Aplicativo móvel para dispositivos registrados.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9f4163cdf7d137756e86dc98529db4f3eb5c6b12
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797955"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="cfad5-103">Tipo de recurso managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="cfad5-103">managedDeviceMobileAppConfiguration resource type</span></span>

> <span data-ttu-id="cfad5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cfad5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cfad5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cfad5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfad5-106">Uma classe abstrata para a configuração do Aplicativo móvel para dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="cfad5-106">An abstract class for Mobile app configuration for enrolled devices.</span></span>

## <a name="methods"></a><span data-ttu-id="cfad5-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="cfad5-107">Methods</span></span>
|<span data-ttu-id="cfad5-108">Método</span><span class="sxs-lookup"><span data-stu-id="cfad5-108">Method</span></span>|<span data-ttu-id="cfad5-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cfad5-109">Return Type</span></span>|<span data-ttu-id="cfad5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfad5-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cfad5-111">Listar managedDeviceMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="cfad5-111">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="cfad5-112">Coleção [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cfad5-112">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="cfad5-113">Lista propriedades e relações dos objetos [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cfad5-113">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="cfad5-114">Obter managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="cfad5-114">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="cfad5-115">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="cfad5-115">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="cfad5-116">Propriedades de leitura e relações do objeto [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="cfad5-116">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="cfad5-117">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="cfad5-117">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="cfad5-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="cfad5-118">None</span></span>|<span data-ttu-id="cfad5-119">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="cfad5-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="cfad5-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cfad5-120">Properties</span></span>
|<span data-ttu-id="cfad5-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cfad5-121">Property</span></span>|<span data-ttu-id="cfad5-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="cfad5-122">Type</span></span>|<span data-ttu-id="cfad5-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfad5-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfad5-124">id</span><span class="sxs-lookup"><span data-stu-id="cfad5-124">id</span></span>|<span data-ttu-id="cfad5-125">String</span><span class="sxs-lookup"><span data-stu-id="cfad5-125">String</span></span>|<span data-ttu-id="cfad5-126">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cfad5-126">Key of the entity.</span></span>|
|<span data-ttu-id="cfad5-127">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="cfad5-127">targetedMobileApps</span></span>|<span data-ttu-id="cfad5-128">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="cfad5-128">String collection</span></span>|<span data-ttu-id="cfad5-129">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="cfad5-129">the associated app.</span></span>|
|<span data-ttu-id="cfad5-130">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cfad5-130">roleScopeTagIds</span></span>|<span data-ttu-id="cfad5-131">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="cfad5-131">String collection</span></span>|<span data-ttu-id="cfad5-132">Lista de marcas de escopo para esta entidade de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cfad5-132">List of Scope Tags for this App configuration entity.</span></span>|
|<span data-ttu-id="cfad5-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cfad5-133">createdDateTime</span></span>|<span data-ttu-id="cfad5-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfad5-134">DateTimeOffset</span></span>|<span data-ttu-id="cfad5-135">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="cfad5-135">DateTime the object was created.</span></span>|
|<span data-ttu-id="cfad5-136">description</span><span class="sxs-lookup"><span data-stu-id="cfad5-136">description</span></span>|<span data-ttu-id="cfad5-137">String</span><span class="sxs-lookup"><span data-stu-id="cfad5-137">String</span></span>|<span data-ttu-id="cfad5-138">Descrição fornecida pelo administrador da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cfad5-138">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="cfad5-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cfad5-139">lastModifiedDateTime</span></span>|<span data-ttu-id="cfad5-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfad5-140">DateTimeOffset</span></span>|<span data-ttu-id="cfad5-141">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="cfad5-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="cfad5-142">displayName</span><span class="sxs-lookup"><span data-stu-id="cfad5-142">displayName</span></span>|<span data-ttu-id="cfad5-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cfad5-143">String</span></span>|<span data-ttu-id="cfad5-144">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cfad5-144">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="cfad5-145">versão</span><span class="sxs-lookup"><span data-stu-id="cfad5-145">version</span></span>|<span data-ttu-id="cfad5-146">Int32</span><span class="sxs-lookup"><span data-stu-id="cfad5-146">Int32</span></span>|<span data-ttu-id="cfad5-147">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cfad5-147">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cfad5-148">Relações</span><span class="sxs-lookup"><span data-stu-id="cfad5-148">Relationships</span></span>
|<span data-ttu-id="cfad5-149">Relação</span><span class="sxs-lookup"><span data-stu-id="cfad5-149">Relationship</span></span>|<span data-ttu-id="cfad5-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="cfad5-150">Type</span></span>|<span data-ttu-id="cfad5-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfad5-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfad5-152">assignments</span><span class="sxs-lookup"><span data-stu-id="cfad5-152">assignments</span></span>|<span data-ttu-id="cfad5-153">Coleção [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="cfad5-153">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="cfad5-154">A lista de atribuições de grupo para configuração de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="cfad5-154">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="cfad5-155">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="cfad5-155">deviceStatuses</span></span>|<span data-ttu-id="cfad5-156">coleção [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="cfad5-156">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="cfad5-157">Lista de ManagedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="cfad5-157">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="cfad5-158">userStatuses</span><span class="sxs-lookup"><span data-stu-id="cfad5-158">userStatuses</span></span>|<span data-ttu-id="cfad5-159">Coleção [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="cfad5-159">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="cfad5-160">Lista de ManagedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="cfad5-160">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="cfad5-161">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="cfad5-161">deviceStatusSummary</span></span>|[<span data-ttu-id="cfad5-162">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="cfad5-162">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="cfad5-163">Resumo do status do dispositivo de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cfad5-163">App configuration device status summary.</span></span>|
|<span data-ttu-id="cfad5-164">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="cfad5-164">userStatusSummary</span></span>|[<span data-ttu-id="cfad5-165">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="cfad5-165">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="cfad5-166">Resumo do status do usuário de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cfad5-166">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cfad5-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cfad5-167">JSON Representation</span></span>
<span data-ttu-id="cfad5-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cfad5-168">Here is a JSON representation of the resource.</span></span>
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
  "roleScopeTagIds": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```



