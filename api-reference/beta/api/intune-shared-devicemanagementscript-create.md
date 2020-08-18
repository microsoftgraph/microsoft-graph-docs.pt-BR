---
title: Criar deviceManagementScript
description: Criar um novo objeto deviceManagementScript.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9fe1cd9b413e3062e6c5ec06770160f0b73c7b08
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46792286"
---
# <a name="create-devicemanagementscript"></a><span data-ttu-id="145d2-103">Criar deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="145d2-103">Create deviceManagementScript</span></span>

<span data-ttu-id="145d2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="145d2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="145d2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="145d2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="145d2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="145d2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="145d2-107">Criar um novo objeto [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="145d2-107">Create a new [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="145d2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="145d2-108">Prerequisites</span></span>
<span data-ttu-id="145d2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="145d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="145d2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="145d2-111">Permission type</span></span>|<span data-ttu-id="145d2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="145d2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="145d2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="145d2-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="145d2-114">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="145d2-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="145d2-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="145d2-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="145d2-116">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="145d2-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="145d2-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="145d2-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="145d2-118">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="145d2-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="145d2-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="145d2-119">Not supported.</span></span>|
|<span data-ttu-id="145d2-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="145d2-120">Application</span></span>||
| <span data-ttu-id="145d2-121">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="145d2-121">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="145d2-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="145d2-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="145d2-123">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="145d2-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="145d2-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="145d2-124">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="145d2-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="145d2-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="145d2-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="145d2-126">Request headers</span></span>
|<span data-ttu-id="145d2-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="145d2-127">Header</span></span>|<span data-ttu-id="145d2-128">Valor</span><span class="sxs-lookup"><span data-stu-id="145d2-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="145d2-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="145d2-129">Authorization</span></span>|<span data-ttu-id="145d2-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="145d2-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="145d2-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="145d2-131">Accept</span></span>|<span data-ttu-id="145d2-132">application/json</span><span class="sxs-lookup"><span data-stu-id="145d2-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="145d2-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="145d2-133">Request body</span></span>
<span data-ttu-id="145d2-134">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementScript.</span><span class="sxs-lookup"><span data-stu-id="145d2-134">In the request body, supply a JSON representation for the deviceManagementScript object.</span></span>

<span data-ttu-id="145d2-135">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementScript.</span><span class="sxs-lookup"><span data-stu-id="145d2-135">The following table shows the properties that are required when you create the deviceManagementScript.</span></span>

|<span data-ttu-id="145d2-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="145d2-136">Property</span></span>|<span data-ttu-id="145d2-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="145d2-137">Type</span></span>|<span data-ttu-id="145d2-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="145d2-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="145d2-139">id</span><span class="sxs-lookup"><span data-stu-id="145d2-139">id</span></span>|<span data-ttu-id="145d2-140">String</span><span class="sxs-lookup"><span data-stu-id="145d2-140">String</span></span>|<span data-ttu-id="145d2-141">Identificador exclusivo do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="145d2-141">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="145d2-142">displayName</span><span class="sxs-lookup"><span data-stu-id="145d2-142">displayName</span></span>|<span data-ttu-id="145d2-143">String</span><span class="sxs-lookup"><span data-stu-id="145d2-143">String</span></span>|<span data-ttu-id="145d2-144">Nome do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="145d2-144">Name of the device management script.</span></span>|
|<span data-ttu-id="145d2-145">description</span><span class="sxs-lookup"><span data-stu-id="145d2-145">description</span></span>|<span data-ttu-id="145d2-146">String</span><span class="sxs-lookup"><span data-stu-id="145d2-146">String</span></span>|<span data-ttu-id="145d2-147">Descrição opcional para o script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="145d2-147">Optional description for the device management script.</span></span>|
|<span data-ttu-id="145d2-148">scriptContent</span><span class="sxs-lookup"><span data-stu-id="145d2-148">scriptContent</span></span>|<span data-ttu-id="145d2-149">Binária</span><span class="sxs-lookup"><span data-stu-id="145d2-149">Binary</span></span>|<span data-ttu-id="145d2-150">O conteúdo de script.</span><span class="sxs-lookup"><span data-stu-id="145d2-150">The script content.</span></span>|
|<span data-ttu-id="145d2-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="145d2-151">createdDateTime</span></span>|<span data-ttu-id="145d2-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="145d2-152">DateTimeOffset</span></span>|<span data-ttu-id="145d2-153">A data e a hora em que o script de gerenciamento de dispositivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="145d2-153">The date and time the device management script was created.</span></span> <span data-ttu-id="145d2-154">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="145d2-154">This property is read-only.</span></span>|
|<span data-ttu-id="145d2-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="145d2-155">lastModifiedDateTime</span></span>|<span data-ttu-id="145d2-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="145d2-156">DateTimeOffset</span></span>|<span data-ttu-id="145d2-157">A data e a hora em que o script de gerenciamento de dispositivo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="145d2-157">The date and time the device management script was last modified.</span></span> <span data-ttu-id="145d2-158">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="145d2-158">This property is read-only.</span></span>|
|<span data-ttu-id="145d2-159">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="145d2-159">runAsAccount</span></span>|[<span data-ttu-id="145d2-160">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="145d2-160">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="145d2-161">Indica o tipo de contexto de execução.</span><span class="sxs-lookup"><span data-stu-id="145d2-161">Indicates the type of execution context.</span></span> <span data-ttu-id="145d2-162">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="145d2-162">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="145d2-163">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="145d2-163">enforceSignatureCheck</span></span>|<span data-ttu-id="145d2-164">Booliano</span><span class="sxs-lookup"><span data-stu-id="145d2-164">Boolean</span></span>|<span data-ttu-id="145d2-165">Indica se a assinatura do script precisa ser verificada.</span><span class="sxs-lookup"><span data-stu-id="145d2-165">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="145d2-166">fileName</span><span class="sxs-lookup"><span data-stu-id="145d2-166">fileName</span></span>|<span data-ttu-id="145d2-167">String</span><span class="sxs-lookup"><span data-stu-id="145d2-167">String</span></span>|<span data-ttu-id="145d2-168">Nome do arquivo de script.</span><span class="sxs-lookup"><span data-stu-id="145d2-168">Script file name.</span></span>|
|<span data-ttu-id="145d2-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="145d2-169">roleScopeTagIds</span></span>|<span data-ttu-id="145d2-170">Coleção de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="145d2-170">String collection</span></span>|<span data-ttu-id="145d2-171">Lista de IDs de marca de escopo para esta instância de PowerShellScript.</span><span class="sxs-lookup"><span data-stu-id="145d2-171">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="145d2-172">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="145d2-172">runAs32Bit</span></span>|<span data-ttu-id="145d2-173">Booliano</span><span class="sxs-lookup"><span data-stu-id="145d2-173">Boolean</span></span>|<span data-ttu-id="145d2-174">Um valor que indica se o script do PowerShell deve ser executado como 32 bits</span><span class="sxs-lookup"><span data-stu-id="145d2-174">A value indicating whether the PowerShell script should run as 32-bit</span></span>|



## <a name="response"></a><span data-ttu-id="145d2-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="145d2-175">Response</span></span>
<span data-ttu-id="145d2-176">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="145d2-176">If successful, this method returns a `201 Created` response code and a [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="145d2-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="145d2-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="145d2-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="145d2-178">Request</span></span>
<span data-ttu-id="145d2-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="145d2-179">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
Content-type: application/json
Content-length: 443

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "displayName": "Display Name value",
  "description": "Description value",
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "runAs32Bit": true
}
```

### <a name="response"></a><span data-ttu-id="145d2-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="145d2-180">Response</span></span>
<span data-ttu-id="145d2-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="145d2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 615

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "id": "59ea4525-4525-59ea-2545-ea592545ea59",
  "displayName": "Display Name value",
  "description": "Description value",
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "runAs32Bit": true
}
```






