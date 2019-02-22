---
title: Atualizar managedDeviceOverview
description: Atualizar as propriedades de um objeto managedDeviceOverview.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 642d565a7555446da1728c0a697598de4d5459cc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147842"
---
# <a name="update-manageddeviceoverview"></a><span data-ttu-id="2f1be-103">Atualizar managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="2f1be-103">Update managedDeviceOverview</span></span>

> <span data-ttu-id="2f1be-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2f1be-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f1be-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2f1be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f1be-106">Atualizar as propriedades de um objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="2f1be-106">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f1be-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2f1be-107">Prerequisites</span></span>
<span data-ttu-id="2f1be-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2f1be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2f1be-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f1be-110">Permission type</span></span>|<span data-ttu-id="2f1be-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2f1be-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f1be-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f1be-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2f1be-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f1be-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2f1be-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f1be-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f1be-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f1be-115">Not supported.</span></span>|
|<span data-ttu-id="2f1be-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f1be-116">Application</span></span>|<span data-ttu-id="2f1be-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f1be-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f1be-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f1be-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceOverview
```

## <a name="request-headers"></a><span data-ttu-id="2f1be-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f1be-119">Request headers</span></span>
|<span data-ttu-id="2f1be-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2f1be-120">Header</span></span>|<span data-ttu-id="2f1be-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2f1be-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f1be-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f1be-122">Authorization</span></span>|<span data-ttu-id="2f1be-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f1be-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f1be-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2f1be-124">Accept</span></span>|<span data-ttu-id="2f1be-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2f1be-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f1be-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f1be-126">Request body</span></span>
<span data-ttu-id="2f1be-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="2f1be-127">In the request body, supply a JSON representation for the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

<span data-ttu-id="2f1be-128">A tabela a seguir mostra as propriedades necessárias ao criar [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="2f1be-128">The following table shows the properties that are required when you create the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span></span>

|<span data-ttu-id="2f1be-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2f1be-129">Property</span></span>|<span data-ttu-id="2f1be-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f1be-130">Type</span></span>|<span data-ttu-id="2f1be-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f1be-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f1be-132">id</span><span class="sxs-lookup"><span data-stu-id="2f1be-132">id</span></span>|<span data-ttu-id="2f1be-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f1be-133">String</span></span>|<span data-ttu-id="2f1be-134">O identificador exclusivo do resumo</span><span class="sxs-lookup"><span data-stu-id="2f1be-134">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="2f1be-135">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2f1be-135">enrolledDeviceCount</span></span>|<span data-ttu-id="2f1be-136">Int32</span><span class="sxs-lookup"><span data-stu-id="2f1be-136">Int32</span></span>|<span data-ttu-id="2f1be-137">Contagem total de dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="2f1be-137">Total enrolled device count.</span></span> <span data-ttu-id="2f1be-138">Não inclui dispositivos PC gerenciados pelo Intune PC Agent</span><span class="sxs-lookup"><span data-stu-id="2f1be-138">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="2f1be-139">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="2f1be-139">mdmEnrolledCount</span></span>|<span data-ttu-id="2f1be-140">Int32</span><span class="sxs-lookup"><span data-stu-id="2f1be-140">Int32</span></span>|<span data-ttu-id="2f1be-141">O número de dispositivos registrados no MDM</span><span class="sxs-lookup"><span data-stu-id="2f1be-141">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="2f1be-142">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2f1be-142">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="2f1be-143">Int32</span><span class="sxs-lookup"><span data-stu-id="2f1be-143">Int32</span></span>|<span data-ttu-id="2f1be-144">O número de dispositivos registrados no MDM e no EAS</span><span class="sxs-lookup"><span data-stu-id="2f1be-144">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="2f1be-145">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="2f1be-145">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="2f1be-146">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="2f1be-146">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="2f1be-147">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2f1be-147">Device operating system summary.</span></span>|
|<span data-ttu-id="2f1be-148">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="2f1be-148">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="2f1be-149">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="2f1be-149">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="2f1be-150">Distribuição do Estado de acesso do Exchange no Intune</span><span class="sxs-lookup"><span data-stu-id="2f1be-150">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="2f1be-151">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="2f1be-151">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="2f1be-152">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="2f1be-152">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="2f1be-153">Modela e fabrica meatadata para dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="2f1be-153">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="2f1be-154">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f1be-154">lastModifiedDateTime</span></span>|<span data-ttu-id="2f1be-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f1be-155">DateTimeOffset</span></span>|<span data-ttu-id="2f1be-156">Data e hora da última modificação da visão geral do dispositivo</span><span class="sxs-lookup"><span data-stu-id="2f1be-156">Last modified date time of device overview</span></span>|



## <a name="response"></a><span data-ttu-id="2f1be-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f1be-157">Response</span></span>
<span data-ttu-id="2f1be-158">Se tiver êxito, esse método retornará um código de resposta `200 OK` e um objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f1be-158">If successful, this method returns a `200 OK` response code and an updated [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f1be-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f1be-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f1be-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f1be-160">Request</span></span>
<span data-ttu-id="2f1be-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f1be-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDeviceOverview
Content-type: application/json
Content-length: 943

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
  },
  "managedDeviceModelsAndManufacturers": {
    "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers",
    "deviceModels": [
      "Device Models value"
    ],
    "deviceManufacturers": [
      "Device Manufacturers value"
    ]
  }
}
```

### <a name="response"></a><span data-ttu-id="2f1be-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f1be-162">Response</span></span>
<span data-ttu-id="2f1be-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f1be-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1056

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
  },
  "managedDeviceModelsAndManufacturers": {
    "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers",
    "deviceModels": [
      "Device Models value"
    ],
    "deviceManufacturers": [
      "Device Manufacturers value"
    ]
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




