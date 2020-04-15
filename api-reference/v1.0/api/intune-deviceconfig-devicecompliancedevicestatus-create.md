---
title: Criar deviceComplianceDeviceStatus
description: Criar um novo objeto deviceComplianceDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b09c3701f22bba5b7f385e92a2db5533931f471c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43400420"
---
# <a name="create-devicecompliancedevicestatus"></a><span data-ttu-id="3337c-103">Criar deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="3337c-103">Create deviceComplianceDeviceStatus</span></span>

<span data-ttu-id="3337c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3337c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3337c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3337c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3337c-106">Criar um novo objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="3337c-106">Create a new [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3337c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3337c-107">Prerequisites</span></span>
<span data-ttu-id="3337c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3337c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3337c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3337c-110">Permission type</span></span>|<span data-ttu-id="3337c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3337c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3337c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3337c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3337c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3337c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3337c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3337c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3337c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3337c-115">Not supported.</span></span>|
|<span data-ttu-id="3337c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3337c-116">Application</span></span>|<span data-ttu-id="3337c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3337c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3337c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3337c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="3337c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3337c-119">Request headers</span></span>
|<span data-ttu-id="3337c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3337c-120">Header</span></span>|<span data-ttu-id="3337c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3337c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3337c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3337c-122">Authorization</span></span>|<span data-ttu-id="3337c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3337c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3337c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3337c-124">Accept</span></span>|<span data-ttu-id="3337c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3337c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3337c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3337c-126">Request body</span></span>
<span data-ttu-id="3337c-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceComplianceDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="3337c-127">In the request body, supply a JSON representation for the deviceComplianceDeviceStatus object.</span></span>

<span data-ttu-id="3337c-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceComplianceDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="3337c-128">The following table shows the properties that are required when you create the deviceComplianceDeviceStatus.</span></span>

|<span data-ttu-id="3337c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3337c-129">Property</span></span>|<span data-ttu-id="3337c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3337c-130">Type</span></span>|<span data-ttu-id="3337c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3337c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3337c-132">id</span><span class="sxs-lookup"><span data-stu-id="3337c-132">id</span></span>|<span data-ttu-id="3337c-133">String</span><span class="sxs-lookup"><span data-stu-id="3337c-133">String</span></span>|<span data-ttu-id="3337c-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3337c-134">Key of the entity.</span></span>|
|<span data-ttu-id="3337c-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="3337c-135">deviceDisplayName</span></span>|<span data-ttu-id="3337c-136">String</span><span class="sxs-lookup"><span data-stu-id="3337c-136">String</span></span>|<span data-ttu-id="3337c-137">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="3337c-137">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="3337c-138">userName</span><span class="sxs-lookup"><span data-stu-id="3337c-138">userName</span></span>|<span data-ttu-id="3337c-139">String</span><span class="sxs-lookup"><span data-stu-id="3337c-139">String</span></span>|<span data-ttu-id="3337c-140">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="3337c-140">The User Name that is being reported</span></span>|
|<span data-ttu-id="3337c-141">deviceModel</span><span class="sxs-lookup"><span data-stu-id="3337c-141">deviceModel</span></span>|<span data-ttu-id="3337c-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3337c-142">String</span></span>|<span data-ttu-id="3337c-143">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="3337c-143">The device model that is being reported</span></span>|
|<span data-ttu-id="3337c-144">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3337c-144">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="3337c-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3337c-145">DateTimeOffset</span></span>|<span data-ttu-id="3337c-146">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="3337c-146">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="3337c-147">status</span><span class="sxs-lookup"><span data-stu-id="3337c-147">status</span></span>|[<span data-ttu-id="3337c-148">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="3337c-148">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="3337c-149">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="3337c-149">Compliance status of the policy report.</span></span> <span data-ttu-id="3337c-150">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="3337c-150">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="3337c-151">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="3337c-151">lastReportedDateTime</span></span>|<span data-ttu-id="3337c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3337c-152">DateTimeOffset</span></span>|<span data-ttu-id="3337c-153">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="3337c-153">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="3337c-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3337c-154">userPrincipalName</span></span>|<span data-ttu-id="3337c-155">String</span><span class="sxs-lookup"><span data-stu-id="3337c-155">String</span></span>|<span data-ttu-id="3337c-156">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="3337c-156">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="3337c-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="3337c-157">Response</span></span>
<span data-ttu-id="3337c-158">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3337c-158">If successful, this method returns a `201 Created` response code and a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3337c-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3337c-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="3337c-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3337c-160">Request</span></span>
<span data-ttu-id="3337c-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3337c-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
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

### <a name="response"></a><span data-ttu-id="3337c-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="3337c-162">Response</span></span>
<span data-ttu-id="3337c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3337c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






