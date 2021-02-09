---
title: Atualizar deviceManagementAutopilotPolicyStatusDetail
description: Atualizar as propriedades de um objeto deviceManagementAutopilotPolicyStatusDetail.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b8e38d9ae11c0eb34d92681725fcd3173e2d9a9b
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155626"
---
# <a name="update-devicemanagementautopilotpolicystatusdetail"></a><span data-ttu-id="d4799-103">Atualizar deviceManagementAutopilotPolicyStatusDetail</span><span class="sxs-lookup"><span data-stu-id="d4799-103">Update deviceManagementAutopilotPolicyStatusDetail</span></span>

<span data-ttu-id="d4799-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4799-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d4799-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d4799-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4799-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d4799-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4799-107">Atualizar as propriedades de um [objeto deviceManagementAutopilotPolicyStatusDetail.](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)</span><span class="sxs-lookup"><span data-stu-id="d4799-107">Update the properties of a [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4799-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d4799-108">Prerequisites</span></span>
<span data-ttu-id="d4799-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4799-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4799-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4799-111">Permission type</span></span>|<span data-ttu-id="d4799-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d4799-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4799-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4799-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d4799-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4799-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="d4799-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4799-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4799-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4799-116">Not supported.</span></span>|
|<span data-ttu-id="d4799-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4799-117">Application</span></span>|<span data-ttu-id="d4799-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4799-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4799-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4799-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails/{deviceManagementAutopilotPolicyStatusDetailId}
```

## <a name="request-headers"></a><span data-ttu-id="d4799-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4799-120">Request headers</span></span>
|<span data-ttu-id="d4799-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d4799-121">Header</span></span>|<span data-ttu-id="d4799-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d4799-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4799-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4799-123">Authorization</span></span>|<span data-ttu-id="d4799-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4799-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4799-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d4799-125">Accept</span></span>|<span data-ttu-id="d4799-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d4799-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4799-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4799-127">Request body</span></span>
<span data-ttu-id="d4799-128">No corpo da solicitação, fornece uma representação JSON do [objeto deviceManagementAutopilotPolicyStatusDetail.](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md)</span><span class="sxs-lookup"><span data-stu-id="d4799-128">In the request body, supply a JSON representation for the [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object.</span></span>

<span data-ttu-id="d4799-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md).</span><span class="sxs-lookup"><span data-stu-id="d4799-129">The following table shows the properties that are required when you create the [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md).</span></span>

|<span data-ttu-id="d4799-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d4799-130">Property</span></span>|<span data-ttu-id="d4799-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4799-131">Type</span></span>|<span data-ttu-id="d4799-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4799-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4799-133">id</span><span class="sxs-lookup"><span data-stu-id="d4799-133">id</span></span>|<span data-ttu-id="d4799-134">String</span><span class="sxs-lookup"><span data-stu-id="d4799-134">String</span></span>|<span data-ttu-id="d4799-135">O UUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="d4799-135">UUID for the object</span></span>|
|<span data-ttu-id="d4799-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d4799-136">displayName</span></span>|<span data-ttu-id="d4799-137">String</span><span class="sxs-lookup"><span data-stu-id="d4799-137">String</span></span>|<span data-ttu-id="d4799-138">O nome amigável da política.</span><span class="sxs-lookup"><span data-stu-id="d4799-138">The friendly name of the policy.</span></span>|
|<span data-ttu-id="d4799-139">policyType</span><span class="sxs-lookup"><span data-stu-id="d4799-139">policyType</span></span>|[<span data-ttu-id="d4799-140">deviceManagementAutopilotPolicyType</span><span class="sxs-lookup"><span data-stu-id="d4799-140">deviceManagementAutopilotPolicyType</span></span>](../resources/intune-troubleshooting-devicemanagementautopilotpolicytype.md)|<span data-ttu-id="d4799-141">O tipo de política.</span><span class="sxs-lookup"><span data-stu-id="d4799-141">The type of policy.</span></span> <span data-ttu-id="d4799-142">Os valores possíveis são: `unknown`, `application`, `appModel`, `configurationPolicy`.</span><span class="sxs-lookup"><span data-stu-id="d4799-142">Possible values are: `unknown`, `application`, `appModel`, `configurationPolicy`.</span></span>|
|<span data-ttu-id="d4799-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="d4799-143">complianceStatus</span></span>|[<span data-ttu-id="d4799-144">deviceManagementAutopilotPolicyComplianceStatus</span><span class="sxs-lookup"><span data-stu-id="d4799-144">deviceManagementAutopilotPolicyComplianceStatus</span></span>](../resources/intune-troubleshooting-devicemanagementautopilotpolicycompliancestatus.md)|<span data-ttu-id="d4799-145">O status de conformidade da política.</span><span class="sxs-lookup"><span data-stu-id="d4799-145">The policy compliance status.</span></span> <span data-ttu-id="d4799-146">Os possíveis valores são: `unknown`, `compliant`, `installed`, `notCompliant`, `notInstalled`, `error`.</span><span class="sxs-lookup"><span data-stu-id="d4799-146">Possible values are: `unknown`, `compliant`, `installed`, `notCompliant`, `notInstalled`, `error`.</span></span>|
|<span data-ttu-id="d4799-147">trackedOnEnrollmentStatus</span><span class="sxs-lookup"><span data-stu-id="d4799-147">trackedOnEnrollmentStatus</span></span>|<span data-ttu-id="d4799-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4799-148">Boolean</span></span>|<span data-ttu-id="d4799-149">Indica se esse prolicy foi rastreado como parte da sessão de sincronização de registro de inicialização do autopilot</span><span class="sxs-lookup"><span data-stu-id="d4799-149">Indicates if this prolicy was tracked as part of the autopilot bootstrap enrollment sync session</span></span>|
|<span data-ttu-id="d4799-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4799-150">lastReportedDateTime</span></span>|<span data-ttu-id="d4799-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4799-151">DateTimeOffset</span></span>|<span data-ttu-id="d4799-152">Timestamp do status de política relatado</span><span class="sxs-lookup"><span data-stu-id="d4799-152">Timestamp of the reported policy status</span></span>|
|<span data-ttu-id="d4799-153">errorCode</span><span class="sxs-lookup"><span data-stu-id="d4799-153">errorCode</span></span>|<span data-ttu-id="d4799-154">Int32</span><span class="sxs-lookup"><span data-stu-id="d4799-154">Int32</span></span>|<span data-ttu-id="d4799-155">O errorode associado ao status de conformidade ou imposição da política.</span><span class="sxs-lookup"><span data-stu-id="d4799-155">The errorode associated with the compliance or enforcement status of the policy.</span></span> <span data-ttu-id="d4799-156">O código de erro para o status de imposição tem precedência, se existir.</span><span class="sxs-lookup"><span data-stu-id="d4799-156">Error code for enforcement status takes precedence if it exists.</span></span>|



## <a name="response"></a><span data-ttu-id="d4799-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4799-157">Response</span></span>
<span data-ttu-id="d4799-158">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4799-158">If successful, this method returns a `200 OK` response code and an updated [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4799-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d4799-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4799-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4799-160">Request</span></span>
<span data-ttu-id="d4799-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4799-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails/{deviceManagementAutopilotPolicyStatusDetailId}
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

### <a name="response"></a><span data-ttu-id="d4799-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4799-162">Response</span></span>
<span data-ttu-id="d4799-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d4799-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




