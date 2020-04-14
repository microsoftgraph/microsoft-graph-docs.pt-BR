---
title: Criar deviceHealthScript
description: Criar um novo objeto deviceHealthScript.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6956bb460b3429cf919e9c2e84ccc751d090a7ed
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43380915"
---
# <a name="create-devicehealthscript"></a><span data-ttu-id="92261-103">Criar deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="92261-103">Create deviceHealthScript</span></span>

<span data-ttu-id="92261-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92261-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92261-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="92261-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92261-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="92261-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92261-107">Criar um novo objeto [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) .</span><span class="sxs-lookup"><span data-stu-id="92261-107">Create a new [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92261-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="92261-108">Prerequisites</span></span>
<span data-ttu-id="92261-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92261-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92261-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92261-111">Permission type</span></span>|<span data-ttu-id="92261-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="92261-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92261-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92261-113">Delegated (work or school account)</span></span>|<span data-ttu-id="92261-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="92261-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="92261-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92261-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92261-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92261-116">Not supported.</span></span>|
|<span data-ttu-id="92261-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92261-117">Application</span></span>|<span data-ttu-id="92261-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="92261-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="92261-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92261-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts
```

## <a name="request-headers"></a><span data-ttu-id="92261-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92261-120">Request headers</span></span>
|<span data-ttu-id="92261-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="92261-121">Header</span></span>|<span data-ttu-id="92261-122">Valor</span><span class="sxs-lookup"><span data-stu-id="92261-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92261-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="92261-123">Authorization</span></span>|<span data-ttu-id="92261-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92261-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92261-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="92261-125">Accept</span></span>|<span data-ttu-id="92261-126">application/json</span><span class="sxs-lookup"><span data-stu-id="92261-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92261-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92261-127">Request body</span></span>
<span data-ttu-id="92261-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceHealthScript.</span><span class="sxs-lookup"><span data-stu-id="92261-128">In the request body, supply a JSON representation for the deviceHealthScript object.</span></span>

<span data-ttu-id="92261-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceHealthScript.</span><span class="sxs-lookup"><span data-stu-id="92261-129">The following table shows the properties that are required when you create the deviceHealthScript.</span></span>

|<span data-ttu-id="92261-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92261-130">Property</span></span>|<span data-ttu-id="92261-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="92261-131">Type</span></span>|<span data-ttu-id="92261-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="92261-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92261-133">id</span><span class="sxs-lookup"><span data-stu-id="92261-133">id</span></span>|<span data-ttu-id="92261-134">String</span><span class="sxs-lookup"><span data-stu-id="92261-134">String</span></span>|<span data-ttu-id="92261-135">Identificador exclusivo do script de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="92261-135">Unique Identifier for the device health script</span></span>|
|<span data-ttu-id="92261-136">publicador</span><span class="sxs-lookup"><span data-stu-id="92261-136">publisher</span></span>|<span data-ttu-id="92261-137">String</span><span class="sxs-lookup"><span data-stu-id="92261-137">String</span></span>|<span data-ttu-id="92261-138">Nome do editor de script de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="92261-138">Name of the device health script publisher</span></span>|
|<span data-ttu-id="92261-139">versão</span><span class="sxs-lookup"><span data-stu-id="92261-139">version</span></span>|<span data-ttu-id="92261-140">String</span><span class="sxs-lookup"><span data-stu-id="92261-140">String</span></span>|<span data-ttu-id="92261-141">Versão do script de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="92261-141">Version of the device health script</span></span>|
|<span data-ttu-id="92261-142">displayName</span><span class="sxs-lookup"><span data-stu-id="92261-142">displayName</span></span>|<span data-ttu-id="92261-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="92261-143">String</span></span>|<span data-ttu-id="92261-144">Nome do script de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="92261-144">Name of the device health script</span></span>|
|<span data-ttu-id="92261-145">description</span><span class="sxs-lookup"><span data-stu-id="92261-145">description</span></span>|<span data-ttu-id="92261-146">String</span><span class="sxs-lookup"><span data-stu-id="92261-146">String</span></span>|<span data-ttu-id="92261-147">Descrição do script de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="92261-147">Description of the device health script</span></span>|
|<span data-ttu-id="92261-148">detectionScriptContent</span><span class="sxs-lookup"><span data-stu-id="92261-148">detectionScriptContent</span></span>|<span data-ttu-id="92261-149">Binária</span><span class="sxs-lookup"><span data-stu-id="92261-149">Binary</span></span>|<span data-ttu-id="92261-150">Todo o conteúdo do script do PowerShell de detecção</span><span class="sxs-lookup"><span data-stu-id="92261-150">The entire content of the detection powershell script</span></span>|
|<span data-ttu-id="92261-151">remediationScriptContent</span><span class="sxs-lookup"><span data-stu-id="92261-151">remediationScriptContent</span></span>|<span data-ttu-id="92261-152">Binária</span><span class="sxs-lookup"><span data-stu-id="92261-152">Binary</span></span>|<span data-ttu-id="92261-153">Todo o conteúdo do script do PowerShell de correção</span><span class="sxs-lookup"><span data-stu-id="92261-153">The entire content of the remediation powershell script</span></span>|
|<span data-ttu-id="92261-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="92261-154">createdDateTime</span></span>|<span data-ttu-id="92261-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92261-155">DateTimeOffset</span></span>|<span data-ttu-id="92261-156">O carimbo de data/hora de quando o script de integridade do dispositivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="92261-156">The timestamp of when the device health script was created.</span></span> <span data-ttu-id="92261-157">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="92261-157">This property is read-only.</span></span>|
|<span data-ttu-id="92261-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="92261-158">lastModifiedDateTime</span></span>|<span data-ttu-id="92261-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92261-159">DateTimeOffset</span></span>|<span data-ttu-id="92261-160">O carimbo de data/hora de quando o script de integridade do dispositivo foi modificado.</span><span class="sxs-lookup"><span data-stu-id="92261-160">The timestamp of when the device health script was modified.</span></span> <span data-ttu-id="92261-161">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="92261-161">This property is read-only.</span></span>|
|<span data-ttu-id="92261-162">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="92261-162">runAsAccount</span></span>|[<span data-ttu-id="92261-163">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="92261-163">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="92261-164">Indica o tipo de contexto de execução.</span><span class="sxs-lookup"><span data-stu-id="92261-164">Indicates the type of execution context.</span></span> <span data-ttu-id="92261-165">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="92261-165">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="92261-166">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="92261-166">enforceSignatureCheck</span></span>|<span data-ttu-id="92261-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="92261-167">Boolean</span></span>|<span data-ttu-id="92261-168">Indicar se a assinatura do script precisa ser verificada</span><span class="sxs-lookup"><span data-stu-id="92261-168">Indicate whether the script signature needs be checked</span></span>|
|<span data-ttu-id="92261-169">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="92261-169">runAs32Bit</span></span>|<span data-ttu-id="92261-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="92261-170">Boolean</span></span>|<span data-ttu-id="92261-171">Indicar se os scripts do PowerShell devem ser executados como 32 bits</span><span class="sxs-lookup"><span data-stu-id="92261-171">Indicate whether PowerShell script(s) should run as 32-bit</span></span>|
|<span data-ttu-id="92261-172">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="92261-172">roleScopeTagIds</span></span>|<span data-ttu-id="92261-173">Coleção String</span><span class="sxs-lookup"><span data-stu-id="92261-173">String collection</span></span>|<span data-ttu-id="92261-174">Lista de IDs de marcas de escopo para o script de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="92261-174">List of Scope Tag IDs for the device health script</span></span>|
|<span data-ttu-id="92261-175">isGlobalScript</span><span class="sxs-lookup"><span data-stu-id="92261-175">isGlobalScript</span></span>|<span data-ttu-id="92261-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="92261-176">Boolean</span></span>|<span data-ttu-id="92261-177">Determina se este é o script proprietário da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="92261-177">Determines if this is Microsoft Proprietary Script.</span></span> <span data-ttu-id="92261-178">Scripts proprietários são somente leitura</span><span class="sxs-lookup"><span data-stu-id="92261-178">Proprietary scripts are read-only</span></span>|
|<span data-ttu-id="92261-179">highestAvailableVersion</span><span class="sxs-lookup"><span data-stu-id="92261-179">highestAvailableVersion</span></span>|<span data-ttu-id="92261-180">String</span><span class="sxs-lookup"><span data-stu-id="92261-180">String</span></span>|<span data-ttu-id="92261-181">Versão mais recente disponível para um script proprietário da Microsoft</span><span class="sxs-lookup"><span data-stu-id="92261-181">Highest available version for a Microsoft Proprietary script</span></span>|



## <a name="response"></a><span data-ttu-id="92261-182">Resposta</span><span class="sxs-lookup"><span data-stu-id="92261-182">Response</span></span>
<span data-ttu-id="92261-183">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92261-183">If successful, this method returns a `201 Created` response code and a [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92261-184">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92261-184">Example</span></span>

### <a name="request"></a><span data-ttu-id="92261-185">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92261-185">Request</span></span>
<span data-ttu-id="92261-186">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="92261-186">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="92261-187">Resposta</span><span class="sxs-lookup"><span data-stu-id="92261-187">Response</span></span>
<span data-ttu-id="92261-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="92261-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



