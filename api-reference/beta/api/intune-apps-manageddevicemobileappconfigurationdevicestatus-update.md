---
title: Atualizar managedDeviceMobileAppConfigurationDeviceStatus
description: Atualize as propriedades de um objeto managedDeviceMobileAppConfigurationDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f9986e295404b5acca50be7cd8ec6809a5a153bd
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51143588"
---
# <a name="update-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="bad87-103">Atualizar managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="bad87-103">Update managedDeviceMobileAppConfigurationDeviceStatus</span></span>

<span data-ttu-id="bad87-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bad87-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bad87-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bad87-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bad87-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bad87-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bad87-107">Atualize as propriedades de [um objeto managedDeviceMobileAppConfigurationDeviceStatus.](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="bad87-107">Update the properties of a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bad87-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bad87-108">Prerequisites</span></span>
<span data-ttu-id="bad87-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bad87-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bad87-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bad87-111">Permission type</span></span>|<span data-ttu-id="bad87-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bad87-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bad87-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bad87-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bad87-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bad87-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bad87-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bad87-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bad87-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bad87-116">Not supported.</span></span>|
|<span data-ttu-id="bad87-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bad87-117">Application</span></span>|<span data-ttu-id="bad87-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bad87-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bad87-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bad87-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="bad87-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bad87-120">Request headers</span></span>
|<span data-ttu-id="bad87-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bad87-121">Header</span></span>|<span data-ttu-id="bad87-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bad87-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bad87-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bad87-123">Authorization</span></span>|<span data-ttu-id="bad87-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bad87-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bad87-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bad87-125">Accept</span></span>|<span data-ttu-id="bad87-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bad87-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bad87-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bad87-127">Request body</span></span>
<span data-ttu-id="bad87-128">No corpo da solicitação, fornece uma representação JSON para o [objeto managedDeviceMobileAppConfigurationDeviceStatus.](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="bad87-128">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="bad87-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="bad87-129">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="bad87-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bad87-130">Property</span></span>|<span data-ttu-id="bad87-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="bad87-131">Type</span></span>|<span data-ttu-id="bad87-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="bad87-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bad87-133">id</span><span class="sxs-lookup"><span data-stu-id="bad87-133">id</span></span>|<span data-ttu-id="bad87-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bad87-134">String</span></span>|<span data-ttu-id="bad87-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bad87-135">Key of the entity.</span></span>|
|<span data-ttu-id="bad87-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="bad87-136">deviceDisplayName</span></span>|<span data-ttu-id="bad87-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bad87-137">String</span></span>|<span data-ttu-id="bad87-138">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="bad87-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="bad87-139">userName</span><span class="sxs-lookup"><span data-stu-id="bad87-139">userName</span></span>|<span data-ttu-id="bad87-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bad87-140">String</span></span>|<span data-ttu-id="bad87-141">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="bad87-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="bad87-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="bad87-142">deviceModel</span></span>|<span data-ttu-id="bad87-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bad87-143">String</span></span>|<span data-ttu-id="bad87-144">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="bad87-144">The device model that is being reported</span></span>|
|<span data-ttu-id="bad87-145">plataforma</span><span class="sxs-lookup"><span data-stu-id="bad87-145">platform</span></span>|<span data-ttu-id="bad87-146">Int32</span><span class="sxs-lookup"><span data-stu-id="bad87-146">Int32</span></span>|<span data-ttu-id="bad87-147">Plataforma do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="bad87-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="bad87-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="bad87-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="bad87-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bad87-149">DateTimeOffset</span></span>|<span data-ttu-id="bad87-150">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="bad87-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="bad87-151">status</span><span class="sxs-lookup"><span data-stu-id="bad87-151">status</span></span>|[<span data-ttu-id="bad87-152">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="bad87-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="bad87-153">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="bad87-153">Compliance status of the policy report.</span></span> <span data-ttu-id="bad87-154">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="bad87-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="bad87-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="bad87-155">lastReportedDateTime</span></span>|<span data-ttu-id="bad87-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bad87-156">DateTimeOffset</span></span>|<span data-ttu-id="bad87-157">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="bad87-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="bad87-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bad87-158">userPrincipalName</span></span>|<span data-ttu-id="bad87-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bad87-159">String</span></span>|<span data-ttu-id="bad87-160">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="bad87-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="bad87-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="bad87-161">Response</span></span>
<span data-ttu-id="bad87-162">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bad87-162">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bad87-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bad87-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="bad87-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bad87-164">Request</span></span>
<span data-ttu-id="bad87-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bad87-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
Content-type: application/json
Content-length: 463

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
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

### <a name="response"></a><span data-ttu-id="bad87-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="bad87-166">Response</span></span>
<span data-ttu-id="bad87-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bad87-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 512

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "id": "477d3651-3651-477d-5136-7d4751367d47",
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




