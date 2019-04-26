---
title: Tipo de recurso managedDeviceMobileAppConfiguration
description: Uma classe abstrata para a configuração do Aplicativo móvel para dispositivos registrados.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a1a249325f7e4c9be196c5adda695b84e5f8a94c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571951"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="d3459-103">Tipo de recurso managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="d3459-103">managedDeviceMobileAppConfiguration resource type</span></span>

> <span data-ttu-id="d3459-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d3459-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3459-105">Uma classe abstrata para a configuração do Aplicativo móvel para dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="d3459-105">An abstract class for Mobile app configuration for enrolled devices.</span></span>

## <a name="methods"></a><span data-ttu-id="d3459-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="d3459-106">Methods</span></span>
|<span data-ttu-id="d3459-107">Método</span><span class="sxs-lookup"><span data-stu-id="d3459-107">Method</span></span>|<span data-ttu-id="d3459-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d3459-108">Return Type</span></span>|<span data-ttu-id="d3459-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3459-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d3459-110">Listar managedDeviceMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="d3459-110">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="d3459-111">Coleção [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d3459-111">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="d3459-112">Lista propriedades e relações dos objetos [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d3459-112">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="d3459-113">Obter managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="d3459-113">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="d3459-114">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="d3459-114">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="d3459-115">Propriedades de leitura e relações do objeto [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d3459-115">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="d3459-116">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="d3459-116">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="d3459-117">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="d3459-117">None</span></span>|<span data-ttu-id="d3459-118">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d3459-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="d3459-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d3459-119">Properties</span></span>
|<span data-ttu-id="d3459-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3459-120">Property</span></span>|<span data-ttu-id="d3459-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3459-121">Type</span></span>|<span data-ttu-id="d3459-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3459-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3459-123">id</span><span class="sxs-lookup"><span data-stu-id="d3459-123">id</span></span>|<span data-ttu-id="d3459-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3459-124">String</span></span>|<span data-ttu-id="d3459-125">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d3459-125">Key of the entity.</span></span>|
|<span data-ttu-id="d3459-126">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="d3459-126">targetedMobileApps</span></span>|<span data-ttu-id="d3459-127">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3459-127">String collection</span></span>|<span data-ttu-id="d3459-128">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="d3459-128">the associated app.</span></span>|
|<span data-ttu-id="d3459-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d3459-129">createdDateTime</span></span>|<span data-ttu-id="d3459-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3459-130">DateTimeOffset</span></span>|<span data-ttu-id="d3459-131">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d3459-131">DateTime the object was created.</span></span>|
|<span data-ttu-id="d3459-132">description</span><span class="sxs-lookup"><span data-stu-id="d3459-132">description</span></span>|<span data-ttu-id="d3459-133">String</span><span class="sxs-lookup"><span data-stu-id="d3459-133">String</span></span>|<span data-ttu-id="d3459-134">Descrição fornecida pelo administrador da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d3459-134">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="d3459-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d3459-135">lastModifiedDateTime</span></span>|<span data-ttu-id="d3459-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d3459-136">DateTimeOffset</span></span>|<span data-ttu-id="d3459-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d3459-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="d3459-138">displayName</span><span class="sxs-lookup"><span data-stu-id="d3459-138">displayName</span></span>|<span data-ttu-id="d3459-139">String</span><span class="sxs-lookup"><span data-stu-id="d3459-139">String</span></span>|<span data-ttu-id="d3459-140">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d3459-140">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="d3459-141">versão</span><span class="sxs-lookup"><span data-stu-id="d3459-141">version</span></span>|<span data-ttu-id="d3459-142">Int32</span><span class="sxs-lookup"><span data-stu-id="d3459-142">Int32</span></span>|<span data-ttu-id="d3459-143">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d3459-143">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3459-144">Relações</span><span class="sxs-lookup"><span data-stu-id="d3459-144">Relationships</span></span>
|<span data-ttu-id="d3459-145">Relação</span><span class="sxs-lookup"><span data-stu-id="d3459-145">Relationship</span></span>|<span data-ttu-id="d3459-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3459-146">Type</span></span>|<span data-ttu-id="d3459-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3459-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3459-148">assignments</span><span class="sxs-lookup"><span data-stu-id="d3459-148">assignments</span></span>|<span data-ttu-id="d3459-149">Coleção [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d3459-149">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="d3459-150">A lista de atribuições de grupo para configuração de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="d3459-150">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="d3459-151">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="d3459-151">deviceStatuses</span></span>|<span data-ttu-id="d3459-152">coleção [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="d3459-152">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="d3459-153">Lista de ManagedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="d3459-153">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="d3459-154">userStatuses</span><span class="sxs-lookup"><span data-stu-id="d3459-154">userStatuses</span></span>|<span data-ttu-id="d3459-155">Coleção [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="d3459-155">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="d3459-156">Lista de ManagedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="d3459-156">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="d3459-157">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="d3459-157">deviceStatusSummary</span></span>|[<span data-ttu-id="d3459-158">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="d3459-158">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="d3459-159">Resumo do status do dispositivo de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d3459-159">App configuration device status summary.</span></span>|
|<span data-ttu-id="d3459-160">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="d3459-160">userStatusSummary</span></span>|[<span data-ttu-id="d3459-161">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="d3459-161">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="d3459-162">Resumo do status do usuário de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d3459-162">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d3459-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d3459-163">JSON Representation</span></span>
<span data-ttu-id="d3459-164">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d3459-164">Here is a JSON representation of the resource.</span></span>
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



