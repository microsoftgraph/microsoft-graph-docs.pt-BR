---
title: Atualizar deviceHealthScript
description: Atualize as propriedades de um objeto deviceHealthScript.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6a3eb34d13008c4dcf572f3418928215ea435761
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146276"
---
# <a name="update-devicehealthscript"></a><span data-ttu-id="91bfd-103">Atualizar deviceHealthScript</span><span class="sxs-lookup"><span data-stu-id="91bfd-103">Update deviceHealthScript</span></span>

<span data-ttu-id="91bfd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91bfd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="91bfd-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="91bfd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91bfd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="91bfd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91bfd-107">Atualize as propriedades de um [objeto deviceHealthScript.](../resources/intune-devices-devicehealthscript.md)</span><span class="sxs-lookup"><span data-stu-id="91bfd-107">Update the properties of a [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="91bfd-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="91bfd-108">Prerequisites</span></span>
<span data-ttu-id="91bfd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91bfd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91bfd-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91bfd-111">Permission type</span></span>|<span data-ttu-id="91bfd-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="91bfd-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91bfd-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91bfd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="91bfd-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91bfd-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="91bfd-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91bfd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91bfd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91bfd-116">Not supported.</span></span>|
|<span data-ttu-id="91bfd-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91bfd-117">Application</span></span>|<span data-ttu-id="91bfd-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91bfd-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="91bfd-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91bfd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="91bfd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91bfd-120">Request headers</span></span>
|<span data-ttu-id="91bfd-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="91bfd-121">Header</span></span>|<span data-ttu-id="91bfd-122">Valor</span><span class="sxs-lookup"><span data-stu-id="91bfd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91bfd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="91bfd-123">Authorization</span></span>|<span data-ttu-id="91bfd-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91bfd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91bfd-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="91bfd-125">Accept</span></span>|<span data-ttu-id="91bfd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="91bfd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91bfd-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91bfd-127">Request body</span></span>
<span data-ttu-id="91bfd-128">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceHealthScript.](../resources/intune-devices-devicehealthscript.md)</span><span class="sxs-lookup"><span data-stu-id="91bfd-128">In the request body, supply a JSON representation for the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.</span></span>

<span data-ttu-id="91bfd-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceHealthScript](../resources/intune-devices-devicehealthscript.md).</span><span class="sxs-lookup"><span data-stu-id="91bfd-129">The following table shows the properties that are required when you create the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md).</span></span>

|<span data-ttu-id="91bfd-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="91bfd-130">Property</span></span>|<span data-ttu-id="91bfd-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="91bfd-131">Type</span></span>|<span data-ttu-id="91bfd-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="91bfd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91bfd-133">id</span><span class="sxs-lookup"><span data-stu-id="91bfd-133">id</span></span>|<span data-ttu-id="91bfd-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91bfd-134">String</span></span>|<span data-ttu-id="91bfd-135">Identificador exclusivo do script de saúde do dispositivo</span><span class="sxs-lookup"><span data-stu-id="91bfd-135">Unique Identifier for the device health script</span></span>|
|<span data-ttu-id="91bfd-136">publicador</span><span class="sxs-lookup"><span data-stu-id="91bfd-136">publisher</span></span>|<span data-ttu-id="91bfd-137">String</span><span class="sxs-lookup"><span data-stu-id="91bfd-137">String</span></span>|<span data-ttu-id="91bfd-138">Nome do editor de scripts de saúde do dispositivo</span><span class="sxs-lookup"><span data-stu-id="91bfd-138">Name of the device health script publisher</span></span>|
|<span data-ttu-id="91bfd-139">versão</span><span class="sxs-lookup"><span data-stu-id="91bfd-139">version</span></span>|<span data-ttu-id="91bfd-140">String</span><span class="sxs-lookup"><span data-stu-id="91bfd-140">String</span></span>|<span data-ttu-id="91bfd-141">Versão do script de saúde do dispositivo</span><span class="sxs-lookup"><span data-stu-id="91bfd-141">Version of the device health script</span></span>|
|<span data-ttu-id="91bfd-142">displayName</span><span class="sxs-lookup"><span data-stu-id="91bfd-142">displayName</span></span>|<span data-ttu-id="91bfd-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91bfd-143">String</span></span>|<span data-ttu-id="91bfd-144">Nome do script de saúde do dispositivo</span><span class="sxs-lookup"><span data-stu-id="91bfd-144">Name of the device health script</span></span>|
|<span data-ttu-id="91bfd-145">descrição</span><span class="sxs-lookup"><span data-stu-id="91bfd-145">description</span></span>|<span data-ttu-id="91bfd-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91bfd-146">String</span></span>|<span data-ttu-id="91bfd-147">Descrição do script de saúde do dispositivo</span><span class="sxs-lookup"><span data-stu-id="91bfd-147">Description of the device health script</span></span>|
|<span data-ttu-id="91bfd-148">detectionScriptContent</span><span class="sxs-lookup"><span data-stu-id="91bfd-148">detectionScriptContent</span></span>|<span data-ttu-id="91bfd-149">Binário</span><span class="sxs-lookup"><span data-stu-id="91bfd-149">Binary</span></span>|<span data-ttu-id="91bfd-150">Todo o conteúdo do script do powershell de detecção</span><span class="sxs-lookup"><span data-stu-id="91bfd-150">The entire content of the detection powershell script</span></span>|
|<span data-ttu-id="91bfd-151">remediationScriptContent</span><span class="sxs-lookup"><span data-stu-id="91bfd-151">remediationScriptContent</span></span>|<span data-ttu-id="91bfd-152">Binário</span><span class="sxs-lookup"><span data-stu-id="91bfd-152">Binary</span></span>|<span data-ttu-id="91bfd-153">Todo o conteúdo do script do powershell de correção</span><span class="sxs-lookup"><span data-stu-id="91bfd-153">The entire content of the remediation powershell script</span></span>|
|<span data-ttu-id="91bfd-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="91bfd-154">createdDateTime</span></span>|<span data-ttu-id="91bfd-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91bfd-155">DateTimeOffset</span></span>|<span data-ttu-id="91bfd-156">O timestamp de quando o script de saúde do dispositivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="91bfd-156">The timestamp of when the device health script was created.</span></span> <span data-ttu-id="91bfd-157">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="91bfd-157">This property is read-only.</span></span>|
|<span data-ttu-id="91bfd-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="91bfd-158">lastModifiedDateTime</span></span>|<span data-ttu-id="91bfd-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91bfd-159">DateTimeOffset</span></span>|<span data-ttu-id="91bfd-160">O data/hora de quando o script de saúde do dispositivo foi modificado.</span><span class="sxs-lookup"><span data-stu-id="91bfd-160">The timestamp of when the device health script was modified.</span></span> <span data-ttu-id="91bfd-161">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="91bfd-161">This property is read-only.</span></span>|
|<span data-ttu-id="91bfd-162">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="91bfd-162">runAsAccount</span></span>|[<span data-ttu-id="91bfd-163">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="91bfd-163">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="91bfd-164">Indica o tipo de contexto de execução.</span><span class="sxs-lookup"><span data-stu-id="91bfd-164">Indicates the type of execution context.</span></span> <span data-ttu-id="91bfd-165">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="91bfd-165">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="91bfd-166">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="91bfd-166">enforceSignatureCheck</span></span>|<span data-ttu-id="91bfd-167">Booleano</span><span class="sxs-lookup"><span data-stu-id="91bfd-167">Boolean</span></span>|<span data-ttu-id="91bfd-168">Indicar se a assinatura de script precisa ser verificada</span><span class="sxs-lookup"><span data-stu-id="91bfd-168">Indicate whether the script signature needs be checked</span></span>|
|<span data-ttu-id="91bfd-169">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="91bfd-169">runAs32Bit</span></span>|<span data-ttu-id="91bfd-170">Booleano</span><span class="sxs-lookup"><span data-stu-id="91bfd-170">Boolean</span></span>|<span data-ttu-id="91bfd-171">Indicar se os scripts do PowerShell devem ser executados como 32 bits</span><span class="sxs-lookup"><span data-stu-id="91bfd-171">Indicate whether PowerShell script(s) should run as 32-bit</span></span>|
|<span data-ttu-id="91bfd-172">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="91bfd-172">roleScopeTagIds</span></span>|<span data-ttu-id="91bfd-173">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="91bfd-173">String collection</span></span>|<span data-ttu-id="91bfd-174">Lista de IDs de marca de escopo para o script de saúde do dispositivo</span><span class="sxs-lookup"><span data-stu-id="91bfd-174">List of Scope Tag IDs for the device health script</span></span>|
|<span data-ttu-id="91bfd-175">isGlobalScript</span><span class="sxs-lookup"><span data-stu-id="91bfd-175">isGlobalScript</span></span>|<span data-ttu-id="91bfd-176">Booleano</span><span class="sxs-lookup"><span data-stu-id="91bfd-176">Boolean</span></span>|<span data-ttu-id="91bfd-177">Determina se esse é o Script Proprietário da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="91bfd-177">Determines if this is Microsoft Proprietary Script.</span></span> <span data-ttu-id="91bfd-178">Scripts proprietários são somente leitura</span><span class="sxs-lookup"><span data-stu-id="91bfd-178">Proprietary scripts are read-only</span></span>|
|<span data-ttu-id="91bfd-179">highestAvailableVersion</span><span class="sxs-lookup"><span data-stu-id="91bfd-179">highestAvailableVersion</span></span>|<span data-ttu-id="91bfd-180">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="91bfd-180">String</span></span>|<span data-ttu-id="91bfd-181">Versão mais alta disponível para um script proprietário da Microsoft</span><span class="sxs-lookup"><span data-stu-id="91bfd-181">Highest available version for a Microsoft Proprietary script</span></span>|
|<span data-ttu-id="91bfd-182">detectionScriptParameters</span><span class="sxs-lookup"><span data-stu-id="91bfd-182">detectionScriptParameters</span></span>|<span data-ttu-id="91bfd-183">[Coleção deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span><span class="sxs-lookup"><span data-stu-id="91bfd-183">[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md) collection</span></span>|<span data-ttu-id="91bfd-184">Lista de objetos ComplexType DetectionScriptParameters.</span><span class="sxs-lookup"><span data-stu-id="91bfd-184">List of ComplexType DetectionScriptParameters objects.</span></span>|
|<span data-ttu-id="91bfd-185">remediationScriptParameters</span><span class="sxs-lookup"><span data-stu-id="91bfd-185">remediationScriptParameters</span></span>|<span data-ttu-id="91bfd-186">[Coleção deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span><span class="sxs-lookup"><span data-stu-id="91bfd-186">[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md) collection</span></span>|<span data-ttu-id="91bfd-187">Lista de objetos ComplexType RemediationScriptParameters.</span><span class="sxs-lookup"><span data-stu-id="91bfd-187">List of ComplexType RemediationScriptParameters objects.</span></span>|



## <a name="response"></a><span data-ttu-id="91bfd-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="91bfd-188">Response</span></span>
<span data-ttu-id="91bfd-189">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceHealthScript](../resources/intune-devices-devicehealthscript.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91bfd-189">If successful, this method returns a `200 OK` response code and an updated [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91bfd-190">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91bfd-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="91bfd-191">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91bfd-191">Request</span></span>
<span data-ttu-id="91bfd-192">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="91bfd-192">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}
Content-type: application/json
Content-length: 1221

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
  "highestAvailableVersion": "Highest Available Version value",
  "detectionScriptParameters": [
    {
      "@odata.type": "microsoft.graph.deviceHealthScriptStringParameter",
      "name": "Name value",
      "description": "Description value",
      "isRequired": true,
      "applyDefaultValueWhenNotAssigned": true,
      "defaultValue": "Default Value value"
    }
  ],
  "remediationScriptParameters": [
    {
      "@odata.type": "microsoft.graph.deviceHealthScriptStringParameter",
      "name": "Name value",
      "description": "Description value",
      "isRequired": true,
      "applyDefaultValueWhenNotAssigned": true,
      "defaultValue": "Default Value value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="91bfd-193">Resposta</span><span class="sxs-lookup"><span data-stu-id="91bfd-193">Response</span></span>
<span data-ttu-id="91bfd-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="91bfd-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1393

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
  "highestAvailableVersion": "Highest Available Version value",
  "detectionScriptParameters": [
    {
      "@odata.type": "microsoft.graph.deviceHealthScriptStringParameter",
      "name": "Name value",
      "description": "Description value",
      "isRequired": true,
      "applyDefaultValueWhenNotAssigned": true,
      "defaultValue": "Default Value value"
    }
  ],
  "remediationScriptParameters": [
    {
      "@odata.type": "microsoft.graph.deviceHealthScriptStringParameter",
      "name": "Name value",
      "description": "Description value",
      "isRequired": true,
      "applyDefaultValueWhenNotAssigned": true,
      "defaultValue": "Default Value value"
    }
  ]
}
```




