---
title: Atualizar deviceComplianceDeviceStatus
description: Atualizar as propriedades de um objeto deviceComplianceDeviceStatus.
author: tfitzmac
ms.openlocfilehash: 5f894c325e6f7732cb41b7472e85e3dbb8361e3b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343677"
---
# <a name="update-devicecompliancedevicestatus"></a><span data-ttu-id="98156-103">Atualizar deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="98156-103">Update deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="98156-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="98156-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="98156-105">Atualizar as propriedades de um objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="98156-105">Update the properties of a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="98156-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="98156-106">Prerequisites</span></span>
<span data-ttu-id="98156-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98156-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98156-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="98156-109">Permission type</span></span>|<span data-ttu-id="98156-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="98156-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98156-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="98156-111">Delegated (work or school account)</span></span>|<span data-ttu-id="98156-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98156-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="98156-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="98156-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98156-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98156-114">Not supported.</span></span>|
|<span data-ttu-id="98156-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="98156-115">Application</span></span>|<span data-ttu-id="98156-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98156-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="98156-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="98156-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="98156-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="98156-118">Request headers</span></span>
|<span data-ttu-id="98156-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="98156-119">Header</span></span>|<span data-ttu-id="98156-120">Valor</span><span class="sxs-lookup"><span data-stu-id="98156-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98156-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="98156-121">Authorization</span></span>|<span data-ttu-id="98156-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98156-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98156-123">Accept</span><span class="sxs-lookup"><span data-stu-id="98156-123">Accept</span></span>|<span data-ttu-id="98156-124">application/json</span><span class="sxs-lookup"><span data-stu-id="98156-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98156-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="98156-125">Request body</span></span>
<span data-ttu-id="98156-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="98156-126">In the request body, supply a JSON representation for the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

<span data-ttu-id="98156-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="98156-127">The following table shows the properties that are required when you create the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span></span>

|<span data-ttu-id="98156-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="98156-128">Property</span></span>|<span data-ttu-id="98156-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="98156-129">Type</span></span>|<span data-ttu-id="98156-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="98156-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98156-131">id</span><span class="sxs-lookup"><span data-stu-id="98156-131">id</span></span>|<span data-ttu-id="98156-132">String</span><span class="sxs-lookup"><span data-stu-id="98156-132">String</span></span>|<span data-ttu-id="98156-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="98156-133">Key of the entity.</span></span>|
|<span data-ttu-id="98156-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="98156-134">deviceDisplayName</span></span>|<span data-ttu-id="98156-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="98156-135">String</span></span>|<span data-ttu-id="98156-136">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="98156-136">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="98156-137">userName</span><span class="sxs-lookup"><span data-stu-id="98156-137">userName</span></span>|<span data-ttu-id="98156-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="98156-138">String</span></span>|<span data-ttu-id="98156-139">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="98156-139">The User Name that is being reported</span></span>|
|<span data-ttu-id="98156-140">deviceModel</span><span class="sxs-lookup"><span data-stu-id="98156-140">deviceModel</span></span>|<span data-ttu-id="98156-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="98156-141">String</span></span>|<span data-ttu-id="98156-142">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="98156-142">The device model that is being reported</span></span>|
|<span data-ttu-id="98156-143">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="98156-143">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="98156-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98156-144">DateTimeOffset</span></span>|<span data-ttu-id="98156-145">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="98156-145">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="98156-146">status</span><span class="sxs-lookup"><span data-stu-id="98156-146">status</span></span>|[<span data-ttu-id="98156-147">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="98156-147">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="98156-148">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="98156-148">Compliance status of the policy report.</span></span> <span data-ttu-id="98156-149">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="98156-149">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="98156-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="98156-150">lastReportedDateTime</span></span>|<span data-ttu-id="98156-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98156-151">DateTimeOffset</span></span>|<span data-ttu-id="98156-152">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="98156-152">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="98156-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="98156-153">userPrincipalName</span></span>|<span data-ttu-id="98156-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="98156-154">String</span></span>|<span data-ttu-id="98156-155">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="98156-155">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="98156-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="98156-156">Response</span></span>
<span data-ttu-id="98156-157">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="98156-157">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98156-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="98156-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="98156-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="98156-159">Request</span></span>
<span data-ttu-id="98156-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="98156-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
Content-type: application/json
Content-length: 426

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="98156-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="98156-161">Response</span></span>
<span data-ttu-id="98156-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="98156-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 475

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "id": "c6c78124-8124-c6c7-2481-c7c62481c7c6",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



