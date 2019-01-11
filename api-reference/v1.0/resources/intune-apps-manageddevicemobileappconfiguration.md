---
title: Tipo de recurso managedDeviceMobileAppConfiguration
description: Uma classe abstrata para a configuração do Aplicativo móvel para dispositivos registrados.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8e2ad71a4927f2b0156d085bad54cf59d45f97c8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811645"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="8a07a-103">Tipo de recurso managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="8a07a-103">managedDeviceMobileAppConfiguration resource type</span></span>

> <span data-ttu-id="8a07a-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8a07a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8a07a-105">Uma classe abstrata para a configuração do Aplicativo móvel para dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="8a07a-105">An abstract class for Mobile app configuration for enrolled devices.</span></span>
## <a name="methods"></a><span data-ttu-id="8a07a-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="8a07a-106">Methods</span></span>
|<span data-ttu-id="8a07a-107">Método</span><span class="sxs-lookup"><span data-stu-id="8a07a-107">Method</span></span>|<span data-ttu-id="8a07a-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8a07a-108">Return Type</span></span>|<span data-ttu-id="8a07a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a07a-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8a07a-110">Listar managedDeviceMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="8a07a-110">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="8a07a-111">Coleção [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8a07a-111">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="8a07a-112">Lista propriedades e relações dos objetos [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8a07a-112">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="8a07a-113">Obter managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="8a07a-113">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="8a07a-114">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="8a07a-114">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="8a07a-115">Propriedades de leitura e relações do objeto [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8a07a-115">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="8a07a-116">Ação assign</span><span class="sxs-lookup"><span data-stu-id="8a07a-116">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="8a07a-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8a07a-117">None</span></span>|<span data-ttu-id="8a07a-118">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8a07a-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="8a07a-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8a07a-119">Properties</span></span>
|<span data-ttu-id="8a07a-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8a07a-120">Property</span></span>|<span data-ttu-id="8a07a-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="8a07a-121">Type</span></span>|<span data-ttu-id="8a07a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a07a-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a07a-123">id</span><span class="sxs-lookup"><span data-stu-id="8a07a-123">id</span></span>|<span data-ttu-id="8a07a-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a07a-124">String</span></span>|<span data-ttu-id="8a07a-125">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8a07a-125">Key of the entity.</span></span>|
|<span data-ttu-id="8a07a-126">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="8a07a-126">targetedMobileApps</span></span>|<span data-ttu-id="8a07a-127">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a07a-127">String collection</span></span>|<span data-ttu-id="8a07a-128">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="8a07a-128">the associated app.</span></span>|
|<span data-ttu-id="8a07a-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8a07a-129">createdDateTime</span></span>|<span data-ttu-id="8a07a-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a07a-130">DateTimeOffset</span></span>|<span data-ttu-id="8a07a-131">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="8a07a-131">DateTime the object was created.</span></span>|
|<span data-ttu-id="8a07a-132">description</span><span class="sxs-lookup"><span data-stu-id="8a07a-132">description</span></span>|<span data-ttu-id="8a07a-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a07a-133">String</span></span>|<span data-ttu-id="8a07a-134">Descrição fornecida pelo administrador da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8a07a-134">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="8a07a-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8a07a-135">lastModifiedDateTime</span></span>|<span data-ttu-id="8a07a-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a07a-136">DateTimeOffset</span></span>|<span data-ttu-id="8a07a-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="8a07a-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="8a07a-138">displayName</span><span class="sxs-lookup"><span data-stu-id="8a07a-138">displayName</span></span>|<span data-ttu-id="8a07a-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a07a-139">String</span></span>|<span data-ttu-id="8a07a-140">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8a07a-140">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="8a07a-141">version</span><span class="sxs-lookup"><span data-stu-id="8a07a-141">version</span></span>|<span data-ttu-id="8a07a-142">Int32</span><span class="sxs-lookup"><span data-stu-id="8a07a-142">Int32</span></span>|<span data-ttu-id="8a07a-143">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8a07a-143">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a07a-144">Relações</span><span class="sxs-lookup"><span data-stu-id="8a07a-144">Relationships</span></span>
|<span data-ttu-id="8a07a-145">Relação</span><span class="sxs-lookup"><span data-stu-id="8a07a-145">Relationship</span></span>|<span data-ttu-id="8a07a-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="8a07a-146">Type</span></span>|<span data-ttu-id="8a07a-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a07a-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a07a-148">assignments</span><span class="sxs-lookup"><span data-stu-id="8a07a-148">assignments</span></span>|<span data-ttu-id="8a07a-149">Coleção [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8a07a-149">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="8a07a-150">A lista de atribuições de grupo para configuração de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="8a07a-150">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="8a07a-151">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="8a07a-151">deviceStatuses</span></span>|<span data-ttu-id="8a07a-152">coleção [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="8a07a-152">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="8a07a-153">Lista de ManagedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="8a07a-153">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="8a07a-154">userStatuses</span><span class="sxs-lookup"><span data-stu-id="8a07a-154">userStatuses</span></span>|<span data-ttu-id="8a07a-155">Coleção [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="8a07a-155">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="8a07a-156">Lista de ManagedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="8a07a-156">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="8a07a-157">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="8a07a-157">deviceStatusSummary</span></span>|[<span data-ttu-id="8a07a-158">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="8a07a-158">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="8a07a-159">Resumo do status do dispositivo de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8a07a-159">App configuration device status summary.</span></span>|
|<span data-ttu-id="8a07a-160">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="8a07a-160">userStatusSummary</span></span>|[<span data-ttu-id="8a07a-161">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="8a07a-161">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="8a07a-162">Resumo do status do usuário de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8a07a-162">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8a07a-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8a07a-163">JSON Representation</span></span>
<span data-ttu-id="8a07a-164">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8a07a-164">Here is a JSON representation of the resource.</span></span>
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



