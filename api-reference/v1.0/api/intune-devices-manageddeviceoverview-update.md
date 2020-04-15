---
title: Atualizar managedDeviceOverview
description: Atualizar as propriedades de um objeto managedDeviceOverview.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 45b164859bd5d53dc05e22c47aa1ca99335b18f3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43388732"
---
# <a name="update-manageddeviceoverview"></a><span data-ttu-id="46564-103">Atualizar managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="46564-103">Update managedDeviceOverview</span></span>

<span data-ttu-id="46564-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46564-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="46564-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="46564-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46564-106">Atualizar as propriedades de um objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="46564-106">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46564-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="46564-107">Prerequisites</span></span>
<span data-ttu-id="46564-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46564-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46564-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46564-110">Permission type</span></span>|<span data-ttu-id="46564-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="46564-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46564-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46564-112">Delegated (work or school account)</span></span>|<span data-ttu-id="46564-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46564-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="46564-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46564-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46564-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46564-115">Not supported.</span></span>|
|<span data-ttu-id="46564-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46564-116">Application</span></span>|<span data-ttu-id="46564-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46564-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46564-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46564-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceOverview
```

## <a name="request-headers"></a><span data-ttu-id="46564-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46564-119">Request headers</span></span>
|<span data-ttu-id="46564-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="46564-120">Header</span></span>|<span data-ttu-id="46564-121">Valor</span><span class="sxs-lookup"><span data-stu-id="46564-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46564-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="46564-122">Authorization</span></span>|<span data-ttu-id="46564-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46564-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46564-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="46564-124">Accept</span></span>|<span data-ttu-id="46564-125">application/json</span><span class="sxs-lookup"><span data-stu-id="46564-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46564-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46564-126">Request body</span></span>
<span data-ttu-id="46564-127">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="46564-127">In the request body, supply a JSON representation for the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

<span data-ttu-id="46564-128">A tabela a seguir mostra as propriedades necessárias ao criar [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="46564-128">The following table shows the properties that are required when you create the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span></span>

|<span data-ttu-id="46564-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="46564-129">Property</span></span>|<span data-ttu-id="46564-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="46564-130">Type</span></span>|<span data-ttu-id="46564-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="46564-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46564-132">id</span><span class="sxs-lookup"><span data-stu-id="46564-132">id</span></span>|<span data-ttu-id="46564-133">String</span><span class="sxs-lookup"><span data-stu-id="46564-133">String</span></span>|<span data-ttu-id="46564-134">O identificador exclusivo do resumo</span><span class="sxs-lookup"><span data-stu-id="46564-134">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="46564-135">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="46564-135">enrolledDeviceCount</span></span>|<span data-ttu-id="46564-136">Int32</span><span class="sxs-lookup"><span data-stu-id="46564-136">Int32</span></span>|<span data-ttu-id="46564-137">Contagem total de dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="46564-137">Total enrolled device count.</span></span> <span data-ttu-id="46564-138">Não inclui dispositivos PC gerenciados pelo Intune PC Agent</span><span class="sxs-lookup"><span data-stu-id="46564-138">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="46564-139">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="46564-139">mdmEnrolledCount</span></span>|<span data-ttu-id="46564-140">Int32</span><span class="sxs-lookup"><span data-stu-id="46564-140">Int32</span></span>|<span data-ttu-id="46564-141">O número de dispositivos registrados no MDM</span><span class="sxs-lookup"><span data-stu-id="46564-141">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="46564-142">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="46564-142">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="46564-143">Int32</span><span class="sxs-lookup"><span data-stu-id="46564-143">Int32</span></span>|<span data-ttu-id="46564-144">O número de dispositivos registrados no MDM e no EAS</span><span class="sxs-lookup"><span data-stu-id="46564-144">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="46564-145">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="46564-145">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="46564-146">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="46564-146">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="46564-147">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="46564-147">Device operating system summary.</span></span>|
|<span data-ttu-id="46564-148">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="46564-148">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="46564-149">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="46564-149">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="46564-150">Distribuição do Estado de acesso do Exchange no Intune</span><span class="sxs-lookup"><span data-stu-id="46564-150">Distribution of Exchange Access State in Intune</span></span>|



## <a name="response"></a><span data-ttu-id="46564-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="46564-151">Response</span></span>
<span data-ttu-id="46564-152">Se tiver êxito, esse método retornará um código de resposta `200 OK` e um objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46564-152">If successful, this method returns a `200 OK` response code and an updated [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46564-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46564-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="46564-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46564-154">Request</span></span>
<span data-ttu-id="46564-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="46564-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="46564-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="46564-156">Response</span></span>
<span data-ttu-id="46564-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="46564-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






