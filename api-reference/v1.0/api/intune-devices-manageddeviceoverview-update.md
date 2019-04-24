---
title: Atualizar managedDeviceOverview
description: Atualizar as propriedades de um objeto managedDeviceOverview.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3808c35b9aae428975ed976b31634c27e7a41286
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585038"
---
# <a name="update-manageddeviceoverview"></a><span data-ttu-id="aa149-103">Atualizar managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="aa149-103">Update managedDeviceOverview</span></span>

> <span data-ttu-id="aa149-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aa149-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa149-105">Atualizar as propriedades de um objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="aa149-105">Update the properties of a [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aa149-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aa149-106">Prerequisites</span></span>
<span data-ttu-id="aa149-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa149-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa149-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aa149-109">Permission type</span></span>|<span data-ttu-id="aa149-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="aa149-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa149-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aa149-111">Delegated (work or school account)</span></span>|<span data-ttu-id="aa149-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa149-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="aa149-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aa149-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa149-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa149-114">Not supported.</span></span>|
|<span data-ttu-id="aa149-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aa149-115">Application</span></span>|<span data-ttu-id="aa149-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aa149-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa149-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aa149-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceOverview
```

## <a name="request-headers"></a><span data-ttu-id="aa149-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aa149-118">Request headers</span></span>
|<span data-ttu-id="aa149-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aa149-119">Header</span></span>|<span data-ttu-id="aa149-120">Valor</span><span class="sxs-lookup"><span data-stu-id="aa149-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa149-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="aa149-121">Authorization</span></span>|<span data-ttu-id="aa149-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aa149-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aa149-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="aa149-123">Accept</span></span>|<span data-ttu-id="aa149-124">application/json</span><span class="sxs-lookup"><span data-stu-id="aa149-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa149-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aa149-125">Request body</span></span>
<span data-ttu-id="aa149-126">No corpo da solicitação, forneça uma representação JSON do objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="aa149-126">In the request body, supply a JSON representation for the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>

<span data-ttu-id="aa149-127">A tabela a seguir mostra as propriedades necessárias ao criar [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="aa149-127">The following table shows the properties that are required when you create the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md).</span></span>

|<span data-ttu-id="aa149-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aa149-128">Property</span></span>|<span data-ttu-id="aa149-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="aa149-129">Type</span></span>|<span data-ttu-id="aa149-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa149-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa149-131">id</span><span class="sxs-lookup"><span data-stu-id="aa149-131">id</span></span>|<span data-ttu-id="aa149-132">String</span><span class="sxs-lookup"><span data-stu-id="aa149-132">String</span></span>|<span data-ttu-id="aa149-133">O identificador exclusivo do resumo</span><span class="sxs-lookup"><span data-stu-id="aa149-133">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="aa149-134">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aa149-134">enrolledDeviceCount</span></span>|<span data-ttu-id="aa149-135">Int32</span><span class="sxs-lookup"><span data-stu-id="aa149-135">Int32</span></span>|<span data-ttu-id="aa149-136">Contagem total de dispositivos registrados.</span><span class="sxs-lookup"><span data-stu-id="aa149-136">Total enrolled device count.</span></span> <span data-ttu-id="aa149-137">Não inclui dispositivos PC gerenciados pelo Intune PC Agent</span><span class="sxs-lookup"><span data-stu-id="aa149-137">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="aa149-138">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="aa149-138">mdmEnrolledCount</span></span>|<span data-ttu-id="aa149-139">Int32</span><span class="sxs-lookup"><span data-stu-id="aa149-139">Int32</span></span>|<span data-ttu-id="aa149-140">O número de dispositivos registrados no MDM</span><span class="sxs-lookup"><span data-stu-id="aa149-140">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="aa149-141">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aa149-141">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="aa149-142">Int32</span><span class="sxs-lookup"><span data-stu-id="aa149-142">Int32</span></span>|<span data-ttu-id="aa149-143">O número de dispositivos registrados no MDM e no EAS</span><span class="sxs-lookup"><span data-stu-id="aa149-143">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="aa149-144">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="aa149-144">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="aa149-145">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="aa149-145">deviceOperatingSystemSummary</span></span>](../resources/intune-devices-deviceoperatingsystemsummary.md)|<span data-ttu-id="aa149-146">Resumo do sistema operacional do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="aa149-146">Device operating system summary.</span></span>|
|<span data-ttu-id="aa149-147">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="aa149-147">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="aa149-148">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="aa149-148">deviceExchangeAccessStateSummary</span></span>](../resources/intune-devices-deviceexchangeaccessstatesummary.md)|<span data-ttu-id="aa149-149">Distribuição do Estado de acesso do Exchange no Intune</span><span class="sxs-lookup"><span data-stu-id="aa149-149">Distribution of Exchange Access State in Intune</span></span>|



## <a name="response"></a><span data-ttu-id="aa149-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa149-150">Response</span></span>
<span data-ttu-id="aa149-151">Se tiver êxito, esse método retornará um código de resposta `200 OK` e um objeto [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aa149-151">If successful, this method returns a `200 OK` response code and an updated [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa149-152">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aa149-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="aa149-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aa149-153">Request</span></span>
<span data-ttu-id="aa149-154">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aa149-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="aa149-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="aa149-155">Response</span></span>
<span data-ttu-id="aa149-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aa149-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



