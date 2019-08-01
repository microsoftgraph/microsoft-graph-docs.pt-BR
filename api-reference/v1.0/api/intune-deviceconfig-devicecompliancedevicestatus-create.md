---
title: Criar deviceComplianceDeviceStatus
description: Criar um novo objeto deviceComplianceDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b33cb80c584df64eb7130d24c706b5bb0c16b413
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997754"
---
# <a name="create-devicecompliancedevicestatus"></a><span data-ttu-id="50724-103">Criar deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="50724-103">Create deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="50724-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="50724-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50724-105">Criar um novo objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="50724-105">Create a new [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50724-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="50724-106">Prerequisites</span></span>
<span data-ttu-id="50724-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50724-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50724-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50724-109">Permission type</span></span>|<span data-ttu-id="50724-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="50724-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50724-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50724-111">Delegated (work or school account)</span></span>|<span data-ttu-id="50724-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50724-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="50724-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50724-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50724-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50724-114">Not supported.</span></span>|
|<span data-ttu-id="50724-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50724-115">Application</span></span>|<span data-ttu-id="50724-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50724-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50724-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50724-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="50724-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50724-118">Request headers</span></span>
|<span data-ttu-id="50724-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="50724-119">Header</span></span>|<span data-ttu-id="50724-120">Valor</span><span class="sxs-lookup"><span data-stu-id="50724-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50724-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="50724-121">Authorization</span></span>|<span data-ttu-id="50724-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50724-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50724-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="50724-123">Accept</span></span>|<span data-ttu-id="50724-124">application/json</span><span class="sxs-lookup"><span data-stu-id="50724-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50724-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50724-125">Request body</span></span>
<span data-ttu-id="50724-126">No corpo da solicitação, forneça uma representação JSON do objeto deviceComplianceDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="50724-126">In the request body, supply a JSON representation for the deviceComplianceDeviceStatus object.</span></span>

<span data-ttu-id="50724-127">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceComplianceDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="50724-127">The following table shows the properties that are required when you create the deviceComplianceDeviceStatus.</span></span>

|<span data-ttu-id="50724-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50724-128">Property</span></span>|<span data-ttu-id="50724-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="50724-129">Type</span></span>|<span data-ttu-id="50724-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="50724-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50724-131">id</span><span class="sxs-lookup"><span data-stu-id="50724-131">id</span></span>|<span data-ttu-id="50724-132">String</span><span class="sxs-lookup"><span data-stu-id="50724-132">String</span></span>|<span data-ttu-id="50724-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="50724-133">Key of the entity.</span></span>|
|<span data-ttu-id="50724-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="50724-134">deviceDisplayName</span></span>|<span data-ttu-id="50724-135">String</span><span class="sxs-lookup"><span data-stu-id="50724-135">String</span></span>|<span data-ttu-id="50724-136">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="50724-136">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="50724-137">userName</span><span class="sxs-lookup"><span data-stu-id="50724-137">userName</span></span>|<span data-ttu-id="50724-138">String</span><span class="sxs-lookup"><span data-stu-id="50724-138">String</span></span>|<span data-ttu-id="50724-139">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="50724-139">The User Name that is being reported</span></span>|
|<span data-ttu-id="50724-140">deviceModel</span><span class="sxs-lookup"><span data-stu-id="50724-140">deviceModel</span></span>|<span data-ttu-id="50724-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50724-141">String</span></span>|<span data-ttu-id="50724-142">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="50724-142">The device model that is being reported</span></span>|
|<span data-ttu-id="50724-143">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="50724-143">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="50724-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50724-144">DateTimeOffset</span></span>|<span data-ttu-id="50724-145">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="50724-145">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="50724-146">status</span><span class="sxs-lookup"><span data-stu-id="50724-146">status</span></span>|[<span data-ttu-id="50724-147">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="50724-147">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="50724-148">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="50724-148">Compliance status of the policy report.</span></span> <span data-ttu-id="50724-149">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="50724-149">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="50724-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="50724-150">lastReportedDateTime</span></span>|<span data-ttu-id="50724-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50724-151">DateTimeOffset</span></span>|<span data-ttu-id="50724-152">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="50724-152">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="50724-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="50724-153">userPrincipalName</span></span>|<span data-ttu-id="50724-154">String</span><span class="sxs-lookup"><span data-stu-id="50724-154">String</span></span>|<span data-ttu-id="50724-155">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="50724-155">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="50724-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="50724-156">Response</span></span>
<span data-ttu-id="50724-157">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="50724-157">If successful, this method returns a `201 Created` response code and a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50724-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="50724-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="50724-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50724-159">Request</span></span>
<span data-ttu-id="50724-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="50724-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="50724-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="50724-161">Response</span></span>
<span data-ttu-id="50724-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="50724-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



