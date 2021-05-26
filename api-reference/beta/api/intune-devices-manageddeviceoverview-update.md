---
title: Atualizar managedDeviceOverview
description: Atualizar as propriedades de um objeto managedDeviceOverview.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: efec1f7dd1748991785c11a143be9a921b0f4440
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666300"
---
# <a name="update-manageddeviceoverview"></a><span data-ttu-id="a00dd-103">Atualizar managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="a00dd-103">Update managedDeviceOverview</span></span>

<span data-ttu-id="a00dd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a00dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a00dd-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a00dd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a00dd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a00dd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a00dd-107">Atualizar as propriedades de um objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="a00dd-107">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a00dd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a00dd-108">Prerequisites</span></span>
<span data-ttu-id="a00dd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a00dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a00dd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a00dd-111">Permission type</span></span>|<span data-ttu-id="a00dd-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a00dd-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a00dd-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a00dd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a00dd-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a00dd-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a00dd-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a00dd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a00dd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a00dd-116">Not supported.</span></span>|
|<span data-ttu-id="a00dd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a00dd-117">Application</span></span>|<span data-ttu-id="a00dd-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a00dd-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a00dd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a00dd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceOverview
```

## <a name="request-headers"></a><span data-ttu-id="a00dd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a00dd-120">Request headers</span></span>
|<span data-ttu-id="a00dd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a00dd-121">Header</span></span>|<span data-ttu-id="a00dd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a00dd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a00dd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a00dd-123">Authorization</span></span>|<span data-ttu-id="a00dd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a00dd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a00dd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a00dd-125">Accept</span></span>|<span data-ttu-id="a00dd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a00dd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a00dd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a00dd-127">Request body</span></span>
<span data-ttu-id="a00dd-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="a00dd-128">In the request body, supply a JSON representation for the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

<span data-ttu-id="a00dd-129">A tabela a seguir mostra as propriedades necessárias ao criar [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="a00dd-129">The following table shows the properties that are required when you create the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span></span>

|<span data-ttu-id="a00dd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a00dd-130">Property</span></span>|<span data-ttu-id="a00dd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a00dd-131">Type</span></span>|<span data-ttu-id="a00dd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a00dd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a00dd-133">id</span><span class="sxs-lookup"><span data-stu-id="a00dd-133">id</span></span>|<span data-ttu-id="a00dd-134">String</span><span class="sxs-lookup"><span data-stu-id="a00dd-134">String</span></span>|<span data-ttu-id="a00dd-135">O identificador exclusivo do resumo</span><span class="sxs-lookup"><span data-stu-id="a00dd-135">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="a00dd-136">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a00dd-136">enrolledDeviceCount</span></span>|<span data-ttu-id="a00dd-137">Int32</span><span class="sxs-lookup"><span data-stu-id="a00dd-137">Int32</span></span>|<span data-ttu-id="a00dd-138">Contagem total de dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="a00dd-138">Total enrolled device count.</span></span> <span data-ttu-id="a00dd-139">Não inclui dispositivos PC gerenciados pelo Intune PC Agent</span><span class="sxs-lookup"><span data-stu-id="a00dd-139">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="a00dd-140">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="a00dd-140">mdmEnrolledCount</span></span>|<span data-ttu-id="a00dd-141">Int32</span><span class="sxs-lookup"><span data-stu-id="a00dd-141">Int32</span></span>|<span data-ttu-id="a00dd-142">O número de dispositivos registrados no MDM</span><span class="sxs-lookup"><span data-stu-id="a00dd-142">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="a00dd-143">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="a00dd-143">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="a00dd-144">Int32</span><span class="sxs-lookup"><span data-stu-id="a00dd-144">Int32</span></span>|<span data-ttu-id="a00dd-145">O número de dispositivos registrados no MDM e no EAS</span><span class="sxs-lookup"><span data-stu-id="a00dd-145">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="a00dd-146">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="a00dd-146">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="a00dd-147">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="a00dd-147">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="a00dd-148">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a00dd-148">Device operating system summary.</span></span>|
|<span data-ttu-id="a00dd-149">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="a00dd-149">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="a00dd-150">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="a00dd-150">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="a00dd-151">Distribuição do Estado de acesso do Exchange no Intune</span><span class="sxs-lookup"><span data-stu-id="a00dd-151">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="a00dd-152">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="a00dd-152">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="a00dd-153">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="a00dd-153">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="a00dd-154">Modelos e Manufaturas de carmadata para dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="a00dd-154">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="a00dd-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a00dd-155">lastModifiedDateTime</span></span>|<span data-ttu-id="a00dd-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a00dd-156">DateTimeOffset</span></span>|<span data-ttu-id="a00dd-157">Última data de modificação da visão geral do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a00dd-157">Last modified date time of device overview</span></span>|



## <a name="response"></a><span data-ttu-id="a00dd-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="a00dd-158">Response</span></span>
<span data-ttu-id="a00dd-159">Se tiver êxito, esse método retornará um código de resposta `200 OK` e um objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a00dd-159">If successful, this method returns a `200 OK` response code and an updated [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a00dd-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a00dd-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="a00dd-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a00dd-161">Request</span></span>
<span data-ttu-id="a00dd-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a00dd-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDeviceOverview
Content-type: application/json
Content-length: 1271

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
    "unknownCount": 12,
    "androidDedicatedCount": 5,
    "androidDeviceAdminCount": 7,
    "androidFullyManagedCount": 8,
    "androidWorkProfileCount": 7,
    "androidCorporateWorkProfileCount": 0,
    "configMgrDeviceCount": 4,
    "aospUserlessCount": 1,
    "aospUserAssociatedCount": 7,
    "linuxCount": 10,
    "chromeOSCount": 13
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

### <a name="response"></a><span data-ttu-id="a00dd-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="a00dd-163">Response</span></span>
<span data-ttu-id="a00dd-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a00dd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1384

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
    "unknownCount": 12,
    "androidDedicatedCount": 5,
    "androidDeviceAdminCount": 7,
    "androidFullyManagedCount": 8,
    "androidWorkProfileCount": 7,
    "androidCorporateWorkProfileCount": 0,
    "configMgrDeviceCount": 4,
    "aospUserlessCount": 1,
    "aospUserAssociatedCount": 7,
    "linuxCount": 10,
    "chromeOSCount": 13
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




