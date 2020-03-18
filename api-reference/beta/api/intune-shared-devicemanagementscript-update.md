---
title: Atualizar deviceManagementScript
description: Atualiza as propriedades de um objeto deviceManagementScript.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b3d27fdbaf7de530783c4751c7898dd972f45db2
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42800946"
---
# <a name="update-devicemanagementscript"></a><span data-ttu-id="2089b-103">Atualizar deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="2089b-103">Update deviceManagementScript</span></span>

> <span data-ttu-id="2089b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2089b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2089b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2089b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2089b-106">Atualiza as propriedades de um objeto [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="2089b-106">Update the properties of a [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2089b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2089b-107">Prerequisites</span></span>
<span data-ttu-id="2089b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2089b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2089b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2089b-110">Permission type</span></span>|<span data-ttu-id="2089b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2089b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2089b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2089b-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2089b-113">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="2089b-113">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="2089b-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2089b-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="2089b-115">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="2089b-115">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="2089b-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2089b-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2089b-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2089b-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2089b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2089b-118">Not supported.</span></span>|
|<span data-ttu-id="2089b-119">Application</span><span class="sxs-lookup"><span data-stu-id="2089b-119">Application</span></span>||
| <span data-ttu-id="2089b-120">&nbsp; &nbsp; **Gerenciamento de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="2089b-120">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="2089b-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2089b-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="2089b-122">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="2089b-122">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="2089b-123">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2089b-123">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2089b-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2089b-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="2089b-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2089b-125">Request headers</span></span>
|<span data-ttu-id="2089b-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2089b-126">Header</span></span>|<span data-ttu-id="2089b-127">Valor</span><span class="sxs-lookup"><span data-stu-id="2089b-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2089b-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="2089b-128">Authorization</span></span>|<span data-ttu-id="2089b-129">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2089b-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2089b-130">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2089b-130">Accept</span></span>|<span data-ttu-id="2089b-131">application/json</span><span class="sxs-lookup"><span data-stu-id="2089b-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2089b-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2089b-132">Request body</span></span>
<span data-ttu-id="2089b-133">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="2089b-133">In the request body, supply a JSON representation for the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>

<span data-ttu-id="2089b-134">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).</span><span class="sxs-lookup"><span data-stu-id="2089b-134">The following table shows the properties that are required when you create the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).</span></span>

|<span data-ttu-id="2089b-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2089b-135">Property</span></span>|<span data-ttu-id="2089b-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="2089b-136">Type</span></span>|<span data-ttu-id="2089b-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="2089b-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2089b-138">id</span><span class="sxs-lookup"><span data-stu-id="2089b-138">id</span></span>|<span data-ttu-id="2089b-139">String</span><span class="sxs-lookup"><span data-stu-id="2089b-139">String</span></span>|<span data-ttu-id="2089b-140">Identificador exclusivo do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2089b-140">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="2089b-141">displayName</span><span class="sxs-lookup"><span data-stu-id="2089b-141">displayName</span></span>|<span data-ttu-id="2089b-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2089b-142">String</span></span>|<span data-ttu-id="2089b-143">Nome do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2089b-143">Name of the device management script.</span></span>|
|<span data-ttu-id="2089b-144">description</span><span class="sxs-lookup"><span data-stu-id="2089b-144">description</span></span>|<span data-ttu-id="2089b-145">String</span><span class="sxs-lookup"><span data-stu-id="2089b-145">String</span></span>|<span data-ttu-id="2089b-146">Descrição opcional para o script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2089b-146">Optional description for the device management script.</span></span>|
|<span data-ttu-id="2089b-147">runSchedule</span><span class="sxs-lookup"><span data-stu-id="2089b-147">runSchedule</span></span>|[<span data-ttu-id="2089b-148">runSchedule</span><span class="sxs-lookup"><span data-stu-id="2089b-148">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="2089b-149">O intervalo de execução do script.</span><span class="sxs-lookup"><span data-stu-id="2089b-149">The interval for script to run.</span></span> <span data-ttu-id="2089b-150">Se não definido, o script será executado uma vez</span><span class="sxs-lookup"><span data-stu-id="2089b-150">If not defined the script will run once</span></span>|
|<span data-ttu-id="2089b-151">scriptContent</span><span class="sxs-lookup"><span data-stu-id="2089b-151">scriptContent</span></span>|<span data-ttu-id="2089b-152">Binária</span><span class="sxs-lookup"><span data-stu-id="2089b-152">Binary</span></span>|<span data-ttu-id="2089b-153">O conteúdo de script.</span><span class="sxs-lookup"><span data-stu-id="2089b-153">The script content.</span></span>|
|<span data-ttu-id="2089b-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2089b-154">createdDateTime</span></span>|<span data-ttu-id="2089b-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2089b-155">DateTimeOffset</span></span>|<span data-ttu-id="2089b-156">A data e a hora em que o script de gerenciamento de dispositivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="2089b-156">The date and time the device management script was created.</span></span> <span data-ttu-id="2089b-157">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2089b-157">This property is read-only.</span></span>|
|<span data-ttu-id="2089b-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2089b-158">lastModifiedDateTime</span></span>|<span data-ttu-id="2089b-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2089b-159">DateTimeOffset</span></span>|<span data-ttu-id="2089b-160">A data e a hora em que o script de gerenciamento de dispositivo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="2089b-160">The date and time the device management script was last modified.</span></span> <span data-ttu-id="2089b-161">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2089b-161">This property is read-only.</span></span>|
|<span data-ttu-id="2089b-162">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="2089b-162">runAsAccount</span></span>|[<span data-ttu-id="2089b-163">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="2089b-163">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="2089b-164">Indica o tipo de contexto de execução.</span><span class="sxs-lookup"><span data-stu-id="2089b-164">Indicates the type of execution context.</span></span> <span data-ttu-id="2089b-165">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="2089b-165">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="2089b-166">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="2089b-166">enforceSignatureCheck</span></span>|<span data-ttu-id="2089b-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="2089b-167">Boolean</span></span>|<span data-ttu-id="2089b-168">Indica se a assinatura do script precisa ser verificada.</span><span class="sxs-lookup"><span data-stu-id="2089b-168">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="2089b-169">fileName</span><span class="sxs-lookup"><span data-stu-id="2089b-169">fileName</span></span>|<span data-ttu-id="2089b-170">String</span><span class="sxs-lookup"><span data-stu-id="2089b-170">String</span></span>|<span data-ttu-id="2089b-171">Nome do arquivo de script.</span><span class="sxs-lookup"><span data-stu-id="2089b-171">Script file name.</span></span>|
|<span data-ttu-id="2089b-172">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2089b-172">roleScopeTagIds</span></span>|<span data-ttu-id="2089b-173">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2089b-173">String collection</span></span>|<span data-ttu-id="2089b-174">Lista de IDs de marca de escopo para esta instância de PowerShellScript.</span><span class="sxs-lookup"><span data-stu-id="2089b-174">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="2089b-175">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="2089b-175">runAs32Bit</span></span>|<span data-ttu-id="2089b-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="2089b-176">Boolean</span></span>|<span data-ttu-id="2089b-177">Um valor que indica se o script do PowerShell deve ser executado como 32 bits</span><span class="sxs-lookup"><span data-stu-id="2089b-177">A value indicating whether the PowerShell script should run as 32-bit</span></span>|



## <a name="response"></a><span data-ttu-id="2089b-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="2089b-178">Response</span></span>
<span data-ttu-id="2089b-179">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2089b-179">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2089b-180">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2089b-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="2089b-181">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2089b-181">Request</span></span>
<span data-ttu-id="2089b-182">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2089b-182">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
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

### <a name="response"></a><span data-ttu-id="2089b-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="2089b-183">Response</span></span>
<span data-ttu-id="2089b-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2089b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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







