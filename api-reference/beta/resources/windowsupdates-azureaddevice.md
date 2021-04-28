---
title: Tipo de recurso do azureADDevice
description: Representa um dispositivo no Azure Active Directory (Azure AD) registrado no serviço de implantação.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: a9d7b68257895674530acfbafcd0fb6b6c9c7b02
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067809"
---
# <a name="azureaddevice-resource-type"></a><span data-ttu-id="d47e3-103">Tipo de recurso do azureADDevice</span><span class="sxs-lookup"><span data-stu-id="d47e3-103">azureADDevice resource type</span></span>

<span data-ttu-id="d47e3-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="d47e3-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d47e3-105">Representa um dispositivo no Azure Active Directory (Azure AD) registrado no serviço de implantação.</span><span class="sxs-lookup"><span data-stu-id="d47e3-105">Represents a device in Azure Active Directory (Azure AD) that is registered with the deployment service.</span></span>

<span data-ttu-id="d47e3-106">Um dispositivo do Azure AD é criado automaticamente por meio de um dos seguintes métodos:</span><span class="sxs-lookup"><span data-stu-id="d47e3-106">An Azure AD device is automatically created through one of the following methods:</span></span>
* [<span data-ttu-id="d47e3-107">updatableAsset: enrollAssets</span><span class="sxs-lookup"><span data-stu-id="d47e3-107">updatableAsset: enrollAssets</span></span>](../api/windowsupdates-updatableasset-enrollassets.md)
* [<span data-ttu-id="d47e3-108">updatableAsset: enrollAssetsById</span><span class="sxs-lookup"><span data-stu-id="d47e3-108">updatableAsset: enrollAssetsById</span></span>](../api/windowsupdates-updatableasset-enrollassetsbyid.md)
* [<span data-ttu-id="d47e3-109">deploymentAudience: updateAudience</span><span class="sxs-lookup"><span data-stu-id="d47e3-109">deploymentAudience: updateAudience</span></span>](../api/windowsupdates-deploymentaudience-updateaudience.md)
* [<span data-ttu-id="d47e3-110">deploymentAudience: updateAudienceById</span><span class="sxs-lookup"><span data-stu-id="d47e3-110">deploymentAudience: updateAudienceById</span></span>](../api/windowsupdates-deploymentaudience-updateaudiencebyid.md)
* [<span data-ttu-id="d47e3-111">updatableAssetGroup: addMembers</span><span class="sxs-lookup"><span data-stu-id="d47e3-111">updatableAssetGroup: addMembers</span></span>](../api/windowsupdates-updatableassetgroup-addmembers.md)
* [<span data-ttu-id="d47e3-112">updatableAssetGroup: addMembersById</span><span class="sxs-lookup"><span data-stu-id="d47e3-112">updatableAssetGroup: addMembersById</span></span>](../api/windowsupdates-updatableassetgroup-addmembersbyid.md)

<span data-ttu-id="d47e3-113">Herda de [updatableAsset](../resources/windowsupdates-updatableasset.md).</span><span class="sxs-lookup"><span data-stu-id="d47e3-113">Inherits from [updatableAsset](../resources/windowsupdates-updatableasset.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d47e3-114">Métodos</span><span class="sxs-lookup"><span data-stu-id="d47e3-114">Methods</span></span>
|<span data-ttu-id="d47e3-115">Método</span><span class="sxs-lookup"><span data-stu-id="d47e3-115">Method</span></span>|<span data-ttu-id="d47e3-116">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d47e3-116">Return type</span></span>|<span data-ttu-id="d47e3-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="d47e3-117">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d47e3-118">Listar recursos do azureADDevice</span><span class="sxs-lookup"><span data-stu-id="d47e3-118">List azureADDevice resources</span></span>](../api/windowsupdates-updates-list-updatableassets-azureaddevice.md)|<span data-ttu-id="d47e3-119">[coleção microsoft.graph.windowsUpdates.azureADDevice](../resources/windowsupdates-azureaddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d47e3-119">[microsoft.graph.windowsUpdates.azureADDevice](../resources/windowsupdates-azureaddevice.md) collection</span></span>|<span data-ttu-id="d47e3-120">Obter uma lista dos [objetos azureADDevice](../resources/windowsupdates-azureaddevice.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="d47e3-120">Get a list of the [azureADDevice](../resources/windowsupdates-azureaddevice.md) objects and their properties.</span></span>|
|[<span data-ttu-id="d47e3-121">Obter azureADDevice</span><span class="sxs-lookup"><span data-stu-id="d47e3-121">Get azureADDevice</span></span>](../api/windowsupdates-azureaddevice-get.md)|[<span data-ttu-id="d47e3-122">microsoft.graph.windowsUpdates.azureADDevice</span><span class="sxs-lookup"><span data-stu-id="d47e3-122">microsoft.graph.windowsUpdates.azureADDevice</span></span>](../resources/windowsupdates-azureaddevice.md)|<span data-ttu-id="d47e3-123">Leia as propriedades e as relações de um [objeto azureADDevice.](../resources/windowsupdates-azureaddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d47e3-123">Read the properties and relationships of an [azureADDevice](../resources/windowsupdates-azureaddevice.md) object.</span></span>|
|[<span data-ttu-id="d47e3-124">Excluir azureADDevice</span><span class="sxs-lookup"><span data-stu-id="d47e3-124">Delete azureADDevice</span></span>](../api/windowsupdates-azureaddevice-delete.md)|<span data-ttu-id="d47e3-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d47e3-125">None</span></span>|<span data-ttu-id="d47e3-126">[Exclua um objeto azureADDevice.](../resources/windowsupdates-azureaddevice.md)</span><span class="sxs-lookup"><span data-stu-id="d47e3-126">Delete an [azureADDevice](../resources/windowsupdates-azureaddevice.md) object.</span></span>|
|[<span data-ttu-id="d47e3-127">Registrar recursos do azureADDevice no gerenciamento</span><span class="sxs-lookup"><span data-stu-id="d47e3-127">Enroll azureADDevice resources in management</span></span>](../api/windowsupdates-updatableasset-enrollassets.md)|<span data-ttu-id="d47e3-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d47e3-128">None</span></span>|<span data-ttu-id="d47e3-129">Registrar [recursos do azureADDevice](../resources/windowsupdates-azureaddevice.md) no gerenciamento de atualizações pelo serviço de implantação.</span><span class="sxs-lookup"><span data-stu-id="d47e3-129">Enroll [azureADDevice](../resources/windowsupdates-azureaddevice.md) resources in update management by the deployment service.</span></span>|
|[<span data-ttu-id="d47e3-130">Registrar recursos do azureADDevice no gerenciamento (por ID)</span><span class="sxs-lookup"><span data-stu-id="d47e3-130">Enroll azureADDevice resources in management (by ID)</span></span>](../api/windowsupdates-updatableasset-enrollassetsbyid.md)|<span data-ttu-id="d47e3-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d47e3-131">None</span></span>|<span data-ttu-id="d47e3-132">Registrar [recursos do azureADDevice](../resources/windowsupdates-azureaddevice.md) no gerenciamento de atualizações pelo serviço de implantação.</span><span class="sxs-lookup"><span data-stu-id="d47e3-132">Enroll [azureADDevice](../resources/windowsupdates-azureaddevice.md) resources in update management by the deployment service.</span></span>|
|[<span data-ttu-id="d47e3-133">Desembre recursos do azureADDevice do gerenciamento</span><span class="sxs-lookup"><span data-stu-id="d47e3-133">Unenroll azureADDevice resources from management</span></span>](../api/windowsupdates-updatableasset-unenrollassets.md)|<span data-ttu-id="d47e3-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d47e3-134">None</span></span>|<span data-ttu-id="d47e3-135">Desembre [recursos do azureADDevice](../resources/windowsupdates-azureaddevice.md) do gerenciamento de atualizações pelo serviço de implantação.</span><span class="sxs-lookup"><span data-stu-id="d47e3-135">Unenroll [azureADDevice](../resources/windowsupdates-azureaddevice.md) resources from update management by the deployment service.</span></span>|
|[<span data-ttu-id="d47e3-136">Desembre recursos do azureADDevice do gerenciamento (por ID)</span><span class="sxs-lookup"><span data-stu-id="d47e3-136">Unenroll azureADDevice resources from management (by ID)</span></span>](../api/windowsupdates-updatableasset-unenrollassetsbyid.md)|<span data-ttu-id="d47e3-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d47e3-137">None</span></span>|<span data-ttu-id="d47e3-138">Desembre [recursos do azureADDevice](../resources/windowsupdates-azureaddevice.md) do gerenciamento de atualizações pelo serviço de implantação.</span><span class="sxs-lookup"><span data-stu-id="d47e3-138">Unenroll [azureADDevice](../resources/windowsupdates-azureaddevice.md) resources from update management by the deployment service.</span></span>|

## <a name="properties"></a><span data-ttu-id="d47e3-139">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d47e3-139">Properties</span></span>
|<span data-ttu-id="d47e3-140">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d47e3-140">Property</span></span>|<span data-ttu-id="d47e3-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="d47e3-141">Type</span></span>|<span data-ttu-id="d47e3-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="d47e3-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d47e3-143">enrollments</span><span class="sxs-lookup"><span data-stu-id="d47e3-143">enrollments</span></span>|<span data-ttu-id="d47e3-144">[coleção microsoft.graph.windowsUpdates.updatableAssetEnrollment](../resources/windowsupdates-updatableassetenrollment.md)</span><span class="sxs-lookup"><span data-stu-id="d47e3-144">[microsoft.graph.windowsUpdates.updatableAssetEnrollment](../resources/windowsupdates-updatableassetenrollment.md) collection</span></span>|<span data-ttu-id="d47e3-145">Especifica áreas do serviço em que o dispositivo está inscrito.</span><span class="sxs-lookup"><span data-stu-id="d47e3-145">Specifies areas of the service in which the device is enrolled.</span></span> <span data-ttu-id="d47e3-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d47e3-146">Read-only.</span></span> <span data-ttu-id="d47e3-147">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="d47e3-147">Returned by default.</span></span>|
|<span data-ttu-id="d47e3-148">erros</span><span class="sxs-lookup"><span data-stu-id="d47e3-148">errors</span></span>|<span data-ttu-id="d47e3-149">[coleção microsoft.graph.windowsUpdates.updatableAssetError](../resources/windowsupdates-updatableasseterror.md)</span><span class="sxs-lookup"><span data-stu-id="d47e3-149">[microsoft.graph.windowsUpdates.updatableAssetError](../resources/windowsupdates-updatableasseterror.md) collection</span></span>|<span data-ttu-id="d47e3-150">Especifica quaisquer erros que impeçam que o dispositivo seja inscrito no gerenciamento de atualizações ou receving conteúdo implantado.</span><span class="sxs-lookup"><span data-stu-id="d47e3-150">Specifies any errors that prevent the device from being enrolled in update management or receving deployed content.</span></span> <span data-ttu-id="d47e3-151">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d47e3-151">Read-only.</span></span> <span data-ttu-id="d47e3-152">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="d47e3-152">Returned by default.</span></span>|
|<span data-ttu-id="d47e3-153">id</span><span class="sxs-lookup"><span data-stu-id="d47e3-153">id</span></span>|<span data-ttu-id="d47e3-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d47e3-154">String</span></span>|<span data-ttu-id="d47e3-155">Um identificador do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d47e3-155">An identifier for the device.</span></span> <span data-ttu-id="d47e3-156">Chave.</span><span class="sxs-lookup"><span data-stu-id="d47e3-156">Key.</span></span> <span data-ttu-id="d47e3-157">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="d47e3-157">Not nullable.</span></span> <span data-ttu-id="d47e3-158">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d47e3-158">Read-only.</span></span> <span data-ttu-id="d47e3-159">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="d47e3-159">Returned by default.</span></span> <span data-ttu-id="d47e3-160">Herdado [de updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="d47e3-160">Inherited from [updatableAsset](../resources/windowsupdates-updatableasset.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="d47e3-161">Relações</span><span class="sxs-lookup"><span data-stu-id="d47e3-161">Relationships</span></span>
<span data-ttu-id="d47e3-162">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d47e3-162">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d47e3-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d47e3-163">JSON representation</span></span>
<span data-ttu-id="d47e3-164">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d47e3-164">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdates.azureADDevice",
  "baseType": "microsoft.graph.windowsUpdates.updatableAsset",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
  "id": "String (identifier)",
  "errors": [
    {
      "@odata.type": "microsoft.graph.windowsUpdates.azureADDeviceRegistrationError"
    }
  ],
  "enrollments": [
    {
      "@odata.type": "microsoft.graph.windowsUpdates.updateManagementEnrollment"
    }
  ]
}
```

