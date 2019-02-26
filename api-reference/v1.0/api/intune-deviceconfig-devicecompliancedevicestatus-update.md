---
title: Atualizar deviceComplianceDeviceStatus
description: Atualizar as propriedades de um objeto deviceComplianceDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6b0a4293d5244d414e67702d1e3b975d842be738
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259700"
---
# <a name="update-devicecompliancedevicestatus"></a><span data-ttu-id="b0274-103">Atualizar deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="b0274-103">Update deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="b0274-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b0274-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0274-105">Atualizar as propriedades de um objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="b0274-105">Update the properties of a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0274-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b0274-106">Prerequisites</span></span>
<span data-ttu-id="b0274-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b0274-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b0274-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0274-109">Permission type</span></span>|<span data-ttu-id="b0274-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b0274-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0274-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0274-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b0274-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0274-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b0274-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b0274-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0274-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0274-114">Not supported.</span></span>|
|<span data-ttu-id="b0274-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0274-115">Application</span></span>|<span data-ttu-id="b0274-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0274-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0274-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b0274-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="b0274-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b0274-118">Request headers</span></span>
|<span data-ttu-id="b0274-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b0274-119">Header</span></span>|<span data-ttu-id="b0274-120">Valor</span><span class="sxs-lookup"><span data-stu-id="b0274-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0274-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b0274-121">Authorization</span></span>|<span data-ttu-id="b0274-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0274-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0274-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b0274-123">Accept</span></span>|<span data-ttu-id="b0274-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b0274-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0274-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b0274-125">Request body</span></span>
<span data-ttu-id="b0274-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="b0274-126">In the request body, supply a JSON representation for the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

<span data-ttu-id="b0274-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="b0274-127">The following table shows the properties that are required when you create the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span></span>

|<span data-ttu-id="b0274-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0274-128">Property</span></span>|<span data-ttu-id="b0274-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0274-129">Type</span></span>|<span data-ttu-id="b0274-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0274-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0274-131">id</span><span class="sxs-lookup"><span data-stu-id="b0274-131">id</span></span>|<span data-ttu-id="b0274-132">String</span><span class="sxs-lookup"><span data-stu-id="b0274-132">String</span></span>|<span data-ttu-id="b0274-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="b0274-133">Key of the entity.</span></span>|
|<span data-ttu-id="b0274-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="b0274-134">deviceDisplayName</span></span>|<span data-ttu-id="b0274-135">String</span><span class="sxs-lookup"><span data-stu-id="b0274-135">String</span></span>|<span data-ttu-id="b0274-136">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="b0274-136">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="b0274-137">userName</span><span class="sxs-lookup"><span data-stu-id="b0274-137">userName</span></span>|<span data-ttu-id="b0274-138">String</span><span class="sxs-lookup"><span data-stu-id="b0274-138">String</span></span>|<span data-ttu-id="b0274-139">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="b0274-139">The User Name that is being reported</span></span>|
|<span data-ttu-id="b0274-140">deviceModel</span><span class="sxs-lookup"><span data-stu-id="b0274-140">deviceModel</span></span>|<span data-ttu-id="b0274-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0274-141">String</span></span>|<span data-ttu-id="b0274-142">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="b0274-142">The device model that is being reported</span></span>|
|<span data-ttu-id="b0274-143">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b0274-143">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="b0274-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0274-144">DateTimeOffset</span></span>|<span data-ttu-id="b0274-145">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="b0274-145">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="b0274-146">status</span><span class="sxs-lookup"><span data-stu-id="b0274-146">status</span></span>|[<span data-ttu-id="b0274-147">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="b0274-147">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="b0274-148">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="b0274-148">Compliance status of the policy report.</span></span> <span data-ttu-id="b0274-149">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="b0274-149">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="b0274-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0274-150">lastReportedDateTime</span></span>|<span data-ttu-id="b0274-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0274-151">DateTimeOffset</span></span>|<span data-ttu-id="b0274-152">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="b0274-152">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="b0274-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b0274-153">userPrincipalName</span></span>|<span data-ttu-id="b0274-154">String</span><span class="sxs-lookup"><span data-stu-id="b0274-154">String</span></span>|<span data-ttu-id="b0274-155">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="b0274-155">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="b0274-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0274-156">Response</span></span>
<span data-ttu-id="b0274-157">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0274-157">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0274-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b0274-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0274-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0274-159">Request</span></span>
<span data-ttu-id="b0274-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0274-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b0274-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0274-161">Response</span></span>
<span data-ttu-id="b0274-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b0274-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



