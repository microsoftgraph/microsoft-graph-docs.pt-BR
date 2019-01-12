---
title: Atualizar managedDeviceOverview
description: Atualizar as propriedades de um objeto managedDeviceOverview.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a4545fb198dcb4c9433a1988392f6388020e37d4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959871"
---
# <a name="update-manageddeviceoverview"></a><span data-ttu-id="61ccf-103">Atualizar managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="61ccf-103">Update managedDeviceOverview</span></span>

> <span data-ttu-id="61ccf-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="61ccf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="61ccf-105">Atualizar as propriedades de um objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="61ccf-105">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="61ccf-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="61ccf-106">Prerequisites</span></span>
<span data-ttu-id="61ccf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61ccf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61ccf-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61ccf-109">Permission type</span></span>|<span data-ttu-id="61ccf-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="61ccf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61ccf-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61ccf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="61ccf-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61ccf-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="61ccf-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61ccf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61ccf-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61ccf-114">Not supported.</span></span>|
|<span data-ttu-id="61ccf-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61ccf-115">Application</span></span>|<span data-ttu-id="61ccf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61ccf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="61ccf-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61ccf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceOverview
```

## <a name="request-headers"></a><span data-ttu-id="61ccf-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61ccf-118">Request headers</span></span>
|<span data-ttu-id="61ccf-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="61ccf-119">Header</span></span>|<span data-ttu-id="61ccf-120">Valor</span><span class="sxs-lookup"><span data-stu-id="61ccf-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61ccf-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="61ccf-121">Authorization</span></span>|<span data-ttu-id="61ccf-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61ccf-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61ccf-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="61ccf-123">Accept</span></span>|<span data-ttu-id="61ccf-124">application/json</span><span class="sxs-lookup"><span data-stu-id="61ccf-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61ccf-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61ccf-125">Request body</span></span>
<span data-ttu-id="61ccf-126">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="61ccf-126">In the request body, supply a JSON representation for the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

<span data-ttu-id="61ccf-127">A tabela a seguir mostra as propriedades necessárias ao criar [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="61ccf-127">The following table shows the properties that are required when you create the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span></span>

|<span data-ttu-id="61ccf-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="61ccf-128">Property</span></span>|<span data-ttu-id="61ccf-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="61ccf-129">Type</span></span>|<span data-ttu-id="61ccf-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="61ccf-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61ccf-131">id</span><span class="sxs-lookup"><span data-stu-id="61ccf-131">id</span></span>|<span data-ttu-id="61ccf-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61ccf-132">String</span></span>|<span data-ttu-id="61ccf-133">O identificador exclusivo do resumo</span><span class="sxs-lookup"><span data-stu-id="61ccf-133">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="61ccf-134">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="61ccf-134">enrolledDeviceCount</span></span>|<span data-ttu-id="61ccf-135">Int32</span><span class="sxs-lookup"><span data-stu-id="61ccf-135">Int32</span></span>|<span data-ttu-id="61ccf-136">Contagem total de dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="61ccf-136">Total enrolled device count.</span></span> <span data-ttu-id="61ccf-137">Não inclui dispositivos PC gerenciados pelo Intune PC Agent</span><span class="sxs-lookup"><span data-stu-id="61ccf-137">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="61ccf-138">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="61ccf-138">mdmEnrolledCount</span></span>|<span data-ttu-id="61ccf-139">Int32</span><span class="sxs-lookup"><span data-stu-id="61ccf-139">Int32</span></span>|<span data-ttu-id="61ccf-140">O número de dispositivos registrados no MDM</span><span class="sxs-lookup"><span data-stu-id="61ccf-140">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="61ccf-141">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="61ccf-141">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="61ccf-142">Int32</span><span class="sxs-lookup"><span data-stu-id="61ccf-142">Int32</span></span>|<span data-ttu-id="61ccf-143">O número de dispositivos registrados no MDM e no EAS</span><span class="sxs-lookup"><span data-stu-id="61ccf-143">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="61ccf-144">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="61ccf-144">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="61ccf-145">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="61ccf-145">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="61ccf-146">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="61ccf-146">Device operating system summary.</span></span>|
|<span data-ttu-id="61ccf-147">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="61ccf-147">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="61ccf-148">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="61ccf-148">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="61ccf-149">Distribuição do Estado de acesso do Exchange no Intune</span><span class="sxs-lookup"><span data-stu-id="61ccf-149">Distribution of Exchange Access State in Intune</span></span>|



## <a name="response"></a><span data-ttu-id="61ccf-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="61ccf-150">Response</span></span>
<span data-ttu-id="61ccf-151">Se tiver êxito, esse método retornará um código de resposta `200 OK` e um objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="61ccf-151">If successful, this method returns a `200 OK` response code and an updated [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61ccf-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="61ccf-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="61ccf-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61ccf-153">Request</span></span>
<span data-ttu-id="61ccf-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="61ccf-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="61ccf-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="61ccf-155">Response</span></span>
<span data-ttu-id="61ccf-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="61ccf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



