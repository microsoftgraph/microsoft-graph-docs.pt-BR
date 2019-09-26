---
title: Criar deviceManagementScript
description: Criar um novo objeto deviceManagementScript.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3c0e304af885579aaf4ad42fb5c5391d7f12d2fb
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199428"
---
# <a name="create-devicemanagementscript"></a><span data-ttu-id="8d23a-103">Criar deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="8d23a-103">Create deviceManagementScript</span></span>

> <span data-ttu-id="8d23a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8d23a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d23a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8d23a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d23a-106">Criar um novo objeto [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="8d23a-106">Create a new [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d23a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8d23a-107">Prerequisites</span></span>
<span data-ttu-id="8d23a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d23a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d23a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8d23a-110">Permission type</span></span>|<span data-ttu-id="8d23a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8d23a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d23a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8d23a-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8d23a-113">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="8d23a-113">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="8d23a-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d23a-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="8d23a-115">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="8d23a-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="8d23a-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d23a-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8d23a-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8d23a-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d23a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8d23a-118">Not supported.</span></span>|
|<span data-ttu-id="8d23a-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8d23a-119">Application</span></span>||
| <span data-ttu-id="8d23a-120">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="8d23a-120">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="8d23a-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d23a-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="8d23a-122">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="8d23a-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="8d23a-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d23a-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d23a-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8d23a-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="8d23a-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8d23a-125">Request headers</span></span>
|<span data-ttu-id="8d23a-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8d23a-126">Header</span></span>|<span data-ttu-id="8d23a-127">Valor</span><span class="sxs-lookup"><span data-stu-id="8d23a-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d23a-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="8d23a-128">Authorization</span></span>|<span data-ttu-id="8d23a-129">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8d23a-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d23a-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8d23a-130">Accept</span></span>|<span data-ttu-id="8d23a-131">application/json</span><span class="sxs-lookup"><span data-stu-id="8d23a-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d23a-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8d23a-132">Request body</span></span>
<span data-ttu-id="8d23a-133">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementScript.</span><span class="sxs-lookup"><span data-stu-id="8d23a-133">In the request body, supply a JSON representation for the deviceManagementScript object.</span></span>

<span data-ttu-id="8d23a-134">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementScript.</span><span class="sxs-lookup"><span data-stu-id="8d23a-134">The following table shows the properties that are required when you create the deviceManagementScript.</span></span>

|<span data-ttu-id="8d23a-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8d23a-135">Property</span></span>|<span data-ttu-id="8d23a-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d23a-136">Type</span></span>|<span data-ttu-id="8d23a-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d23a-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d23a-138">id</span><span class="sxs-lookup"><span data-stu-id="8d23a-138">id</span></span>|<span data-ttu-id="8d23a-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8d23a-139">String</span></span>|<span data-ttu-id="8d23a-140">Identificador exclusivo do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8d23a-140">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="8d23a-141">displayName</span><span class="sxs-lookup"><span data-stu-id="8d23a-141">displayName</span></span>|<span data-ttu-id="8d23a-142">String</span><span class="sxs-lookup"><span data-stu-id="8d23a-142">String</span></span>|<span data-ttu-id="8d23a-143">Nome do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8d23a-143">Name of the device management script.</span></span>|
|<span data-ttu-id="8d23a-144">descrição</span><span class="sxs-lookup"><span data-stu-id="8d23a-144">description</span></span>|<span data-ttu-id="8d23a-145">String</span><span class="sxs-lookup"><span data-stu-id="8d23a-145">String</span></span>|<span data-ttu-id="8d23a-146">Descrição opcional para o script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8d23a-146">Optional description for the device management script.</span></span>|
|<span data-ttu-id="8d23a-147">runSchedule</span><span class="sxs-lookup"><span data-stu-id="8d23a-147">runSchedule</span></span>|[<span data-ttu-id="8d23a-148">runSchedule</span><span class="sxs-lookup"><span data-stu-id="8d23a-148">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="8d23a-149">O intervalo de execução do script.</span><span class="sxs-lookup"><span data-stu-id="8d23a-149">The interval for script to run.</span></span> <span data-ttu-id="8d23a-150">Se não definido, o script será executado uma vez</span><span class="sxs-lookup"><span data-stu-id="8d23a-150">If not defined the script will run once</span></span>|
|<span data-ttu-id="8d23a-151">scriptContent</span><span class="sxs-lookup"><span data-stu-id="8d23a-151">scriptContent</span></span>|<span data-ttu-id="8d23a-152">Binária</span><span class="sxs-lookup"><span data-stu-id="8d23a-152">Binary</span></span>|<span data-ttu-id="8d23a-153">O conteúdo de script.</span><span class="sxs-lookup"><span data-stu-id="8d23a-153">The script content.</span></span>|
|<span data-ttu-id="8d23a-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8d23a-154">createdDateTime</span></span>|<span data-ttu-id="8d23a-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d23a-155">DateTimeOffset</span></span>|<span data-ttu-id="8d23a-156">A data e a hora em que o script de gerenciamento de dispositivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="8d23a-156">The date and time the device management script was created.</span></span> <span data-ttu-id="8d23a-157">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8d23a-157">This property is read-only.</span></span>|
|<span data-ttu-id="8d23a-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d23a-158">lastModifiedDateTime</span></span>|<span data-ttu-id="8d23a-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d23a-159">DateTimeOffset</span></span>|<span data-ttu-id="8d23a-160">A data e a hora em que o script de gerenciamento de dispositivo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="8d23a-160">The date and time the device management script was last modified.</span></span> <span data-ttu-id="8d23a-161">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8d23a-161">This property is read-only.</span></span>|
|<span data-ttu-id="8d23a-162">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="8d23a-162">runAsAccount</span></span>|[<span data-ttu-id="8d23a-163">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="8d23a-163">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="8d23a-164">Indica o tipo de contexto de execução.</span><span class="sxs-lookup"><span data-stu-id="8d23a-164">Indicates the type of execution context.</span></span> <span data-ttu-id="8d23a-165">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="8d23a-165">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="8d23a-166">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="8d23a-166">enforceSignatureCheck</span></span>|<span data-ttu-id="8d23a-167">Booliano</span><span class="sxs-lookup"><span data-stu-id="8d23a-167">Boolean</span></span>|<span data-ttu-id="8d23a-168">Indica se a assinatura do script precisa ser verificada.</span><span class="sxs-lookup"><span data-stu-id="8d23a-168">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="8d23a-169">fileName</span><span class="sxs-lookup"><span data-stu-id="8d23a-169">fileName</span></span>|<span data-ttu-id="8d23a-170">String</span><span class="sxs-lookup"><span data-stu-id="8d23a-170">String</span></span>|<span data-ttu-id="8d23a-171">Nome do arquivo de script.</span><span class="sxs-lookup"><span data-stu-id="8d23a-171">Script file name.</span></span>|
|<span data-ttu-id="8d23a-172">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8d23a-172">roleScopeTagIds</span></span>|<span data-ttu-id="8d23a-173">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8d23a-173">String collection</span></span>|<span data-ttu-id="8d23a-174">Lista de IDs de marca de escopo para esta instância de PowerShellScript.</span><span class="sxs-lookup"><span data-stu-id="8d23a-174">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="8d23a-175">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="8d23a-175">runAs32Bit</span></span>|<span data-ttu-id="8d23a-176">Booliano</span><span class="sxs-lookup"><span data-stu-id="8d23a-176">Boolean</span></span>|<span data-ttu-id="8d23a-177">Um valor que indica se o script do PowerShell deve ser executado como 32 bits</span><span class="sxs-lookup"><span data-stu-id="8d23a-177">A value indicating whether the PowerShell script should run as 32-bit</span></span>|



## <a name="response"></a><span data-ttu-id="8d23a-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d23a-178">Response</span></span>
<span data-ttu-id="8d23a-179">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8d23a-179">If successful, this method returns a `201 Created` response code and a [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d23a-180">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8d23a-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d23a-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8d23a-181">Request</span></span>
<span data-ttu-id="8d23a-182">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8d23a-182">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
Content-type: application/json
Content-length: 443

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
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
  "runAs32Bit": true
}
```

### <a name="response"></a><span data-ttu-id="8d23a-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="8d23a-183">Response</span></span>
<span data-ttu-id="8d23a-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8d23a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 615

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "id": "59ea4525-4525-59ea-2545-ea592545ea59",
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
  "runAs32Bit": true
}
```




