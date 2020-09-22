---
title: Criar deviceManagementScript
description: Criar um novo objeto deviceManagementScript.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 703532841c6e738b5c06930766ad0478a33677d8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48074374"
---
# <a name="create-devicemanagementscript"></a><span data-ttu-id="73660-103">Criar deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="73660-103">Create deviceManagementScript</span></span>

<span data-ttu-id="73660-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73660-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="73660-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="73660-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73660-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="73660-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73660-107">Criar um novo objeto [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="73660-107">Create a new [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73660-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="73660-108">Prerequisites</span></span>
<span data-ttu-id="73660-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73660-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73660-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="73660-111">Permission type</span></span>|<span data-ttu-id="73660-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="73660-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73660-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="73660-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="73660-114">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="73660-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="73660-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73660-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="73660-116">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="73660-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="73660-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73660-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="73660-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="73660-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73660-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73660-119">Not supported.</span></span>|
|<span data-ttu-id="73660-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="73660-120">Application</span></span>||
| <span data-ttu-id="73660-121">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="73660-121">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="73660-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73660-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="73660-123">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="73660-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="73660-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73660-124">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="73660-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="73660-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="73660-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="73660-126">Request headers</span></span>
|<span data-ttu-id="73660-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="73660-127">Header</span></span>|<span data-ttu-id="73660-128">Valor</span><span class="sxs-lookup"><span data-stu-id="73660-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73660-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="73660-129">Authorization</span></span>|<span data-ttu-id="73660-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73660-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73660-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="73660-131">Accept</span></span>|<span data-ttu-id="73660-132">application/json</span><span class="sxs-lookup"><span data-stu-id="73660-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73660-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="73660-133">Request body</span></span>
<span data-ttu-id="73660-134">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementScript.</span><span class="sxs-lookup"><span data-stu-id="73660-134">In the request body, supply a JSON representation for the deviceManagementScript object.</span></span>

<span data-ttu-id="73660-135">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementScript.</span><span class="sxs-lookup"><span data-stu-id="73660-135">The following table shows the properties that are required when you create the deviceManagementScript.</span></span>

|<span data-ttu-id="73660-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73660-136">Property</span></span>|<span data-ttu-id="73660-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="73660-137">Type</span></span>|<span data-ttu-id="73660-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="73660-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73660-139">id</span><span class="sxs-lookup"><span data-stu-id="73660-139">id</span></span>|<span data-ttu-id="73660-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73660-140">String</span></span>|<span data-ttu-id="73660-141">Identificador exclusivo do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="73660-141">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="73660-142">displayName</span><span class="sxs-lookup"><span data-stu-id="73660-142">displayName</span></span>|<span data-ttu-id="73660-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="73660-143">String</span></span>|<span data-ttu-id="73660-144">Nome do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="73660-144">Name of the device management script.</span></span>|
|<span data-ttu-id="73660-145">description</span><span class="sxs-lookup"><span data-stu-id="73660-145">description</span></span>|<span data-ttu-id="73660-146">String</span><span class="sxs-lookup"><span data-stu-id="73660-146">String</span></span>|<span data-ttu-id="73660-147">Descrição opcional para o script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="73660-147">Optional description for the device management script.</span></span>|
|<span data-ttu-id="73660-148">runSchedule</span><span class="sxs-lookup"><span data-stu-id="73660-148">runSchedule</span></span>|[<span data-ttu-id="73660-149">runSchedule</span><span class="sxs-lookup"><span data-stu-id="73660-149">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="73660-150">O intervalo de execução do script.</span><span class="sxs-lookup"><span data-stu-id="73660-150">The interval for script to run.</span></span> <span data-ttu-id="73660-151">Se não definido, o script será executado uma vez</span><span class="sxs-lookup"><span data-stu-id="73660-151">If not defined the script will run once</span></span>|
|<span data-ttu-id="73660-152">scriptContent</span><span class="sxs-lookup"><span data-stu-id="73660-152">scriptContent</span></span>|<span data-ttu-id="73660-153">Binária</span><span class="sxs-lookup"><span data-stu-id="73660-153">Binary</span></span>|<span data-ttu-id="73660-154">O conteúdo de script.</span><span class="sxs-lookup"><span data-stu-id="73660-154">The script content.</span></span>|
|<span data-ttu-id="73660-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="73660-155">createdDateTime</span></span>|<span data-ttu-id="73660-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73660-156">DateTimeOffset</span></span>|<span data-ttu-id="73660-157">A data e a hora em que o script de gerenciamento de dispositivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="73660-157">The date and time the device management script was created.</span></span> <span data-ttu-id="73660-158">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73660-158">This property is read-only.</span></span>|
|<span data-ttu-id="73660-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="73660-159">lastModifiedDateTime</span></span>|<span data-ttu-id="73660-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73660-160">DateTimeOffset</span></span>|<span data-ttu-id="73660-161">A data e a hora em que o script de gerenciamento de dispositivo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="73660-161">The date and time the device management script was last modified.</span></span> <span data-ttu-id="73660-162">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="73660-162">This property is read-only.</span></span>|
|<span data-ttu-id="73660-163">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="73660-163">runAsAccount</span></span>|[<span data-ttu-id="73660-164">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="73660-164">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="73660-165">Indica o tipo de contexto de execução.</span><span class="sxs-lookup"><span data-stu-id="73660-165">Indicates the type of execution context.</span></span> <span data-ttu-id="73660-166">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="73660-166">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="73660-167">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="73660-167">enforceSignatureCheck</span></span>|<span data-ttu-id="73660-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="73660-168">Boolean</span></span>|<span data-ttu-id="73660-169">Indica se a assinatura do script precisa ser verificada.</span><span class="sxs-lookup"><span data-stu-id="73660-169">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="73660-170">fileName</span><span class="sxs-lookup"><span data-stu-id="73660-170">fileName</span></span>|<span data-ttu-id="73660-171">String</span><span class="sxs-lookup"><span data-stu-id="73660-171">String</span></span>|<span data-ttu-id="73660-172">Nome do arquivo de script.</span><span class="sxs-lookup"><span data-stu-id="73660-172">Script file name.</span></span>|
|<span data-ttu-id="73660-173">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="73660-173">roleScopeTagIds</span></span>|<span data-ttu-id="73660-174">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="73660-174">String collection</span></span>|<span data-ttu-id="73660-175">Lista de IDs de marca de escopo para esta instância de PowerShellScript.</span><span class="sxs-lookup"><span data-stu-id="73660-175">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="73660-176">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="73660-176">runAs32Bit</span></span>|<span data-ttu-id="73660-177">Booliano</span><span class="sxs-lookup"><span data-stu-id="73660-177">Boolean</span></span>|<span data-ttu-id="73660-178">Um valor que indica se o script do PowerShell deve ser executado como 32 bits</span><span class="sxs-lookup"><span data-stu-id="73660-178">A value indicating whether the PowerShell script should run as 32-bit</span></span>|



## <a name="response"></a><span data-ttu-id="73660-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="73660-179">Response</span></span>
<span data-ttu-id="73660-180">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="73660-180">If successful, this method returns a `201 Created` response code and a [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73660-181">Exemplo</span><span class="sxs-lookup"><span data-stu-id="73660-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="73660-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73660-182">Request</span></span>
<span data-ttu-id="73660-183">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="73660-183">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="73660-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="73660-184">Response</span></span>
<span data-ttu-id="73660-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="73660-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









