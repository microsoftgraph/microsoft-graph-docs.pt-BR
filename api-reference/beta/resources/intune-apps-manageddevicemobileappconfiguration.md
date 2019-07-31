---
title: Tipo de recurso managedDeviceMobileAppConfiguration
description: Uma classe abstrata para a configuração do Aplicativo móvel para dispositivos registrados.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: de75ee42f0e87c6d150d86bccfccb278ebcd29b2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005342"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="536be-103">Tipo de recurso managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="536be-103">managedDeviceMobileAppConfiguration resource type</span></span>

> <span data-ttu-id="536be-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="536be-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="536be-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="536be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="536be-106">Uma classe abstrata para a configuração do Aplicativo móvel para dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="536be-106">An abstract class for Mobile app configuration for enrolled devices.</span></span>

## <a name="methods"></a><span data-ttu-id="536be-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="536be-107">Methods</span></span>
|<span data-ttu-id="536be-108">Método</span><span class="sxs-lookup"><span data-stu-id="536be-108">Method</span></span>|<span data-ttu-id="536be-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="536be-109">Return Type</span></span>|<span data-ttu-id="536be-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="536be-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="536be-111">Listar managedDeviceMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="536be-111">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="536be-112">Coleção [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="536be-112">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="536be-113">Lista propriedades e relações dos objetos [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="536be-113">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="536be-114">Obter managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="536be-114">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="536be-115">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="536be-115">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="536be-116">Propriedades de leitura e relações do objeto [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="536be-116">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="536be-117">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="536be-117">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="536be-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="536be-118">None</span></span>|<span data-ttu-id="536be-119">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="536be-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="536be-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="536be-120">Properties</span></span>
|<span data-ttu-id="536be-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="536be-121">Property</span></span>|<span data-ttu-id="536be-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="536be-122">Type</span></span>|<span data-ttu-id="536be-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="536be-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="536be-124">id</span><span class="sxs-lookup"><span data-stu-id="536be-124">id</span></span>|<span data-ttu-id="536be-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="536be-125">String</span></span>|<span data-ttu-id="536be-126">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="536be-126">Key of the entity.</span></span>|
|<span data-ttu-id="536be-127">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="536be-127">targetedMobileApps</span></span>|<span data-ttu-id="536be-128">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="536be-128">String collection</span></span>|<span data-ttu-id="536be-129">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="536be-129">the associated app.</span></span>|
|<span data-ttu-id="536be-130">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="536be-130">roleScopeTagIds</span></span>|<span data-ttu-id="536be-131">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="536be-131">String collection</span></span>|<span data-ttu-id="536be-132">Lista de marcas de escopo para esta entidade de configuração de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="536be-132">List of Scope Tags for this App configuration entity.</span></span>|
|<span data-ttu-id="536be-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="536be-133">createdDateTime</span></span>|<span data-ttu-id="536be-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="536be-134">DateTimeOffset</span></span>|<span data-ttu-id="536be-135">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="536be-135">DateTime the object was created.</span></span>|
|<span data-ttu-id="536be-136">descrição</span><span class="sxs-lookup"><span data-stu-id="536be-136">description</span></span>|<span data-ttu-id="536be-137">String</span><span class="sxs-lookup"><span data-stu-id="536be-137">String</span></span>|<span data-ttu-id="536be-138">Descrição fornecida pelo administrador da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="536be-138">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="536be-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="536be-139">lastModifiedDateTime</span></span>|<span data-ttu-id="536be-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="536be-140">DateTimeOffset</span></span>|<span data-ttu-id="536be-141">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="536be-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="536be-142">displayName</span><span class="sxs-lookup"><span data-stu-id="536be-142">displayName</span></span>|<span data-ttu-id="536be-143">String</span><span class="sxs-lookup"><span data-stu-id="536be-143">String</span></span>|<span data-ttu-id="536be-144">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="536be-144">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="536be-145">versão</span><span class="sxs-lookup"><span data-stu-id="536be-145">version</span></span>|<span data-ttu-id="536be-146">Int32</span><span class="sxs-lookup"><span data-stu-id="536be-146">Int32</span></span>|<span data-ttu-id="536be-147">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="536be-147">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="536be-148">Relações</span><span class="sxs-lookup"><span data-stu-id="536be-148">Relationships</span></span>
|<span data-ttu-id="536be-149">Relação</span><span class="sxs-lookup"><span data-stu-id="536be-149">Relationship</span></span>|<span data-ttu-id="536be-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="536be-150">Type</span></span>|<span data-ttu-id="536be-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="536be-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="536be-152">assignments</span><span class="sxs-lookup"><span data-stu-id="536be-152">assignments</span></span>|<span data-ttu-id="536be-153">Coleção [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="536be-153">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="536be-154">A lista de atribuições de grupo para configuração de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="536be-154">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="536be-155">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="536be-155">deviceStatuses</span></span>|<span data-ttu-id="536be-156">coleção [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="536be-156">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="536be-157">Lista de ManagedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="536be-157">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="536be-158">userStatuses</span><span class="sxs-lookup"><span data-stu-id="536be-158">userStatuses</span></span>|<span data-ttu-id="536be-159">Coleção [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="536be-159">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="536be-160">Lista de ManagedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="536be-160">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="536be-161">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="536be-161">deviceStatusSummary</span></span>|[<span data-ttu-id="536be-162">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="536be-162">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="536be-163">Resumo do status do dispositivo de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="536be-163">App configuration device status summary.</span></span>|
|<span data-ttu-id="536be-164">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="536be-164">userStatusSummary</span></span>|[<span data-ttu-id="536be-165">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="536be-165">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="536be-166">Resumo do status do usuário de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="536be-166">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="536be-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="536be-167">JSON Representation</span></span>
<span data-ttu-id="536be-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="536be-168">Here is a JSON representation of the resource.</span></span>
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





