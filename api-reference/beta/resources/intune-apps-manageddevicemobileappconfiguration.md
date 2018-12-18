---
title: Tipo de recurso managedDeviceMobileAppConfiguration
description: Uma classe abstrata para a configuração do Aplicativo móvel para dispositivos registrados.
author: tfitzmac
ms.openlocfilehash: a533d5d7c15a32d811a7fd23f9ab39b89db9b7da
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352035"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="8867c-103">Tipo de recurso managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="8867c-103">managedDeviceMobileAppConfiguration resource type</span></span>

> <span data-ttu-id="8867c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8867c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8867c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8867c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8867c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8867c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8867c-107">Uma classe abstrata para a configuração do Aplicativo móvel para dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="8867c-107">An abstract class for Mobile app configuration for enrolled devices.</span></span>
## <a name="methods"></a><span data-ttu-id="8867c-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="8867c-108">Methods</span></span>
|<span data-ttu-id="8867c-109">Método</span><span class="sxs-lookup"><span data-stu-id="8867c-109">Method</span></span>|<span data-ttu-id="8867c-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8867c-110">Return Type</span></span>|<span data-ttu-id="8867c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8867c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8867c-112">Listar managedDeviceMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="8867c-112">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="8867c-113">Coleção [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8867c-113">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="8867c-114">Lista propriedades e relações dos objetos [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8867c-114">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="8867c-115">Obter managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="8867c-115">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="8867c-116">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="8867c-116">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="8867c-117">Propriedades de leitura e relações do objeto [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="8867c-117">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="8867c-118">Ação assign</span><span class="sxs-lookup"><span data-stu-id="8867c-118">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="8867c-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8867c-119">None</span></span>|<span data-ttu-id="8867c-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8867c-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="8867c-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8867c-121">Properties</span></span>
|<span data-ttu-id="8867c-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8867c-122">Property</span></span>|<span data-ttu-id="8867c-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="8867c-123">Type</span></span>|<span data-ttu-id="8867c-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="8867c-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8867c-125">id</span><span class="sxs-lookup"><span data-stu-id="8867c-125">id</span></span>|<span data-ttu-id="8867c-126">String</span><span class="sxs-lookup"><span data-stu-id="8867c-126">String</span></span>|<span data-ttu-id="8867c-127">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="8867c-127">Key of the entity.</span></span>|
|<span data-ttu-id="8867c-128">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="8867c-128">targetedMobileApps</span></span>|<span data-ttu-id="8867c-129">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8867c-129">String collection</span></span>|<span data-ttu-id="8867c-130">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="8867c-130">the associated app.</span></span>|
|<span data-ttu-id="8867c-131">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8867c-131">roleScopeTagIds</span></span>|<span data-ttu-id="8867c-132">String collection</span><span class="sxs-lookup"><span data-stu-id="8867c-132">String collection</span></span>|<span data-ttu-id="8867c-133">Lista de escopo marcas para essa entidade de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8867c-133">List of Scope Tags for this App configuration entity.</span></span>|
|<span data-ttu-id="8867c-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8867c-134">createdDateTime</span></span>|<span data-ttu-id="8867c-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8867c-135">DateTimeOffset</span></span>|<span data-ttu-id="8867c-136">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="8867c-136">DateTime the object was created.</span></span>|
|<span data-ttu-id="8867c-137">description</span><span class="sxs-lookup"><span data-stu-id="8867c-137">description</span></span>|<span data-ttu-id="8867c-138">String</span><span class="sxs-lookup"><span data-stu-id="8867c-138">String</span></span>|<span data-ttu-id="8867c-139">Descrição fornecida pelo administrador da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8867c-139">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="8867c-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8867c-140">lastModifiedDateTime</span></span>|<span data-ttu-id="8867c-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8867c-141">DateTimeOffset</span></span>|<span data-ttu-id="8867c-142">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="8867c-142">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="8867c-143">displayName</span><span class="sxs-lookup"><span data-stu-id="8867c-143">displayName</span></span>|<span data-ttu-id="8867c-144">String</span><span class="sxs-lookup"><span data-stu-id="8867c-144">String</span></span>|<span data-ttu-id="8867c-145">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8867c-145">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="8867c-146">version</span><span class="sxs-lookup"><span data-stu-id="8867c-146">version</span></span>|<span data-ttu-id="8867c-147">Int32</span><span class="sxs-lookup"><span data-stu-id="8867c-147">Int32</span></span>|<span data-ttu-id="8867c-148">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8867c-148">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8867c-149">Relações</span><span class="sxs-lookup"><span data-stu-id="8867c-149">Relationships</span></span>
|<span data-ttu-id="8867c-150">Relação</span><span class="sxs-lookup"><span data-stu-id="8867c-150">Relationship</span></span>|<span data-ttu-id="8867c-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="8867c-151">Type</span></span>|<span data-ttu-id="8867c-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="8867c-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8867c-153">assignments</span><span class="sxs-lookup"><span data-stu-id="8867c-153">assignments</span></span>|<span data-ttu-id="8867c-154">Coleção [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="8867c-154">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="8867c-155">A lista de atribuições de grupo para configuração de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="8867c-155">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="8867c-156">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="8867c-156">deviceStatuses</span></span>|<span data-ttu-id="8867c-157">coleção [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="8867c-157">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="8867c-158">Lista de ManagedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="8867c-158">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="8867c-159">userStatuses</span><span class="sxs-lookup"><span data-stu-id="8867c-159">userStatuses</span></span>|<span data-ttu-id="8867c-160">Coleção [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="8867c-160">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="8867c-161">Lista de ManagedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="8867c-161">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="8867c-162">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="8867c-162">deviceStatusSummary</span></span>|[<span data-ttu-id="8867c-163">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="8867c-163">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="8867c-164">Resumo do status do dispositivo de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8867c-164">App configuration device status summary.</span></span>|
|<span data-ttu-id="8867c-165">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="8867c-165">userStatusSummary</span></span>|[<span data-ttu-id="8867c-166">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="8867c-166">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="8867c-167">Resumo do status do usuário de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8867c-167">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8867c-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8867c-168">JSON Representation</span></span>
<span data-ttu-id="8867c-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8867c-169">Here is a JSON representation of the resource.</span></span>
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





