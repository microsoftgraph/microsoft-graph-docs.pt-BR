---
title: Criar deviceComplianceDeviceStatus
description: Criar um novo objeto deviceComplianceDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 73b65d3b8751b5ad417719ec4e4d3aba136a4b0d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155579"
---
# <a name="create-devicecompliancedevicestatus"></a><span data-ttu-id="b1862-103">Criar deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="b1862-103">Create deviceComplianceDeviceStatus</span></span>

<span data-ttu-id="b1862-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1862-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1862-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b1862-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1862-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b1862-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1862-107">Criar um novo objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="b1862-107">Create a new [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1862-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b1862-108">Prerequisites</span></span>
<span data-ttu-id="b1862-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1862-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1862-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1862-111">Permission type</span></span>|<span data-ttu-id="b1862-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b1862-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1862-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1862-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b1862-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1862-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b1862-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b1862-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1862-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1862-116">Not supported.</span></span>|
|<span data-ttu-id="b1862-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1862-117">Application</span></span>|<span data-ttu-id="b1862-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1862-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1862-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1862-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="b1862-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1862-120">Request headers</span></span>
|<span data-ttu-id="b1862-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b1862-121">Header</span></span>|<span data-ttu-id="b1862-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b1862-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1862-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b1862-123">Authorization</span></span>|<span data-ttu-id="b1862-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b1862-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1862-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b1862-125">Accept</span></span>|<span data-ttu-id="b1862-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b1862-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1862-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1862-127">Request body</span></span>
<span data-ttu-id="b1862-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceComplianceDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="b1862-128">In the request body, supply a JSON representation for the deviceComplianceDeviceStatus object.</span></span>

<span data-ttu-id="b1862-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceComplianceDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="b1862-129">The following table shows the properties that are required when you create the deviceComplianceDeviceStatus.</span></span>

|<span data-ttu-id="b1862-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1862-130">Property</span></span>|<span data-ttu-id="b1862-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1862-131">Type</span></span>|<span data-ttu-id="b1862-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1862-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1862-133">id</span><span class="sxs-lookup"><span data-stu-id="b1862-133">id</span></span>|<span data-ttu-id="b1862-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1862-134">String</span></span>|<span data-ttu-id="b1862-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b1862-135">Key of the entity.</span></span>|
|<span data-ttu-id="b1862-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="b1862-136">deviceDisplayName</span></span>|<span data-ttu-id="b1862-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1862-137">String</span></span>|<span data-ttu-id="b1862-138">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="b1862-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="b1862-139">userName</span><span class="sxs-lookup"><span data-stu-id="b1862-139">userName</span></span>|<span data-ttu-id="b1862-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1862-140">String</span></span>|<span data-ttu-id="b1862-141">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="b1862-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="b1862-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="b1862-142">deviceModel</span></span>|<span data-ttu-id="b1862-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1862-143">String</span></span>|<span data-ttu-id="b1862-144">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="b1862-144">The device model that is being reported</span></span>|
|<span data-ttu-id="b1862-145">plataforma</span><span class="sxs-lookup"><span data-stu-id="b1862-145">platform</span></span>|<span data-ttu-id="b1862-146">Int32</span><span class="sxs-lookup"><span data-stu-id="b1862-146">Int32</span></span>|<span data-ttu-id="b1862-147">Plataforma do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="b1862-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="b1862-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b1862-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="b1862-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1862-149">DateTimeOffset</span></span>|<span data-ttu-id="b1862-150">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="b1862-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="b1862-151">status</span><span class="sxs-lookup"><span data-stu-id="b1862-151">status</span></span>|[<span data-ttu-id="b1862-152">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="b1862-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="b1862-153">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="b1862-153">Compliance status of the policy report.</span></span> <span data-ttu-id="b1862-154">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="b1862-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="b1862-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1862-155">lastReportedDateTime</span></span>|<span data-ttu-id="b1862-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1862-156">DateTimeOffset</span></span>|<span data-ttu-id="b1862-157">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="b1862-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="b1862-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b1862-158">userPrincipalName</span></span>|<span data-ttu-id="b1862-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1862-159">String</span></span>|<span data-ttu-id="b1862-160">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="b1862-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="b1862-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1862-161">Response</span></span>
<span data-ttu-id="b1862-162">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1862-162">If successful, this method returns a `201 Created` response code and a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1862-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b1862-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1862-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1862-164">Request</span></span>
<span data-ttu-id="b1862-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b1862-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b1862-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1862-166">Response</span></span>
<span data-ttu-id="b1862-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b1862-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




