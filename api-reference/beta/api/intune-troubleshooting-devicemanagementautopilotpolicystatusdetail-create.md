---
title: Criar deviceManagementAutopilotPolicyStatusDetail
description: Criar um novo objeto deviceManagementAutopilotPolicyStatusDetail.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b7ea81e9099f3154d2139760bb310a8459ffa592
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47999500"
---
# <a name="create-devicemanagementautopilotpolicystatusdetail"></a><span data-ttu-id="626a8-103">Criar deviceManagementAutopilotPolicyStatusDetail</span><span class="sxs-lookup"><span data-stu-id="626a8-103">Create deviceManagementAutopilotPolicyStatusDetail</span></span>

<span data-ttu-id="626a8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="626a8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="626a8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="626a8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="626a8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="626a8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="626a8-107">Criar um novo objeto [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) .</span><span class="sxs-lookup"><span data-stu-id="626a8-107">Create a new [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="626a8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="626a8-108">Prerequisites</span></span>
<span data-ttu-id="626a8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="626a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="626a8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="626a8-111">Permission type</span></span>|<span data-ttu-id="626a8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="626a8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="626a8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="626a8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="626a8-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="626a8-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="626a8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="626a8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="626a8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="626a8-116">Not supported.</span></span>|
|<span data-ttu-id="626a8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="626a8-117">Application</span></span>|<span data-ttu-id="626a8-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="626a8-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="626a8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="626a8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails
```

## <a name="request-headers"></a><span data-ttu-id="626a8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="626a8-120">Request headers</span></span>
|<span data-ttu-id="626a8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="626a8-121">Header</span></span>|<span data-ttu-id="626a8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="626a8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="626a8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="626a8-123">Authorization</span></span>|<span data-ttu-id="626a8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="626a8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="626a8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="626a8-125">Accept</span></span>|<span data-ttu-id="626a8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="626a8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="626a8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="626a8-127">Request body</span></span>
<span data-ttu-id="626a8-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementAutopilotPolicyStatusDetail.</span><span class="sxs-lookup"><span data-stu-id="626a8-128">In the request body, supply a JSON representation for the deviceManagementAutopilotPolicyStatusDetail object.</span></span>

<span data-ttu-id="626a8-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementAutopilotPolicyStatusDetail.</span><span class="sxs-lookup"><span data-stu-id="626a8-129">The following table shows the properties that are required when you create the deviceManagementAutopilotPolicyStatusDetail.</span></span>

|<span data-ttu-id="626a8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="626a8-130">Property</span></span>|<span data-ttu-id="626a8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="626a8-131">Type</span></span>|<span data-ttu-id="626a8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="626a8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="626a8-133">id</span><span class="sxs-lookup"><span data-stu-id="626a8-133">id</span></span>|<span data-ttu-id="626a8-134">String</span><span class="sxs-lookup"><span data-stu-id="626a8-134">String</span></span>|<span data-ttu-id="626a8-135">O UUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="626a8-135">UUID for the object</span></span>|
|<span data-ttu-id="626a8-136">displayName</span><span class="sxs-lookup"><span data-stu-id="626a8-136">displayName</span></span>|<span data-ttu-id="626a8-137">String</span><span class="sxs-lookup"><span data-stu-id="626a8-137">String</span></span>|<span data-ttu-id="626a8-138">O nome amigável da política.</span><span class="sxs-lookup"><span data-stu-id="626a8-138">The friendly name of the policy.</span></span>|
|<span data-ttu-id="626a8-139">PolicyType</span><span class="sxs-lookup"><span data-stu-id="626a8-139">policyType</span></span>|[<span data-ttu-id="626a8-140">deviceManagementAutopilotPolicyType</span><span class="sxs-lookup"><span data-stu-id="626a8-140">deviceManagementAutopilotPolicyType</span></span>](../resources/intune-troubleshooting-devicemanagementautopilotpolicytype.md)|<span data-ttu-id="626a8-141">O tipo de política.</span><span class="sxs-lookup"><span data-stu-id="626a8-141">The type of policy.</span></span> <span data-ttu-id="626a8-142">Os valores possíveis são: `unknown`, `application`, `appModel`, `configurationPolicy`.</span><span class="sxs-lookup"><span data-stu-id="626a8-142">Possible values are: `unknown`, `application`, `appModel`, `configurationPolicy`.</span></span>|
|<span data-ttu-id="626a8-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="626a8-143">complianceStatus</span></span>|[<span data-ttu-id="626a8-144">deviceManagementAutopilotPolicyComplianceStatus</span><span class="sxs-lookup"><span data-stu-id="626a8-144">deviceManagementAutopilotPolicyComplianceStatus</span></span>](../resources/intune-troubleshooting-devicemanagementautopilotpolicycompliancestatus.md)|<span data-ttu-id="626a8-145">O status de conformidade da política.</span><span class="sxs-lookup"><span data-stu-id="626a8-145">The policy compliance status.</span></span> <span data-ttu-id="626a8-146">Os possíveis valores são: `unknown`, `compliant`, `installed`, `notCompliant`, `notInstalled`, `error`.</span><span class="sxs-lookup"><span data-stu-id="626a8-146">Possible values are: `unknown`, `compliant`, `installed`, `notCompliant`, `notInstalled`, `error`.</span></span>|
|<span data-ttu-id="626a8-147">trackedOnEnrollmentStatus</span><span class="sxs-lookup"><span data-stu-id="626a8-147">trackedOnEnrollmentStatus</span></span>|<span data-ttu-id="626a8-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="626a8-148">Boolean</span></span>|<span data-ttu-id="626a8-149">Indica se este prolicy foi rastreado como parte da sessão de sincronização do registro de inicialização do AutoPilot</span><span class="sxs-lookup"><span data-stu-id="626a8-149">Indicates if this prolicy was tracked as part of the autopilot bootstrap enrollment sync session</span></span>|
|<span data-ttu-id="626a8-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="626a8-150">lastReportedDateTime</span></span>|<span data-ttu-id="626a8-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="626a8-151">DateTimeOffset</span></span>|<span data-ttu-id="626a8-152">Carimbo de data/hora do status da política relatado</span><span class="sxs-lookup"><span data-stu-id="626a8-152">Timestamp of the reported policy status</span></span>|



## <a name="response"></a><span data-ttu-id="626a8-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="626a8-153">Response</span></span>
<span data-ttu-id="626a8-154">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="626a8-154">If successful, this method returns a `201 Created` response code and a [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="626a8-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="626a8-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="626a8-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="626a8-156">Request</span></span>
<span data-ttu-id="626a8-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="626a8-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails
Content-type: application/json
Content-length: 295

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotPolicyStatusDetail",
  "displayName": "Display Name value",
  "policyType": "application",
  "complianceStatus": "compliant",
  "trackedOnEnrollmentStatus": true,
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
}
```

### <a name="response"></a><span data-ttu-id="626a8-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="626a8-158">Response</span></span>
<span data-ttu-id="626a8-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="626a8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 344

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotPolicyStatusDetail",
  "id": "dbe093ee-93ee-dbe0-ee93-e0dbee93e0db",
  "displayName": "Display Name value",
  "policyType": "application",
  "complianceStatus": "compliant",
  "trackedOnEnrollmentStatus": true,
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
}
```






