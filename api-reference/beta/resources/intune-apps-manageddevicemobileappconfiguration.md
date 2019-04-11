---
title: Tipo de recurso managedDeviceMobileAppConfiguration
description: Uma classe abstrata para a configuração do Aplicativo móvel para dispositivos registrados.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4646ebc07865cadda7005e25b4b30a2547a41f8b
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31781600"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="813d2-103">Tipo de recurso managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="813d2-103">managedDeviceMobileAppConfiguration resource type</span></span>

> <span data-ttu-id="813d2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="813d2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="813d2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="813d2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="813d2-106">Uma classe abstrata para a configuração do Aplicativo móvel para dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="813d2-106">An abstract class for Mobile app configuration for enrolled devices.</span></span>

## <a name="methods"></a><span data-ttu-id="813d2-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="813d2-107">Methods</span></span>
|<span data-ttu-id="813d2-108">Método</span><span class="sxs-lookup"><span data-stu-id="813d2-108">Method</span></span>|<span data-ttu-id="813d2-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="813d2-109">Return Type</span></span>|<span data-ttu-id="813d2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="813d2-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="813d2-111">Listar managedDeviceMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="813d2-111">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="813d2-112">Coleção [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="813d2-112">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="813d2-113">Lista propriedades e relações dos objetos [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="813d2-113">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="813d2-114">Obter managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="813d2-114">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="813d2-115">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="813d2-115">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="813d2-116">Ler propriedades e relações do objeto [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="813d2-116">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="813d2-117">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="813d2-117">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="813d2-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="813d2-118">None</span></span>|<span data-ttu-id="813d2-119">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="813d2-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="813d2-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="813d2-120">Properties</span></span>
|<span data-ttu-id="813d2-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="813d2-121">Property</span></span>|<span data-ttu-id="813d2-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="813d2-122">Type</span></span>|<span data-ttu-id="813d2-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="813d2-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="813d2-124">id</span><span class="sxs-lookup"><span data-stu-id="813d2-124">id</span></span>|<span data-ttu-id="813d2-125">String</span><span class="sxs-lookup"><span data-stu-id="813d2-125">String</span></span>|<span data-ttu-id="813d2-126">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="813d2-126">Key of the entity.</span></span>|
|<span data-ttu-id="813d2-127">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="813d2-127">targetedMobileApps</span></span>|<span data-ttu-id="813d2-128">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="813d2-128">String collection</span></span>|<span data-ttu-id="813d2-129">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="813d2-129">the associated app.</span></span>|
|<span data-ttu-id="813d2-130">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="813d2-130">roleScopeTagIds</span></span>|<span data-ttu-id="813d2-131">Coleção String</span><span class="sxs-lookup"><span data-stu-id="813d2-131">String collection</span></span>|<span data-ttu-id="813d2-132">Lista de marcas de escopo para esta entidade de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="813d2-132">List of Scope Tags for this App configuration entity.</span></span>|
|<span data-ttu-id="813d2-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="813d2-133">createdDateTime</span></span>|<span data-ttu-id="813d2-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="813d2-134">DateTimeOffset</span></span>|<span data-ttu-id="813d2-135">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="813d2-135">DateTime the object was created.</span></span>|
|<span data-ttu-id="813d2-136">description</span><span class="sxs-lookup"><span data-stu-id="813d2-136">description</span></span>|<span data-ttu-id="813d2-137">String</span><span class="sxs-lookup"><span data-stu-id="813d2-137">String</span></span>|<span data-ttu-id="813d2-138">Descrição fornecida pelo administrador da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="813d2-138">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="813d2-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="813d2-139">lastModifiedDateTime</span></span>|<span data-ttu-id="813d2-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="813d2-140">DateTimeOffset</span></span>|<span data-ttu-id="813d2-141">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="813d2-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="813d2-142">displayName</span><span class="sxs-lookup"><span data-stu-id="813d2-142">displayName</span></span>|<span data-ttu-id="813d2-143">String</span><span class="sxs-lookup"><span data-stu-id="813d2-143">String</span></span>|<span data-ttu-id="813d2-144">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="813d2-144">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="813d2-145">versão</span><span class="sxs-lookup"><span data-stu-id="813d2-145">version</span></span>|<span data-ttu-id="813d2-146">Int32</span><span class="sxs-lookup"><span data-stu-id="813d2-146">Int32</span></span>|<span data-ttu-id="813d2-147">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="813d2-147">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="813d2-148">Relações</span><span class="sxs-lookup"><span data-stu-id="813d2-148">Relationships</span></span>
|<span data-ttu-id="813d2-149">Relação</span><span class="sxs-lookup"><span data-stu-id="813d2-149">Relationship</span></span>|<span data-ttu-id="813d2-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="813d2-150">Type</span></span>|<span data-ttu-id="813d2-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="813d2-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="813d2-152">assignments</span><span class="sxs-lookup"><span data-stu-id="813d2-152">assignments</span></span>|<span data-ttu-id="813d2-153">Coleção [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="813d2-153">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="813d2-154">A lista de atribuições de grupo para configuração de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="813d2-154">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="813d2-155">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="813d2-155">deviceStatuses</span></span>|<span data-ttu-id="813d2-156">coleção [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="813d2-156">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="813d2-157">Lista de ManagedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="813d2-157">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="813d2-158">userStatuses</span><span class="sxs-lookup"><span data-stu-id="813d2-158">userStatuses</span></span>|<span data-ttu-id="813d2-159">Coleção [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="813d2-159">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="813d2-160">Lista de ManagedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="813d2-160">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="813d2-161">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="813d2-161">deviceStatusSummary</span></span>|[<span data-ttu-id="813d2-162">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="813d2-162">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="813d2-163">Resumo do status do dispositivo de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="813d2-163">App configuration device status summary.</span></span>|
|<span data-ttu-id="813d2-164">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="813d2-164">userStatusSummary</span></span>|[<span data-ttu-id="813d2-165">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="813d2-165">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="813d2-166">Resumo do status do usuário de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="813d2-166">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="813d2-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="813d2-167">JSON Representation</span></span>
<span data-ttu-id="813d2-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="813d2-168">Here is a JSON representation of the resource.</span></span>
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





