---
title: Tipo de recurso managedDeviceMobileAppConfiguration
description: Uma classe abstrata para a configuração do Aplicativo móvel para dispositivos registrados.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 90ac67285ba856916194d30831f556ce6b521dbd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400141"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="0232d-103">Tipo de recurso managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="0232d-103">managedDeviceMobileAppConfiguration resource type</span></span>

> <span data-ttu-id="0232d-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="0232d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0232d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0232d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0232d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="0232d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0232d-107">Uma classe abstrata para a configuração do Aplicativo móvel para dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="0232d-107">An abstract class for Mobile app configuration for enrolled devices.</span></span>

## <a name="methods"></a><span data-ttu-id="0232d-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="0232d-108">Methods</span></span>
|<span data-ttu-id="0232d-109">Método</span><span class="sxs-lookup"><span data-stu-id="0232d-109">Method</span></span>|<span data-ttu-id="0232d-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0232d-110">Return Type</span></span>|<span data-ttu-id="0232d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0232d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0232d-112">Listar managedDeviceMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="0232d-112">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="0232d-113">Coleção [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0232d-113">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="0232d-114">Lista propriedades e relações dos objetos [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0232d-114">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="0232d-115">Obter managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="0232d-115">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="0232d-116">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="0232d-116">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="0232d-117">Propriedades de leitura e relações do objeto [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="0232d-117">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="0232d-118">Ação assign</span><span class="sxs-lookup"><span data-stu-id="0232d-118">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="0232d-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0232d-119">None</span></span>|<span data-ttu-id="0232d-120">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0232d-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="0232d-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0232d-121">Properties</span></span>
|<span data-ttu-id="0232d-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0232d-122">Property</span></span>|<span data-ttu-id="0232d-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="0232d-123">Type</span></span>|<span data-ttu-id="0232d-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="0232d-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0232d-125">id</span><span class="sxs-lookup"><span data-stu-id="0232d-125">id</span></span>|<span data-ttu-id="0232d-126">String</span><span class="sxs-lookup"><span data-stu-id="0232d-126">String</span></span>|<span data-ttu-id="0232d-127">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0232d-127">Key of the entity.</span></span>|
|<span data-ttu-id="0232d-128">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="0232d-128">targetedMobileApps</span></span>|<span data-ttu-id="0232d-129">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0232d-129">String collection</span></span>|<span data-ttu-id="0232d-130">o aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="0232d-130">the associated app.</span></span>|
|<span data-ttu-id="0232d-131">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0232d-131">roleScopeTagIds</span></span>|<span data-ttu-id="0232d-132">String collection</span><span class="sxs-lookup"><span data-stu-id="0232d-132">String collection</span></span>|<span data-ttu-id="0232d-133">Lista de escopo marcas para essa entidade de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0232d-133">List of Scope Tags for this App configuration entity.</span></span>|
|<span data-ttu-id="0232d-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0232d-134">createdDateTime</span></span>|<span data-ttu-id="0232d-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0232d-135">DateTimeOffset</span></span>|<span data-ttu-id="0232d-136">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="0232d-136">DateTime the object was created.</span></span>|
|<span data-ttu-id="0232d-137">description</span><span class="sxs-lookup"><span data-stu-id="0232d-137">description</span></span>|<span data-ttu-id="0232d-138">String</span><span class="sxs-lookup"><span data-stu-id="0232d-138">String</span></span>|<span data-ttu-id="0232d-139">Descrição fornecida pelo administrador da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0232d-139">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="0232d-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0232d-140">lastModifiedDateTime</span></span>|<span data-ttu-id="0232d-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0232d-141">DateTimeOffset</span></span>|<span data-ttu-id="0232d-142">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="0232d-142">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="0232d-143">displayName</span><span class="sxs-lookup"><span data-stu-id="0232d-143">displayName</span></span>|<span data-ttu-id="0232d-144">String</span><span class="sxs-lookup"><span data-stu-id="0232d-144">String</span></span>|<span data-ttu-id="0232d-145">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0232d-145">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="0232d-146">version</span><span class="sxs-lookup"><span data-stu-id="0232d-146">version</span></span>|<span data-ttu-id="0232d-147">Int32</span><span class="sxs-lookup"><span data-stu-id="0232d-147">Int32</span></span>|<span data-ttu-id="0232d-148">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0232d-148">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0232d-149">Relações</span><span class="sxs-lookup"><span data-stu-id="0232d-149">Relationships</span></span>
|<span data-ttu-id="0232d-150">Relação</span><span class="sxs-lookup"><span data-stu-id="0232d-150">Relationship</span></span>|<span data-ttu-id="0232d-151">Tipo</span><span class="sxs-lookup"><span data-stu-id="0232d-151">Type</span></span>|<span data-ttu-id="0232d-152">Descrição</span><span class="sxs-lookup"><span data-stu-id="0232d-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0232d-153">assignments</span><span class="sxs-lookup"><span data-stu-id="0232d-153">assignments</span></span>|<span data-ttu-id="0232d-154">Coleção [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="0232d-154">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="0232d-155">A lista de atribuições de grupo para configuração de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="0232d-155">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="0232d-156">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="0232d-156">deviceStatuses</span></span>|<span data-ttu-id="0232d-157">coleção [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="0232d-157">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="0232d-158">Lista de ManagedDeviceMobileAppConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="0232d-158">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="0232d-159">userStatuses</span><span class="sxs-lookup"><span data-stu-id="0232d-159">userStatuses</span></span>|<span data-ttu-id="0232d-160">Coleção [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md)</span><span class="sxs-lookup"><span data-stu-id="0232d-160">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="0232d-161">Lista de ManagedDeviceMobileAppConfigurationUserStatus.</span><span class="sxs-lookup"><span data-stu-id="0232d-161">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="0232d-162">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="0232d-162">deviceStatusSummary</span></span>|[<span data-ttu-id="0232d-163">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="0232d-163">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="0232d-164">Resumo do status do dispositivo de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0232d-164">App configuration device status summary.</span></span>|
|<span data-ttu-id="0232d-165">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="0232d-165">userStatusSummary</span></span>|[<span data-ttu-id="0232d-166">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="0232d-166">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="0232d-167">Resumo do status do usuário de configuração do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0232d-167">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0232d-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0232d-168">JSON Representation</span></span>
<span data-ttu-id="0232d-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0232d-169">Here is a JSON representation of the resource.</span></span>
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




