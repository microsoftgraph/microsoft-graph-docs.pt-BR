---
title: Atualizar deviceComplianceDeviceStatus
description: Atualizar as propriedades de um objeto deviceComplianceDeviceStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2e5d2c9712351ad51bf53a06e9a9da17ab5e3159
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34968487"
---
# <a name="update-devicecompliancedevicestatus"></a><span data-ttu-id="a5a89-103">Atualizar deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="a5a89-103">Update deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="a5a89-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a5a89-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a5a89-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a5a89-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5a89-106">Atualizar as propriedades de um objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="a5a89-106">Update the properties of a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a5a89-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a5a89-107">Prerequisites</span></span>
<span data-ttu-id="a5a89-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5a89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5a89-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5a89-110">Permission type</span></span>|<span data-ttu-id="a5a89-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a5a89-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5a89-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5a89-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a5a89-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5a89-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a5a89-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5a89-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5a89-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5a89-115">Not supported.</span></span>|
|<span data-ttu-id="a5a89-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a5a89-116">Application</span></span>|<span data-ttu-id="a5a89-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5a89-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5a89-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5a89-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="a5a89-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5a89-119">Request headers</span></span>
|<span data-ttu-id="a5a89-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a5a89-120">Header</span></span>|<span data-ttu-id="a5a89-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a5a89-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5a89-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a5a89-122">Authorization</span></span>|<span data-ttu-id="a5a89-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5a89-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5a89-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a5a89-124">Accept</span></span>|<span data-ttu-id="a5a89-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a5a89-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5a89-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5a89-126">Request body</span></span>
<span data-ttu-id="a5a89-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="a5a89-127">In the request body, supply a JSON representation for the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

<span data-ttu-id="a5a89-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="a5a89-128">The following table shows the properties that are required when you create the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span></span>

|<span data-ttu-id="a5a89-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a5a89-129">Property</span></span>|<span data-ttu-id="a5a89-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5a89-130">Type</span></span>|<span data-ttu-id="a5a89-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5a89-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5a89-132">id</span><span class="sxs-lookup"><span data-stu-id="a5a89-132">id</span></span>|<span data-ttu-id="a5a89-133">String</span><span class="sxs-lookup"><span data-stu-id="a5a89-133">String</span></span>|<span data-ttu-id="a5a89-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a5a89-134">Key of the entity.</span></span>|
|<span data-ttu-id="a5a89-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="a5a89-135">deviceDisplayName</span></span>|<span data-ttu-id="a5a89-136">String</span><span class="sxs-lookup"><span data-stu-id="a5a89-136">String</span></span>|<span data-ttu-id="a5a89-137">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="a5a89-137">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="a5a89-138">userName</span><span class="sxs-lookup"><span data-stu-id="a5a89-138">userName</span></span>|<span data-ttu-id="a5a89-139">String</span><span class="sxs-lookup"><span data-stu-id="a5a89-139">String</span></span>|<span data-ttu-id="a5a89-140">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="a5a89-140">The User Name that is being reported</span></span>|
|<span data-ttu-id="a5a89-141">deviceModel</span><span class="sxs-lookup"><span data-stu-id="a5a89-141">deviceModel</span></span>|<span data-ttu-id="a5a89-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a5a89-142">String</span></span>|<span data-ttu-id="a5a89-143">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="a5a89-143">The device model that is being reported</span></span>|
|<span data-ttu-id="a5a89-144">platform</span><span class="sxs-lookup"><span data-stu-id="a5a89-144">platform</span></span>|<span data-ttu-id="a5a89-145">Int32</span><span class="sxs-lookup"><span data-stu-id="a5a89-145">Int32</span></span>|<span data-ttu-id="a5a89-146">Plataforma do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="a5a89-146">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="a5a89-147">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a5a89-147">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="a5a89-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5a89-148">DateTimeOffset</span></span>|<span data-ttu-id="a5a89-149">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="a5a89-149">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="a5a89-150">status</span><span class="sxs-lookup"><span data-stu-id="a5a89-150">status</span></span>|[<span data-ttu-id="a5a89-151">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="a5a89-151">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="a5a89-152">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="a5a89-152">Compliance status of the policy report.</span></span> <span data-ttu-id="a5a89-153">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="a5a89-153">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="a5a89-154">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="a5a89-154">lastReportedDateTime</span></span>|<span data-ttu-id="a5a89-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5a89-155">DateTimeOffset</span></span>|<span data-ttu-id="a5a89-156">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="a5a89-156">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="a5a89-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a5a89-157">userPrincipalName</span></span>|<span data-ttu-id="a5a89-158">String</span><span class="sxs-lookup"><span data-stu-id="a5a89-158">String</span></span>|<span data-ttu-id="a5a89-159">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="a5a89-159">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="a5a89-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5a89-160">Response</span></span>
<span data-ttu-id="a5a89-161">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5a89-161">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5a89-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a5a89-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="a5a89-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5a89-163">Request</span></span>
<span data-ttu-id="a5a89-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a5a89-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
Content-type: application/json
Content-length: 444

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
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

### <a name="response"></a><span data-ttu-id="a5a89-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5a89-165">Response</span></span>
<span data-ttu-id="a5a89-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a5a89-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 493

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "id": "c6c78124-8124-c6c7-2481-c7c62481c7c6",
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





