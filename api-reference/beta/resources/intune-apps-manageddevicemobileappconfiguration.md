---
title: Tipo de recurso managedDeviceMobileAppConfiguration
description: Uma classe abstrata para a configuração do Aplicativo móvel para dispositivos registrados.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 170045c1c83542ced8b1a4d1c631da65b6467a0e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48702604"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="4f530-103">Tipo de recurso managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="4f530-103">managedDeviceMobileAppConfiguration resource type</span></span>

<span data-ttu-id="4f530-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f530-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f530-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4f530-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f530-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4f530-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f530-107">Uma classe abstrata para a configuração do Aplicativo móvel para dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="4f530-107">An abstract class for Mobile app configuration for enrolled devices.</span></span>

## <a name="methods"></a><span data-ttu-id="4f530-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="4f530-108">Methods</span></span>
|<span data-ttu-id="4f530-109">Método</span><span class="sxs-lookup"><span data-stu-id="4f530-109">Method</span></span>|<span data-ttu-id="4f530-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4f530-110">Return Type</span></span>|<span data-ttu-id="4f530-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f530-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4f530-112">Listar managedDeviceMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="4f530-112">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="4f530-113">Coleção [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4f530-113">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="4f530-114">Lista propriedades e relações dos objetos [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f530-114">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="4f530-115">Obter managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="4f530-115">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="4f530-116">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="4f530-116">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="4f530-117">Propriedades de leitura e relações do objeto [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4f530-117">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="4f530-118">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="4f530-118">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="4f530-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="4f530-119">None</span></span>|<span data-ttu-id="4f530-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4f530-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="4f530-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4f530-121">Properties</span></span>
|<span data-ttu-id="4f530-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4f530-122">Property</span></span>|<span data-ttu-id="4f530-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f530-123">Type</span></span>|<span data-ttu-id="4f530-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f530-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f530-125">id</span><span class="sxs-lookup"><span data-stu-id="4f530-125">id</span></span>|<span data-ttu-id="4f530-126">String</span><span class="sxs-lookup"><span data-stu-id="4f530-126">String</span></span>|<span data-ttu-id="4f530-127">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4f530-127">Key of the entity.</span></span>|
|<span data-ttu-id="4f530-128">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="4f530-128">targetedMobileApps</span></span>|<span data-ttu-id="4f530-129">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f530-129">String collection</span></span>|<span data-ttu-id="4f530-130">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="4f530-130">the associated app.</span></span>|
|<span data-ttu-id="4f530-131">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4f530-131">roleScopeTagIds</span></span>|<span data-ttu-id="4f530-132">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4f530-132">String collection</span></span>|<span data-ttu-id="4f530-133">Lista de marcas de escopo para esta entidade de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4f530-133">List of Scope Tags for this App configuration entity.</span></span>|
|<span data-ttu-id="4f530-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4f530-134">createdDateTime</span></span>|<span data-ttu-id="4f530-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f530-135">DateTimeOffset</span></span>|<span data-ttu-id="4f530-136">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="4f530-136">DateTime the object was created.</span></span>|
|<span data-ttu-id="4f530-137">description</span><span class="sxs-lookup"><span data-stu-id="4f530-137">description</span></span>|<span data-ttu-id="4f530-138">String</span><span class="sxs-lookup"><span data-stu-id="4f530-138">String</span></span>|<span data-ttu-id="4f530-139">Descrição fornecida pelo administrador da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4f530-139">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="4f530-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4f530-140">lastModifiedDateTime</span></span>|<span data-ttu-id="4f530-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f530-141">DateTimeOffset</span></span>|<span data-ttu-id="4f530-142">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="4f530-142">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="4f530-143">displayName</span><span class="sxs-lookup"><span data-stu-id="4f530-143">displayName</span></span>|<span data-ttu-id="4f530-144">String</span><span class="sxs-lookup"><span data-stu-id="4f530-144">String</span></span>|<span data-ttu-id="4f530-145">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4f530-145">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="4f530-146">versão</span><span class="sxs-lookup"><span data-stu-id="4f530-146">version</span></span>|<span data-ttu-id="4f530-147">Int32</span><span class="sxs-lookup"><span data-stu-id="4f530-147">Int32</span></span>|<span data-ttu-id="4f530-148">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4f530-148">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4f530-149">Relações</span><span class="sxs-lookup"><span data-stu-id="4f530-149">Relationships</span></span>
|<span data-ttu-id="4f530-150">Relação</span><span class="sxs-lookup"><span data-stu-id="4f530-150">Relationship</span></span>|<span data-ttu-id="4f530-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f530-151">Type</span></span>|<span data-ttu-id="4f530-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f530-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f530-153">assignments</span><span class="sxs-lookup"><span data-stu-id="4f530-153">assignments</span></span>|<span data-ttu-id="4f530-154">Coleção [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="4f530-154">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="4f530-155">A lista de atribuições de grupo para configuração de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="4f530-155">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="4f530-156">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="4f530-156">deviceStatuses</span></span>|<span data-ttu-id="4f530-157">coleção [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="4f530-157">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="4f530-158">Lista de ManagedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="4f530-158">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="4f530-159">userStatuses</span><span class="sxs-lookup"><span data-stu-id="4f530-159">userStatuses</span></span>|<span data-ttu-id="4f530-160">Coleção [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="4f530-160">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="4f530-161">Lista de ManagedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="4f530-161">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="4f530-162">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="4f530-162">deviceStatusSummary</span></span>|[<span data-ttu-id="4f530-163">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="4f530-163">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="4f530-164">Resumo do status do dispositivo de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4f530-164">App configuration device status summary.</span></span>|
|<span data-ttu-id="4f530-165">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="4f530-165">userStatusSummary</span></span>|[<span data-ttu-id="4f530-166">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="4f530-166">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="4f530-167">Resumo do status do usuário de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4f530-167">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4f530-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4f530-168">JSON Representation</span></span>
<span data-ttu-id="4f530-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4f530-169">Here is a JSON representation of the resource.</span></span>
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





