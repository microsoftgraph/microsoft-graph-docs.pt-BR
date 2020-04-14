---
title: Atualizar deviceConfigurationDeviceOverview
description: Atualizar as propriedades de um objeto deviceConfigurationDeviceOverview.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fa6a665e75692bf528879001bf8af29e80bedb99
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43433493"
---
# <a name="update-deviceconfigurationdeviceoverview"></a><span data-ttu-id="55be3-103">Atualizar deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="55be3-103">Update deviceConfigurationDeviceOverview</span></span>

<span data-ttu-id="55be3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55be3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="55be3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="55be3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55be3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="55be3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55be3-107">Atualizar as propriedades de um objeto [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="55be3-107">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55be3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="55be3-108">Prerequisites</span></span>
<span data-ttu-id="55be3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55be3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55be3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55be3-111">Permission type</span></span>|<span data-ttu-id="55be3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="55be3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55be3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55be3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="55be3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55be3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="55be3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55be3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55be3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55be3-116">Not supported.</span></span>|
|<span data-ttu-id="55be3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55be3-117">Application</span></span>|<span data-ttu-id="55be3-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55be3-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="55be3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55be3-119">HTTP Request</span></span>
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
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatusOverview
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="55be3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55be3-120">Request headers</span></span>
|<span data-ttu-id="55be3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="55be3-121">Header</span></span>|<span data-ttu-id="55be3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="55be3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55be3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="55be3-123">Authorization</span></span>|<span data-ttu-id="55be3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55be3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55be3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="55be3-125">Accept</span></span>|<span data-ttu-id="55be3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="55be3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55be3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55be3-127">Request body</span></span>
<span data-ttu-id="55be3-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="55be3-128">In the request body, supply a JSON representation for the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

<span data-ttu-id="55be3-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span><span class="sxs-lookup"><span data-stu-id="55be3-129">The following table shows the properties that are required when you create the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span></span>

|<span data-ttu-id="55be3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="55be3-130">Property</span></span>|<span data-ttu-id="55be3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="55be3-131">Type</span></span>|<span data-ttu-id="55be3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="55be3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55be3-133">id</span><span class="sxs-lookup"><span data-stu-id="55be3-133">id</span></span>|<span data-ttu-id="55be3-134">String</span><span class="sxs-lookup"><span data-stu-id="55be3-134">String</span></span>|<span data-ttu-id="55be3-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="55be3-135">Key of the entity.</span></span>|
|<span data-ttu-id="55be3-136">pendingCount</span><span class="sxs-lookup"><span data-stu-id="55be3-136">pendingCount</span></span>|<span data-ttu-id="55be3-137">Int32</span><span class="sxs-lookup"><span data-stu-id="55be3-137">Int32</span></span>|<span data-ttu-id="55be3-138">Número de dispositivos pendentes</span><span class="sxs-lookup"><span data-stu-id="55be3-138">Number of pending devices</span></span>|
|<span data-ttu-id="55be3-139">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="55be3-139">notApplicableCount</span></span>|<span data-ttu-id="55be3-140">Int32</span><span class="sxs-lookup"><span data-stu-id="55be3-140">Int32</span></span>|<span data-ttu-id="55be3-141">Número de dispositivos não aplicáveis</span><span class="sxs-lookup"><span data-stu-id="55be3-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="55be3-142">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="55be3-142">notApplicablePlatformCount</span></span>|<span data-ttu-id="55be3-143">Int32</span><span class="sxs-lookup"><span data-stu-id="55be3-143">Int32</span></span>|<span data-ttu-id="55be3-144">Número de dispositivos não aplicáveis devido à plataforma e à política incompatíveis</span><span class="sxs-lookup"><span data-stu-id="55be3-144">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="55be3-145">successCount</span><span class="sxs-lookup"><span data-stu-id="55be3-145">successCount</span></span>|<span data-ttu-id="55be3-146">Int32</span><span class="sxs-lookup"><span data-stu-id="55be3-146">Int32</span></span>|<span data-ttu-id="55be3-147">Número de dispositivos com êxito</span><span class="sxs-lookup"><span data-stu-id="55be3-147">Number of succeeded devices</span></span>|
|<span data-ttu-id="55be3-148">errorCount</span><span class="sxs-lookup"><span data-stu-id="55be3-148">errorCount</span></span>|<span data-ttu-id="55be3-149">Int32</span><span class="sxs-lookup"><span data-stu-id="55be3-149">Int32</span></span>|<span data-ttu-id="55be3-150">Número de dispositivos com erro</span><span class="sxs-lookup"><span data-stu-id="55be3-150">Number of error devices</span></span>|
|<span data-ttu-id="55be3-151">failedCount</span><span class="sxs-lookup"><span data-stu-id="55be3-151">failedCount</span></span>|<span data-ttu-id="55be3-152">Int32</span><span class="sxs-lookup"><span data-stu-id="55be3-152">Int32</span></span>|<span data-ttu-id="55be3-153">Número de dispositivos com falha</span><span class="sxs-lookup"><span data-stu-id="55be3-153">Number of failed devices</span></span>|
|<span data-ttu-id="55be3-154">conflictCount</span><span class="sxs-lookup"><span data-stu-id="55be3-154">conflictCount</span></span>|<span data-ttu-id="55be3-155">Int32</span><span class="sxs-lookup"><span data-stu-id="55be3-155">Int32</span></span>|<span data-ttu-id="55be3-156">Número de dispositivos em conflito</span><span class="sxs-lookup"><span data-stu-id="55be3-156">Number of devices in conflict</span></span>|
|<span data-ttu-id="55be3-157">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="55be3-157">lastUpdateDateTime</span></span>|<span data-ttu-id="55be3-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55be3-158">DateTimeOffset</span></span>|<span data-ttu-id="55be3-159">Hora da última atualização</span><span class="sxs-lookup"><span data-stu-id="55be3-159">Last update time</span></span>|
|<span data-ttu-id="55be3-160">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="55be3-160">configurationVersion</span></span>|<span data-ttu-id="55be3-161">Int32</span><span class="sxs-lookup"><span data-stu-id="55be3-161">Int32</span></span>|<span data-ttu-id="55be3-162">Versão da política para essa visão geral</span><span class="sxs-lookup"><span data-stu-id="55be3-162">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="55be3-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="55be3-163">Response</span></span>
<span data-ttu-id="55be3-164">Se tiver êxito, este método retornará um código de resposta `200 OK` e o objeto [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55be3-164">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55be3-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="55be3-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="55be3-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55be3-166">Request</span></span>
<span data-ttu-id="55be3-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55be3-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="55be3-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="55be3-168">Response</span></span>
<span data-ttu-id="55be3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="55be3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



