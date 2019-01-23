---
title: tipo de recurso de importedDeviceIdentity
description: O recurso de importedDeviceIdentity representa uma identidade exclusiva de hardware de um dispositivo que tenha sido esses transferidos para configuração de inscrição prévia.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c151257a95d1161e07de17ed6d9fc01fc021146e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421442"
---
# <a name="importeddeviceidentity-resource-type"></a><span data-ttu-id="5f825-103">tipo de recurso de importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="5f825-103">importedDeviceIdentity resource type</span></span>

> <span data-ttu-id="5f825-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="5f825-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5f825-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5f825-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5f825-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="5f825-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f825-107">O recurso de importedDeviceIdentity representa uma identidade exclusiva de hardware de um dispositivo que tenha sido esses transferidos para configuração de inscrição prévia.</span><span class="sxs-lookup"><span data-stu-id="5f825-107">The importedDeviceIdentity resource represents a unique hardware identity of a device that has been pre-staged for pre-enrollment configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="5f825-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="5f825-108">Methods</span></span>
|<span data-ttu-id="5f825-109">Método</span><span class="sxs-lookup"><span data-stu-id="5f825-109">Method</span></span>|<span data-ttu-id="5f825-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5f825-110">Return Type</span></span>|<span data-ttu-id="5f825-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f825-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5f825-112">Lista importedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="5f825-112">List importedDeviceIdentities</span></span>](../api/intune-enrollment-importeddeviceidentity-list.md)|<span data-ttu-id="5f825-113">coleção [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="5f825-113">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="5f825-114">Lista as propriedades e os relacionamentos dos objetos [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="5f825-114">List properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) objects.</span></span>|
|[<span data-ttu-id="5f825-115">Obter importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="5f825-115">Get importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-get.md)|[<span data-ttu-id="5f825-116">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="5f825-116">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="5f825-117">Leia as propriedades e os relacionamentos do objeto [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="5f825-117">Read properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="5f825-118">Criar importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="5f825-118">Create importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-create.md)|[<span data-ttu-id="5f825-119">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="5f825-119">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="5f825-120">Crie um novo objeto de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="5f825-120">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="5f825-121">Excluir importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="5f825-121">Delete importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-delete.md)|<span data-ttu-id="5f825-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5f825-122">None</span></span>|<span data-ttu-id="5f825-123">Exclui um [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="5f825-123">Deletes a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>|
|[<span data-ttu-id="5f825-124">Atualizar importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="5f825-124">Update importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-update.md)|[<span data-ttu-id="5f825-125">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="5f825-125">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="5f825-126">Atualize as propriedades de um objeto [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="5f825-126">Update the properties of a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="5f825-127">ação de importDeviceIdentityList</span><span class="sxs-lookup"><span data-stu-id="5f825-127">importDeviceIdentityList action</span></span>](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|<span data-ttu-id="5f825-128">coleção [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)</span><span class="sxs-lookup"><span data-stu-id="5f825-128">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection</span></span>|<span data-ttu-id="5f825-129">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5f825-129">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="5f825-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5f825-130">Properties</span></span>
|<span data-ttu-id="5f825-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5f825-131">Property</span></span>|<span data-ttu-id="5f825-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f825-132">Type</span></span>|<span data-ttu-id="5f825-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f825-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f825-134">id</span><span class="sxs-lookup"><span data-stu-id="5f825-134">id</span></span>|<span data-ttu-id="5f825-135">String</span><span class="sxs-lookup"><span data-stu-id="5f825-135">String</span></span>|<span data-ttu-id="5f825-136">ID da identidade do dispositivo importada</span><span class="sxs-lookup"><span data-stu-id="5f825-136">Id of the imported device identity</span></span>|
|<span data-ttu-id="5f825-137">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="5f825-137">importedDeviceIdentifier</span></span>|<span data-ttu-id="5f825-138">String</span><span class="sxs-lookup"><span data-stu-id="5f825-138">String</span></span>|<span data-ttu-id="5f825-139">Identificador de dispositivo importada</span><span class="sxs-lookup"><span data-stu-id="5f825-139">Imported Device Identifier</span></span>|
|<span data-ttu-id="5f825-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="5f825-140">importedDeviceIdentityType</span></span>|[<span data-ttu-id="5f825-141">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="5f825-141">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="5f825-142">Tipo de identidade do dispositivo importada.</span><span class="sxs-lookup"><span data-stu-id="5f825-142">Type of Imported Device Identity.</span></span> <span data-ttu-id="5f825-143">Os valores possíveis são: `unknown`, `imei`, `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="5f825-143">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="5f825-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5f825-144">lastModifiedDateTime</span></span>|<span data-ttu-id="5f825-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f825-145">DateTimeOffset</span></span>|<span data-ttu-id="5f825-146">Última data e hora modificadas da descrição</span><span class="sxs-lookup"><span data-stu-id="5f825-146">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="5f825-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5f825-147">createdDateTime</span></span>|<span data-ttu-id="5f825-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f825-148">DateTimeOffset</span></span>|<span data-ttu-id="5f825-149">Criada data hora do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5f825-149">Created Date Time of the device</span></span>|
|<span data-ttu-id="5f825-150">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="5f825-150">lastContactedDateTime</span></span>|<span data-ttu-id="5f825-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f825-151">DateTimeOffset</span></span>|<span data-ttu-id="5f825-152">Última contatado data hora do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5f825-152">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="5f825-153">description</span><span class="sxs-lookup"><span data-stu-id="5f825-153">description</span></span>|<span data-ttu-id="5f825-154">String</span><span class="sxs-lookup"><span data-stu-id="5f825-154">String</span></span>|<span data-ttu-id="5f825-155">A descrição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5f825-155">The description of the device</span></span>|
|<span data-ttu-id="5f825-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="5f825-156">enrollmentState</span></span>|[<span data-ttu-id="5f825-157">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="5f825-157">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="5f825-158">O estado do dispositivo em Intune.</span><span class="sxs-lookup"><span data-stu-id="5f825-158">The state of the device in Intune.</span></span> <span data-ttu-id="5f825-159">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="5f825-159">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="5f825-160">platform</span><span class="sxs-lookup"><span data-stu-id="5f825-160">platform</span></span>|[<span data-ttu-id="5f825-161">plataforma</span><span class="sxs-lookup"><span data-stu-id="5f825-161">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="5f825-162">A plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5f825-162">The platform of the Device.</span></span> <span data-ttu-id="5f825-163">Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="5f825-163">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f825-164">Relações</span><span class="sxs-lookup"><span data-stu-id="5f825-164">Relationships</span></span>
<span data-ttu-id="5f825-165">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5f825-165">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5f825-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5f825-166">JSON Representation</span></span>
<span data-ttu-id="5f825-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5f825-167">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedDeviceIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedDeviceIdentity",
  "id": "String (identifier)",
  "importedDeviceIdentifier": "String",
  "importedDeviceIdentityType": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "lastContactedDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "platform": "String"
}
```




