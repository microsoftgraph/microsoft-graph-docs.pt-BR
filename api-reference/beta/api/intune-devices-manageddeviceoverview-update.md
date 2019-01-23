---
title: Atualizar managedDeviceOverview
description: Atualizar as propriedades de um objeto managedDeviceOverview.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 34271db88490fba3ac635892daac66bf9cf904b8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424529"
---
# <a name="update-manageddeviceoverview"></a><span data-ttu-id="80ba2-103">Atualizar managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="80ba2-103">Update managedDeviceOverview</span></span>

> <span data-ttu-id="80ba2-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="80ba2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="80ba2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="80ba2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="80ba2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="80ba2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80ba2-107">Atualizar as propriedades de um objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="80ba2-107">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80ba2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="80ba2-108">Prerequisites</span></span>
<span data-ttu-id="80ba2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="80ba2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="80ba2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="80ba2-111">Permission type</span></span>|<span data-ttu-id="80ba2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="80ba2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80ba2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="80ba2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="80ba2-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80ba2-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="80ba2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="80ba2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80ba2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80ba2-116">Not supported.</span></span>|
|<span data-ttu-id="80ba2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="80ba2-117">Application</span></span>|<span data-ttu-id="80ba2-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80ba2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80ba2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="80ba2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceOverview
```

## <a name="request-headers"></a><span data-ttu-id="80ba2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="80ba2-120">Request headers</span></span>
|<span data-ttu-id="80ba2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="80ba2-121">Header</span></span>|<span data-ttu-id="80ba2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="80ba2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80ba2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="80ba2-123">Authorization</span></span>|<span data-ttu-id="80ba2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="80ba2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80ba2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="80ba2-125">Accept</span></span>|<span data-ttu-id="80ba2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="80ba2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80ba2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="80ba2-127">Request body</span></span>
<span data-ttu-id="80ba2-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="80ba2-128">In the request body, supply a JSON representation for the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

<span data-ttu-id="80ba2-129">A tabela a seguir mostra as propriedades necessárias ao criar [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="80ba2-129">The following table shows the properties that are required when you create the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span></span>

|<span data-ttu-id="80ba2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80ba2-130">Property</span></span>|<span data-ttu-id="80ba2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="80ba2-131">Type</span></span>|<span data-ttu-id="80ba2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="80ba2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80ba2-133">id</span><span class="sxs-lookup"><span data-stu-id="80ba2-133">id</span></span>|<span data-ttu-id="80ba2-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80ba2-134">String</span></span>|<span data-ttu-id="80ba2-135">O identificador exclusivo do resumo</span><span class="sxs-lookup"><span data-stu-id="80ba2-135">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="80ba2-136">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="80ba2-136">enrolledDeviceCount</span></span>|<span data-ttu-id="80ba2-137">Int32</span><span class="sxs-lookup"><span data-stu-id="80ba2-137">Int32</span></span>|<span data-ttu-id="80ba2-138">Contagem total de dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="80ba2-138">Total enrolled device count.</span></span> <span data-ttu-id="80ba2-139">Não inclui dispositivos PC gerenciados pelo Intune PC Agent</span><span class="sxs-lookup"><span data-stu-id="80ba2-139">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="80ba2-140">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="80ba2-140">mdmEnrolledCount</span></span>|<span data-ttu-id="80ba2-141">Int32</span><span class="sxs-lookup"><span data-stu-id="80ba2-141">Int32</span></span>|<span data-ttu-id="80ba2-142">O número de dispositivos registrados no MDM</span><span class="sxs-lookup"><span data-stu-id="80ba2-142">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="80ba2-143">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="80ba2-143">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="80ba2-144">Int32</span><span class="sxs-lookup"><span data-stu-id="80ba2-144">Int32</span></span>|<span data-ttu-id="80ba2-145">O número de dispositivos registrados no MDM e no EAS</span><span class="sxs-lookup"><span data-stu-id="80ba2-145">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="80ba2-146">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="80ba2-146">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="80ba2-147">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="80ba2-147">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="80ba2-148">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="80ba2-148">Device operating system summary.</span></span>|
|<span data-ttu-id="80ba2-149">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="80ba2-149">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="80ba2-150">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="80ba2-150">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="80ba2-151">Distribuição do Estado de acesso do Exchange no Intune</span><span class="sxs-lookup"><span data-stu-id="80ba2-151">Distribution of Exchange Access State in Intune</span></span>|
|<span data-ttu-id="80ba2-152">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="80ba2-152">managedDeviceModelsAndManufacturers</span></span>|[<span data-ttu-id="80ba2-153">managedDeviceModelsAndManufacturers</span><span class="sxs-lookup"><span data-stu-id="80ba2-153">managedDeviceModelsAndManufacturers</span></span>](../resources/intune-devices-manageddevicemodelsandmanufacturers.md)|<span data-ttu-id="80ba2-154">Modelos e fabricantes meatadata para dispositivos gerenciados na conta</span><span class="sxs-lookup"><span data-stu-id="80ba2-154">Models and Manufactures meatadata for managed devices in the account</span></span>|
|<span data-ttu-id="80ba2-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="80ba2-155">lastModifiedDateTime</span></span>|<span data-ttu-id="80ba2-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80ba2-156">DateTimeOffset</span></span>|<span data-ttu-id="80ba2-157">Última data modificada hora de visão geral do dispositivo</span><span class="sxs-lookup"><span data-stu-id="80ba2-157">Last modified date time of device overview</span></span>|



## <a name="response"></a><span data-ttu-id="80ba2-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="80ba2-158">Response</span></span>
<span data-ttu-id="80ba2-159">Se tiver êxito, esse método retornará um código de resposta `200 OK` e um objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="80ba2-159">If successful, this method returns a `200 OK` response code and an updated [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80ba2-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="80ba2-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="80ba2-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80ba2-161">Request</span></span>
<span data-ttu-id="80ba2-162">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="80ba2-162">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="80ba2-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="80ba2-163">Response</span></span>
<span data-ttu-id="80ba2-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="80ba2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




