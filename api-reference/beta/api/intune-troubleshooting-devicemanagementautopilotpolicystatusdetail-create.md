---
title: Criar deviceManagementAutopilotPolicyStatusDetail
description: Crie um novo objeto deviceManagementAutopilotPolicyStatusDetail.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dabf8f2a81a01a696a0402f1cb23771e82c89ce0
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154982"
---
# <a name="create-devicemanagementautopilotpolicystatusdetail"></a><span data-ttu-id="2785e-103">Criar deviceManagementAutopilotPolicyStatusDetail</span><span class="sxs-lookup"><span data-stu-id="2785e-103">Create deviceManagementAutopilotPolicyStatusDetail</span></span>

<span data-ttu-id="2785e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2785e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2785e-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2785e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2785e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2785e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2785e-107">Crie um novo [objeto deviceManagementAutopilotPolicyStatusDetail.](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)</span><span class="sxs-lookup"><span data-stu-id="2785e-107">Create a new [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2785e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2785e-108">Prerequisites</span></span>
<span data-ttu-id="2785e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2785e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2785e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2785e-111">Permission type</span></span>|<span data-ttu-id="2785e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2785e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2785e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2785e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2785e-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2785e-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2785e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2785e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2785e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2785e-116">Not supported.</span></span>|
|<span data-ttu-id="2785e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2785e-117">Application</span></span>|<span data-ttu-id="2785e-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2785e-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2785e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2785e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails
```

## <a name="request-headers"></a><span data-ttu-id="2785e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2785e-120">Request headers</span></span>
|<span data-ttu-id="2785e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2785e-121">Header</span></span>|<span data-ttu-id="2785e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2785e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2785e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2785e-123">Authorization</span></span>|<span data-ttu-id="2785e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2785e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2785e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2785e-125">Accept</span></span>|<span data-ttu-id="2785e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2785e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2785e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2785e-127">Request body</span></span>
<span data-ttu-id="2785e-128">No corpo da solicitação, fornece uma representação JSON do objeto deviceManagementAutopilotPolicyStatusDetail.</span><span class="sxs-lookup"><span data-stu-id="2785e-128">In the request body, supply a JSON representation for the deviceManagementAutopilotPolicyStatusDetail object.</span></span>

<span data-ttu-id="2785e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementAutopilotPolicyStatusDetail.</span><span class="sxs-lookup"><span data-stu-id="2785e-129">The following table shows the properties that are required when you create the deviceManagementAutopilotPolicyStatusDetail.</span></span>

|<span data-ttu-id="2785e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2785e-130">Property</span></span>|<span data-ttu-id="2785e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2785e-131">Type</span></span>|<span data-ttu-id="2785e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2785e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2785e-133">id</span><span class="sxs-lookup"><span data-stu-id="2785e-133">id</span></span>|<span data-ttu-id="2785e-134">String</span><span class="sxs-lookup"><span data-stu-id="2785e-134">String</span></span>|<span data-ttu-id="2785e-135">O UUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="2785e-135">UUID for the object</span></span>|
|<span data-ttu-id="2785e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="2785e-136">displayName</span></span>|<span data-ttu-id="2785e-137">String</span><span class="sxs-lookup"><span data-stu-id="2785e-137">String</span></span>|<span data-ttu-id="2785e-138">O nome amigável da política.</span><span class="sxs-lookup"><span data-stu-id="2785e-138">The friendly name of the policy.</span></span>|
|<span data-ttu-id="2785e-139">policyType</span><span class="sxs-lookup"><span data-stu-id="2785e-139">policyType</span></span>|[<span data-ttu-id="2785e-140">deviceManagementAutopilotPolicyType</span><span class="sxs-lookup"><span data-stu-id="2785e-140">deviceManagementAutopilotPolicyType</span></span>](../resources/intune-troubleshooting-devicemanagementautopilotpolicytype.md)|<span data-ttu-id="2785e-141">O tipo de política.</span><span class="sxs-lookup"><span data-stu-id="2785e-141">The type of policy.</span></span> <span data-ttu-id="2785e-142">Os valores possíveis são: `unknown`, `application`, `appModel`, `configurationPolicy`.</span><span class="sxs-lookup"><span data-stu-id="2785e-142">Possible values are: `unknown`, `application`, `appModel`, `configurationPolicy`.</span></span>|
|<span data-ttu-id="2785e-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="2785e-143">complianceStatus</span></span>|[<span data-ttu-id="2785e-144">deviceManagementAutopilotPolicyComplianceStatus</span><span class="sxs-lookup"><span data-stu-id="2785e-144">deviceManagementAutopilotPolicyComplianceStatus</span></span>](../resources/intune-troubleshooting-devicemanagementautopilotpolicycompliancestatus.md)|<span data-ttu-id="2785e-145">O status de conformidade da política.</span><span class="sxs-lookup"><span data-stu-id="2785e-145">The policy compliance status.</span></span> <span data-ttu-id="2785e-146">Os possíveis valores são: `unknown`, `compliant`, `installed`, `notCompliant`, `notInstalled`, `error`.</span><span class="sxs-lookup"><span data-stu-id="2785e-146">Possible values are: `unknown`, `compliant`, `installed`, `notCompliant`, `notInstalled`, `error`.</span></span>|
|<span data-ttu-id="2785e-147">trackedOnEnrollmentStatus</span><span class="sxs-lookup"><span data-stu-id="2785e-147">trackedOnEnrollmentStatus</span></span>|<span data-ttu-id="2785e-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="2785e-148">Boolean</span></span>|<span data-ttu-id="2785e-149">Indica se esse prolicy foi rastreado como parte da sessão de sincronização de registro de inicialização do autopilot</span><span class="sxs-lookup"><span data-stu-id="2785e-149">Indicates if this prolicy was tracked as part of the autopilot bootstrap enrollment sync session</span></span>|
|<span data-ttu-id="2785e-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="2785e-150">lastReportedDateTime</span></span>|<span data-ttu-id="2785e-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2785e-151">DateTimeOffset</span></span>|<span data-ttu-id="2785e-152">Timestamp do status de política relatado</span><span class="sxs-lookup"><span data-stu-id="2785e-152">Timestamp of the reported policy status</span></span>|
|<span data-ttu-id="2785e-153">errorCode</span><span class="sxs-lookup"><span data-stu-id="2785e-153">errorCode</span></span>|<span data-ttu-id="2785e-154">Int32</span><span class="sxs-lookup"><span data-stu-id="2785e-154">Int32</span></span>|<span data-ttu-id="2785e-155">O errorode associado ao status de conformidade ou imposição da política.</span><span class="sxs-lookup"><span data-stu-id="2785e-155">The errorode associated with the compliance or enforcement status of the policy.</span></span> <span data-ttu-id="2785e-156">O código de erro para o status de imposição tem precedência, se existir.</span><span class="sxs-lookup"><span data-stu-id="2785e-156">Error code for enforcement status takes precedence if it exists.</span></span>|



## <a name="response"></a><span data-ttu-id="2785e-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="2785e-157">Response</span></span>
<span data-ttu-id="2785e-158">Se tiver êxito, este método retornará um código de resposta e um objeto `201 Created` [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2785e-158">If successful, this method returns a `201 Created` response code and a [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2785e-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2785e-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="2785e-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2785e-160">Request</span></span>
<span data-ttu-id="2785e-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2785e-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails
Content-type: application/json
Content-length: 314

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotPolicyStatusDetail",
  "displayName": "Display Name value",
  "policyType": "application",
  "complianceStatus": "compliant",
  "trackedOnEnrollmentStatus": true,
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "errorCode": 9
}
```

### <a name="response"></a><span data-ttu-id="2785e-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="2785e-162">Response</span></span>
<span data-ttu-id="2785e-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2785e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 363

{
  "@odata.type": "#microsoft.graph.deviceManagementAutopilotPolicyStatusDetail",
  "id": "dbe093ee-93ee-dbe0-ee93-e0dbee93e0db",
  "displayName": "Display Name value",
  "policyType": "application",
  "complianceStatus": "compliant",
  "trackedOnEnrollmentStatus": true,
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "errorCode": 9
}
```




