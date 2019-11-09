---
title: Atualizar deviceConfigurationDeviceStatus
description: Atualizar as propriedades de um objeto deviceConfigurationDeviceStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 166d7ce4e61e64e1a4b7180a5774fe1dfd86335e
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38084472"
---
# <a name="update-deviceconfigurationdevicestatus"></a><span data-ttu-id="6a49e-103">Atualizar deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="6a49e-103">Update deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="6a49e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6a49e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a49e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6a49e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a49e-106">Atualizar as propriedades de um objeto [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="6a49e-106">Update the properties of a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a49e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6a49e-107">Prerequisites</span></span>
<span data-ttu-id="6a49e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a49e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a49e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6a49e-110">Permission type</span></span>|<span data-ttu-id="6a49e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6a49e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a49e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6a49e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6a49e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a49e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6a49e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6a49e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a49e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6a49e-115">Not supported.</span></span>|
|<span data-ttu-id="6a49e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6a49e-116">Application</span></span>|<span data-ttu-id="6a49e-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a49e-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a49e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6a49e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatuses/{deviceConfigurationDeviceStatusId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="6a49e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6a49e-119">Request headers</span></span>
|<span data-ttu-id="6a49e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6a49e-120">Header</span></span>|<span data-ttu-id="6a49e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6a49e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a49e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6a49e-122">Authorization</span></span>|<span data-ttu-id="6a49e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6a49e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a49e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6a49e-124">Accept</span></span>|<span data-ttu-id="6a49e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6a49e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a49e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6a49e-126">Request body</span></span>
<span data-ttu-id="6a49e-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="6a49e-127">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="6a49e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="6a49e-128">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="6a49e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a49e-129">Property</span></span>|<span data-ttu-id="6a49e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a49e-130">Type</span></span>|<span data-ttu-id="6a49e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a49e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a49e-132">id</span><span class="sxs-lookup"><span data-stu-id="6a49e-132">id</span></span>|<span data-ttu-id="6a49e-133">String</span><span class="sxs-lookup"><span data-stu-id="6a49e-133">String</span></span>|<span data-ttu-id="6a49e-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6a49e-134">Key of the entity.</span></span>|
|<span data-ttu-id="6a49e-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="6a49e-135">deviceDisplayName</span></span>|<span data-ttu-id="6a49e-136">String</span><span class="sxs-lookup"><span data-stu-id="6a49e-136">String</span></span>|<span data-ttu-id="6a49e-137">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="6a49e-137">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="6a49e-138">userName</span><span class="sxs-lookup"><span data-stu-id="6a49e-138">userName</span></span>|<span data-ttu-id="6a49e-139">String</span><span class="sxs-lookup"><span data-stu-id="6a49e-139">String</span></span>|<span data-ttu-id="6a49e-140">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="6a49e-140">The User Name that is being reported</span></span>|
|<span data-ttu-id="6a49e-141">deviceModel</span><span class="sxs-lookup"><span data-stu-id="6a49e-141">deviceModel</span></span>|<span data-ttu-id="6a49e-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a49e-142">String</span></span>|<span data-ttu-id="6a49e-143">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="6a49e-143">The device model that is being reported</span></span>|
|<span data-ttu-id="6a49e-144">platform</span><span class="sxs-lookup"><span data-stu-id="6a49e-144">platform</span></span>|<span data-ttu-id="6a49e-145">Int32</span><span class="sxs-lookup"><span data-stu-id="6a49e-145">Int32</span></span>|<span data-ttu-id="6a49e-146">Plataforma do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="6a49e-146">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="6a49e-147">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="6a49e-147">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="6a49e-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a49e-148">DateTimeOffset</span></span>|<span data-ttu-id="6a49e-149">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="6a49e-149">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="6a49e-150">status</span><span class="sxs-lookup"><span data-stu-id="6a49e-150">status</span></span>|[<span data-ttu-id="6a49e-151">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="6a49e-151">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="6a49e-152">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="6a49e-152">Compliance status of the policy report.</span></span> <span data-ttu-id="6a49e-153">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="6a49e-153">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="6a49e-154">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a49e-154">lastReportedDateTime</span></span>|<span data-ttu-id="6a49e-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a49e-155">DateTimeOffset</span></span>|<span data-ttu-id="6a49e-156">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="6a49e-156">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="6a49e-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6a49e-157">userPrincipalName</span></span>|<span data-ttu-id="6a49e-158">String</span><span class="sxs-lookup"><span data-stu-id="6a49e-158">String</span></span>|<span data-ttu-id="6a49e-159">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="6a49e-159">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="6a49e-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a49e-160">Response</span></span>
<span data-ttu-id="6a49e-161">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6a49e-161">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a49e-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6a49e-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a49e-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6a49e-163">Request</span></span>
<span data-ttu-id="6a49e-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a49e-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
Content-type: application/json
Content-length: 447

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="6a49e-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="6a49e-165">Response</span></span>
<span data-ttu-id="6a49e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6a49e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 496

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "id": "674e98e5-98e5-674e-e598-4e67e5984e67",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "platform": 8,
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```






