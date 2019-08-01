---
title: Atualizar deviceComplianceDeviceStatus
description: Atualizar as propriedades de um objeto deviceComplianceDeviceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 73c593319851ef93a326814ff3f5cc950b6a5545
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36017844"
---
# <a name="update-devicecompliancedevicestatus"></a><span data-ttu-id="c480e-103">Atualizar deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="c480e-103">Update deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="c480e-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c480e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c480e-105">Atualizar as propriedades de um objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="c480e-105">Update the properties of a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c480e-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c480e-106">Prerequisites</span></span>
<span data-ttu-id="c480e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c480e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c480e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c480e-109">Permission type</span></span>|<span data-ttu-id="c480e-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c480e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c480e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c480e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c480e-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c480e-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c480e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c480e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c480e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c480e-114">Not supported.</span></span>|
|<span data-ttu-id="c480e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c480e-115">Application</span></span>|<span data-ttu-id="c480e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c480e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c480e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c480e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="c480e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c480e-118">Request headers</span></span>
|<span data-ttu-id="c480e-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c480e-119">Header</span></span>|<span data-ttu-id="c480e-120">Valor</span><span class="sxs-lookup"><span data-stu-id="c480e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c480e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c480e-121">Authorization</span></span>|<span data-ttu-id="c480e-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c480e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c480e-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c480e-123">Accept</span></span>|<span data-ttu-id="c480e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c480e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c480e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c480e-125">Request body</span></span>
<span data-ttu-id="c480e-126">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="c480e-126">In the request body, supply a JSON representation for the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

<span data-ttu-id="c480e-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="c480e-127">The following table shows the properties that are required when you create the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span></span>

|<span data-ttu-id="c480e-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c480e-128">Property</span></span>|<span data-ttu-id="c480e-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="c480e-129">Type</span></span>|<span data-ttu-id="c480e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="c480e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c480e-131">id</span><span class="sxs-lookup"><span data-stu-id="c480e-131">id</span></span>|<span data-ttu-id="c480e-132">String</span><span class="sxs-lookup"><span data-stu-id="c480e-132">String</span></span>|<span data-ttu-id="c480e-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c480e-133">Key of the entity.</span></span>|
|<span data-ttu-id="c480e-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="c480e-134">deviceDisplayName</span></span>|<span data-ttu-id="c480e-135">String</span><span class="sxs-lookup"><span data-stu-id="c480e-135">String</span></span>|<span data-ttu-id="c480e-136">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="c480e-136">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="c480e-137">userName</span><span class="sxs-lookup"><span data-stu-id="c480e-137">userName</span></span>|<span data-ttu-id="c480e-138">String</span><span class="sxs-lookup"><span data-stu-id="c480e-138">String</span></span>|<span data-ttu-id="c480e-139">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="c480e-139">The User Name that is being reported</span></span>|
|<span data-ttu-id="c480e-140">deviceModel</span><span class="sxs-lookup"><span data-stu-id="c480e-140">deviceModel</span></span>|<span data-ttu-id="c480e-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c480e-141">String</span></span>|<span data-ttu-id="c480e-142">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="c480e-142">The device model that is being reported</span></span>|
|<span data-ttu-id="c480e-143">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c480e-143">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="c480e-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c480e-144">DateTimeOffset</span></span>|<span data-ttu-id="c480e-145">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="c480e-145">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="c480e-146">status</span><span class="sxs-lookup"><span data-stu-id="c480e-146">status</span></span>|[<span data-ttu-id="c480e-147">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="c480e-147">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="c480e-148">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="c480e-148">Compliance status of the policy report.</span></span> <span data-ttu-id="c480e-149">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="c480e-149">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="c480e-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="c480e-150">lastReportedDateTime</span></span>|<span data-ttu-id="c480e-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c480e-151">DateTimeOffset</span></span>|<span data-ttu-id="c480e-152">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="c480e-152">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="c480e-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c480e-153">userPrincipalName</span></span>|<span data-ttu-id="c480e-154">String</span><span class="sxs-lookup"><span data-stu-id="c480e-154">String</span></span>|<span data-ttu-id="c480e-155">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="c480e-155">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="c480e-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="c480e-156">Response</span></span>
<span data-ttu-id="c480e-157">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c480e-157">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c480e-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c480e-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="c480e-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c480e-159">Request</span></span>
<span data-ttu-id="c480e-160">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c480e-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c480e-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="c480e-161">Response</span></span>
<span data-ttu-id="c480e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c480e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



