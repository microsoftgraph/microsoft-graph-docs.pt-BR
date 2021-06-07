---
title: Tipo de recurso deviceManagement
description: Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bff42d331ac2fe67bdca2193a4ab8ad230b36113
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755173"
---
# <a name="devicemanagement-resource-type"></a><span data-ttu-id="e411d-103">Tipo de recurso deviceManagement</span><span class="sxs-lookup"><span data-stu-id="e411d-103">deviceManagement resource type</span></span>

<span data-ttu-id="e411d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e411d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e411d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e411d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e411d-106">Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="e411d-106">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="e411d-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="e411d-107">Methods</span></span>
|<span data-ttu-id="e411d-108">Método</span><span class="sxs-lookup"><span data-stu-id="e411d-108">Method</span></span>|<span data-ttu-id="e411d-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e411d-109">Return Type</span></span>|<span data-ttu-id="e411d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e411d-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e411d-111">Obter deviceManagement</span><span class="sxs-lookup"><span data-stu-id="e411d-111">Get deviceManagement</span></span>](../api/intune-devices-devicemanagement-get.md)|[<span data-ttu-id="e411d-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="e411d-112">deviceManagement</span></span>](../resources/intune-devices-devicemanagement.md)|<span data-ttu-id="e411d-113">Leia as propriedades e as relações do objeto [deviceManagement](../resources/intune-devices-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="e411d-113">Read properties and relationships of the [deviceManagement](../resources/intune-devices-devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="e411d-114">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="e411d-114">Update deviceManagement</span></span>](../api/intune-devices-devicemanagement-update.md)|[<span data-ttu-id="e411d-115">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="e411d-115">deviceManagement</span></span>](../resources/intune-devices-devicemanagement.md)|<span data-ttu-id="e411d-116">Atualizar as propriedades de um objeto de [deviceManagement](../resources/intune-devices-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="e411d-116">Update the properties of a [deviceManagement](../resources/intune-devices-devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e411d-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e411d-117">Properties</span></span>
|<span data-ttu-id="e411d-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e411d-118">Property</span></span>|<span data-ttu-id="e411d-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="e411d-119">Type</span></span>|<span data-ttu-id="e411d-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e411d-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e411d-121">id</span><span class="sxs-lookup"><span data-stu-id="e411d-121">id</span></span>|<span data-ttu-id="e411d-122">String</span><span class="sxs-lookup"><span data-stu-id="e411d-122">String</span></span>|<span data-ttu-id="e411d-123">O identificador exclusivo do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e411d-123">Unique Identifier for the device</span></span>|
|<span data-ttu-id="e411d-124">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="e411d-124">subscriptionState</span></span>|[<span data-ttu-id="e411d-125">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="e411d-125">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="e411d-126">Estado de assinatura de gerenciamento de dispositivo móvel do locatário.</span><span class="sxs-lookup"><span data-stu-id="e411d-126">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="e411d-127">Os valores possíveis são: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span><span class="sxs-lookup"><span data-stu-id="e411d-127">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e411d-128">Relações</span><span class="sxs-lookup"><span data-stu-id="e411d-128">Relationships</span></span>
|<span data-ttu-id="e411d-129">Relação</span><span class="sxs-lookup"><span data-stu-id="e411d-129">Relationship</span></span>|<span data-ttu-id="e411d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e411d-130">Type</span></span>|<span data-ttu-id="e411d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e411d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e411d-132">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="e411d-132">applePushNotificationCertificate</span></span>|[<span data-ttu-id="e411d-133">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="e411d-133">applePushNotificationCertificate</span></span>](../resources/intune-devices-applepushnotificationcertificate.md)|<span data-ttu-id="e411d-134">Certificado de notificação por push da Apple.</span><span class="sxs-lookup"><span data-stu-id="e411d-134">Apple push notification certificate.</span></span>|
|<span data-ttu-id="e411d-135">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="e411d-135">managedDeviceOverview</span></span>|[<span data-ttu-id="e411d-136">managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="e411d-136">managedDeviceOverview</span></span>](../resources/intune-devices-manageddeviceoverview.md)|<span data-ttu-id="e411d-137">Visão geral do dispositivo</span><span class="sxs-lookup"><span data-stu-id="e411d-137">Device overview</span></span>|
|<span data-ttu-id="e411d-138">detectedApps</span><span class="sxs-lookup"><span data-stu-id="e411d-138">detectedApps</span></span>|<span data-ttu-id="e411d-139">Conjunto [detectedApp](../resources/intune-devices-detectedapp.md)</span><span class="sxs-lookup"><span data-stu-id="e411d-139">[detectedApp](../resources/intune-devices-detectedapp.md) collection</span></span>|<span data-ttu-id="e411d-140">A lista de aplicativos detectados associados a um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e411d-140">The list of detected apps associated with a device.</span></span>|
|<span data-ttu-id="e411d-141">managedDevices</span><span class="sxs-lookup"><span data-stu-id="e411d-141">managedDevices</span></span>|<span data-ttu-id="e411d-142">Conjunto [managedDevice](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="e411d-142">[managedDevice](../resources/intune-devices-manageddevice.md) collection</span></span>|<span data-ttu-id="e411d-143">A lista de dispositivos gerenciados.</span><span class="sxs-lookup"><span data-stu-id="e411d-143">The list of managed devices.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e411d-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e411d-144">JSON Representation</span></span>
<span data-ttu-id="e411d-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e411d-145">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)",
  "subscriptionState": "String"
}
```




