---
title: Atualizar managedDeviceMobileAppConfigurationDeviceStatus
description: Atualize as propriedades de um objeto managedDeviceMobileAppConfigurationDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2551684b76de5f9a6f74c68f662a6c19db98b141
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759858"
---
# <a name="update-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="237b4-103">Atualizar managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="237b4-103">Update managedDeviceMobileAppConfigurationDeviceStatus</span></span>

<span data-ttu-id="237b4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="237b4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="237b4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="237b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="237b4-106">Atualize as propriedades de [um objeto managedDeviceMobileAppConfigurationDeviceStatus.](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="237b4-106">Update the properties of a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="237b4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="237b4-107">Prerequisites</span></span>
<span data-ttu-id="237b4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="237b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="237b4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="237b4-110">Permission type</span></span>|<span data-ttu-id="237b4-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="237b4-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="237b4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="237b4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="237b4-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="237b4-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="237b4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="237b4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="237b4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="237b4-115">Not supported.</span></span>|
|<span data-ttu-id="237b4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="237b4-116">Application</span></span>|<span data-ttu-id="237b4-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="237b4-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="237b4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="237b4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="237b4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="237b4-119">Request headers</span></span>
|<span data-ttu-id="237b4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="237b4-120">Header</span></span>|<span data-ttu-id="237b4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="237b4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="237b4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="237b4-122">Authorization</span></span>|<span data-ttu-id="237b4-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="237b4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="237b4-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="237b4-124">Accept</span></span>|<span data-ttu-id="237b4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="237b4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="237b4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="237b4-126">Request body</span></span>
<span data-ttu-id="237b4-127">No corpo da solicitação, fornece uma representação JSON para o [objeto managedDeviceMobileAppConfigurationDeviceStatus.](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)</span><span class="sxs-lookup"><span data-stu-id="237b4-127">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

<span data-ttu-id="237b4-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="237b4-128">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span></span>

|<span data-ttu-id="237b4-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="237b4-129">Property</span></span>|<span data-ttu-id="237b4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="237b4-130">Type</span></span>|<span data-ttu-id="237b4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="237b4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="237b4-132">id</span><span class="sxs-lookup"><span data-stu-id="237b4-132">id</span></span>|<span data-ttu-id="237b4-133">String</span><span class="sxs-lookup"><span data-stu-id="237b4-133">String</span></span>|<span data-ttu-id="237b4-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="237b4-134">Key of the entity.</span></span>|
|<span data-ttu-id="237b4-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="237b4-135">deviceDisplayName</span></span>|<span data-ttu-id="237b4-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="237b4-136">String</span></span>|<span data-ttu-id="237b4-137">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="237b4-137">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="237b4-138">userName</span><span class="sxs-lookup"><span data-stu-id="237b4-138">userName</span></span>|<span data-ttu-id="237b4-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="237b4-139">String</span></span>|<span data-ttu-id="237b4-140">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="237b4-140">The User Name that is being reported</span></span>|
|<span data-ttu-id="237b4-141">deviceModel</span><span class="sxs-lookup"><span data-stu-id="237b4-141">deviceModel</span></span>|<span data-ttu-id="237b4-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="237b4-142">String</span></span>|<span data-ttu-id="237b4-143">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="237b4-143">The device model that is being reported</span></span>|
|<span data-ttu-id="237b4-144">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="237b4-144">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="237b4-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="237b4-145">DateTimeOffset</span></span>|<span data-ttu-id="237b4-146">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="237b4-146">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="237b4-147">status</span><span class="sxs-lookup"><span data-stu-id="237b4-147">status</span></span>|[<span data-ttu-id="237b4-148">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="237b4-148">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="237b4-149">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="237b4-149">Compliance status of the policy report.</span></span> <span data-ttu-id="237b4-150">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="237b4-150">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="237b4-151">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="237b4-151">lastReportedDateTime</span></span>|<span data-ttu-id="237b4-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="237b4-152">DateTimeOffset</span></span>|<span data-ttu-id="237b4-153">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="237b4-153">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="237b4-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="237b4-154">userPrincipalName</span></span>|<span data-ttu-id="237b4-155">String</span><span class="sxs-lookup"><span data-stu-id="237b4-155">String</span></span>|<span data-ttu-id="237b4-156">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="237b4-156">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="237b4-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="237b4-157">Response</span></span>
<span data-ttu-id="237b4-158">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="237b4-158">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="237b4-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="237b4-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="237b4-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="237b4-160">Request</span></span>
<span data-ttu-id="237b4-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="237b4-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
Content-type: application/json
Content-length: 445

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="237b4-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="237b4-162">Response</span></span>
<span data-ttu-id="237b4-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="237b4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 494

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "id": "477d3651-3651-477d-5136-7d4751367d47",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```




