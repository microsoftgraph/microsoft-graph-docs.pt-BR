---
title: Criar deviceComplianceDeviceStatus
description: Criar um novo objeto deviceComplianceDeviceStatus.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a6075eb432a8b39061f5b2dc2d8cca01e08d4605
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33927892"
---
# <a name="create-devicecompliancedevicestatus"></a><span data-ttu-id="29d58-103">Criar deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="29d58-103">Create deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="29d58-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="29d58-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29d58-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="29d58-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29d58-106">Criar um novo objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="29d58-106">Create a new [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29d58-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="29d58-107">Prerequisites</span></span>
<span data-ttu-id="29d58-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29d58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29d58-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29d58-110">Permission type</span></span>|<span data-ttu-id="29d58-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="29d58-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29d58-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29d58-112">Delegated (work or school account)</span></span>|<span data-ttu-id="29d58-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29d58-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="29d58-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29d58-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29d58-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29d58-115">Not supported.</span></span>|
|<span data-ttu-id="29d58-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29d58-116">Application</span></span>|<span data-ttu-id="29d58-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29d58-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="29d58-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29d58-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="29d58-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29d58-119">Request headers</span></span>
|<span data-ttu-id="29d58-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="29d58-120">Header</span></span>|<span data-ttu-id="29d58-121">Valor</span><span class="sxs-lookup"><span data-stu-id="29d58-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29d58-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="29d58-122">Authorization</span></span>|<span data-ttu-id="29d58-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29d58-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29d58-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="29d58-124">Accept</span></span>|<span data-ttu-id="29d58-125">application/json</span><span class="sxs-lookup"><span data-stu-id="29d58-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29d58-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29d58-126">Request body</span></span>
<span data-ttu-id="29d58-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceComplianceDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="29d58-127">In the request body, supply a JSON representation for the deviceComplianceDeviceStatus object.</span></span>

<span data-ttu-id="29d58-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceComplianceDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="29d58-128">The following table shows the properties that are required when you create the deviceComplianceDeviceStatus.</span></span>

|<span data-ttu-id="29d58-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="29d58-129">Property</span></span>|<span data-ttu-id="29d58-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="29d58-130">Type</span></span>|<span data-ttu-id="29d58-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="29d58-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29d58-132">id</span><span class="sxs-lookup"><span data-stu-id="29d58-132">id</span></span>|<span data-ttu-id="29d58-133">String</span><span class="sxs-lookup"><span data-stu-id="29d58-133">String</span></span>|<span data-ttu-id="29d58-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="29d58-134">Key of the entity.</span></span>|
|<span data-ttu-id="29d58-135">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="29d58-135">deviceDisplayName</span></span>|<span data-ttu-id="29d58-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29d58-136">String</span></span>|<span data-ttu-id="29d58-137">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="29d58-137">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="29d58-138">userName</span><span class="sxs-lookup"><span data-stu-id="29d58-138">userName</span></span>|<span data-ttu-id="29d58-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29d58-139">String</span></span>|<span data-ttu-id="29d58-140">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="29d58-140">The User Name that is being reported</span></span>|
|<span data-ttu-id="29d58-141">deviceModel</span><span class="sxs-lookup"><span data-stu-id="29d58-141">deviceModel</span></span>|<span data-ttu-id="29d58-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29d58-142">String</span></span>|<span data-ttu-id="29d58-143">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="29d58-143">The device model that is being reported</span></span>|
|<span data-ttu-id="29d58-144">platform</span><span class="sxs-lookup"><span data-stu-id="29d58-144">platform</span></span>|<span data-ttu-id="29d58-145">Int32</span><span class="sxs-lookup"><span data-stu-id="29d58-145">Int32</span></span>|<span data-ttu-id="29d58-146">Plataforma do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="29d58-146">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="29d58-147">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="29d58-147">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="29d58-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29d58-148">DateTimeOffset</span></span>|<span data-ttu-id="29d58-149">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="29d58-149">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="29d58-150">status</span><span class="sxs-lookup"><span data-stu-id="29d58-150">status</span></span>|[<span data-ttu-id="29d58-151">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="29d58-151">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="29d58-152">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="29d58-152">Compliance status of the policy report.</span></span> <span data-ttu-id="29d58-153">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="29d58-153">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="29d58-154">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="29d58-154">lastReportedDateTime</span></span>|<span data-ttu-id="29d58-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29d58-155">DateTimeOffset</span></span>|<span data-ttu-id="29d58-156">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="29d58-156">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="29d58-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="29d58-157">userPrincipalName</span></span>|<span data-ttu-id="29d58-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29d58-158">String</span></span>|<span data-ttu-id="29d58-159">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="29d58-159">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="29d58-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="29d58-160">Response</span></span>
<span data-ttu-id="29d58-161">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29d58-161">If successful, this method returns a `201 Created` response code and a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29d58-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="29d58-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="29d58-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29d58-163">Request</span></span>
<span data-ttu-id="29d58-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="29d58-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
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

### <a name="response"></a><span data-ttu-id="29d58-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="29d58-165">Response</span></span>
<span data-ttu-id="29d58-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="29d58-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




