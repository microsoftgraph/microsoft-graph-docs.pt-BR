---
title: tipo de recurso importedDeviceIdentity
description: O recurso importedDeviceIdentity representa uma identidade de hardware exclusiva de um dispositivo que foi pré-configurado para configuração de pré-registro.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 197f4d9fd3377e6359d93a75ac36c8c15be3e0f5
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941524"
---
# <a name="importeddeviceidentity-resource-type"></a><span data-ttu-id="d4051-103">tipo de recurso importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="d4051-103">importedDeviceIdentity resource type</span></span>

> <span data-ttu-id="d4051-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d4051-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4051-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d4051-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4051-106">O recurso importedDeviceIdentity representa uma identidade de hardware exclusiva de um dispositivo que foi pré-configurado para configuração de pré-registro.</span><span class="sxs-lookup"><span data-stu-id="d4051-106">The importedDeviceIdentity resource represents a unique hardware identity of a device that has been pre-staged for pre-enrollment configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="d4051-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="d4051-107">Methods</span></span>
|<span data-ttu-id="d4051-108">Método</span><span class="sxs-lookup"><span data-stu-id="d4051-108">Method</span></span>|<span data-ttu-id="d4051-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d4051-109">Return Type</span></span>|<span data-ttu-id="d4051-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4051-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d4051-111">Listar importedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="d4051-111">List importedDeviceIdentities</span></span>](../api/intune-enrollment-importeddeviceidentity-list.md)|<span data-ttu-id="d4051-112">coleção [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="d4051-112">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="d4051-113">Listar Propriedades e relações dos objetos [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="d4051-113">List properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) objects.</span></span>|
|[<span data-ttu-id="d4051-114">Obter importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="d4051-114">Get importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-get.md)|[<span data-ttu-id="d4051-115">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="d4051-115">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="d4051-116">Leia as propriedades e as relações do objeto [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="d4051-116">Read properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="d4051-117">Criar importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="d4051-117">Create importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-create.md)|[<span data-ttu-id="d4051-118">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="d4051-118">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="d4051-119">Criar um novo objeto [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="d4051-119">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="d4051-120">Excluir importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="d4051-120">Delete importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-delete.md)|<span data-ttu-id="d4051-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d4051-121">None</span></span>|<span data-ttu-id="d4051-122">Exclui [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="d4051-122">Deletes a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>|
|[<span data-ttu-id="d4051-123">Atualizar importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="d4051-123">Update importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-update.md)|[<span data-ttu-id="d4051-124">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="d4051-124">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="d4051-125">Atualiza as propriedades de um objeto [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="d4051-125">Update the properties of a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="d4051-126">Ação importDeviceIdentityList</span><span class="sxs-lookup"><span data-stu-id="d4051-126">importDeviceIdentityList action</span></span>](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|<span data-ttu-id="d4051-127">coleção [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)</span><span class="sxs-lookup"><span data-stu-id="d4051-127">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection</span></span>|<span data-ttu-id="d4051-128">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d4051-128">Not yet documented</span></span>|
|[<span data-ttu-id="d4051-129">Ação searchExistingIdentities</span><span class="sxs-lookup"><span data-stu-id="d4051-129">searchExistingIdentities action</span></span>](../api/intune-enrollment-importeddeviceidentity-searchexistingidentities.md)|<span data-ttu-id="d4051-130">coleção [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="d4051-130">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="d4051-131">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d4051-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="d4051-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d4051-132">Properties</span></span>
|<span data-ttu-id="d4051-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d4051-133">Property</span></span>|<span data-ttu-id="d4051-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4051-134">Type</span></span>|<span data-ttu-id="d4051-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4051-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4051-136">id</span><span class="sxs-lookup"><span data-stu-id="d4051-136">id</span></span>|<span data-ttu-id="d4051-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4051-137">String</span></span>|<span data-ttu-id="d4051-138">ID da identidade do dispositivo importado</span><span class="sxs-lookup"><span data-stu-id="d4051-138">Id of the imported device identity</span></span>|
|<span data-ttu-id="d4051-139">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="d4051-139">importedDeviceIdentifier</span></span>|<span data-ttu-id="d4051-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4051-140">String</span></span>|<span data-ttu-id="d4051-141">Identificador de dispositivo importado</span><span class="sxs-lookup"><span data-stu-id="d4051-141">Imported Device Identifier</span></span>|
|<span data-ttu-id="d4051-142">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="d4051-142">importedDeviceIdentityType</span></span>|[<span data-ttu-id="d4051-143">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="d4051-143">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="d4051-144">Tipo de identidade de dispositivo importada.</span><span class="sxs-lookup"><span data-stu-id="d4051-144">Type of Imported Device Identity.</span></span> <span data-ttu-id="d4051-145">Os valores possíveis são: `unknown`, `imei`, `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="d4051-145">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="d4051-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4051-146">lastModifiedDateTime</span></span>|<span data-ttu-id="d4051-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4051-147">DateTimeOffset</span></span>|<span data-ttu-id="d4051-148">Data e hora da última modificação da descrição</span><span class="sxs-lookup"><span data-stu-id="d4051-148">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="d4051-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d4051-149">createdDateTime</span></span>|<span data-ttu-id="d4051-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4051-150">DateTimeOffset</span></span>|<span data-ttu-id="d4051-151">Data e hora de criação do dispositivo</span><span class="sxs-lookup"><span data-stu-id="d4051-151">Created Date Time of the device</span></span>|
|<span data-ttu-id="d4051-152">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4051-152">lastContactedDateTime</span></span>|<span data-ttu-id="d4051-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4051-153">DateTimeOffset</span></span>|<span data-ttu-id="d4051-154">Data e hora do último contato do dispositivo</span><span class="sxs-lookup"><span data-stu-id="d4051-154">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="d4051-155">description</span><span class="sxs-lookup"><span data-stu-id="d4051-155">description</span></span>|<span data-ttu-id="d4051-156">String</span><span class="sxs-lookup"><span data-stu-id="d4051-156">String</span></span>|<span data-ttu-id="d4051-157">A descrição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="d4051-157">The description of the device</span></span>|
|<span data-ttu-id="d4051-158">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="d4051-158">enrollmentState</span></span>|[<span data-ttu-id="d4051-159">enrollmentid</span><span class="sxs-lookup"><span data-stu-id="d4051-159">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="d4051-160">O estado do dispositivo no Intune.</span><span class="sxs-lookup"><span data-stu-id="d4051-160">The state of the device in Intune.</span></span> <span data-ttu-id="d4051-161">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="d4051-161">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="d4051-162">platform</span><span class="sxs-lookup"><span data-stu-id="d4051-162">platform</span></span>|[<span data-ttu-id="d4051-163">plataforma</span><span class="sxs-lookup"><span data-stu-id="d4051-163">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="d4051-164">A plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d4051-164">The platform of the Device.</span></span> <span data-ttu-id="d4051-165">Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="d4051-165">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4051-166">Relações</span><span class="sxs-lookup"><span data-stu-id="d4051-166">Relationships</span></span>
<span data-ttu-id="d4051-167">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d4051-167">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4051-168">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d4051-168">JSON Representation</span></span>
<span data-ttu-id="d4051-169">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d4051-169">Here is a JSON representation of the resource.</span></span>
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




