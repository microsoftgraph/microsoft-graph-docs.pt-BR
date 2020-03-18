---
title: Criar deviceHealthScript
description: Criar um novo objeto deviceHealthScript.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5638b7ac4452531e4da173dd3bab53a42ce7e339
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42814642"
---
# <a name="create-devicehealthscript"></a><span data-ttu-id="8952e-103">Criar deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="8952e-103">Create deviceHealthScript</span></span>

> <span data-ttu-id="8952e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8952e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8952e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8952e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8952e-106">Criar um novo objeto [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) .</span><span class="sxs-lookup"><span data-stu-id="8952e-106">Create a new [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8952e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8952e-107">Prerequisites</span></span>
<span data-ttu-id="8952e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8952e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8952e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8952e-110">Permission type</span></span>|<span data-ttu-id="8952e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8952e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8952e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8952e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8952e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8952e-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8952e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8952e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8952e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8952e-115">Not supported.</span></span>|
|<span data-ttu-id="8952e-116">Application</span><span class="sxs-lookup"><span data-stu-id="8952e-116">Application</span></span>|<span data-ttu-id="8952e-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8952e-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8952e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8952e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts
```

## <a name="request-headers"></a><span data-ttu-id="8952e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8952e-119">Request headers</span></span>
|<span data-ttu-id="8952e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8952e-120">Header</span></span>|<span data-ttu-id="8952e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8952e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8952e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8952e-122">Authorization</span></span>|<span data-ttu-id="8952e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8952e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8952e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8952e-124">Accept</span></span>|<span data-ttu-id="8952e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8952e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8952e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8952e-126">Request body</span></span>
<span data-ttu-id="8952e-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceHealthScript.</span><span class="sxs-lookup"><span data-stu-id="8952e-127">In the request body, supply a JSON representation for the deviceHealthScript object.</span></span>

<span data-ttu-id="8952e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceHealthScript.</span><span class="sxs-lookup"><span data-stu-id="8952e-128">The following table shows the properties that are required when you create the deviceHealthScript.</span></span>

|<span data-ttu-id="8952e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8952e-129">Property</span></span>|<span data-ttu-id="8952e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8952e-130">Type</span></span>|<span data-ttu-id="8952e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8952e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8952e-132">id</span><span class="sxs-lookup"><span data-stu-id="8952e-132">id</span></span>|<span data-ttu-id="8952e-133">String</span><span class="sxs-lookup"><span data-stu-id="8952e-133">String</span></span>|<span data-ttu-id="8952e-134">Identificador exclusivo do script de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="8952e-134">Unique Identifier for the device health script</span></span>|
|<span data-ttu-id="8952e-135">publicador</span><span class="sxs-lookup"><span data-stu-id="8952e-135">publisher</span></span>|<span data-ttu-id="8952e-136">String</span><span class="sxs-lookup"><span data-stu-id="8952e-136">String</span></span>|<span data-ttu-id="8952e-137">Nome do editor de script de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="8952e-137">Name of the device health script publisher</span></span>|
|<span data-ttu-id="8952e-138">versão</span><span class="sxs-lookup"><span data-stu-id="8952e-138">version</span></span>|<span data-ttu-id="8952e-139">String</span><span class="sxs-lookup"><span data-stu-id="8952e-139">String</span></span>|<span data-ttu-id="8952e-140">Versão do script de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="8952e-140">Version of the device health script</span></span>|
|<span data-ttu-id="8952e-141">displayName</span><span class="sxs-lookup"><span data-stu-id="8952e-141">displayName</span></span>|<span data-ttu-id="8952e-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8952e-142">String</span></span>|<span data-ttu-id="8952e-143">Nome do script de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="8952e-143">Name of the device health script</span></span>|
|<span data-ttu-id="8952e-144">description</span><span class="sxs-lookup"><span data-stu-id="8952e-144">description</span></span>|<span data-ttu-id="8952e-145">String</span><span class="sxs-lookup"><span data-stu-id="8952e-145">String</span></span>|<span data-ttu-id="8952e-146">Descrição do script de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="8952e-146">Description of the device health script</span></span>|
|<span data-ttu-id="8952e-147">detectionScriptContent</span><span class="sxs-lookup"><span data-stu-id="8952e-147">detectionScriptContent</span></span>|<span data-ttu-id="8952e-148">Binária</span><span class="sxs-lookup"><span data-stu-id="8952e-148">Binary</span></span>|<span data-ttu-id="8952e-149">Todo o conteúdo do script do PowerShell de detecção</span><span class="sxs-lookup"><span data-stu-id="8952e-149">The entire content of the detection powershell script</span></span>|
|<span data-ttu-id="8952e-150">remediationScriptContent</span><span class="sxs-lookup"><span data-stu-id="8952e-150">remediationScriptContent</span></span>|<span data-ttu-id="8952e-151">Binária</span><span class="sxs-lookup"><span data-stu-id="8952e-151">Binary</span></span>|<span data-ttu-id="8952e-152">Todo o conteúdo do script do PowerShell de correção</span><span class="sxs-lookup"><span data-stu-id="8952e-152">The entire content of the remediation powershell script</span></span>|
|<span data-ttu-id="8952e-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8952e-153">createdDateTime</span></span>|<span data-ttu-id="8952e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8952e-154">DateTimeOffset</span></span>|<span data-ttu-id="8952e-155">O carimbo de data/hora de quando o script de integridade do dispositivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="8952e-155">The timestamp of when the device health script was created.</span></span> <span data-ttu-id="8952e-156">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8952e-156">This property is read-only.</span></span>|
|<span data-ttu-id="8952e-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8952e-157">lastModifiedDateTime</span></span>|<span data-ttu-id="8952e-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8952e-158">DateTimeOffset</span></span>|<span data-ttu-id="8952e-159">O carimbo de data/hora de quando o script de integridade do dispositivo foi modificado.</span><span class="sxs-lookup"><span data-stu-id="8952e-159">The timestamp of when the device health script was modified.</span></span> <span data-ttu-id="8952e-160">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8952e-160">This property is read-only.</span></span>|
|<span data-ttu-id="8952e-161">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="8952e-161">runAsAccount</span></span>|[<span data-ttu-id="8952e-162">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="8952e-162">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="8952e-163">Indica o tipo de contexto de execução.</span><span class="sxs-lookup"><span data-stu-id="8952e-163">Indicates the type of execution context.</span></span> <span data-ttu-id="8952e-164">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="8952e-164">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="8952e-165">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="8952e-165">enforceSignatureCheck</span></span>|<span data-ttu-id="8952e-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="8952e-166">Boolean</span></span>|<span data-ttu-id="8952e-167">Indicar se a assinatura do script precisa ser verificada</span><span class="sxs-lookup"><span data-stu-id="8952e-167">Indicate whether the script signature needs be checked</span></span>|
|<span data-ttu-id="8952e-168">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="8952e-168">runAs32Bit</span></span>|<span data-ttu-id="8952e-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="8952e-169">Boolean</span></span>|<span data-ttu-id="8952e-170">Indicar se os scripts do PowerShell devem ser executados como 32 bits</span><span class="sxs-lookup"><span data-stu-id="8952e-170">Indicate whether PowerShell script(s) should run as 32-bit</span></span>|
|<span data-ttu-id="8952e-171">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8952e-171">roleScopeTagIds</span></span>|<span data-ttu-id="8952e-172">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8952e-172">String collection</span></span>|<span data-ttu-id="8952e-173">Lista de IDs de marcas de escopo para o script de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="8952e-173">List of Scope Tag IDs for the device health script</span></span>|
|<span data-ttu-id="8952e-174">isGlobalScript</span><span class="sxs-lookup"><span data-stu-id="8952e-174">isGlobalScript</span></span>|<span data-ttu-id="8952e-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="8952e-175">Boolean</span></span>|<span data-ttu-id="8952e-176">Determina se este é o script proprietário da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8952e-176">Determines if this is Microsoft Proprietary Script.</span></span> <span data-ttu-id="8952e-177">Scripts proprietários são somente leitura</span><span class="sxs-lookup"><span data-stu-id="8952e-177">Proprietary scripts are read-only</span></span>|
|<span data-ttu-id="8952e-178">highestAvailableVersion</span><span class="sxs-lookup"><span data-stu-id="8952e-178">highestAvailableVersion</span></span>|<span data-ttu-id="8952e-179">String</span><span class="sxs-lookup"><span data-stu-id="8952e-179">String</span></span>|<span data-ttu-id="8952e-180">Versão mais recente disponível para um script proprietário da Microsoft</span><span class="sxs-lookup"><span data-stu-id="8952e-180">Highest available version for a Microsoft Proprietary script</span></span>|



## <a name="response"></a><span data-ttu-id="8952e-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="8952e-181">Response</span></span>
<span data-ttu-id="8952e-182">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8952e-182">If successful, this method returns a `201 Created` response code and a [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8952e-183">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8952e-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="8952e-184">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8952e-184">Request</span></span>
<span data-ttu-id="8952e-185">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8952e-185">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts
Content-type: application/json
Content-length: 575

{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
  "publisher": "Publisher value",
  "version": "Version value",
  "displayName": "Display Name value",
  "description": "Description value",
  "detectionScriptContent": "ZGV0ZWN0aW9uU2NyaXB0Q29udGVudA==",
  "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "isGlobalScript": true,
  "highestAvailableVersion": "Highest Available Version value"
}
```

### <a name="response"></a><span data-ttu-id="8952e-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="8952e-186">Response</span></span>
<span data-ttu-id="8952e-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8952e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 747

{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
  "id": "bcb60502-0502-bcb6-0205-b6bc0205b6bc",
  "publisher": "Publisher value",
  "version": "Version value",
  "displayName": "Display Name value",
  "description": "Description value",
  "detectionScriptContent": "ZGV0ZWN0aW9uU2NyaXB0Q29udGVudA==",
  "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "isGlobalScript": true,
  "highestAvailableVersion": "Highest Available Version value"
}
```




