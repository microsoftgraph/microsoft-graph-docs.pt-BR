---
title: Criar deviceManagementAutopilotPolicyStatusDetail
description: Crie um novo objeto deviceManagementAutopilotPolicyStatusDetail.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f3f2b6614d980911c35babfa71425a2e5b0ac7e3
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134190"
---
# <a name="create-devicemanagementautopilotpolicystatusdetail"></a><span data-ttu-id="6c769-103">Criar deviceManagementAutopilotPolicyStatusDetail</span><span class="sxs-lookup"><span data-stu-id="6c769-103">Create deviceManagementAutopilotPolicyStatusDetail</span></span>

<span data-ttu-id="6c769-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c769-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6c769-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6c769-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c769-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6c769-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c769-107">Crie um novo [objeto deviceManagementAutopilotPolicyStatusDetail.](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)</span><span class="sxs-lookup"><span data-stu-id="6c769-107">Create a new [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c769-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6c769-108">Prerequisites</span></span>
<span data-ttu-id="6c769-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c769-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c769-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c769-111">Permission type</span></span>|<span data-ttu-id="6c769-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6c769-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c769-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c769-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6c769-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c769-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6c769-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c769-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c769-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c769-116">Not supported.</span></span>|
|<span data-ttu-id="6c769-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c769-117">Application</span></span>|<span data-ttu-id="6c769-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c769-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c769-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c769-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails
```

## <a name="request-headers"></a><span data-ttu-id="6c769-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c769-120">Request headers</span></span>
|<span data-ttu-id="6c769-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6c769-121">Header</span></span>|<span data-ttu-id="6c769-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6c769-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c769-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c769-123">Authorization</span></span>|<span data-ttu-id="6c769-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c769-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c769-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6c769-125">Accept</span></span>|<span data-ttu-id="6c769-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6c769-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c769-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c769-127">Request body</span></span>
<span data-ttu-id="6c769-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceManagementAutopilotPolicyStatusDetail.</span><span class="sxs-lookup"><span data-stu-id="6c769-128">In the request body, supply a JSON representation for the deviceManagementAutopilotPolicyStatusDetail object.</span></span>

<span data-ttu-id="6c769-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementAutopilotPolicyStatusDetail.</span><span class="sxs-lookup"><span data-stu-id="6c769-129">The following table shows the properties that are required when you create the deviceManagementAutopilotPolicyStatusDetail.</span></span>

|<span data-ttu-id="6c769-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c769-130">Property</span></span>|<span data-ttu-id="6c769-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c769-131">Type</span></span>|<span data-ttu-id="6c769-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c769-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c769-133">id</span><span class="sxs-lookup"><span data-stu-id="6c769-133">id</span></span>|<span data-ttu-id="6c769-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c769-134">String</span></span>|<span data-ttu-id="6c769-135">O UUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="6c769-135">UUID for the object</span></span>|
|<span data-ttu-id="6c769-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6c769-136">displayName</span></span>|<span data-ttu-id="6c769-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c769-137">String</span></span>|<span data-ttu-id="6c769-138">O nome amigável da política.</span><span class="sxs-lookup"><span data-stu-id="6c769-138">The friendly name of the policy.</span></span>|
|<span data-ttu-id="6c769-139">policyType</span><span class="sxs-lookup"><span data-stu-id="6c769-139">policyType</span></span>|[<span data-ttu-id="6c769-140">deviceManagementAutopilotPolicyType</span><span class="sxs-lookup"><span data-stu-id="6c769-140">deviceManagementAutopilotPolicyType</span></span>](../resources/intune-troubleshooting-devicemanagementautopilotpolicytype.md)|<span data-ttu-id="6c769-141">O tipo de política.</span><span class="sxs-lookup"><span data-stu-id="6c769-141">The type of policy.</span></span> <span data-ttu-id="6c769-142">Os valores possíveis são: `unknown`, `application`, `appModel`, `configurationPolicy`.</span><span class="sxs-lookup"><span data-stu-id="6c769-142">Possible values are: `unknown`, `application`, `appModel`, `configurationPolicy`.</span></span>|
|<span data-ttu-id="6c769-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="6c769-143">complianceStatus</span></span>|[<span data-ttu-id="6c769-144">deviceManagementAutopilotPolicyComplianceStatus</span><span class="sxs-lookup"><span data-stu-id="6c769-144">deviceManagementAutopilotPolicyComplianceStatus</span></span>](../resources/intune-troubleshooting-devicemanagementautopilotpolicycompliancestatus.md)|<span data-ttu-id="6c769-145">O status de conformidade da política.</span><span class="sxs-lookup"><span data-stu-id="6c769-145">The policy compliance status.</span></span> <span data-ttu-id="6c769-146">Os possíveis valores são: `unknown`, `compliant`, `installed`, `notCompliant`, `notInstalled`, `error`.</span><span class="sxs-lookup"><span data-stu-id="6c769-146">Possible values are: `unknown`, `compliant`, `installed`, `notCompliant`, `notInstalled`, `error`.</span></span>|
|<span data-ttu-id="6c769-147">trackedOnEnrollmentStatus</span><span class="sxs-lookup"><span data-stu-id="6c769-147">trackedOnEnrollmentStatus</span></span>|<span data-ttu-id="6c769-148">Booleano</span><span class="sxs-lookup"><span data-stu-id="6c769-148">Boolean</span></span>|<span data-ttu-id="6c769-149">Indica se essa prolicy foi controlada como parte da sessão de sincronização de registro de inicialização de inicialização do piloto automático</span><span class="sxs-lookup"><span data-stu-id="6c769-149">Indicates if this prolicy was tracked as part of the autopilot bootstrap enrollment sync session</span></span>|
|<span data-ttu-id="6c769-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c769-150">lastReportedDateTime</span></span>|<span data-ttu-id="6c769-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c769-151">DateTimeOffset</span></span>|<span data-ttu-id="6c769-152">Timestamp do status da política relatada</span><span class="sxs-lookup"><span data-stu-id="6c769-152">Timestamp of the reported policy status</span></span>|
|<span data-ttu-id="6c769-153">errorCode</span><span class="sxs-lookup"><span data-stu-id="6c769-153">errorCode</span></span>|<span data-ttu-id="6c769-154">Int32</span><span class="sxs-lookup"><span data-stu-id="6c769-154">Int32</span></span>|<span data-ttu-id="6c769-155">O errorode associado ao status de conformidade ou imposição da política.</span><span class="sxs-lookup"><span data-stu-id="6c769-155">The errorode associated with the compliance or enforcement status of the policy.</span></span> <span data-ttu-id="6c769-156">O código de erro para o status de imposição tem precedência se existir.</span><span class="sxs-lookup"><span data-stu-id="6c769-156">Error code for enforcement status takes precedence if it exists.</span></span>|



## <a name="response"></a><span data-ttu-id="6c769-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c769-157">Response</span></span>
<span data-ttu-id="6c769-158">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6c769-158">If successful, this method returns a `201 Created` response code and a [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c769-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6c769-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c769-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c769-160">Request</span></span>
<span data-ttu-id="6c769-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c769-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6c769-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c769-162">Response</span></span>
<span data-ttu-id="6c769-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c769-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




