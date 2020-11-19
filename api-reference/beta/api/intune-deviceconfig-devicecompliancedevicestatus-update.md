---
title: Atualizar deviceComplianceDeviceStatus
description: Atualizar as propriedades de um objeto deviceComplianceDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5f7c8c00e2d03f49c10a5a37d5c97ba5a611885c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49292467"
---
# <a name="update-devicecompliancedevicestatus"></a><span data-ttu-id="f1eff-103">Atualizar deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="f1eff-103">Update deviceComplianceDeviceStatus</span></span>

<span data-ttu-id="f1eff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1eff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f1eff-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f1eff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1eff-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f1eff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1eff-107">Atualizar as propriedades de um objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="f1eff-107">Update the properties of a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1eff-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f1eff-108">Prerequisites</span></span>
<span data-ttu-id="f1eff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1eff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1eff-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1eff-111">Permission type</span></span>|<span data-ttu-id="f1eff-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f1eff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1eff-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1eff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f1eff-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1eff-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f1eff-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1eff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1eff-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1eff-116">Not supported.</span></span>|
|<span data-ttu-id="f1eff-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1eff-117">Application</span></span>|<span data-ttu-id="f1eff-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1eff-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1eff-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1eff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="f1eff-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1eff-120">Request headers</span></span>
|<span data-ttu-id="f1eff-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f1eff-121">Header</span></span>|<span data-ttu-id="f1eff-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f1eff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1eff-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1eff-123">Authorization</span></span>|<span data-ttu-id="f1eff-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1eff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1eff-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f1eff-125">Accept</span></span>|<span data-ttu-id="f1eff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f1eff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1eff-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1eff-127">Request body</span></span>
<span data-ttu-id="f1eff-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="f1eff-128">In the request body, supply a JSON representation for the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

<span data-ttu-id="f1eff-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="f1eff-129">The following table shows the properties that are required when you create the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span></span>

|<span data-ttu-id="f1eff-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1eff-130">Property</span></span>|<span data-ttu-id="f1eff-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1eff-131">Type</span></span>|<span data-ttu-id="f1eff-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1eff-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1eff-133">id</span><span class="sxs-lookup"><span data-stu-id="f1eff-133">id</span></span>|<span data-ttu-id="f1eff-134">String</span><span class="sxs-lookup"><span data-stu-id="f1eff-134">String</span></span>|<span data-ttu-id="f1eff-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f1eff-135">Key of the entity.</span></span>|
|<span data-ttu-id="f1eff-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="f1eff-136">deviceDisplayName</span></span>|<span data-ttu-id="f1eff-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1eff-137">String</span></span>|<span data-ttu-id="f1eff-138">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="f1eff-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="f1eff-139">userName</span><span class="sxs-lookup"><span data-stu-id="f1eff-139">userName</span></span>|<span data-ttu-id="f1eff-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1eff-140">String</span></span>|<span data-ttu-id="f1eff-141">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="f1eff-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="f1eff-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="f1eff-142">deviceModel</span></span>|<span data-ttu-id="f1eff-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1eff-143">String</span></span>|<span data-ttu-id="f1eff-144">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="f1eff-144">The device model that is being reported</span></span>|
|<span data-ttu-id="f1eff-145">plataforma</span><span class="sxs-lookup"><span data-stu-id="f1eff-145">platform</span></span>|<span data-ttu-id="f1eff-146">Int32</span><span class="sxs-lookup"><span data-stu-id="f1eff-146">Int32</span></span>|<span data-ttu-id="f1eff-147">Plataforma do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="f1eff-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="f1eff-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f1eff-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="f1eff-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1eff-149">DateTimeOffset</span></span>|<span data-ttu-id="f1eff-150">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="f1eff-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="f1eff-151">status</span><span class="sxs-lookup"><span data-stu-id="f1eff-151">status</span></span>|[<span data-ttu-id="f1eff-152">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="f1eff-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="f1eff-153">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="f1eff-153">Compliance status of the policy report.</span></span> <span data-ttu-id="f1eff-154">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="f1eff-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="f1eff-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="f1eff-155">lastReportedDateTime</span></span>|<span data-ttu-id="f1eff-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1eff-156">DateTimeOffset</span></span>|<span data-ttu-id="f1eff-157">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="f1eff-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="f1eff-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f1eff-158">userPrincipalName</span></span>|<span data-ttu-id="f1eff-159">String</span><span class="sxs-lookup"><span data-stu-id="f1eff-159">String</span></span>|<span data-ttu-id="f1eff-160">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="f1eff-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="f1eff-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1eff-161">Response</span></span>
<span data-ttu-id="f1eff-162">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1eff-162">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1eff-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1eff-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1eff-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1eff-164">Request</span></span>
<span data-ttu-id="f1eff-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1eff-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f1eff-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1eff-166">Response</span></span>
<span data-ttu-id="f1eff-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1eff-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




