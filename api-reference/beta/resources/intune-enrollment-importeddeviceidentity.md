---
title: tipo de recurso de importedDeviceIdentity
description: O recurso de importedDeviceIdentity representa uma identidade exclusiva de hardware de um dispositivo que tenha sido esses transferidos para configuração de inscrição prévia.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6fe03159f79bb1198db80cbba130601614df8865
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966563"
---
# <a name="importeddeviceidentity-resource-type"></a><span data-ttu-id="fb28c-103">tipo de recurso de importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="fb28c-103">importedDeviceIdentity resource type</span></span>

> <span data-ttu-id="fb28c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fb28c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fb28c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fb28c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fb28c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fb28c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fb28c-107">O recurso de importedDeviceIdentity representa uma identidade exclusiva de hardware de um dispositivo que tenha sido esses transferidos para configuração de inscrição prévia.</span><span class="sxs-lookup"><span data-stu-id="fb28c-107">The importedDeviceIdentity resource represents a unique hardware identity of a device that has been pre-staged for pre-enrollment configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="fb28c-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="fb28c-108">Methods</span></span>
|<span data-ttu-id="fb28c-109">Método</span><span class="sxs-lookup"><span data-stu-id="fb28c-109">Method</span></span>|<span data-ttu-id="fb28c-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="fb28c-110">Return Type</span></span>|<span data-ttu-id="fb28c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb28c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fb28c-112">Lista importedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="fb28c-112">List importedDeviceIdentities</span></span>](../api/intune-enrollment-importeddeviceidentity-list.md)|<span data-ttu-id="fb28c-113">coleção [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="fb28c-113">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="fb28c-114">Lista as propriedades e os relacionamentos dos objetos [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="fb28c-114">List properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) objects.</span></span>|
|[<span data-ttu-id="fb28c-115">Obter importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="fb28c-115">Get importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-get.md)|[<span data-ttu-id="fb28c-116">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="fb28c-116">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="fb28c-117">Leia as propriedades e os relacionamentos do objeto [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="fb28c-117">Read properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="fb28c-118">Criar importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="fb28c-118">Create importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-create.md)|[<span data-ttu-id="fb28c-119">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="fb28c-119">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="fb28c-120">Crie um novo objeto de [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="fb28c-120">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="fb28c-121">Excluir importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="fb28c-121">Delete importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-delete.md)|<span data-ttu-id="fb28c-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fb28c-122">None</span></span>|<span data-ttu-id="fb28c-123">Exclui um [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="fb28c-123">Deletes a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>|
|[<span data-ttu-id="fb28c-124">Atualizar importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="fb28c-124">Update importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-update.md)|[<span data-ttu-id="fb28c-125">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="fb28c-125">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="fb28c-126">Atualize as propriedades de um objeto [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) .</span><span class="sxs-lookup"><span data-stu-id="fb28c-126">Update the properties of a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="fb28c-127">ação de importDeviceIdentityList</span><span class="sxs-lookup"><span data-stu-id="fb28c-127">importDeviceIdentityList action</span></span>](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|<span data-ttu-id="fb28c-128">coleção [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)</span><span class="sxs-lookup"><span data-stu-id="fb28c-128">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection</span></span>|<span data-ttu-id="fb28c-129">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fb28c-129">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="fb28c-130">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fb28c-130">Properties</span></span>
|<span data-ttu-id="fb28c-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fb28c-131">Property</span></span>|<span data-ttu-id="fb28c-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb28c-132">Type</span></span>|<span data-ttu-id="fb28c-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb28c-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb28c-134">id</span><span class="sxs-lookup"><span data-stu-id="fb28c-134">id</span></span>|<span data-ttu-id="fb28c-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb28c-135">String</span></span>|<span data-ttu-id="fb28c-136">ID da identidade do dispositivo importada</span><span class="sxs-lookup"><span data-stu-id="fb28c-136">Id of the imported device identity</span></span>|
|<span data-ttu-id="fb28c-137">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="fb28c-137">importedDeviceIdentifier</span></span>|<span data-ttu-id="fb28c-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb28c-138">String</span></span>|<span data-ttu-id="fb28c-139">Identificador de dispositivo importada</span><span class="sxs-lookup"><span data-stu-id="fb28c-139">Imported Device Identifier</span></span>|
|<span data-ttu-id="fb28c-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="fb28c-140">importedDeviceIdentityType</span></span>|[<span data-ttu-id="fb28c-141">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="fb28c-141">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="fb28c-142">Tipo de identidade do dispositivo importada.</span><span class="sxs-lookup"><span data-stu-id="fb28c-142">Type of Imported Device Identity.</span></span> <span data-ttu-id="fb28c-143">Os valores possíveis são: `unknown`, `imei`, `serialNumber`.</span><span class="sxs-lookup"><span data-stu-id="fb28c-143">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="fb28c-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb28c-144">lastModifiedDateTime</span></span>|<span data-ttu-id="fb28c-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb28c-145">DateTimeOffset</span></span>|<span data-ttu-id="fb28c-146">Última data e hora modificadas da descrição</span><span class="sxs-lookup"><span data-stu-id="fb28c-146">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="fb28c-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fb28c-147">createdDateTime</span></span>|<span data-ttu-id="fb28c-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb28c-148">DateTimeOffset</span></span>|<span data-ttu-id="fb28c-149">Criada data hora do dispositivo</span><span class="sxs-lookup"><span data-stu-id="fb28c-149">Created Date Time of the device</span></span>|
|<span data-ttu-id="fb28c-150">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="fb28c-150">lastContactedDateTime</span></span>|<span data-ttu-id="fb28c-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb28c-151">DateTimeOffset</span></span>|<span data-ttu-id="fb28c-152">Última contatado data hora do dispositivo</span><span class="sxs-lookup"><span data-stu-id="fb28c-152">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="fb28c-153">description</span><span class="sxs-lookup"><span data-stu-id="fb28c-153">description</span></span>|<span data-ttu-id="fb28c-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb28c-154">String</span></span>|<span data-ttu-id="fb28c-155">A descrição do dispositivo</span><span class="sxs-lookup"><span data-stu-id="fb28c-155">The description of the device</span></span>|
|<span data-ttu-id="fb28c-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="fb28c-156">enrollmentState</span></span>|[<span data-ttu-id="fb28c-157">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="fb28c-157">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="fb28c-158">O estado do dispositivo em Intune.</span><span class="sxs-lookup"><span data-stu-id="fb28c-158">The state of the device in Intune.</span></span> <span data-ttu-id="fb28c-159">Os possíveis valores são: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span><span class="sxs-lookup"><span data-stu-id="fb28c-159">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="fb28c-160">platform</span><span class="sxs-lookup"><span data-stu-id="fb28c-160">platform</span></span>|[<span data-ttu-id="fb28c-161">plataforma</span><span class="sxs-lookup"><span data-stu-id="fb28c-161">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="fb28c-162">A plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fb28c-162">The platform of the Device.</span></span> <span data-ttu-id="fb28c-163">Os possíveis valores são: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span><span class="sxs-lookup"><span data-stu-id="fb28c-163">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fb28c-164">Relações</span><span class="sxs-lookup"><span data-stu-id="fb28c-164">Relationships</span></span>
<span data-ttu-id="fb28c-165">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fb28c-165">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fb28c-166">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fb28c-166">JSON Representation</span></span>
<span data-ttu-id="fb28c-167">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fb28c-167">Here is a JSON representation of the resource.</span></span>
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





