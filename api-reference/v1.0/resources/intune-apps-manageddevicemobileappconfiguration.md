---
title: Tipo de recurso managedDeviceMobileAppConfiguration
description: Uma classe abstrata para a configuração do Aplicativo móvel para dispositivos registrados.
author: tfitzmac
ms.openlocfilehash: c51db6ddad8b23957da9ed9b8d132c416e52f073
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360022"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="6fc6d-103">Tipo de recurso managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="6fc6d-103">managedDeviceMobileAppConfiguration resource type</span></span>

> <span data-ttu-id="6fc6d-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6fc6d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6fc6d-105">Uma classe abstrata para a configuração do Aplicativo móvel para dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="6fc6d-105">An abstract class for Mobile app configuration for enrolled devices.</span></span>
## <a name="methods"></a><span data-ttu-id="6fc6d-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="6fc6d-106">Methods</span></span>
|<span data-ttu-id="6fc6d-107">Método</span><span class="sxs-lookup"><span data-stu-id="6fc6d-107">Method</span></span>|<span data-ttu-id="6fc6d-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6fc6d-108">Return Type</span></span>|<span data-ttu-id="6fc6d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fc6d-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6fc6d-110">Listar managedDeviceMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="6fc6d-110">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="6fc6d-111">Coleção [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6fc6d-111">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="6fc6d-112">Lista propriedades e relações dos objetos [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6fc6d-112">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="6fc6d-113">Obter managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="6fc6d-113">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="6fc6d-114">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="6fc6d-114">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="6fc6d-115">Propriedades de leitura e relações do objeto [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6fc6d-115">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="6fc6d-116">Ação assign</span><span class="sxs-lookup"><span data-stu-id="6fc6d-116">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="6fc6d-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6fc6d-117">None</span></span>|<span data-ttu-id="6fc6d-118">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6fc6d-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="6fc6d-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6fc6d-119">Properties</span></span>
|<span data-ttu-id="6fc6d-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6fc6d-120">Property</span></span>|<span data-ttu-id="6fc6d-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="6fc6d-121">Type</span></span>|<span data-ttu-id="6fc6d-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fc6d-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fc6d-123">id</span><span class="sxs-lookup"><span data-stu-id="6fc6d-123">id</span></span>|<span data-ttu-id="6fc6d-124">String</span><span class="sxs-lookup"><span data-stu-id="6fc6d-124">String</span></span>|<span data-ttu-id="6fc6d-125">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6fc6d-125">Key of the entity.</span></span>|
|<span data-ttu-id="6fc6d-126">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="6fc6d-126">targetedMobileApps</span></span>|<span data-ttu-id="6fc6d-127">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="6fc6d-127">String collection</span></span>|<span data-ttu-id="6fc6d-128">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="6fc6d-128">the associated app.</span></span>|
|<span data-ttu-id="6fc6d-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6fc6d-129">createdDateTime</span></span>|<span data-ttu-id="6fc6d-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fc6d-130">DateTimeOffset</span></span>|<span data-ttu-id="6fc6d-131">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6fc6d-131">DateTime the object was created.</span></span>|
|<span data-ttu-id="6fc6d-132">description</span><span class="sxs-lookup"><span data-stu-id="6fc6d-132">description</span></span>|<span data-ttu-id="6fc6d-133">String</span><span class="sxs-lookup"><span data-stu-id="6fc6d-133">String</span></span>|<span data-ttu-id="6fc6d-134">Descrição fornecida pelo administrador da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6fc6d-134">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="6fc6d-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6fc6d-135">lastModifiedDateTime</span></span>|<span data-ttu-id="6fc6d-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fc6d-136">DateTimeOffset</span></span>|<span data-ttu-id="6fc6d-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6fc6d-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="6fc6d-138">displayName</span><span class="sxs-lookup"><span data-stu-id="6fc6d-138">displayName</span></span>|<span data-ttu-id="6fc6d-139">String</span><span class="sxs-lookup"><span data-stu-id="6fc6d-139">String</span></span>|<span data-ttu-id="6fc6d-140">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6fc6d-140">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="6fc6d-141">version</span><span class="sxs-lookup"><span data-stu-id="6fc6d-141">version</span></span>|<span data-ttu-id="6fc6d-142">Int32</span><span class="sxs-lookup"><span data-stu-id="6fc6d-142">Int32</span></span>|<span data-ttu-id="6fc6d-143">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6fc6d-143">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6fc6d-144">Relações</span><span class="sxs-lookup"><span data-stu-id="6fc6d-144">Relationships</span></span>
|<span data-ttu-id="6fc6d-145">Relação</span><span class="sxs-lookup"><span data-stu-id="6fc6d-145">Relationship</span></span>|<span data-ttu-id="6fc6d-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="6fc6d-146">Type</span></span>|<span data-ttu-id="6fc6d-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fc6d-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fc6d-148">assignments</span><span class="sxs-lookup"><span data-stu-id="6fc6d-148">assignments</span></span>|<span data-ttu-id="6fc6d-149">Coleção [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="6fc6d-149">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="6fc6d-150">A lista de atribuições de grupo para configuração de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="6fc6d-150">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="6fc6d-151">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="6fc6d-151">deviceStatuses</span></span>|<span data-ttu-id="6fc6d-152">coleção [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="6fc6d-152">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="6fc6d-153">Lista de ManagedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="6fc6d-153">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="6fc6d-154">userStatuses</span><span class="sxs-lookup"><span data-stu-id="6fc6d-154">userStatuses</span></span>|<span data-ttu-id="6fc6d-155">Coleção [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="6fc6d-155">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="6fc6d-156">Lista de ManagedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="6fc6d-156">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="6fc6d-157">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="6fc6d-157">deviceStatusSummary</span></span>|[<span data-ttu-id="6fc6d-158">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="6fc6d-158">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="6fc6d-159">Resumo do status do dispositivo de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6fc6d-159">App configuration device status summary.</span></span>|
|<span data-ttu-id="6fc6d-160">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="6fc6d-160">userStatusSummary</span></span>|[<span data-ttu-id="6fc6d-161">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="6fc6d-161">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="6fc6d-162">Resumo do status do usuário de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6fc6d-162">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6fc6d-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6fc6d-163">JSON Representation</span></span>
<span data-ttu-id="6fc6d-164">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6fc6d-164">Here is a JSON representation of the resource.</span></span>
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



