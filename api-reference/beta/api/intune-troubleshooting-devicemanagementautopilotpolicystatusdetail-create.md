---
title: Criar deviceManagementAutopilotPolicyStatusDetail
description: Criar um novo objeto deviceManagementAutopilotPolicyStatusDetail.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 11b7f197a69022c9de547cb998fb14c8d6e9f2d1
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800225"
---
# <a name="create-devicemanagementautopilotpolicystatusdetail"></a><span data-ttu-id="6887c-103">Criar deviceManagementAutopilotPolicyStatusDetail</span><span class="sxs-lookup"><span data-stu-id="6887c-103">Create deviceManagementAutopilotPolicyStatusDetail</span></span>

> <span data-ttu-id="6887c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6887c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6887c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6887c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6887c-106">Criar um novo objeto [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) .</span><span class="sxs-lookup"><span data-stu-id="6887c-106">Create a new [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6887c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6887c-107">Prerequisites</span></span>
<span data-ttu-id="6887c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6887c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6887c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6887c-110">Permission type</span></span>|<span data-ttu-id="6887c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6887c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6887c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6887c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6887c-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6887c-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6887c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6887c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6887c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6887c-115">Not supported.</span></span>|
|<span data-ttu-id="6887c-116">Application</span><span class="sxs-lookup"><span data-stu-id="6887c-116">Application</span></span>|<span data-ttu-id="6887c-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6887c-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6887c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6887c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/autopilotEvents/{deviceManagementAutopilotEventId}/policyStatusDetails
```

## <a name="request-headers"></a><span data-ttu-id="6887c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6887c-119">Request headers</span></span>
|<span data-ttu-id="6887c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6887c-120">Header</span></span>|<span data-ttu-id="6887c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6887c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6887c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6887c-122">Authorization</span></span>|<span data-ttu-id="6887c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6887c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6887c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6887c-124">Accept</span></span>|<span data-ttu-id="6887c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6887c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6887c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6887c-126">Request body</span></span>
<span data-ttu-id="6887c-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementAutopilotPolicyStatusDetail.</span><span class="sxs-lookup"><span data-stu-id="6887c-127">In the request body, supply a JSON representation for the deviceManagementAutopilotPolicyStatusDetail object.</span></span>

<span data-ttu-id="6887c-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementAutopilotPolicyStatusDetail.</span><span class="sxs-lookup"><span data-stu-id="6887c-128">The following table shows the properties that are required when you create the deviceManagementAutopilotPolicyStatusDetail.</span></span>

|<span data-ttu-id="6887c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6887c-129">Property</span></span>|<span data-ttu-id="6887c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6887c-130">Type</span></span>|<span data-ttu-id="6887c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6887c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6887c-132">id</span><span class="sxs-lookup"><span data-stu-id="6887c-132">id</span></span>|<span data-ttu-id="6887c-133">String</span><span class="sxs-lookup"><span data-stu-id="6887c-133">String</span></span>|<span data-ttu-id="6887c-134">O UUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="6887c-134">UUID for the object</span></span>|
|<span data-ttu-id="6887c-135">displayName</span><span class="sxs-lookup"><span data-stu-id="6887c-135">displayName</span></span>|<span data-ttu-id="6887c-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6887c-136">String</span></span>|<span data-ttu-id="6887c-137">O nome amigável da política.</span><span class="sxs-lookup"><span data-stu-id="6887c-137">The friendly name of the policy.</span></span>|
|<span data-ttu-id="6887c-138">PolicyType</span><span class="sxs-lookup"><span data-stu-id="6887c-138">policyType</span></span>|[<span data-ttu-id="6887c-139">deviceManagementAutopilotPolicyType</span><span class="sxs-lookup"><span data-stu-id="6887c-139">deviceManagementAutopilotPolicyType</span></span>](../resources/intune-troubleshooting-devicemanagementautopilotpolicytype.md)|<span data-ttu-id="6887c-140">O tipo de política.</span><span class="sxs-lookup"><span data-stu-id="6887c-140">The type of policy.</span></span> <span data-ttu-id="6887c-141">Os valores possíveis são: `unknown`, `application`, `appModel`, `configurationPolicy`.</span><span class="sxs-lookup"><span data-stu-id="6887c-141">Possible values are: `unknown`, `application`, `appModel`, `configurationPolicy`.</span></span>|
|<span data-ttu-id="6887c-142">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="6887c-142">complianceStatus</span></span>|[<span data-ttu-id="6887c-143">deviceManagementAutopilotPolicyComplianceStatus</span><span class="sxs-lookup"><span data-stu-id="6887c-143">deviceManagementAutopilotPolicyComplianceStatus</span></span>](../resources/intune-troubleshooting-devicemanagementautopilotpolicycompliancestatus.md)|<span data-ttu-id="6887c-144">O status de conformidade da política.</span><span class="sxs-lookup"><span data-stu-id="6887c-144">The policy compliance status.</span></span> <span data-ttu-id="6887c-145">Os possíveis valores são: `unknown`, `compliant`, `installed`, `notCompliant`, `notInstalled`, `error`.</span><span class="sxs-lookup"><span data-stu-id="6887c-145">Possible values are: `unknown`, `compliant`, `installed`, `notCompliant`, `notInstalled`, `error`.</span></span>|
|<span data-ttu-id="6887c-146">trackedOnEnrollmentStatus</span><span class="sxs-lookup"><span data-stu-id="6887c-146">trackedOnEnrollmentStatus</span></span>|<span data-ttu-id="6887c-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="6887c-147">Boolean</span></span>|<span data-ttu-id="6887c-148">Indica se este prolicy foi rastreado como parte da sessão de sincronização do registro de inicialização do AutoPilot</span><span class="sxs-lookup"><span data-stu-id="6887c-148">Indicates if this prolicy was tracked as part of the autopilot bootstrap enrollment sync session</span></span>|
|<span data-ttu-id="6887c-149">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="6887c-149">lastReportedDateTime</span></span>|<span data-ttu-id="6887c-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6887c-150">DateTimeOffset</span></span>|<span data-ttu-id="6887c-151">Carimbo de data/hora do status da política relatado</span><span class="sxs-lookup"><span data-stu-id="6887c-151">Timestamp of the reported policy status</span></span>|



## <a name="response"></a><span data-ttu-id="6887c-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="6887c-152">Response</span></span>
<span data-ttu-id="6887c-153">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6887c-153">If successful, this method returns a `201 Created` response code and a [deviceManagementAutopilotPolicyStatusDetail](../resources/intune-troubleshooting-devicemanagementautopilotpolicystatusdetail.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6887c-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6887c-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="6887c-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6887c-155">Request</span></span>
<span data-ttu-id="6887c-156">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6887c-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6887c-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="6887c-157">Response</span></span>
<span data-ttu-id="6887c-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6887c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




