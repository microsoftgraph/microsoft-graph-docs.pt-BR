---
title: Tipo de recurso managedDeviceMobileAppConfiguration
description: Uma classe abstrata para a configuração do Aplicativo móvel para dispositivos registrados.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 462533c75ebbad87409032c1769edc3d399fda4d
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756040"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="36714-103">Tipo de recurso managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="36714-103">managedDeviceMobileAppConfiguration resource type</span></span>

<span data-ttu-id="36714-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36714-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="36714-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="36714-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36714-106">Uma classe abstrata para a configuração do Aplicativo móvel para dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="36714-106">An abstract class for Mobile app configuration for enrolled devices.</span></span>

## <a name="methods"></a><span data-ttu-id="36714-107">Methods</span><span class="sxs-lookup"><span data-stu-id="36714-107">Methods</span></span>
|<span data-ttu-id="36714-108">Método</span><span class="sxs-lookup"><span data-stu-id="36714-108">Method</span></span>|<span data-ttu-id="36714-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="36714-109">Return Type</span></span>|<span data-ttu-id="36714-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="36714-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="36714-111">Listar managedDeviceMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="36714-111">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="36714-112">Coleção [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="36714-112">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="36714-113">Lista propriedades e relações dos objetos [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36714-113">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="36714-114">Obter managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="36714-114">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="36714-115">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="36714-115">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="36714-116">Propriedades de leitura e relações do objeto [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36714-116">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="36714-117">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="36714-117">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="36714-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="36714-118">None</span></span>|<span data-ttu-id="36714-119">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="36714-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="36714-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="36714-120">Properties</span></span>
|<span data-ttu-id="36714-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="36714-121">Property</span></span>|<span data-ttu-id="36714-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="36714-122">Type</span></span>|<span data-ttu-id="36714-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="36714-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36714-124">id</span><span class="sxs-lookup"><span data-stu-id="36714-124">id</span></span>|<span data-ttu-id="36714-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="36714-125">String</span></span>|<span data-ttu-id="36714-126">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="36714-126">Key of the entity.</span></span>|
|<span data-ttu-id="36714-127">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="36714-127">targetedMobileApps</span></span>|<span data-ttu-id="36714-128">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="36714-128">String collection</span></span>|<span data-ttu-id="36714-129">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="36714-129">the associated app.</span></span>|
|<span data-ttu-id="36714-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="36714-130">createdDateTime</span></span>|<span data-ttu-id="36714-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36714-131">DateTimeOffset</span></span>|<span data-ttu-id="36714-132">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="36714-132">DateTime the object was created.</span></span>|
|<span data-ttu-id="36714-133">descrição</span><span class="sxs-lookup"><span data-stu-id="36714-133">description</span></span>|<span data-ttu-id="36714-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="36714-134">String</span></span>|<span data-ttu-id="36714-135">Descrição fornecida pelo administrador da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="36714-135">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="36714-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="36714-136">lastModifiedDateTime</span></span>|<span data-ttu-id="36714-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36714-137">DateTimeOffset</span></span>|<span data-ttu-id="36714-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="36714-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="36714-139">displayName</span><span class="sxs-lookup"><span data-stu-id="36714-139">displayName</span></span>|<span data-ttu-id="36714-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="36714-140">String</span></span>|<span data-ttu-id="36714-141">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="36714-141">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="36714-142">versão</span><span class="sxs-lookup"><span data-stu-id="36714-142">version</span></span>|<span data-ttu-id="36714-143">Int32</span><span class="sxs-lookup"><span data-stu-id="36714-143">Int32</span></span>|<span data-ttu-id="36714-144">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="36714-144">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="36714-145">Relações</span><span class="sxs-lookup"><span data-stu-id="36714-145">Relationships</span></span>
|<span data-ttu-id="36714-146">Relação</span><span class="sxs-lookup"><span data-stu-id="36714-146">Relationship</span></span>|<span data-ttu-id="36714-147">Tipo</span><span class="sxs-lookup"><span data-stu-id="36714-147">Type</span></span>|<span data-ttu-id="36714-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="36714-148">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36714-149">assignments</span><span class="sxs-lookup"><span data-stu-id="36714-149">assignments</span></span>|<span data-ttu-id="36714-150">Coleção [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="36714-150">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="36714-151">A lista de atribuições de grupo para configuração de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="36714-151">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="36714-152">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="36714-152">deviceStatuses</span></span>|<span data-ttu-id="36714-153">[coleção managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="36714-153">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="36714-154">Lista de ManagedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="36714-154">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="36714-155">userStatuses</span><span class="sxs-lookup"><span data-stu-id="36714-155">userStatuses</span></span>|<span data-ttu-id="36714-156">Coleção [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="36714-156">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="36714-157">Lista de ManagedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="36714-157">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="36714-158">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="36714-158">deviceStatusSummary</span></span>|[<span data-ttu-id="36714-159">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="36714-159">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="36714-160">Resumo do status do dispositivo de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="36714-160">App configuration device status summary.</span></span>|
|<span data-ttu-id="36714-161">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="36714-161">userStatusSummary</span></span>|[<span data-ttu-id="36714-162">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="36714-162">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="36714-163">Resumo do status do usuário de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="36714-163">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="36714-164">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="36714-164">JSON Representation</span></span>
<span data-ttu-id="36714-165">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="36714-165">Here is a JSON representation of the resource.</span></span>
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




