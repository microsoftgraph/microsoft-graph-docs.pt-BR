---
title: Atualizar deviceManagementAutopilotPolicyStatusDetail
description: Atualiza as propriedades de um objeto deviceManagementAutopilotPolicyStatusDetail.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d5b1d364bdfbbbdde7088cb8f7150665bb03392a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43467118"
---
# <a name="update-devicemanagementautopilotpolicystatusdetail"></a><span data-ttu-id="745b7-103">Atualizar deviceManagementAutopilotPolicyStatusDetail</span><span class="sxs-lookup"><span data-stu-id="745b7-103">Update deviceManagementAutopilotPolicyStatusDetail</span></span>

<span data-ttu-id="745b7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="745b7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="745b7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="745b7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="745b7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="745b7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="745b7-107">Atualiza as propriedades de um objeto [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) .</span><span class="sxs-lookup"><span data-stu-id="745b7-107">Update the properties of a [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="745b7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="745b7-108">Prerequisites</span></span>
<span data-ttu-id="745b7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="745b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="745b7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="745b7-111">Permission type</span></span>|<span data-ttu-id="745b7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="745b7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="745b7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="745b7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="745b7-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="745b7-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="745b7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="745b7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="745b7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="745b7-116">Not supported.</span></span>|
|<span data-ttu-id="745b7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="745b7-117">Application</span></span>|<span data-ttu-id="745b7-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="745b7-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="745b7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="745b7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails/{deviceManagementAutopilotPolicyStatusDetailId}
```

## <a name="request-headers"></a><span data-ttu-id="745b7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="745b7-120">Request headers</span></span>
|<span data-ttu-id="745b7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="745b7-121">Header</span></span>|<span data-ttu-id="745b7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="745b7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="745b7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="745b7-123">Authorization</span></span>|<span data-ttu-id="745b7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="745b7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="745b7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="745b7-125">Accept</span></span>|<span data-ttu-id="745b7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="745b7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="745b7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="745b7-127">Request body</span></span>
<span data-ttu-id="745b7-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) .</span><span class="sxs-lookup"><span data-stu-id="745b7-128">In the request body, supply a JSON representation for the [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object.</span></span>

<span data-ttu-id="745b7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md).</span><span class="sxs-lookup"><span data-stu-id="745b7-129">The following table shows the properties that are required when you create the [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md).</span></span>

|<span data-ttu-id="745b7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="745b7-130">Property</span></span>|<span data-ttu-id="745b7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="745b7-131">Type</span></span>|<span data-ttu-id="745b7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="745b7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="745b7-133">id</span><span class="sxs-lookup"><span data-stu-id="745b7-133">id</span></span>|<span data-ttu-id="745b7-134">String</span><span class="sxs-lookup"><span data-stu-id="745b7-134">String</span></span>|<span data-ttu-id="745b7-135">O UUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="745b7-135">UUID for the object</span></span>|
|<span data-ttu-id="745b7-136">displayName</span><span class="sxs-lookup"><span data-stu-id="745b7-136">displayName</span></span>|<span data-ttu-id="745b7-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="745b7-137">String</span></span>|<span data-ttu-id="745b7-138">O nome amigável da política.</span><span class="sxs-lookup"><span data-stu-id="745b7-138">The friendly name of the policy.</span></span>|
|<span data-ttu-id="745b7-139">PolicyType</span><span class="sxs-lookup"><span data-stu-id="745b7-139">policyType</span></span>|[<span data-ttu-id="745b7-140">deviceManagementAutopilotPolicyType</span><span class="sxs-lookup"><span data-stu-id="745b7-140">deviceManagementAutopilotPolicyType</span></span>](../resources/intune-troubleshooting-devicemanagementautopilotpolicytype.md)|<span data-ttu-id="745b7-141">O tipo de política.</span><span class="sxs-lookup"><span data-stu-id="745b7-141">The type of policy.</span></span> <span data-ttu-id="745b7-142">Os valores possíveis são: `unknown`, `application`, `appModel`, `configurationPolicy`.</span><span class="sxs-lookup"><span data-stu-id="745b7-142">Possible values are: `unknown`, `application`, `appModel`, `configurationPolicy`.</span></span>|
|<span data-ttu-id="745b7-143">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="745b7-143">complianceStatus</span></span>|[<span data-ttu-id="745b7-144">deviceManagementAutopilotPolicyComplianceStatus</span><span class="sxs-lookup"><span data-stu-id="745b7-144">deviceManagementAutopilotPolicyComplianceStatus</span></span>](../resources/intune-troubleshooting-devicemanagementautopilotpolicycompliancestatus.md)|<span data-ttu-id="745b7-145">O status de conformidade da política.</span><span class="sxs-lookup"><span data-stu-id="745b7-145">The policy compliance status.</span></span> <span data-ttu-id="745b7-146">Os possíveis valores são: `unknown`, `compliant`, `installed`, `notCompliant`, `notInstalled`, `error`.</span><span class="sxs-lookup"><span data-stu-id="745b7-146">Possible values are: `unknown`, `compliant`, `installed`, `notCompliant`, `notInstalled`, `error`.</span></span>|
|<span data-ttu-id="745b7-147">trackedOnEnrollmentStatus</span><span class="sxs-lookup"><span data-stu-id="745b7-147">trackedOnEnrollmentStatus</span></span>|<span data-ttu-id="745b7-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="745b7-148">Boolean</span></span>|<span data-ttu-id="745b7-149">Indica se este prolicy foi rastreado como parte da sessão de sincronização do registro de inicialização do AutoPilot</span><span class="sxs-lookup"><span data-stu-id="745b7-149">Indicates if this prolicy was tracked as part of the autopilot bootstrap enrollment sync session</span></span>|
|<span data-ttu-id="745b7-150">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="745b7-150">lastReportedDateTime</span></span>|<span data-ttu-id="745b7-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="745b7-151">DateTimeOffset</span></span>|<span data-ttu-id="745b7-152">Carimbo de data/hora do status da política relatado</span><span class="sxs-lookup"><span data-stu-id="745b7-152">Timestamp of the reported policy status</span></span>|



## <a name="response"></a><span data-ttu-id="745b7-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="745b7-153">Response</span></span>
<span data-ttu-id="745b7-154">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="745b7-154">If successful, this method returns a `200 OK` response code and an updated [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="745b7-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="745b7-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="745b7-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="745b7-156">Request</span></span>
<span data-ttu-id="745b7-157">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="745b7-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails/{deviceManagementAutopilotPolicyStatusDetailId}
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

### <a name="response"></a><span data-ttu-id="745b7-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="745b7-158">Response</span></span>
<span data-ttu-id="745b7-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="745b7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



