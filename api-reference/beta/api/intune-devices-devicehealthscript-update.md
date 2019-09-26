---
title: Atualizar deviceHealthScript
description: Atualiza as propriedades de um objeto deviceHealthScript.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 246f7d00920a096e4e1af328e7bcb7d76c3ba448
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37188630"
---
# <a name="update-devicehealthscript"></a><span data-ttu-id="14107-103">Atualizar deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="14107-103">Update deviceHealthScript</span></span>

> <span data-ttu-id="14107-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="14107-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14107-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="14107-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14107-106">Atualiza as propriedades de um objeto [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) .</span><span class="sxs-lookup"><span data-stu-id="14107-106">Update the properties of a [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14107-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="14107-107">Prerequisites</span></span>
<span data-ttu-id="14107-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14107-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14107-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14107-110">Permission type</span></span>|<span data-ttu-id="14107-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="14107-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14107-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14107-112">Delegated (work or school account)</span></span>|<span data-ttu-id="14107-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14107-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="14107-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14107-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14107-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14107-115">Not supported.</span></span>|
|<span data-ttu-id="14107-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="14107-116">Application</span></span>|<span data-ttu-id="14107-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14107-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="14107-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14107-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="14107-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14107-119">Request headers</span></span>
|<span data-ttu-id="14107-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="14107-120">Header</span></span>|<span data-ttu-id="14107-121">Valor</span><span class="sxs-lookup"><span data-stu-id="14107-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14107-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="14107-122">Authorization</span></span>|<span data-ttu-id="14107-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14107-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14107-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="14107-124">Accept</span></span>|<span data-ttu-id="14107-125">application/json</span><span class="sxs-lookup"><span data-stu-id="14107-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14107-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="14107-126">Request body</span></span>
<span data-ttu-id="14107-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) .</span><span class="sxs-lookup"><span data-stu-id="14107-127">In the request body, supply a JSON representation for the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

<span data-ttu-id="14107-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceHealthScript](../resources/intune-devices-devicehealthscript.md).</span><span class="sxs-lookup"><span data-stu-id="14107-128">The following table shows the properties that are required when you create the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md).</span></span>

|<span data-ttu-id="14107-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="14107-129">Property</span></span>|<span data-ttu-id="14107-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="14107-130">Type</span></span>|<span data-ttu-id="14107-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="14107-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14107-132">id</span><span class="sxs-lookup"><span data-stu-id="14107-132">id</span></span>|<span data-ttu-id="14107-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="14107-133">String</span></span>|<span data-ttu-id="14107-134">Identificador exclusivo do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="14107-134">Unique Identifier for the device management script.</span></span> <span data-ttu-id="14107-135">Herdado de [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="14107-135">Inherited from [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="14107-136">displayName</span><span class="sxs-lookup"><span data-stu-id="14107-136">displayName</span></span>|<span data-ttu-id="14107-137">String</span><span class="sxs-lookup"><span data-stu-id="14107-137">String</span></span>|<span data-ttu-id="14107-138">Nome do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="14107-138">Name of the device management script.</span></span> <span data-ttu-id="14107-139">Herdado de [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="14107-139">Inherited from [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="14107-140">descrição</span><span class="sxs-lookup"><span data-stu-id="14107-140">description</span></span>|<span data-ttu-id="14107-141">String</span><span class="sxs-lookup"><span data-stu-id="14107-141">String</span></span>|<span data-ttu-id="14107-142">Descrição opcional para o script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="14107-142">Optional description for the device management script.</span></span> <span data-ttu-id="14107-143">Herdado de [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="14107-143">Inherited from [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="14107-144">runSchedule</span><span class="sxs-lookup"><span data-stu-id="14107-144">runSchedule</span></span>|[<span data-ttu-id="14107-145">runSchedule</span><span class="sxs-lookup"><span data-stu-id="14107-145">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="14107-146">O intervalo de execução do script.</span><span class="sxs-lookup"><span data-stu-id="14107-146">The interval for script to run.</span></span> <span data-ttu-id="14107-147">Se não definido, o script será executado uma vez herdado de [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="14107-147">If not defined the script will run once Inherited from [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="14107-148">scriptContent</span><span class="sxs-lookup"><span data-stu-id="14107-148">scriptContent</span></span>|<span data-ttu-id="14107-149">Binária</span><span class="sxs-lookup"><span data-stu-id="14107-149">Binary</span></span>|<span data-ttu-id="14107-150">O conteúdo de script.</span><span class="sxs-lookup"><span data-stu-id="14107-150">The script content.</span></span> <span data-ttu-id="14107-151">Herdado de [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="14107-151">Inherited from [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="14107-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="14107-152">createdDateTime</span></span>|<span data-ttu-id="14107-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14107-153">DateTimeOffset</span></span>|<span data-ttu-id="14107-154">A data e a hora em que o script de gerenciamento de dispositivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="14107-154">The date and time the device management script was created.</span></span> <span data-ttu-id="14107-155">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="14107-155">This property is read-only.</span></span> <span data-ttu-id="14107-156">Herdado de [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="14107-156">Inherited from [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="14107-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="14107-157">lastModifiedDateTime</span></span>|<span data-ttu-id="14107-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14107-158">DateTimeOffset</span></span>|<span data-ttu-id="14107-159">A data e a hora em que o script de gerenciamento de dispositivo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="14107-159">The date and time the device management script was last modified.</span></span> <span data-ttu-id="14107-160">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="14107-160">This property is read-only.</span></span> <span data-ttu-id="14107-161">Herdado de [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="14107-161">Inherited from [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="14107-162">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="14107-162">runAsAccount</span></span>|[<span data-ttu-id="14107-163">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="14107-163">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="14107-164">Indica o tipo de contexto de execução.</span><span class="sxs-lookup"><span data-stu-id="14107-164">Indicates the type of execution context.</span></span> <span data-ttu-id="14107-165">Herdado de [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).</span><span class="sxs-lookup"><span data-stu-id="14107-165">Inherited from [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).</span></span> <span data-ttu-id="14107-166">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="14107-166">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="14107-167">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="14107-167">enforceSignatureCheck</span></span>|<span data-ttu-id="14107-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="14107-168">Boolean</span></span>|<span data-ttu-id="14107-169">Indica se a assinatura do script precisa ser verificada.</span><span class="sxs-lookup"><span data-stu-id="14107-169">Indicate whether the script signature needs be checked.</span></span> <span data-ttu-id="14107-170">Herdado de [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="14107-170">Inherited from [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="14107-171">fileName</span><span class="sxs-lookup"><span data-stu-id="14107-171">fileName</span></span>|<span data-ttu-id="14107-172">String</span><span class="sxs-lookup"><span data-stu-id="14107-172">String</span></span>|<span data-ttu-id="14107-173">Nome do arquivo de script.</span><span class="sxs-lookup"><span data-stu-id="14107-173">Script file name.</span></span> <span data-ttu-id="14107-174">Herdado de [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="14107-174">Inherited from [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="14107-175">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="14107-175">roleScopeTagIds</span></span>|<span data-ttu-id="14107-176">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="14107-176">String collection</span></span>|<span data-ttu-id="14107-177">Lista de IDs de marca de escopo para esta instância de PowerShellScript.</span><span class="sxs-lookup"><span data-stu-id="14107-177">List of Scope Tag IDs for this PowerShellScript instance.</span></span> <span data-ttu-id="14107-178">Herdado de [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="14107-178">Inherited from [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="14107-179">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="14107-179">runAs32Bit</span></span>|<span data-ttu-id="14107-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="14107-180">Boolean</span></span>|<span data-ttu-id="14107-181">Um valor que indica se o script do PowerShell deve ser executado como 32 bits herdado de [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="14107-181">A value indicating whether the PowerShell script should run as 32-bit Inherited from [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md)</span></span>|
|<span data-ttu-id="14107-182">complianceRule</span><span class="sxs-lookup"><span data-stu-id="14107-182">complianceRule</span></span>|[<span data-ttu-id="14107-183">deviceHealthScriptComplianceRule</span><span class="sxs-lookup"><span data-stu-id="14107-183">deviceHealthScriptComplianceRule</span></span>](../resources/intune-devices-devicehealthscriptcompliancerule.md)|<span data-ttu-id="14107-184">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="14107-184">Not yet documented</span></span>|
|<span data-ttu-id="14107-185">remediationScriptContent</span><span class="sxs-lookup"><span data-stu-id="14107-185">remediationScriptContent</span></span>|<span data-ttu-id="14107-186">Binária</span><span class="sxs-lookup"><span data-stu-id="14107-186">Binary</span></span>|<span data-ttu-id="14107-187">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="14107-187">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="14107-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="14107-188">Response</span></span>
<span data-ttu-id="14107-189">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="14107-189">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14107-190">Exemplo</span><span class="sxs-lookup"><span data-stu-id="14107-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="14107-191">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14107-191">Request</span></span>
<span data-ttu-id="14107-192">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="14107-192">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
Content-type: application/json
Content-length: 712

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
  "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50"
}
```

### <a name="response"></a><span data-ttu-id="14107-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="14107-193">Response</span></span>
<span data-ttu-id="14107-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="14107-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 884

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
  "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50"
}
```




