---
title: Criar deviceComplianceScript
description: Criar um novo objeto deviceComplianceScript.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bbd57133d102a6c0e8d7e28e275388cb13ecbee8
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792503"
---
# <a name="create-devicecompliancescript"></a><span data-ttu-id="3fc34-103">Criar deviceComplianceScript</span><span class="sxs-lookup"><span data-stu-id="3fc34-103">Create deviceComplianceScript</span></span>

<span data-ttu-id="3fc34-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3fc34-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3fc34-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3fc34-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3fc34-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3fc34-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3fc34-107">Criar um novo objeto [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) .</span><span class="sxs-lookup"><span data-stu-id="3fc34-107">Create a new [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3fc34-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3fc34-108">Prerequisites</span></span>
<span data-ttu-id="3fc34-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="3fc34-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="3fc34-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3fc34-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fc34-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3fc34-111">Permission type</span></span>|<span data-ttu-id="3fc34-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3fc34-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3fc34-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3fc34-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3fc34-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fc34-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3fc34-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3fc34-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3fc34-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3fc34-116">Not supported.</span></span>|
|<span data-ttu-id="3fc34-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3fc34-117">Application</span></span>|<span data-ttu-id="3fc34-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fc34-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3fc34-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3fc34-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceComplianceScripts
```

## <a name="request-headers"></a><span data-ttu-id="3fc34-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3fc34-120">Request headers</span></span>
|<span data-ttu-id="3fc34-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3fc34-121">Header</span></span>|<span data-ttu-id="3fc34-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3fc34-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3fc34-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3fc34-123">Authorization</span></span>|<span data-ttu-id="3fc34-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3fc34-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3fc34-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3fc34-125">Accept</span></span>|<span data-ttu-id="3fc34-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3fc34-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fc34-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3fc34-127">Request body</span></span>
<span data-ttu-id="3fc34-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceComplianceScript.</span><span class="sxs-lookup"><span data-stu-id="3fc34-128">In the request body, supply a JSON representation for the deviceComplianceScript object.</span></span>

<span data-ttu-id="3fc34-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceComplianceScript.</span><span class="sxs-lookup"><span data-stu-id="3fc34-129">The following table shows the properties that are required when you create the deviceComplianceScript.</span></span>

|<span data-ttu-id="3fc34-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3fc34-130">Property</span></span>|<span data-ttu-id="3fc34-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3fc34-131">Type</span></span>|<span data-ttu-id="3fc34-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3fc34-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3fc34-133">id</span><span class="sxs-lookup"><span data-stu-id="3fc34-133">id</span></span>|<span data-ttu-id="3fc34-134">String</span><span class="sxs-lookup"><span data-stu-id="3fc34-134">String</span></span>|<span data-ttu-id="3fc34-135">Identificador exclusivo do script de conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="3fc34-135">Unique Identifier for the device compliance script</span></span>|
|<span data-ttu-id="3fc34-136">publicador</span><span class="sxs-lookup"><span data-stu-id="3fc34-136">publisher</span></span>|<span data-ttu-id="3fc34-137">String</span><span class="sxs-lookup"><span data-stu-id="3fc34-137">String</span></span>|<span data-ttu-id="3fc34-138">Nome do editor de scripts de conformidade de dispositivos</span><span class="sxs-lookup"><span data-stu-id="3fc34-138">Name of the device compliance script publisher</span></span>|
|<span data-ttu-id="3fc34-139">versão</span><span class="sxs-lookup"><span data-stu-id="3fc34-139">version</span></span>|<span data-ttu-id="3fc34-140">String</span><span class="sxs-lookup"><span data-stu-id="3fc34-140">String</span></span>|<span data-ttu-id="3fc34-141">Versão do script de conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="3fc34-141">Version of the device compliance script</span></span>|
|<span data-ttu-id="3fc34-142">displayName</span><span class="sxs-lookup"><span data-stu-id="3fc34-142">displayName</span></span>|<span data-ttu-id="3fc34-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3fc34-143">String</span></span>|<span data-ttu-id="3fc34-144">Nome do script de conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="3fc34-144">Name of the device compliance script</span></span>|
|<span data-ttu-id="3fc34-145">description</span><span class="sxs-lookup"><span data-stu-id="3fc34-145">description</span></span>|<span data-ttu-id="3fc34-146">String</span><span class="sxs-lookup"><span data-stu-id="3fc34-146">String</span></span>|<span data-ttu-id="3fc34-147">Descrição do script de conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="3fc34-147">Description of the device compliance script</span></span>|
|<span data-ttu-id="3fc34-148">detectionScriptContent</span><span class="sxs-lookup"><span data-stu-id="3fc34-148">detectionScriptContent</span></span>|<span data-ttu-id="3fc34-149">Binária</span><span class="sxs-lookup"><span data-stu-id="3fc34-149">Binary</span></span>|<span data-ttu-id="3fc34-150">Todo o conteúdo do script do PowerShell de detecção</span><span class="sxs-lookup"><span data-stu-id="3fc34-150">The entire content of the detection powershell script</span></span>|
|<span data-ttu-id="3fc34-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3fc34-151">createdDateTime</span></span>|<span data-ttu-id="3fc34-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3fc34-152">DateTimeOffset</span></span>|<span data-ttu-id="3fc34-153">O carimbo de data/hora de quando o script de conformidade do dispositivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="3fc34-153">The timestamp of when the device compliance script was created.</span></span> <span data-ttu-id="3fc34-154">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3fc34-154">This property is read-only.</span></span>|
|<span data-ttu-id="3fc34-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3fc34-155">lastModifiedDateTime</span></span>|<span data-ttu-id="3fc34-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3fc34-156">DateTimeOffset</span></span>|<span data-ttu-id="3fc34-157">O carimbo de data/hora de quando o script de conformidade do dispositivo foi modificado.</span><span class="sxs-lookup"><span data-stu-id="3fc34-157">The timestamp of when the device compliance script was modified.</span></span> <span data-ttu-id="3fc34-158">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3fc34-158">This property is read-only.</span></span>|
|<span data-ttu-id="3fc34-159">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="3fc34-159">runAsAccount</span></span>|[<span data-ttu-id="3fc34-160">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="3fc34-160">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="3fc34-161">Indica o tipo de contexto de execução.</span><span class="sxs-lookup"><span data-stu-id="3fc34-161">Indicates the type of execution context.</span></span> <span data-ttu-id="3fc34-162">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="3fc34-162">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="3fc34-163">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="3fc34-163">enforceSignatureCheck</span></span>|<span data-ttu-id="3fc34-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="3fc34-164">Boolean</span></span>|<span data-ttu-id="3fc34-165">Indicar se a assinatura do script precisa ser verificada</span><span class="sxs-lookup"><span data-stu-id="3fc34-165">Indicate whether the script signature needs be checked</span></span>|
|<span data-ttu-id="3fc34-166">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="3fc34-166">runAs32Bit</span></span>|<span data-ttu-id="3fc34-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="3fc34-167">Boolean</span></span>|<span data-ttu-id="3fc34-168">Indicar se os scripts do PowerShell devem ser executados como 32 bits</span><span class="sxs-lookup"><span data-stu-id="3fc34-168">Indicate whether PowerShell script(s) should run as 32-bit</span></span>|
|<span data-ttu-id="3fc34-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3fc34-169">roleScopeTagIds</span></span>|<span data-ttu-id="3fc34-170">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3fc34-170">String collection</span></span>|<span data-ttu-id="3fc34-171">Lista de IDs de marca de escopo para o script de conformidade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="3fc34-171">List of Scope Tag IDs for the device compliance script</span></span>|



## <a name="response"></a><span data-ttu-id="3fc34-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="3fc34-172">Response</span></span>
<span data-ttu-id="3fc34-173">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3fc34-173">If successful, this method returns a `201 Created` response code and a [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fc34-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3fc34-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="3fc34-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3fc34-175">Request</span></span>
<span data-ttu-id="3fc34-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3fc34-176">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3fc34-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="3fc34-177">Response</span></span>
<span data-ttu-id="3fc34-178">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="3fc34-178">Here is an example of the response.</span></span> <span data-ttu-id="3fc34-179">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="3fc34-179">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3fc34-180">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="3fc34-180">All of the properties will be returned from an actual call.</span></span>
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



