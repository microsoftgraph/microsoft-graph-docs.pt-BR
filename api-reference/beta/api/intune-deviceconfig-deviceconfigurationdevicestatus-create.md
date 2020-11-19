---
title: Criar deviceConfigurationDeviceStatus
description: Criar um novo objeto deviceConfigurationDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f70c43d319308d0dce58c0beb6f547e338f68ed9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49291607"
---
# <a name="create-deviceconfigurationdevicestatus"></a><span data-ttu-id="21b86-103">Criar deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="21b86-103">Create deviceConfigurationDeviceStatus</span></span>

<span data-ttu-id="21b86-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21b86-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="21b86-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="21b86-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21b86-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="21b86-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21b86-107">Criar um novo objeto [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="21b86-107">Create a new [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21b86-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="21b86-108">Prerequisites</span></span>
<span data-ttu-id="21b86-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21b86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21b86-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21b86-111">Permission type</span></span>|<span data-ttu-id="21b86-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="21b86-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21b86-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21b86-113">Delegated (work or school account)</span></span>|<span data-ttu-id="21b86-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21b86-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="21b86-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21b86-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21b86-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21b86-116">Not supported.</span></span>|
|<span data-ttu-id="21b86-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="21b86-117">Application</span></span>|<span data-ttu-id="21b86-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21b86-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="21b86-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21b86-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/rootCertificateForServerValidation/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSWiredNetworkConfiguration/identityCertificateForClientAuthentication/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="21b86-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21b86-120">Request headers</span></span>
|<span data-ttu-id="21b86-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="21b86-121">Header</span></span>|<span data-ttu-id="21b86-122">Valor</span><span class="sxs-lookup"><span data-stu-id="21b86-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21b86-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="21b86-123">Authorization</span></span>|<span data-ttu-id="21b86-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21b86-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21b86-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="21b86-125">Accept</span></span>|<span data-ttu-id="21b86-126">application/json</span><span class="sxs-lookup"><span data-stu-id="21b86-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21b86-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21b86-127">Request body</span></span>
<span data-ttu-id="21b86-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="21b86-128">In the request body, supply a JSON representation for the deviceConfigurationDeviceStatus object.</span></span>

<span data-ttu-id="21b86-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="21b86-129">The following table shows the properties that are required when you create the deviceConfigurationDeviceStatus.</span></span>

|<span data-ttu-id="21b86-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21b86-130">Property</span></span>|<span data-ttu-id="21b86-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="21b86-131">Type</span></span>|<span data-ttu-id="21b86-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="21b86-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21b86-133">id</span><span class="sxs-lookup"><span data-stu-id="21b86-133">id</span></span>|<span data-ttu-id="21b86-134">String</span><span class="sxs-lookup"><span data-stu-id="21b86-134">String</span></span>|<span data-ttu-id="21b86-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="21b86-135">Key of the entity.</span></span>|
|<span data-ttu-id="21b86-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="21b86-136">deviceDisplayName</span></span>|<span data-ttu-id="21b86-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="21b86-137">String</span></span>|<span data-ttu-id="21b86-138">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="21b86-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="21b86-139">userName</span><span class="sxs-lookup"><span data-stu-id="21b86-139">userName</span></span>|<span data-ttu-id="21b86-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="21b86-140">String</span></span>|<span data-ttu-id="21b86-141">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="21b86-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="21b86-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="21b86-142">deviceModel</span></span>|<span data-ttu-id="21b86-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="21b86-143">String</span></span>|<span data-ttu-id="21b86-144">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="21b86-144">The device model that is being reported</span></span>|
|<span data-ttu-id="21b86-145">plataforma</span><span class="sxs-lookup"><span data-stu-id="21b86-145">platform</span></span>|<span data-ttu-id="21b86-146">Int32</span><span class="sxs-lookup"><span data-stu-id="21b86-146">Int32</span></span>|<span data-ttu-id="21b86-147">Plataforma do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="21b86-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="21b86-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="21b86-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="21b86-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21b86-149">DateTimeOffset</span></span>|<span data-ttu-id="21b86-150">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="21b86-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="21b86-151">status</span><span class="sxs-lookup"><span data-stu-id="21b86-151">status</span></span>|[<span data-ttu-id="21b86-152">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="21b86-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="21b86-153">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="21b86-153">Compliance status of the policy report.</span></span> <span data-ttu-id="21b86-154">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="21b86-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="21b86-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="21b86-155">lastReportedDateTime</span></span>|<span data-ttu-id="21b86-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21b86-156">DateTimeOffset</span></span>|<span data-ttu-id="21b86-157">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="21b86-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="21b86-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="21b86-158">userPrincipalName</span></span>|<span data-ttu-id="21b86-159">String</span><span class="sxs-lookup"><span data-stu-id="21b86-159">String</span></span>|<span data-ttu-id="21b86-160">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="21b86-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="21b86-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="21b86-161">Response</span></span>
<span data-ttu-id="21b86-162">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21b86-162">If successful, this method returns a `201 Created` response code and a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21b86-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="21b86-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="21b86-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21b86-164">Request</span></span>
<span data-ttu-id="21b86-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="21b86-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
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

### <a name="response"></a><span data-ttu-id="21b86-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="21b86-166">Response</span></span>
<span data-ttu-id="21b86-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="21b86-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




