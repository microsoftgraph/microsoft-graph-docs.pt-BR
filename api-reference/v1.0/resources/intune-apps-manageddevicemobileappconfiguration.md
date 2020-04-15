---
title: Tipo de recurso managedDeviceMobileAppConfiguration
description: Uma classe abstrata para a configuração do Aplicativo móvel para dispositivos registrados.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b3904ae731a4867cbc2592f1cccec2569cd27406
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43474249"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="aa735-103">Tipo de recurso managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="aa735-103">managedDeviceMobileAppConfiguration resource type</span></span>

<span data-ttu-id="aa735-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa735-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aa735-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aa735-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa735-106">Uma classe abstrata para a configuração do Aplicativo móvel para dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="aa735-106">An abstract class for Mobile app configuration for enrolled devices.</span></span>

## <a name="methods"></a><span data-ttu-id="aa735-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="aa735-107">Methods</span></span>
|<span data-ttu-id="aa735-108">Método</span><span class="sxs-lookup"><span data-stu-id="aa735-108">Method</span></span>|<span data-ttu-id="aa735-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="aa735-109">Return Type</span></span>|<span data-ttu-id="aa735-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa735-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="aa735-111">Listar managedDeviceMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="aa735-111">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="aa735-112">Coleção [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa735-112">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="aa735-113">Lista propriedades e relações dos objetos [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aa735-113">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="aa735-114">Obter managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="aa735-114">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="aa735-115">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="aa735-115">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="aa735-116">Propriedades de leitura e relações do objeto [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aa735-116">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="aa735-117">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="aa735-117">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="aa735-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="aa735-118">None</span></span>|<span data-ttu-id="aa735-119">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="aa735-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="aa735-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aa735-120">Properties</span></span>
|<span data-ttu-id="aa735-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aa735-121">Property</span></span>|<span data-ttu-id="aa735-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="aa735-122">Type</span></span>|<span data-ttu-id="aa735-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa735-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa735-124">id</span><span class="sxs-lookup"><span data-stu-id="aa735-124">id</span></span>|<span data-ttu-id="aa735-125">String</span><span class="sxs-lookup"><span data-stu-id="aa735-125">String</span></span>|<span data-ttu-id="aa735-126">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="aa735-126">Key of the entity.</span></span>|
|<span data-ttu-id="aa735-127">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="aa735-127">targetedMobileApps</span></span>|<span data-ttu-id="aa735-128">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="aa735-128">String collection</span></span>|<span data-ttu-id="aa735-129">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="aa735-129">the associated app.</span></span>|
|<span data-ttu-id="aa735-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aa735-130">createdDateTime</span></span>|<span data-ttu-id="aa735-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa735-131">DateTimeOffset</span></span>|<span data-ttu-id="aa735-132">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="aa735-132">DateTime the object was created.</span></span>|
|<span data-ttu-id="aa735-133">description</span><span class="sxs-lookup"><span data-stu-id="aa735-133">description</span></span>|<span data-ttu-id="aa735-134">String</span><span class="sxs-lookup"><span data-stu-id="aa735-134">String</span></span>|<span data-ttu-id="aa735-135">Descrição fornecida pelo administrador da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aa735-135">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="aa735-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aa735-136">lastModifiedDateTime</span></span>|<span data-ttu-id="aa735-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa735-137">DateTimeOffset</span></span>|<span data-ttu-id="aa735-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="aa735-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="aa735-139">displayName</span><span class="sxs-lookup"><span data-stu-id="aa735-139">displayName</span></span>|<span data-ttu-id="aa735-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="aa735-140">String</span></span>|<span data-ttu-id="aa735-141">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aa735-141">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="aa735-142">versão</span><span class="sxs-lookup"><span data-stu-id="aa735-142">version</span></span>|<span data-ttu-id="aa735-143">Int32</span><span class="sxs-lookup"><span data-stu-id="aa735-143">Int32</span></span>|<span data-ttu-id="aa735-144">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aa735-144">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa735-145">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="aa735-145">Relationships</span></span>
|<span data-ttu-id="aa735-146">Relação</span><span class="sxs-lookup"><span data-stu-id="aa735-146">Relationship</span></span>|<span data-ttu-id="aa735-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="aa735-147">Type</span></span>|<span data-ttu-id="aa735-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa735-148">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa735-149">assignments</span><span class="sxs-lookup"><span data-stu-id="aa735-149">assignments</span></span>|<span data-ttu-id="aa735-150">Coleção [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="aa735-150">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="aa735-151">A lista de atribuições de grupo para configuração de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="aa735-151">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="aa735-152">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="aa735-152">deviceStatuses</span></span>|<span data-ttu-id="aa735-153">coleção [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="aa735-153">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="aa735-154">Lista de ManagedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="aa735-154">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="aa735-155">userStatuses</span><span class="sxs-lookup"><span data-stu-id="aa735-155">userStatuses</span></span>|<span data-ttu-id="aa735-156">Coleção [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="aa735-156">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="aa735-157">Lista de ManagedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="aa735-157">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="aa735-158">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="aa735-158">deviceStatusSummary</span></span>|[<span data-ttu-id="aa735-159">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="aa735-159">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="aa735-160">Resumo do status do dispositivo de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="aa735-160">App configuration device status summary.</span></span>|
|<span data-ttu-id="aa735-161">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="aa735-161">userStatusSummary</span></span>|[<span data-ttu-id="aa735-162">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="aa735-162">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="aa735-163">Resumo do status do usuário de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="aa735-163">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aa735-164">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="aa735-164">JSON Representation</span></span>
<span data-ttu-id="aa735-165">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="aa735-165">Here is a JSON representation of the resource.</span></span>
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







