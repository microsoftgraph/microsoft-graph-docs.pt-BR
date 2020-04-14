---
title: Tipo de recurso managedDeviceMobileAppConfiguration
description: Uma classe abstrata para a configuração do Aplicativo móvel para dispositivos registrados.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d4deb062c7b927712d0557aa3257ba719e45bc12
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43458719"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="b7879-103">Tipo de recurso managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="b7879-103">managedDeviceMobileAppConfiguration resource type</span></span>

<span data-ttu-id="b7879-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7879-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b7879-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b7879-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7879-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b7879-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7879-107">Uma classe abstrata para a configuração do Aplicativo móvel para dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="b7879-107">An abstract class for Mobile app configuration for enrolled devices.</span></span>

## <a name="methods"></a><span data-ttu-id="b7879-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="b7879-108">Methods</span></span>
|<span data-ttu-id="b7879-109">Método</span><span class="sxs-lookup"><span data-stu-id="b7879-109">Method</span></span>|<span data-ttu-id="b7879-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b7879-110">Return Type</span></span>|<span data-ttu-id="b7879-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7879-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b7879-112">Listar managedDeviceMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="b7879-112">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="b7879-113">Coleção [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b7879-113">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="b7879-114">Lista propriedades e relações dos objetos [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b7879-114">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="b7879-115">Obter managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="b7879-115">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="b7879-116">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="b7879-116">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="b7879-117">Propriedades de leitura e relações do objeto [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b7879-117">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="b7879-118">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="b7879-118">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="b7879-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="b7879-119">None</span></span>|<span data-ttu-id="b7879-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b7879-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="b7879-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b7879-121">Properties</span></span>
|<span data-ttu-id="b7879-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b7879-122">Property</span></span>|<span data-ttu-id="b7879-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7879-123">Type</span></span>|<span data-ttu-id="b7879-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7879-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7879-125">id</span><span class="sxs-lookup"><span data-stu-id="b7879-125">id</span></span>|<span data-ttu-id="b7879-126">String</span><span class="sxs-lookup"><span data-stu-id="b7879-126">String</span></span>|<span data-ttu-id="b7879-127">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b7879-127">Key of the entity.</span></span>|
|<span data-ttu-id="b7879-128">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="b7879-128">targetedMobileApps</span></span>|<span data-ttu-id="b7879-129">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b7879-129">String collection</span></span>|<span data-ttu-id="b7879-130">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="b7879-130">the associated app.</span></span>|
|<span data-ttu-id="b7879-131">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b7879-131">roleScopeTagIds</span></span>|<span data-ttu-id="b7879-132">Coleção String</span><span class="sxs-lookup"><span data-stu-id="b7879-132">String collection</span></span>|<span data-ttu-id="b7879-133">Lista de marcas de escopo para esta entidade de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b7879-133">List of Scope Tags for this App configuration entity.</span></span>|
|<span data-ttu-id="b7879-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b7879-134">createdDateTime</span></span>|<span data-ttu-id="b7879-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7879-135">DateTimeOffset</span></span>|<span data-ttu-id="b7879-136">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="b7879-136">DateTime the object was created.</span></span>|
|<span data-ttu-id="b7879-137">description</span><span class="sxs-lookup"><span data-stu-id="b7879-137">description</span></span>|<span data-ttu-id="b7879-138">String</span><span class="sxs-lookup"><span data-stu-id="b7879-138">String</span></span>|<span data-ttu-id="b7879-139">Descrição fornecida pelo administrador da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b7879-139">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="b7879-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b7879-140">lastModifiedDateTime</span></span>|<span data-ttu-id="b7879-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7879-141">DateTimeOffset</span></span>|<span data-ttu-id="b7879-142">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="b7879-142">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="b7879-143">displayName</span><span class="sxs-lookup"><span data-stu-id="b7879-143">displayName</span></span>|<span data-ttu-id="b7879-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b7879-144">String</span></span>|<span data-ttu-id="b7879-145">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b7879-145">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="b7879-146">versão</span><span class="sxs-lookup"><span data-stu-id="b7879-146">version</span></span>|<span data-ttu-id="b7879-147">Int32</span><span class="sxs-lookup"><span data-stu-id="b7879-147">Int32</span></span>|<span data-ttu-id="b7879-148">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b7879-148">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b7879-149">Relações</span><span class="sxs-lookup"><span data-stu-id="b7879-149">Relationships</span></span>
|<span data-ttu-id="b7879-150">Relação</span><span class="sxs-lookup"><span data-stu-id="b7879-150">Relationship</span></span>|<span data-ttu-id="b7879-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7879-151">Type</span></span>|<span data-ttu-id="b7879-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7879-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7879-153">assignments</span><span class="sxs-lookup"><span data-stu-id="b7879-153">assignments</span></span>|<span data-ttu-id="b7879-154">Coleção [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b7879-154">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="b7879-155">A lista de atribuições de grupo para configuração de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="b7879-155">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="b7879-156">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="b7879-156">deviceStatuses</span></span>|<span data-ttu-id="b7879-157">coleção [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="b7879-157">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="b7879-158">Lista de ManagedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="b7879-158">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="b7879-159">userStatuses</span><span class="sxs-lookup"><span data-stu-id="b7879-159">userStatuses</span></span>|<span data-ttu-id="b7879-160">Coleção [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="b7879-160">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="b7879-161">Lista de ManagedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="b7879-161">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="b7879-162">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="b7879-162">deviceStatusSummary</span></span>|[<span data-ttu-id="b7879-163">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="b7879-163">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="b7879-164">Resumo do status do dispositivo de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b7879-164">App configuration device status summary.</span></span>|
|<span data-ttu-id="b7879-165">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="b7879-165">userStatusSummary</span></span>|[<span data-ttu-id="b7879-166">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="b7879-166">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="b7879-167">Resumo do status do usuário de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b7879-167">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b7879-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b7879-168">JSON Representation</span></span>
<span data-ttu-id="b7879-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b7879-169">Here is a JSON representation of the resource.</span></span>
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



