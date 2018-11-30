---
title: Atualizar managedDeviceOverview
description: Atualizar as propriedades de um objeto managedDeviceOverview.
ms.openlocfilehash: 31a061a5c75e312901d642071255716272dfe564
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036646"
---
# <a name="update-manageddeviceoverview"></a><span data-ttu-id="30984-103">Atualizar managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="30984-103">Update managedDeviceOverview</span></span>

> <span data-ttu-id="30984-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="30984-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="30984-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="30984-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="30984-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="30984-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="30984-107">Atualizar as propriedades de um objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="30984-107">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="30984-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="30984-108">Prerequisites</span></span>
<span data-ttu-id="30984-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30984-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30984-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="30984-111">Permission type</span></span>|<span data-ttu-id="30984-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="30984-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30984-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="30984-113">Delegated (work or school account)</span></span>|<span data-ttu-id="30984-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30984-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="30984-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="30984-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30984-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30984-116">Not supported.</span></span>|
|<span data-ttu-id="30984-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="30984-117">Application</span></span>|<span data-ttu-id="30984-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30984-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="30984-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="30984-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceOverview
```

## <a name="request-headers"></a><span data-ttu-id="30984-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="30984-120">Request headers</span></span>
|<span data-ttu-id="30984-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="30984-121">Header</span></span>|<span data-ttu-id="30984-122">Valor</span><span class="sxs-lookup"><span data-stu-id="30984-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30984-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="30984-123">Authorization</span></span>|<span data-ttu-id="30984-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30984-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30984-125">Accept</span><span class="sxs-lookup"><span data-stu-id="30984-125">Accept</span></span>|<span data-ttu-id="30984-126">application/json</span><span class="sxs-lookup"><span data-stu-id="30984-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30984-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="30984-127">Request body</span></span>
<span data-ttu-id="30984-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="30984-128">In the request body, supply a JSON representation for the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

<span data-ttu-id="30984-129">A tabela a seguir mostra as propriedades necessárias ao criar [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="30984-129">The following table shows the properties that are required when you create the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span></span>

|<span data-ttu-id="30984-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="30984-130">Property</span></span>|<span data-ttu-id="30984-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="30984-131">Type</span></span>|<span data-ttu-id="30984-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="30984-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30984-133">id</span><span class="sxs-lookup"><span data-stu-id="30984-133">id</span></span>|<span data-ttu-id="30984-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="30984-134">String</span></span>|<span data-ttu-id="30984-135">O identificador exclusivo do resumo</span><span class="sxs-lookup"><span data-stu-id="30984-135">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="30984-136">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="30984-136">enrolledDeviceCount</span></span>|<span data-ttu-id="30984-137">Int32</span><span class="sxs-lookup"><span data-stu-id="30984-137">Int32</span></span>|<span data-ttu-id="30984-138">Contagem total de dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="30984-138">Total enrolled device count.</span></span> <span data-ttu-id="30984-139">Não inclui dispositivos PC gerenciados pelo Intune PC Agent</span><span class="sxs-lookup"><span data-stu-id="30984-139">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="30984-140">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="30984-140">mdmEnrolledCount</span></span>|<span data-ttu-id="30984-141">Int32</span><span class="sxs-lookup"><span data-stu-id="30984-141">Int32</span></span>|<span data-ttu-id="30984-142">O número de dispositivos registrados no MDM</span><span class="sxs-lookup"><span data-stu-id="30984-142">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="30984-143">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="30984-143">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="30984-144">Int32</span><span class="sxs-lookup"><span data-stu-id="30984-144">Int32</span></span>|<span data-ttu-id="30984-145">O número de dispositivos registrados no MDM e no EAS</span><span class="sxs-lookup"><span data-stu-id="30984-145">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="30984-146">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="30984-146">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="30984-147">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="30984-147">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="30984-148">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="30984-148">Device operating system summary.</span></span>|
|<span data-ttu-id="30984-149">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="30984-149">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="30984-150">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="30984-150">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="30984-151">Distribuição do Estado de acesso do Exchange no Intune</span><span class="sxs-lookup"><span data-stu-id="30984-151">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="30984-152">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="30984-152">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="30984-153">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="30984-153">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="30984-154">Modelos e fabricantes meatadata para dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="30984-154">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="30984-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="30984-155">lastModifiedDateTime</span></span>|<span data-ttu-id="30984-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30984-156">DateTimeOffset</span></span>|<span data-ttu-id="30984-157">Última data modificada hora de visão geral do dispositivo</span><span class="sxs-lookup"><span data-stu-id="30984-157">Last modified date time of device overview</span></span>|



## <a name="response"></a><span data-ttu-id="30984-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="30984-158">Response</span></span>
<span data-ttu-id="30984-159">Se tiver êxito, esse método retornará um código de resposta `200 OK` e um objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="30984-159">If successful, this method returns a `200 OK` response code and an updated [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30984-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="30984-160">Example</span></span>
### <a name="request"></a><span data-ttu-id="30984-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="30984-161">Request</span></span>
<span data-ttu-id="30984-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="30984-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDeviceOverview
Content-type: application/json
Content-length: 947

{
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

### <a name="response"></a><span data-ttu-id="30984-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="30984-163">Response</span></span>
<span data-ttu-id="30984-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="30984-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





