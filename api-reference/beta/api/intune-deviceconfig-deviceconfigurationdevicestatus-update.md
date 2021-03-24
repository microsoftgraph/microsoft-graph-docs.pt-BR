---
title: Atualizar deviceConfigurationDeviceStatus
description: Atualizar as propriedades de um objeto deviceConfigurationDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ec35af9bf43501a41716e757343f61531d776508
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128065"
---
# <a name="update-deviceconfigurationdevicestatus"></a><span data-ttu-id="b5483-103">Atualizar deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="b5483-103">Update deviceConfigurationDeviceStatus</span></span>

<span data-ttu-id="b5483-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5483-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b5483-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b5483-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5483-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b5483-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5483-107">Atualizar as propriedades de um objeto [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="b5483-107">Update the properties of a [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b5483-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b5483-108">Prerequisites</span></span>
<span data-ttu-id="b5483-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5483-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5483-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b5483-111">Permission type</span></span>|<span data-ttu-id="b5483-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b5483-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5483-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b5483-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b5483-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5483-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b5483-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b5483-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5483-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b5483-116">Not supported.</span></span>|
|<span data-ttu-id="b5483-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b5483-117">Application</span></span>|<span data-ttu-id="b5483-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5483-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5483-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b5483-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="b5483-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b5483-120">Request headers</span></span>
|<span data-ttu-id="b5483-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b5483-121">Header</span></span>|<span data-ttu-id="b5483-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b5483-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5483-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b5483-123">Authorization</span></span>|<span data-ttu-id="b5483-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b5483-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5483-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b5483-125">Accept</span></span>|<span data-ttu-id="b5483-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b5483-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5483-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b5483-127">Request body</span></span>
<span data-ttu-id="b5483-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="b5483-128">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="b5483-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="b5483-129">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="b5483-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b5483-130">Property</span></span>|<span data-ttu-id="b5483-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5483-131">Type</span></span>|<span data-ttu-id="b5483-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5483-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5483-133">id</span><span class="sxs-lookup"><span data-stu-id="b5483-133">id</span></span>|<span data-ttu-id="b5483-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5483-134">String</span></span>|<span data-ttu-id="b5483-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b5483-135">Key of the entity.</span></span>|
|<span data-ttu-id="b5483-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="b5483-136">deviceDisplayName</span></span>|<span data-ttu-id="b5483-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5483-137">String</span></span>|<span data-ttu-id="b5483-138">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="b5483-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="b5483-139">userName</span><span class="sxs-lookup"><span data-stu-id="b5483-139">userName</span></span>|<span data-ttu-id="b5483-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5483-140">String</span></span>|<span data-ttu-id="b5483-141">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="b5483-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="b5483-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="b5483-142">deviceModel</span></span>|<span data-ttu-id="b5483-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5483-143">String</span></span>|<span data-ttu-id="b5483-144">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="b5483-144">The device model that is being reported</span></span>|
|<span data-ttu-id="b5483-145">plataforma</span><span class="sxs-lookup"><span data-stu-id="b5483-145">platform</span></span>|<span data-ttu-id="b5483-146">Int32</span><span class="sxs-lookup"><span data-stu-id="b5483-146">Int32</span></span>|<span data-ttu-id="b5483-147">Plataforma do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="b5483-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="b5483-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b5483-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="b5483-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5483-149">DateTimeOffset</span></span>|<span data-ttu-id="b5483-150">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="b5483-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="b5483-151">status</span><span class="sxs-lookup"><span data-stu-id="b5483-151">status</span></span>|[<span data-ttu-id="b5483-152">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="b5483-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="b5483-153">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="b5483-153">Compliance status of the policy report.</span></span> <span data-ttu-id="b5483-154">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="b5483-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="b5483-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="b5483-155">lastReportedDateTime</span></span>|<span data-ttu-id="b5483-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5483-156">DateTimeOffset</span></span>|<span data-ttu-id="b5483-157">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="b5483-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="b5483-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b5483-158">userPrincipalName</span></span>|<span data-ttu-id="b5483-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b5483-159">String</span></span>|<span data-ttu-id="b5483-160">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="b5483-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="b5483-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5483-161">Response</span></span>
<span data-ttu-id="b5483-162">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b5483-162">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5483-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b5483-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5483-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b5483-164">Request</span></span>
<span data-ttu-id="b5483-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b5483-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b5483-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="b5483-166">Response</span></span>
<span data-ttu-id="b5483-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b5483-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




