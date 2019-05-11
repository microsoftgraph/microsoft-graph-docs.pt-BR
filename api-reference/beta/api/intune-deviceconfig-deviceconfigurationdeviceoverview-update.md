---
title: Atualizar deviceConfigurationDeviceOverview
description: Atualizar as propriedades de um objeto deviceConfigurationDeviceOverview.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c536d5dbd1f295ea85e58c0fa6592969253a717f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33927416"
---
# <a name="update-deviceconfigurationdeviceoverview"></a><span data-ttu-id="cf154-103">Atualizar deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="cf154-103">Update deviceConfigurationDeviceOverview</span></span>

> <span data-ttu-id="cf154-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cf154-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf154-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cf154-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf154-106">Atualizar as propriedades de um objeto [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="cf154-106">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf154-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cf154-107">Prerequisites</span></span>
<span data-ttu-id="cf154-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf154-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf154-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf154-110">Permission type</span></span>|<span data-ttu-id="cf154-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cf154-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf154-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf154-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cf154-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf154-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cf154-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf154-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf154-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf154-115">Not supported.</span></span>|
|<span data-ttu-id="cf154-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf154-116">Application</span></span>|<span data-ttu-id="cf154-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf154-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf154-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf154-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="cf154-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf154-119">Request headers</span></span>
|<span data-ttu-id="cf154-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cf154-120">Header</span></span>|<span data-ttu-id="cf154-121">Valor</span><span class="sxs-lookup"><span data-stu-id="cf154-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf154-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf154-122">Authorization</span></span>|<span data-ttu-id="cf154-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf154-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf154-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cf154-124">Accept</span></span>|<span data-ttu-id="cf154-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cf154-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf154-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf154-126">Request body</span></span>
<span data-ttu-id="cf154-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="cf154-127">In the request body, supply a JSON representation for the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

<span data-ttu-id="cf154-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="cf154-128">The following table shows the properties that are required when you create the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span></span>

|<span data-ttu-id="cf154-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf154-129">Property</span></span>|<span data-ttu-id="cf154-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf154-130">Type</span></span>|<span data-ttu-id="cf154-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf154-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf154-132">id</span><span class="sxs-lookup"><span data-stu-id="cf154-132">id</span></span>|<span data-ttu-id="cf154-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf154-133">String</span></span>|<span data-ttu-id="cf154-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="cf154-134">Key of the entity.</span></span>|
|<span data-ttu-id="cf154-135">pendingCount</span><span class="sxs-lookup"><span data-stu-id="cf154-135">pendingCount</span></span>|<span data-ttu-id="cf154-136">Int32</span><span class="sxs-lookup"><span data-stu-id="cf154-136">Int32</span></span>|<span data-ttu-id="cf154-137">Número de dispositivos pendentes</span><span class="sxs-lookup"><span data-stu-id="cf154-137">Number of pending devices</span></span>|
|<span data-ttu-id="cf154-138">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="cf154-138">notApplicableCount</span></span>|<span data-ttu-id="cf154-139">Int32</span><span class="sxs-lookup"><span data-stu-id="cf154-139">Int32</span></span>|<span data-ttu-id="cf154-140">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="cf154-140">Number of not applicable devices</span></span>|
|<span data-ttu-id="cf154-141">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="cf154-141">notApplicablePlatformCount</span></span>|<span data-ttu-id="cf154-142">Int32</span><span class="sxs-lookup"><span data-stu-id="cf154-142">Int32</span></span>|<span data-ttu-id="cf154-143">Número de dispositivos não aplicáveis devido à plataforma e à política incompatíveis</span><span class="sxs-lookup"><span data-stu-id="cf154-143">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="cf154-144">successCount</span><span class="sxs-lookup"><span data-stu-id="cf154-144">successCount</span></span>|<span data-ttu-id="cf154-145">Int32</span><span class="sxs-lookup"><span data-stu-id="cf154-145">Int32</span></span>|<span data-ttu-id="cf154-146">Número de dispositivos com êxito</span><span class="sxs-lookup"><span data-stu-id="cf154-146">Number of succeeded devices</span></span>|
|<span data-ttu-id="cf154-147">errorCount</span><span class="sxs-lookup"><span data-stu-id="cf154-147">errorCount</span></span>|<span data-ttu-id="cf154-148">Int32</span><span class="sxs-lookup"><span data-stu-id="cf154-148">Int32</span></span>|<span data-ttu-id="cf154-149">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="cf154-149">Number of error devices</span></span>|
|<span data-ttu-id="cf154-150">failedCount</span><span class="sxs-lookup"><span data-stu-id="cf154-150">failedCount</span></span>|<span data-ttu-id="cf154-151">Int32</span><span class="sxs-lookup"><span data-stu-id="cf154-151">Int32</span></span>|<span data-ttu-id="cf154-152">Número de dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="cf154-152">Number of failed devices</span></span>|
|<span data-ttu-id="cf154-153">conflictCount</span><span class="sxs-lookup"><span data-stu-id="cf154-153">conflictCount</span></span>|<span data-ttu-id="cf154-154">Int32</span><span class="sxs-lookup"><span data-stu-id="cf154-154">Int32</span></span>|<span data-ttu-id="cf154-155">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="cf154-155">Number of devices in conflict</span></span>|
|<span data-ttu-id="cf154-156">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="cf154-156">lastUpdateDateTime</span></span>|<span data-ttu-id="cf154-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf154-157">DateTimeOffset</span></span>|<span data-ttu-id="cf154-158">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="cf154-158">Last update time</span></span>|
|<span data-ttu-id="cf154-159">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="cf154-159">configurationVersion</span></span>|<span data-ttu-id="cf154-160">Int32</span><span class="sxs-lookup"><span data-stu-id="cf154-160">Int32</span></span>|<span data-ttu-id="cf154-161">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="cf154-161">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="cf154-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf154-162">Response</span></span>
<span data-ttu-id="cf154-163">Se tiver êxito, este método retornará um código de resposta `200 OK` e o objeto [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf154-163">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf154-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cf154-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf154-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf154-165">Request</span></span>
<span data-ttu-id="cf154-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf154-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
Content-type: application/json
Content-length: 345

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="cf154-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf154-167">Response</span></span>
<span data-ttu-id="cf154-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cf154-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 394

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "id": "62d48e3a-8e3a-62d4-3a8e-d4623a8ed462",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "conflictCount": 13,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```




