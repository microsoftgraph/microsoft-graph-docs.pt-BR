---
title: Tipo de recurso managedDeviceMobileAppConfiguration
description: Uma classe abstrata para a configuração do Aplicativo móvel para dispositivos registrados.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f9a642f00e9dce09628083a8278e6010a220bee2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918984"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="7039b-103">Tipo de recurso managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="7039b-103">managedDeviceMobileAppConfiguration resource type</span></span>

> <span data-ttu-id="7039b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7039b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7039b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7039b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7039b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7039b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7039b-107">Uma classe abstrata para a configuração do Aplicativo móvel para dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="7039b-107">An abstract class for Mobile app configuration for enrolled devices.</span></span>
## <a name="methods"></a><span data-ttu-id="7039b-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="7039b-108">Methods</span></span>
|<span data-ttu-id="7039b-109">Método</span><span class="sxs-lookup"><span data-stu-id="7039b-109">Method</span></span>|<span data-ttu-id="7039b-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7039b-110">Return Type</span></span>|<span data-ttu-id="7039b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7039b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7039b-112">Listar managedDeviceMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="7039b-112">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="7039b-113">Coleção [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7039b-113">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="7039b-114">Lista propriedades e relações dos objetos [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7039b-114">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="7039b-115">Obter managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="7039b-115">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="7039b-116">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="7039b-116">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="7039b-117">Propriedades de leitura e relações do objeto [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7039b-117">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="7039b-118">Ação assign</span><span class="sxs-lookup"><span data-stu-id="7039b-118">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="7039b-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7039b-119">None</span></span>|<span data-ttu-id="7039b-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7039b-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="7039b-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7039b-121">Properties</span></span>
|<span data-ttu-id="7039b-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7039b-122">Property</span></span>|<span data-ttu-id="7039b-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="7039b-123">Type</span></span>|<span data-ttu-id="7039b-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="7039b-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7039b-125">id</span><span class="sxs-lookup"><span data-stu-id="7039b-125">id</span></span>|<span data-ttu-id="7039b-126">String</span><span class="sxs-lookup"><span data-stu-id="7039b-126">String</span></span>|<span data-ttu-id="7039b-127">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="7039b-127">Key of the entity.</span></span>|
|<span data-ttu-id="7039b-128">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="7039b-128">targetedMobileApps</span></span>|<span data-ttu-id="7039b-129">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7039b-129">String collection</span></span>|<span data-ttu-id="7039b-130">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="7039b-130">the associated app.</span></span>|
|<span data-ttu-id="7039b-131">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7039b-131">roleScopeTagIds</span></span>|<span data-ttu-id="7039b-132">String collection</span><span class="sxs-lookup"><span data-stu-id="7039b-132">String collection</span></span>|<span data-ttu-id="7039b-133">Lista de escopo marcas para essa entidade de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7039b-133">List of Scope Tags for this App configuration entity.</span></span>|
|<span data-ttu-id="7039b-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7039b-134">createdDateTime</span></span>|<span data-ttu-id="7039b-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7039b-135">DateTimeOffset</span></span>|<span data-ttu-id="7039b-136">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="7039b-136">DateTime the object was created.</span></span>|
|<span data-ttu-id="7039b-137">description</span><span class="sxs-lookup"><span data-stu-id="7039b-137">description</span></span>|<span data-ttu-id="7039b-138">String</span><span class="sxs-lookup"><span data-stu-id="7039b-138">String</span></span>|<span data-ttu-id="7039b-139">Descrição fornecida pelo administrador da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7039b-139">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="7039b-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7039b-140">lastModifiedDateTime</span></span>|<span data-ttu-id="7039b-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7039b-141">DateTimeOffset</span></span>|<span data-ttu-id="7039b-142">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="7039b-142">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="7039b-143">displayName</span><span class="sxs-lookup"><span data-stu-id="7039b-143">displayName</span></span>|<span data-ttu-id="7039b-144">String</span><span class="sxs-lookup"><span data-stu-id="7039b-144">String</span></span>|<span data-ttu-id="7039b-145">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7039b-145">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="7039b-146">version</span><span class="sxs-lookup"><span data-stu-id="7039b-146">version</span></span>|<span data-ttu-id="7039b-147">Int32</span><span class="sxs-lookup"><span data-stu-id="7039b-147">Int32</span></span>|<span data-ttu-id="7039b-148">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7039b-148">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7039b-149">Relações</span><span class="sxs-lookup"><span data-stu-id="7039b-149">Relationships</span></span>
|<span data-ttu-id="7039b-150">Relação</span><span class="sxs-lookup"><span data-stu-id="7039b-150">Relationship</span></span>|<span data-ttu-id="7039b-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="7039b-151">Type</span></span>|<span data-ttu-id="7039b-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="7039b-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7039b-153">assignments</span><span class="sxs-lookup"><span data-stu-id="7039b-153">assignments</span></span>|<span data-ttu-id="7039b-154">Coleção [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7039b-154">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="7039b-155">A lista de atribuições de grupo para configuração de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="7039b-155">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="7039b-156">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="7039b-156">deviceStatuses</span></span>|<span data-ttu-id="7039b-157">coleção [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="7039b-157">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="7039b-158">Lista de ManagedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="7039b-158">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="7039b-159">userStatuses</span><span class="sxs-lookup"><span data-stu-id="7039b-159">userStatuses</span></span>|<span data-ttu-id="7039b-160">Coleção [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="7039b-160">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="7039b-161">Lista de ManagedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="7039b-161">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="7039b-162">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="7039b-162">deviceStatusSummary</span></span>|[<span data-ttu-id="7039b-163">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="7039b-163">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="7039b-164">Resumo do status do dispositivo de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7039b-164">App configuration device status summary.</span></span>|
|<span data-ttu-id="7039b-165">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="7039b-165">userStatusSummary</span></span>|[<span data-ttu-id="7039b-166">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="7039b-166">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="7039b-167">Resumo do status do usuário de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7039b-167">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7039b-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7039b-168">JSON Representation</span></span>
<span data-ttu-id="7039b-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7039b-169">Here is a JSON representation of the resource.</span></span>
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





