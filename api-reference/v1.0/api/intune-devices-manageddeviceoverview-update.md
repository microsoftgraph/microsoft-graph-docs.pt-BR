---
title: Atualizar managedDeviceOverview
description: Atualizar as propriedades de um objeto managedDeviceOverview.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3e4b7acf2b03ee37bf9171bfe83164c25e993f5f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260575"
---
# <a name="update-manageddeviceoverview"></a><span data-ttu-id="8fec0-103">Atualizar managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="8fec0-103">Update managedDeviceOverview</span></span>

> <span data-ttu-id="8fec0-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8fec0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8fec0-105">Atualizar as propriedades de um objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="8fec0-105">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8fec0-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8fec0-106">Prerequisites</span></span>
<span data-ttu-id="8fec0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8fec0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8fec0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8fec0-109">Permission type</span></span>|<span data-ttu-id="8fec0-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8fec0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8fec0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8fec0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8fec0-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fec0-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8fec0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8fec0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8fec0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8fec0-114">Not supported.</span></span>|
|<span data-ttu-id="8fec0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8fec0-115">Application</span></span>|<span data-ttu-id="8fec0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8fec0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8fec0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8fec0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceOverview
```

## <a name="request-headers"></a><span data-ttu-id="8fec0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8fec0-118">Request headers</span></span>
|<span data-ttu-id="8fec0-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8fec0-119">Header</span></span>|<span data-ttu-id="8fec0-120">Valor</span><span class="sxs-lookup"><span data-stu-id="8fec0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8fec0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8fec0-121">Authorization</span></span>|<span data-ttu-id="8fec0-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8fec0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8fec0-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8fec0-123">Accept</span></span>|<span data-ttu-id="8fec0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8fec0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8fec0-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8fec0-125">Request body</span></span>
<span data-ttu-id="8fec0-126">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="8fec0-126">In the request body, supply a JSON representation for the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

<span data-ttu-id="8fec0-127">A tabela a seguir mostra as propriedades necessárias ao criar [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="8fec0-127">The following table shows the properties that are required when you create the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span></span>

|<span data-ttu-id="8fec0-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8fec0-128">Property</span></span>|<span data-ttu-id="8fec0-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="8fec0-129">Type</span></span>|<span data-ttu-id="8fec0-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="8fec0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fec0-131">id</span><span class="sxs-lookup"><span data-stu-id="8fec0-131">id</span></span>|<span data-ttu-id="8fec0-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8fec0-132">String</span></span>|<span data-ttu-id="8fec0-133">O identificador exclusivo do resumo</span><span class="sxs-lookup"><span data-stu-id="8fec0-133">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="8fec0-134">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8fec0-134">enrolledDeviceCount</span></span>|<span data-ttu-id="8fec0-135">Int32</span><span class="sxs-lookup"><span data-stu-id="8fec0-135">Int32</span></span>|<span data-ttu-id="8fec0-136">Contagem total de dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="8fec0-136">Total enrolled device count.</span></span> <span data-ttu-id="8fec0-137">Não inclui dispositivos PC gerenciados pelo Intune PC Agent</span><span class="sxs-lookup"><span data-stu-id="8fec0-137">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="8fec0-138">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="8fec0-138">mdmEnrolledCount</span></span>|<span data-ttu-id="8fec0-139">Int32</span><span class="sxs-lookup"><span data-stu-id="8fec0-139">Int32</span></span>|<span data-ttu-id="8fec0-140">O número de dispositivos registrados no MDM</span><span class="sxs-lookup"><span data-stu-id="8fec0-140">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="8fec0-141">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8fec0-141">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="8fec0-142">Int32</span><span class="sxs-lookup"><span data-stu-id="8fec0-142">Int32</span></span>|<span data-ttu-id="8fec0-143">O número de dispositivos registrados no MDM e no EAS</span><span class="sxs-lookup"><span data-stu-id="8fec0-143">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="8fec0-144">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="8fec0-144">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="8fec0-145">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="8fec0-145">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="8fec0-146">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8fec0-146">Device operating system summary.</span></span>|
|<span data-ttu-id="8fec0-147">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="8fec0-147">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="8fec0-148">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="8fec0-148">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="8fec0-149">Distribuição do Estado de acesso do Exchange no Intune</span><span class="sxs-lookup"><span data-stu-id="8fec0-149">Distribution of Exchange Access State in Intune</span></span>|



## <a name="response"></a><span data-ttu-id="8fec0-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="8fec0-150">Response</span></span>
<span data-ttu-id="8fec0-151">Se tiver êxito, esse método retornará um código de resposta `200 OK` e um objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8fec0-151">If successful, this method returns a `200 OK` response code and an updated [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fec0-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8fec0-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="8fec0-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8fec0-153">Request</span></span>
<span data-ttu-id="8fec0-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8fec0-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/managedDeviceOverview
Content-type: application/json
Content-length: 685

{
  "@odata.type": "#microsoft.graph.managedDeviceOverview",
  "enrolledDeviceCount": 3,
  "mdmEnrolledCount": 0,
  "dualEnrolledDeviceCount": 7,
  "deviceOperatingSystemSummary": {
    "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
    "androidCount": 12,
    "iosCount": 8,
    "macOSCount": 10,
    "windowsMobileCount": 2,
    "windowsCount": 12,
    "unknownCount": 12
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
    "allowedDeviceCount": 2,
    "blockedDeviceCount": 2,
    "quarantinedDeviceCount": 6,
    "unknownDeviceCount": 2,
    "unavailableDeviceCount": 6
  }
}
```

### <a name="response"></a><span data-ttu-id="8fec0-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="8fec0-155">Response</span></span>
<span data-ttu-id="8fec0-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8fec0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 734

{
  "@odata.type": "#microsoft.graph.managedDeviceOverview",
  "id": "42a91653-1653-42a9-5316-a9425316a942",
  "enrolledDeviceCount": 3,
  "mdmEnrolledCount": 0,
  "dualEnrolledDeviceCount": 7,
  "deviceOperatingSystemSummary": {
    "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
    "androidCount": 12,
    "iosCount": 8,
    "macOSCount": 10,
    "windowsMobileCount": 2,
    "windowsCount": 12,
    "unknownCount": 12
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
    "allowedDeviceCount": 2,
    "blockedDeviceCount": 2,
    "quarantinedDeviceCount": 6,
    "unknownDeviceCount": 2,
    "unavailableDeviceCount": 6
  }
}
```



