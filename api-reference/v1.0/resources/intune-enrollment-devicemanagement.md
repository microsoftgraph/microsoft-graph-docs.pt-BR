---
title: Tipo de recurso deviceManagement
description: O recurso deviceManagement representa as identidades de dispositivos da coleção do locatário pré-configuradas no Intune e os perfis de registro que podem ser atribuídos às identidades de dispositivos com suporte para configuração de pré-registro.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 38c93be6c71f97e828901f51c7d6851a346f0bd1
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755169"
---
# <a name="devicemanagement-resource-type"></a><span data-ttu-id="44748-103">Tipo de recurso deviceManagement</span><span class="sxs-lookup"><span data-stu-id="44748-103">deviceManagement resource type</span></span>

<span data-ttu-id="44748-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44748-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="44748-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="44748-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44748-106">O recurso deviceManagement representa as identidades de dispositivos da coleção do locatário pré-configuradas no Intune e os perfis de registro que podem ser atribuídos às identidades de dispositivos com suporte para configuração de pré-registro.</span><span class="sxs-lookup"><span data-stu-id="44748-106">The deviceManagement resource represents a tenant's collection device identities that have been pre-staged in Intune, and the enrollment profiles that may be assigned to device identities that support pre-enrollment configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="44748-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="44748-107">Methods</span></span>
|<span data-ttu-id="44748-108">Método</span><span class="sxs-lookup"><span data-stu-id="44748-108">Method</span></span>|<span data-ttu-id="44748-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="44748-109">Return Type</span></span>|<span data-ttu-id="44748-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="44748-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="44748-111">Obter deviceManagement</span><span class="sxs-lookup"><span data-stu-id="44748-111">Get deviceManagement</span></span>](../api/intune-enrollment-devicemanagement-get.md)|[<span data-ttu-id="44748-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="44748-112">deviceManagement</span></span>](../resources/intune-enrollment-devicemanagement.md)|<span data-ttu-id="44748-113">Leia as propriedades e as relações do objeto [deviceManagement](../resources/intune-enrollment-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="44748-113">Read properties and relationships of the [deviceManagement](../resources/intune-enrollment-devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="44748-114">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="44748-114">Update deviceManagement</span></span>](../api/intune-enrollment-devicemanagement-update.md)|[<span data-ttu-id="44748-115">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="44748-115">deviceManagement</span></span>](../resources/intune-enrollment-devicemanagement.md)|<span data-ttu-id="44748-116">Atualizar as propriedades de um objeto de [deviceManagement](../resources/intune-enrollment-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="44748-116">Update the properties of a [deviceManagement](../resources/intune-enrollment-devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="44748-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="44748-117">Properties</span></span>
|<span data-ttu-id="44748-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="44748-118">Property</span></span>|<span data-ttu-id="44748-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="44748-119">Type</span></span>|<span data-ttu-id="44748-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="44748-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44748-121">id</span><span class="sxs-lookup"><span data-stu-id="44748-121">id</span></span>|<span data-ttu-id="44748-122">String</span><span class="sxs-lookup"><span data-stu-id="44748-122">String</span></span>|<span data-ttu-id="44748-123">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="44748-123">The GUID for the object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="44748-124">Relações</span><span class="sxs-lookup"><span data-stu-id="44748-124">Relationships</span></span>
|<span data-ttu-id="44748-125">Relação</span><span class="sxs-lookup"><span data-stu-id="44748-125">Relationship</span></span>|<span data-ttu-id="44748-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="44748-126">Type</span></span>|<span data-ttu-id="44748-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="44748-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44748-128">windowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="44748-128">windowsAutopilotDeviceIdentities</span></span>|<span data-ttu-id="44748-129">[Coleção windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="44748-129">[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="44748-130">As Windows do dispositivo autopilot continham coleção.</span><span class="sxs-lookup"><span data-stu-id="44748-130">The Windows autopilot device identities contained collection.</span></span>|
|<span data-ttu-id="44748-131">importedWindowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="44748-131">importedWindowsAutopilotDeviceIdentities</span></span>|<span data-ttu-id="44748-132">Coleção [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="44748-132">[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="44748-133">Coleção de dispositivos do Windows AutoPilot importados.</span><span class="sxs-lookup"><span data-stu-id="44748-133">Collection of imported Windows autopilot devices.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="44748-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="44748-134">JSON Representation</span></span>
<span data-ttu-id="44748-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="44748-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```




