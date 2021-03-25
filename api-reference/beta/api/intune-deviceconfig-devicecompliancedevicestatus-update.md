---
title: Atualizar deviceComplianceDeviceStatus
description: Atualizar as propriedades de um objeto deviceComplianceDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d5f35b4c400c77ab56f7cd8a8902785b612b0508
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51155551"
---
# <a name="update-devicecompliancedevicestatus"></a><span data-ttu-id="027ba-103">Atualizar deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="027ba-103">Update deviceComplianceDeviceStatus</span></span>

<span data-ttu-id="027ba-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="027ba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="027ba-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="027ba-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="027ba-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="027ba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="027ba-107">Atualizar as propriedades de um objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="027ba-107">Update the properties of a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="027ba-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="027ba-108">Prerequisites</span></span>
<span data-ttu-id="027ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="027ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="027ba-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="027ba-111">Permission type</span></span>|<span data-ttu-id="027ba-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="027ba-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="027ba-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="027ba-113">Delegated (work or school account)</span></span>|<span data-ttu-id="027ba-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="027ba-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="027ba-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="027ba-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="027ba-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="027ba-116">Not supported.</span></span>|
|<span data-ttu-id="027ba-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="027ba-117">Application</span></span>|<span data-ttu-id="027ba-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="027ba-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="027ba-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="027ba-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="027ba-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="027ba-120">Request headers</span></span>
|<span data-ttu-id="027ba-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="027ba-121">Header</span></span>|<span data-ttu-id="027ba-122">Valor</span><span class="sxs-lookup"><span data-stu-id="027ba-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="027ba-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="027ba-123">Authorization</span></span>|<span data-ttu-id="027ba-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="027ba-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="027ba-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="027ba-125">Accept</span></span>|<span data-ttu-id="027ba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="027ba-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="027ba-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="027ba-127">Request body</span></span>
<span data-ttu-id="027ba-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="027ba-128">In the request body, supply a JSON representation for the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

<span data-ttu-id="027ba-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="027ba-129">The following table shows the properties that are required when you create the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span></span>

|<span data-ttu-id="027ba-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="027ba-130">Property</span></span>|<span data-ttu-id="027ba-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="027ba-131">Type</span></span>|<span data-ttu-id="027ba-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="027ba-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="027ba-133">id</span><span class="sxs-lookup"><span data-stu-id="027ba-133">id</span></span>|<span data-ttu-id="027ba-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="027ba-134">String</span></span>|<span data-ttu-id="027ba-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="027ba-135">Key of the entity.</span></span>|
|<span data-ttu-id="027ba-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="027ba-136">deviceDisplayName</span></span>|<span data-ttu-id="027ba-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="027ba-137">String</span></span>|<span data-ttu-id="027ba-138">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="027ba-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="027ba-139">userName</span><span class="sxs-lookup"><span data-stu-id="027ba-139">userName</span></span>|<span data-ttu-id="027ba-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="027ba-140">String</span></span>|<span data-ttu-id="027ba-141">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="027ba-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="027ba-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="027ba-142">deviceModel</span></span>|<span data-ttu-id="027ba-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="027ba-143">String</span></span>|<span data-ttu-id="027ba-144">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="027ba-144">The device model that is being reported</span></span>|
|<span data-ttu-id="027ba-145">plataforma</span><span class="sxs-lookup"><span data-stu-id="027ba-145">platform</span></span>|<span data-ttu-id="027ba-146">Int32</span><span class="sxs-lookup"><span data-stu-id="027ba-146">Int32</span></span>|<span data-ttu-id="027ba-147">Plataforma do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="027ba-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="027ba-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="027ba-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="027ba-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="027ba-149">DateTimeOffset</span></span>|<span data-ttu-id="027ba-150">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="027ba-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="027ba-151">status</span><span class="sxs-lookup"><span data-stu-id="027ba-151">status</span></span>|[<span data-ttu-id="027ba-152">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="027ba-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="027ba-153">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="027ba-153">Compliance status of the policy report.</span></span> <span data-ttu-id="027ba-154">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="027ba-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="027ba-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="027ba-155">lastReportedDateTime</span></span>|<span data-ttu-id="027ba-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="027ba-156">DateTimeOffset</span></span>|<span data-ttu-id="027ba-157">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="027ba-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="027ba-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="027ba-158">userPrincipalName</span></span>|<span data-ttu-id="027ba-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="027ba-159">String</span></span>|<span data-ttu-id="027ba-160">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="027ba-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="027ba-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="027ba-161">Response</span></span>
<span data-ttu-id="027ba-162">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="027ba-162">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="027ba-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="027ba-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="027ba-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="027ba-164">Request</span></span>
<span data-ttu-id="027ba-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="027ba-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="027ba-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="027ba-166">Response</span></span>
<span data-ttu-id="027ba-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="027ba-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




