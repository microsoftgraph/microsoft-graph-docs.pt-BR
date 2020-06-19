---
title: Criar deviceConfigurationDeviceStatus
description: Criar um novo objeto deviceConfigurationDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 76fd149dd1116079d636808b46af1e614416799f
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792951"
---
# <a name="create-deviceconfigurationdevicestatus"></a><span data-ttu-id="9a38a-103">Criar deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="9a38a-103">Create deviceConfigurationDeviceStatus</span></span>

<span data-ttu-id="9a38a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a38a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9a38a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9a38a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a38a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9a38a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a38a-107">Criar um novo objeto [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="9a38a-107">Create a new [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9a38a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9a38a-108">Prerequisites</span></span>
<span data-ttu-id="9a38a-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="9a38a-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="9a38a-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a38a-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a38a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a38a-111">Permission type</span></span>|<span data-ttu-id="9a38a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9a38a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a38a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a38a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9a38a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a38a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9a38a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a38a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a38a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9a38a-116">Not supported.</span></span>|
|<span data-ttu-id="9a38a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a38a-117">Application</span></span>|<span data-ttu-id="9a38a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a38a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a38a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a38a-119">HTTP Request</span></span>
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
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidDeviceOwnerEnterpriseWiFiConfiguration/identityCertificateForClientAuthentication/deviceStatuses
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="9a38a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a38a-120">Request headers</span></span>
|<span data-ttu-id="9a38a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9a38a-121">Header</span></span>|<span data-ttu-id="9a38a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9a38a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a38a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a38a-123">Authorization</span></span>|<span data-ttu-id="9a38a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a38a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a38a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9a38a-125">Accept</span></span>|<span data-ttu-id="9a38a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9a38a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a38a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a38a-127">Request body</span></span>
<span data-ttu-id="9a38a-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="9a38a-128">In the request body, supply a JSON representation for the deviceConfigurationDeviceStatus object.</span></span>

<span data-ttu-id="9a38a-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceConfigurationDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="9a38a-129">The following table shows the properties that are required when you create the deviceConfigurationDeviceStatus.</span></span>

|<span data-ttu-id="9a38a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a38a-130">Property</span></span>|<span data-ttu-id="9a38a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a38a-131">Type</span></span>|<span data-ttu-id="9a38a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a38a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a38a-133">id</span><span class="sxs-lookup"><span data-stu-id="9a38a-133">id</span></span>|<span data-ttu-id="9a38a-134">String</span><span class="sxs-lookup"><span data-stu-id="9a38a-134">String</span></span>|<span data-ttu-id="9a38a-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9a38a-135">Key of the entity.</span></span>|
|<span data-ttu-id="9a38a-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="9a38a-136">deviceDisplayName</span></span>|<span data-ttu-id="9a38a-137">String</span><span class="sxs-lookup"><span data-stu-id="9a38a-137">String</span></span>|<span data-ttu-id="9a38a-138">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="9a38a-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="9a38a-139">userName</span><span class="sxs-lookup"><span data-stu-id="9a38a-139">userName</span></span>|<span data-ttu-id="9a38a-140">String</span><span class="sxs-lookup"><span data-stu-id="9a38a-140">String</span></span>|<span data-ttu-id="9a38a-141">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="9a38a-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="9a38a-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="9a38a-142">deviceModel</span></span>|<span data-ttu-id="9a38a-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a38a-143">String</span></span>|<span data-ttu-id="9a38a-144">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="9a38a-144">The device model that is being reported</span></span>|
|<span data-ttu-id="9a38a-145">platform</span><span class="sxs-lookup"><span data-stu-id="9a38a-145">platform</span></span>|<span data-ttu-id="9a38a-146">Int32</span><span class="sxs-lookup"><span data-stu-id="9a38a-146">Int32</span></span>|<span data-ttu-id="9a38a-147">Plataforma do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="9a38a-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="9a38a-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="9a38a-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="9a38a-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a38a-149">DateTimeOffset</span></span>|<span data-ttu-id="9a38a-150">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="9a38a-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="9a38a-151">status</span><span class="sxs-lookup"><span data-stu-id="9a38a-151">status</span></span>|[<span data-ttu-id="9a38a-152">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="9a38a-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="9a38a-153">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="9a38a-153">Compliance status of the policy report.</span></span> <span data-ttu-id="9a38a-154">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="9a38a-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="9a38a-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="9a38a-155">lastReportedDateTime</span></span>|<span data-ttu-id="9a38a-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a38a-156">DateTimeOffset</span></span>|<span data-ttu-id="9a38a-157">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="9a38a-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="9a38a-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9a38a-158">userPrincipalName</span></span>|<span data-ttu-id="9a38a-159">String</span><span class="sxs-lookup"><span data-stu-id="9a38a-159">String</span></span>|<span data-ttu-id="9a38a-160">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="9a38a-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="9a38a-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a38a-161">Response</span></span>
<span data-ttu-id="9a38a-162">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a38a-162">If successful, this method returns a `201 Created` response code and a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a38a-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9a38a-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a38a-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a38a-164">Request</span></span>
<span data-ttu-id="9a38a-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a38a-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9a38a-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a38a-166">Response</span></span>
<span data-ttu-id="9a38a-167">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="9a38a-167">Here is an example of the response.</span></span> <span data-ttu-id="9a38a-168">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="9a38a-168">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9a38a-169">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="9a38a-169">All of the properties will be returned from an actual call.</span></span>
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



