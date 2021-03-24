---
title: Criar deviceComplianceScript
description: Crie um novo objeto deviceComplianceScript.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c900a21083ec1ee775a355a514c9e323ae96314f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128660"
---
# <a name="create-devicecompliancescript"></a><span data-ttu-id="3b6cc-103">Criar deviceComplianceScript</span><span class="sxs-lookup"><span data-stu-id="3b6cc-103">Create deviceComplianceScript</span></span>

<span data-ttu-id="3b6cc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b6cc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3b6cc-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3b6cc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b6cc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3b6cc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b6cc-107">Crie um novo [objeto deviceComplianceScript.](../resources/intune-devices-devicecompliancescript.md)</span><span class="sxs-lookup"><span data-stu-id="3b6cc-107">Create a new [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b6cc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3b6cc-108">Prerequisites</span></span>
<span data-ttu-id="3b6cc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b6cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b6cc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b6cc-111">Permission type</span></span>|<span data-ttu-id="3b6cc-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3b6cc-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b6cc-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b6cc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3b6cc-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b6cc-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3b6cc-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b6cc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b6cc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b6cc-116">Not supported.</span></span>|
|<span data-ttu-id="3b6cc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b6cc-117">Application</span></span>|<span data-ttu-id="3b6cc-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b6cc-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b6cc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b6cc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceComplianceScripts
```

## <a name="request-headers"></a><span data-ttu-id="3b6cc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b6cc-120">Request headers</span></span>
|<span data-ttu-id="3b6cc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3b6cc-121">Header</span></span>|<span data-ttu-id="3b6cc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3b6cc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b6cc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b6cc-123">Authorization</span></span>|<span data-ttu-id="3b6cc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b6cc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b6cc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3b6cc-125">Accept</span></span>|<span data-ttu-id="3b6cc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3b6cc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b6cc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b6cc-127">Request body</span></span>
<span data-ttu-id="3b6cc-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceComplianceScript.</span><span class="sxs-lookup"><span data-stu-id="3b6cc-128">In the request body, supply a JSON representation for the deviceComplianceScript object.</span></span>

<span data-ttu-id="3b6cc-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceComplianceScript.</span><span class="sxs-lookup"><span data-stu-id="3b6cc-129">The following table shows the properties that are required when you create the deviceComplianceScript.</span></span>

|<span data-ttu-id="3b6cc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3b6cc-130">Property</span></span>|<span data-ttu-id="3b6cc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b6cc-131">Type</span></span>|<span data-ttu-id="3b6cc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b6cc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b6cc-133">id</span><span class="sxs-lookup"><span data-stu-id="3b6cc-133">id</span></span>|<span data-ttu-id="3b6cc-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b6cc-134">String</span></span>|<span data-ttu-id="3b6cc-135">Identificador exclusivo do script de conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="3b6cc-135">Unique Identifier for the device compliance script</span></span>|
|<span data-ttu-id="3b6cc-136">publicador</span><span class="sxs-lookup"><span data-stu-id="3b6cc-136">publisher</span></span>|<span data-ttu-id="3b6cc-137">String</span><span class="sxs-lookup"><span data-stu-id="3b6cc-137">String</span></span>|<span data-ttu-id="3b6cc-138">Nome do editor de scripts de conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="3b6cc-138">Name of the device compliance script publisher</span></span>|
|<span data-ttu-id="3b6cc-139">versão</span><span class="sxs-lookup"><span data-stu-id="3b6cc-139">version</span></span>|<span data-ttu-id="3b6cc-140">String</span><span class="sxs-lookup"><span data-stu-id="3b6cc-140">String</span></span>|<span data-ttu-id="3b6cc-141">Versão do script de conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="3b6cc-141">Version of the device compliance script</span></span>|
|<span data-ttu-id="3b6cc-142">displayName</span><span class="sxs-lookup"><span data-stu-id="3b6cc-142">displayName</span></span>|<span data-ttu-id="3b6cc-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b6cc-143">String</span></span>|<span data-ttu-id="3b6cc-144">Nome do script de conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="3b6cc-144">Name of the device compliance script</span></span>|
|<span data-ttu-id="3b6cc-145">descrição</span><span class="sxs-lookup"><span data-stu-id="3b6cc-145">description</span></span>|<span data-ttu-id="3b6cc-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b6cc-146">String</span></span>|<span data-ttu-id="3b6cc-147">Descrição do script de conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="3b6cc-147">Description of the device compliance script</span></span>|
|<span data-ttu-id="3b6cc-148">detectionScriptContent</span><span class="sxs-lookup"><span data-stu-id="3b6cc-148">detectionScriptContent</span></span>|<span data-ttu-id="3b6cc-149">Binário</span><span class="sxs-lookup"><span data-stu-id="3b6cc-149">Binary</span></span>|<span data-ttu-id="3b6cc-150">Todo o conteúdo do script do powershell de detecção</span><span class="sxs-lookup"><span data-stu-id="3b6cc-150">The entire content of the detection powershell script</span></span>|
|<span data-ttu-id="3b6cc-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3b6cc-151">createdDateTime</span></span>|<span data-ttu-id="3b6cc-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b6cc-152">DateTimeOffset</span></span>|<span data-ttu-id="3b6cc-153">O data/hora de quando o script de conformidade do dispositivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="3b6cc-153">The timestamp of when the device compliance script was created.</span></span> <span data-ttu-id="3b6cc-154">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3b6cc-154">This property is read-only.</span></span>|
|<span data-ttu-id="3b6cc-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3b6cc-155">lastModifiedDateTime</span></span>|<span data-ttu-id="3b6cc-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b6cc-156">DateTimeOffset</span></span>|<span data-ttu-id="3b6cc-157">O data/hora de quando o script de conformidade do dispositivo foi modificado.</span><span class="sxs-lookup"><span data-stu-id="3b6cc-157">The timestamp of when the device compliance script was modified.</span></span> <span data-ttu-id="3b6cc-158">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3b6cc-158">This property is read-only.</span></span>|
|<span data-ttu-id="3b6cc-159">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="3b6cc-159">runAsAccount</span></span>|[<span data-ttu-id="3b6cc-160">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="3b6cc-160">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="3b6cc-161">Indica o tipo de contexto de execução.</span><span class="sxs-lookup"><span data-stu-id="3b6cc-161">Indicates the type of execution context.</span></span> <span data-ttu-id="3b6cc-162">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="3b6cc-162">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="3b6cc-163">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="3b6cc-163">enforceSignatureCheck</span></span>|<span data-ttu-id="3b6cc-164">Booleano</span><span class="sxs-lookup"><span data-stu-id="3b6cc-164">Boolean</span></span>|<span data-ttu-id="3b6cc-165">Indicar se a assinatura de script precisa ser verificada</span><span class="sxs-lookup"><span data-stu-id="3b6cc-165">Indicate whether the script signature needs be checked</span></span>|
|<span data-ttu-id="3b6cc-166">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="3b6cc-166">runAs32Bit</span></span>|<span data-ttu-id="3b6cc-167">Booleano</span><span class="sxs-lookup"><span data-stu-id="3b6cc-167">Boolean</span></span>|<span data-ttu-id="3b6cc-168">Indicar se os scripts do PowerShell devem ser executados como 32 bits</span><span class="sxs-lookup"><span data-stu-id="3b6cc-168">Indicate whether PowerShell script(s) should run as 32-bit</span></span>|
|<span data-ttu-id="3b6cc-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3b6cc-169">roleScopeTagIds</span></span>|<span data-ttu-id="3b6cc-170">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b6cc-170">String collection</span></span>|<span data-ttu-id="3b6cc-171">Lista de IDs de marca de escopo para o script de conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="3b6cc-171">List of Scope Tag IDs for the device compliance script</span></span>|



## <a name="response"></a><span data-ttu-id="3b6cc-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b6cc-172">Response</span></span>
<span data-ttu-id="3b6cc-173">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b6cc-173">If successful, this method returns a `201 Created` response code and a [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b6cc-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3b6cc-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b6cc-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b6cc-175">Request</span></span>
<span data-ttu-id="3b6cc-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b6cc-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceComplianceScripts
Content-type: application/json
Content-length: 420

{
  "@odata.type": "#microsoft.graph.deviceComplianceScript",
  "publisher": "Publisher value",
  "version": "Version value",
  "displayName": "Display Name value",
  "description": "Description value",
  "detectionScriptContent": "ZGV0ZWN0aW9uU2NyaXB0Q29udGVudA==",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="3b6cc-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b6cc-177">Response</span></span>
<span data-ttu-id="3b6cc-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b6cc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 592

{
  "@odata.type": "#microsoft.graph.deviceComplianceScript",
  "id": "14e72a7b-2a7b-14e7-7b2a-e7147b2ae714",
  "publisher": "Publisher value",
  "version": "Version value",
  "displayName": "Display Name value",
  "description": "Description value",
  "detectionScriptContent": "ZGV0ZWN0aW9uU2NyaXB0Q29udGVudA==",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




