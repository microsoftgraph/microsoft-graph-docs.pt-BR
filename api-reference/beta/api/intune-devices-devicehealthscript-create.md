---
title: Criar deviceHealthScript
description: Criar um novo objeto deviceHealthScript.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0084852f4c0cb236931ee532f12e54a08c1e2fc2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36311613"
---
# <a name="create-devicehealthscript"></a><span data-ttu-id="e1183-103">Criar deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="e1183-103">Create deviceHealthScript</span></span>

> <span data-ttu-id="e1183-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e1183-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1183-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e1183-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1183-106">Criar um novo objeto [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) .</span><span class="sxs-lookup"><span data-stu-id="e1183-106">Create a new [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1183-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e1183-107">Prerequisites</span></span>
<span data-ttu-id="e1183-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1183-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1183-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1183-110">Permission type</span></span>|<span data-ttu-id="e1183-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e1183-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1183-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1183-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e1183-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1183-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e1183-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1183-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1183-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1183-115">Not supported.</span></span>|
|<span data-ttu-id="e1183-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1183-116">Application</span></span>|<span data-ttu-id="e1183-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1183-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1183-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1183-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="e1183-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1183-119">Request headers</span></span>
|<span data-ttu-id="e1183-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e1183-120">Header</span></span>|<span data-ttu-id="e1183-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e1183-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1183-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1183-122">Authorization</span></span>|<span data-ttu-id="e1183-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1183-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1183-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e1183-124">Accept</span></span>|<span data-ttu-id="e1183-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e1183-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1183-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1183-126">Request body</span></span>
<span data-ttu-id="e1183-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceHealthScript.</span><span class="sxs-lookup"><span data-stu-id="e1183-127">In the request body, supply a JSON representation for the deviceHealthScript object.</span></span>

<span data-ttu-id="e1183-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceHealthScript.</span><span class="sxs-lookup"><span data-stu-id="e1183-128">The following table shows the properties that are required when you create the deviceHealthScript.</span></span>

|<span data-ttu-id="e1183-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1183-129">Property</span></span>|<span data-ttu-id="e1183-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1183-130">Type</span></span>|<span data-ttu-id="e1183-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1183-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1183-132">id</span><span class="sxs-lookup"><span data-stu-id="e1183-132">id</span></span>|<span data-ttu-id="e1183-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1183-133">String</span></span>|<span data-ttu-id="e1183-134">Identificador exclusivo do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e1183-134">Unique Identifier for the device management script.</span></span> <span data-ttu-id="e1183-135">Herdado de [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="e1183-135">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="e1183-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e1183-136">displayName</span></span>|<span data-ttu-id="e1183-137">String</span><span class="sxs-lookup"><span data-stu-id="e1183-137">String</span></span>|<span data-ttu-id="e1183-138">Nome do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e1183-138">Name of the device management script.</span></span> <span data-ttu-id="e1183-139">Herdado de [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="e1183-139">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="e1183-140">descrição</span><span class="sxs-lookup"><span data-stu-id="e1183-140">description</span></span>|<span data-ttu-id="e1183-141">String</span><span class="sxs-lookup"><span data-stu-id="e1183-141">String</span></span>|<span data-ttu-id="e1183-142">Descrição opcional para o script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e1183-142">Optional description for the device management script.</span></span> <span data-ttu-id="e1183-143">Herdado de [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="e1183-143">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="e1183-144">runSchedule</span><span class="sxs-lookup"><span data-stu-id="e1183-144">runSchedule</span></span>|[<span data-ttu-id="e1183-145">runSchedule</span><span class="sxs-lookup"><span data-stu-id="e1183-145">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="e1183-146">O intervalo de execução do script.</span><span class="sxs-lookup"><span data-stu-id="e1183-146">The interval for script to run.</span></span> <span data-ttu-id="e1183-147">Se não definido, o script será executado uma vez herdado de [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="e1183-147">If not defined the script will run once Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="e1183-148">scriptContent</span><span class="sxs-lookup"><span data-stu-id="e1183-148">scriptContent</span></span>|<span data-ttu-id="e1183-149">Binária</span><span class="sxs-lookup"><span data-stu-id="e1183-149">Binary</span></span>|<span data-ttu-id="e1183-150">O conteúdo de script.</span><span class="sxs-lookup"><span data-stu-id="e1183-150">The script content.</span></span> <span data-ttu-id="e1183-151">Herdado de [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="e1183-151">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="e1183-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e1183-152">createdDateTime</span></span>|<span data-ttu-id="e1183-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1183-153">DateTimeOffset</span></span>|<span data-ttu-id="e1183-154">A data e a hora em que o script de gerenciamento de dispositivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="e1183-154">The date and time the device management script was created.</span></span> <span data-ttu-id="e1183-155">Herdado de [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="e1183-155">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="e1183-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e1183-156">lastModifiedDateTime</span></span>|<span data-ttu-id="e1183-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1183-157">DateTimeOffset</span></span>|<span data-ttu-id="e1183-158">A data e a hora em que o script de gerenciamento de dispositivo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="e1183-158">The date and time the device management script was last modified.</span></span> <span data-ttu-id="e1183-159">Herdado de [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="e1183-159">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="e1183-160">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="e1183-160">runAsAccount</span></span>|[<span data-ttu-id="e1183-161">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="e1183-161">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="e1183-162">Indica o tipo de contexto de execução.</span><span class="sxs-lookup"><span data-stu-id="e1183-162">Indicates the type of execution context.</span></span> <span data-ttu-id="e1183-163">Herdado de [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).</span><span class="sxs-lookup"><span data-stu-id="e1183-163">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).</span></span> <span data-ttu-id="e1183-164">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="e1183-164">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="e1183-165">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="e1183-165">enforceSignatureCheck</span></span>|<span data-ttu-id="e1183-166">Booliano</span><span class="sxs-lookup"><span data-stu-id="e1183-166">Boolean</span></span>|<span data-ttu-id="e1183-167">Indica se a assinatura do script precisa ser verificada.</span><span class="sxs-lookup"><span data-stu-id="e1183-167">Indicate whether the script signature needs be checked.</span></span> <span data-ttu-id="e1183-168">Herdado de [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="e1183-168">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="e1183-169">fileName</span><span class="sxs-lookup"><span data-stu-id="e1183-169">fileName</span></span>|<span data-ttu-id="e1183-170">String</span><span class="sxs-lookup"><span data-stu-id="e1183-170">String</span></span>|<span data-ttu-id="e1183-171">Nome do arquivo de script.</span><span class="sxs-lookup"><span data-stu-id="e1183-171">Script file name.</span></span> <span data-ttu-id="e1183-172">Herdado de [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="e1183-172">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="e1183-173">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e1183-173">roleScopeTagIds</span></span>|<span data-ttu-id="e1183-174">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e1183-174">String collection</span></span>|<span data-ttu-id="e1183-175">Lista de IDs de marca de escopo para esta instância de PowerShellScript.</span><span class="sxs-lookup"><span data-stu-id="e1183-175">List of Scope Tag IDs for this PowerShellScript instance.</span></span> <span data-ttu-id="e1183-176">Herdado de [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="e1183-176">Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="e1183-177">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="e1183-177">runAs32Bit</span></span>|<span data-ttu-id="e1183-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="e1183-178">Boolean</span></span>|<span data-ttu-id="e1183-179">Um valor que indica se o script do PowerShell deve ser executado como 32 bits herdado de [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="e1183-179">A value indicating whether the PowerShell script should run as 32-bit Inherited from [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="e1183-180">complianceRule</span><span class="sxs-lookup"><span data-stu-id="e1183-180">complianceRule</span></span>|[<span data-ttu-id="e1183-181">deviceHealthScriptComplianceRule</span><span class="sxs-lookup"><span data-stu-id="e1183-181">deviceHealthScriptComplianceRule</span></span>](../resources/intune-devices-devicehealthscriptcompliancerule.md)|<span data-ttu-id="e1183-182">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e1183-182">Not yet documented</span></span>|
|<span data-ttu-id="e1183-183">remediationScriptContent</span><span class="sxs-lookup"><span data-stu-id="e1183-183">remediationScriptContent</span></span>|<span data-ttu-id="e1183-184">Binária</span><span class="sxs-lookup"><span data-stu-id="e1183-184">Binary</span></span>|<span data-ttu-id="e1183-185">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e1183-185">Not yet documented</span></span>|
|<span data-ttu-id="e1183-186">runRemediationScript</span><span class="sxs-lookup"><span data-stu-id="e1183-186">runRemediationScript</span></span>|<span data-ttu-id="e1183-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="e1183-187">Boolean</span></span>|<span data-ttu-id="e1183-188">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e1183-188">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e1183-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1183-189">Response</span></span>
<span data-ttu-id="e1183-190">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1183-190">If successful, this method returns a `201 Created` response code and a [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1183-191">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1183-191">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1183-192">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1183-192">Request</span></span>
<span data-ttu-id="e1183-193">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1183-193">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
Content-type: application/json
Content-length: 745

{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
  "displayName": "Display Name value",
  "description": "Description value",
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "runAs32Bit": true,
  "complianceRule": {
    "@odata.type": "microsoft.graph.deviceHealthScriptComplianceRule",
    "detectionType": "string",
    "operator": "equal",
    "detectionValue": "Detection Value value"
  },
  "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
  "runRemediationScript": true
}
```

### <a name="response"></a><span data-ttu-id="e1183-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1183-194">Response</span></span>
<span data-ttu-id="e1183-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1183-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 917

{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
  "id": "bcb60502-0502-bcb6-0205-b6bc0205b6bc",
  "displayName": "Display Name value",
  "description": "Description value",
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "runAs32Bit": true,
  "complianceRule": {
    "@odata.type": "microsoft.graph.deviceHealthScriptComplianceRule",
    "detectionType": "string",
    "operator": "equal",
    "detectionValue": "Detection Value value"
  },
  "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
  "runRemediationScript": true
}
```






