---
title: Criar deviceComplianceDeviceStatus
description: Criar um novo objeto deviceComplianceDeviceStatus.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3290655a596d114530d8d309354b6ce285b089a8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725097"
---
# <a name="create-devicecompliancedevicestatus"></a><span data-ttu-id="16dc1-103">Criar deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="16dc1-103">Create deviceComplianceDeviceStatus</span></span>

<span data-ttu-id="16dc1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16dc1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="16dc1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="16dc1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16dc1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="16dc1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16dc1-107">Criar um novo objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="16dc1-107">Create a new [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="16dc1-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="16dc1-108">Prerequisites</span></span>
<span data-ttu-id="16dc1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16dc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16dc1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="16dc1-111">Permission type</span></span>|<span data-ttu-id="16dc1-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="16dc1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16dc1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="16dc1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="16dc1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16dc1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="16dc1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="16dc1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16dc1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="16dc1-116">Not supported.</span></span>|
|<span data-ttu-id="16dc1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="16dc1-117">Application</span></span>|<span data-ttu-id="16dc1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16dc1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="16dc1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="16dc1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="16dc1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="16dc1-120">Request headers</span></span>
|<span data-ttu-id="16dc1-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="16dc1-121">Header</span></span>|<span data-ttu-id="16dc1-122">Valor</span><span class="sxs-lookup"><span data-stu-id="16dc1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16dc1-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="16dc1-123">Authorization</span></span>|<span data-ttu-id="16dc1-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="16dc1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16dc1-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="16dc1-125">Accept</span></span>|<span data-ttu-id="16dc1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="16dc1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16dc1-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="16dc1-127">Request body</span></span>
<span data-ttu-id="16dc1-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceComplianceDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="16dc1-128">In the request body, supply a JSON representation for the deviceComplianceDeviceStatus object.</span></span>

<span data-ttu-id="16dc1-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceComplianceDeviceStatus.</span><span class="sxs-lookup"><span data-stu-id="16dc1-129">The following table shows the properties that are required when you create the deviceComplianceDeviceStatus.</span></span>

|<span data-ttu-id="16dc1-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="16dc1-130">Property</span></span>|<span data-ttu-id="16dc1-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="16dc1-131">Type</span></span>|<span data-ttu-id="16dc1-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="16dc1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16dc1-133">id</span><span class="sxs-lookup"><span data-stu-id="16dc1-133">id</span></span>|<span data-ttu-id="16dc1-134">String</span><span class="sxs-lookup"><span data-stu-id="16dc1-134">String</span></span>|<span data-ttu-id="16dc1-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="16dc1-135">Key of the entity.</span></span>|
|<span data-ttu-id="16dc1-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="16dc1-136">deviceDisplayName</span></span>|<span data-ttu-id="16dc1-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16dc1-137">String</span></span>|<span data-ttu-id="16dc1-138">Nome do dispositivo de DevicePolicyStatus.</span><span class="sxs-lookup"><span data-stu-id="16dc1-138">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="16dc1-139">userName</span><span class="sxs-lookup"><span data-stu-id="16dc1-139">userName</span></span>|<span data-ttu-id="16dc1-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16dc1-140">String</span></span>|<span data-ttu-id="16dc1-141">O nome de usuário que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="16dc1-141">The User Name that is being reported</span></span>|
|<span data-ttu-id="16dc1-142">deviceModel</span><span class="sxs-lookup"><span data-stu-id="16dc1-142">deviceModel</span></span>|<span data-ttu-id="16dc1-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16dc1-143">String</span></span>|<span data-ttu-id="16dc1-144">O modelo do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="16dc1-144">The device model that is being reported</span></span>|
|<span data-ttu-id="16dc1-145">plataforma</span><span class="sxs-lookup"><span data-stu-id="16dc1-145">platform</span></span>|<span data-ttu-id="16dc1-146">Int32</span><span class="sxs-lookup"><span data-stu-id="16dc1-146">Int32</span></span>|<span data-ttu-id="16dc1-147">Plataforma do dispositivo que está sendo relatado</span><span class="sxs-lookup"><span data-stu-id="16dc1-147">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="16dc1-148">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="16dc1-148">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="16dc1-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16dc1-149">DateTimeOffset</span></span>|<span data-ttu-id="16dc1-150">DateTime em que o período de cortesia de conformidade do dispositivo termina</span><span class="sxs-lookup"><span data-stu-id="16dc1-150">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="16dc1-151">status</span><span class="sxs-lookup"><span data-stu-id="16dc1-151">status</span></span>|[<span data-ttu-id="16dc1-152">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="16dc1-152">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="16dc1-153">Status de conformidade do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="16dc1-153">Compliance status of the policy report.</span></span> <span data-ttu-id="16dc1-154">Os valores possíveis são: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span><span class="sxs-lookup"><span data-stu-id="16dc1-154">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="16dc1-155">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="16dc1-155">lastReportedDateTime</span></span>|<span data-ttu-id="16dc1-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16dc1-156">DateTimeOffset</span></span>|<span data-ttu-id="16dc1-157">Data e hora da última modificação do relatório de políticas.</span><span class="sxs-lookup"><span data-stu-id="16dc1-157">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="16dc1-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="16dc1-158">userPrincipalName</span></span>|<span data-ttu-id="16dc1-159">String</span><span class="sxs-lookup"><span data-stu-id="16dc1-159">String</span></span>|<span data-ttu-id="16dc1-160">UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="16dc1-160">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="16dc1-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="16dc1-161">Response</span></span>
<span data-ttu-id="16dc1-162">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="16dc1-162">If successful, this method returns a `201 Created` response code and a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16dc1-163">Exemplo</span><span class="sxs-lookup"><span data-stu-id="16dc1-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="16dc1-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="16dc1-164">Request</span></span>
<span data-ttu-id="16dc1-165">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="16dc1-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="16dc1-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="16dc1-166">Response</span></span>
<span data-ttu-id="16dc1-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="16dc1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





