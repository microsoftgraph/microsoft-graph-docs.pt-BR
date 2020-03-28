---
title: Atualizar deviceShellScript
description: Atualiza as propriedades de um objeto deviceShellScript.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f9e3c2da2008b5e44f4b13449abd6b63251fe08f
ms.sourcegitcommit: d93fcc2212491567f8322b1cc0c02d37829b6051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/28/2020
ms.locfileid: "43034745"
---
# <a name="update-deviceshellscript"></a><span data-ttu-id="e78e6-103">Atualizar deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="e78e6-103">Update deviceShellScript</span></span>

> <span data-ttu-id="e78e6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e78e6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e78e6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e78e6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e78e6-106">Atualiza as propriedades de um objeto [deviceShellScript](../resources/intune-devices-deviceshellscript.md) .</span><span class="sxs-lookup"><span data-stu-id="e78e6-106">Update the properties of a [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e78e6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e78e6-107">Prerequisites</span></span>
<span data-ttu-id="e78e6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e78e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e78e6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e78e6-110">Permission type</span></span>|<span data-ttu-id="e78e6-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e78e6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e78e6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e78e6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e78e6-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e78e6-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e78e6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e78e6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e78e6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e78e6-115">Not supported.</span></span>|
|<span data-ttu-id="e78e6-116">Application</span><span class="sxs-lookup"><span data-stu-id="e78e6-116">Application</span></span>|<span data-ttu-id="e78e6-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e78e6-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e78e6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e78e6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="e78e6-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e78e6-119">Request headers</span></span>
|<span data-ttu-id="e78e6-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e78e6-120">Header</span></span>|<span data-ttu-id="e78e6-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e78e6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e78e6-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e78e6-122">Authorization</span></span>|<span data-ttu-id="e78e6-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e78e6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e78e6-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e78e6-124">Accept</span></span>|<span data-ttu-id="e78e6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e78e6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e78e6-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e78e6-126">Request body</span></span>
<span data-ttu-id="e78e6-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceShellScript](../resources/intune-devices-deviceshellscript.md) .</span><span class="sxs-lookup"><span data-stu-id="e78e6-127">In the request body, supply a JSON representation for the [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>

<span data-ttu-id="e78e6-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceShellScript](../resources/intune-devices-deviceshellscript.md).</span><span class="sxs-lookup"><span data-stu-id="e78e6-128">The following table shows the properties that are required when you create the [deviceShellScript](../resources/intune-devices-deviceshellscript.md).</span></span>

|<span data-ttu-id="e78e6-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e78e6-129">Property</span></span>|<span data-ttu-id="e78e6-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e78e6-130">Type</span></span>|<span data-ttu-id="e78e6-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e78e6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e78e6-132">executionFrequency</span><span class="sxs-lookup"><span data-stu-id="e78e6-132">executionFrequency</span></span>|<span data-ttu-id="e78e6-133">Duração</span><span class="sxs-lookup"><span data-stu-id="e78e6-133">Duration</span></span>|<span data-ttu-id="e78e6-134">O intervalo de execução do script.</span><span class="sxs-lookup"><span data-stu-id="e78e6-134">The interval for script to run.</span></span> <span data-ttu-id="e78e6-135">Se não definido, o script é executado uma vez.</span><span class="sxs-lookup"><span data-stu-id="e78e6-135">If not defined, the script runs once.</span></span>|
|<span data-ttu-id="e78e6-136">retryCount</span><span class="sxs-lookup"><span data-stu-id="e78e6-136">retryCount</span></span>|<span data-ttu-id="e78e6-137">Int32</span><span class="sxs-lookup"><span data-stu-id="e78e6-137">Int32</span></span>|<span data-ttu-id="e78e6-138">O número de vezes que o script deve ser repetido se falhar.</span><span class="sxs-lookup"><span data-stu-id="e78e6-138">The number of times for the script to be retried if it fails.</span></span>|
|<span data-ttu-id="e78e6-139">blockExecutionNotifications</span><span class="sxs-lookup"><span data-stu-id="e78e6-139">blockExecutionNotifications</span></span>|<span data-ttu-id="e78e6-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="e78e6-140">Boolean</span></span>|<span data-ttu-id="e78e6-141">Indica se o usuário é notificado quando um script é executado.</span><span class="sxs-lookup"><span data-stu-id="e78e6-141">Indicates whether the user is notified when a script runs.</span></span>|
|<span data-ttu-id="e78e6-142">id</span><span class="sxs-lookup"><span data-stu-id="e78e6-142">id</span></span>|<span data-ttu-id="e78e6-143">String</span><span class="sxs-lookup"><span data-stu-id="e78e6-143">String</span></span>|<span data-ttu-id="e78e6-144">Identificador exclusivo do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e78e6-144">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="e78e6-145">displayName</span><span class="sxs-lookup"><span data-stu-id="e78e6-145">displayName</span></span>|<span data-ttu-id="e78e6-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e78e6-146">String</span></span>|<span data-ttu-id="e78e6-147">O nome do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e78e6-147">The name of the device management script.</span></span>|
|<span data-ttu-id="e78e6-148">description</span><span class="sxs-lookup"><span data-stu-id="e78e6-148">description</span></span>|<span data-ttu-id="e78e6-149">String</span><span class="sxs-lookup"><span data-stu-id="e78e6-149">String</span></span>|<span data-ttu-id="e78e6-150">Descrição opcional para o script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e78e6-150">Optional description for the device management script.</span></span>|
|<span data-ttu-id="e78e6-151">scriptContent</span><span class="sxs-lookup"><span data-stu-id="e78e6-151">scriptContent</span></span>|<span data-ttu-id="e78e6-152">Binária</span><span class="sxs-lookup"><span data-stu-id="e78e6-152">Binary</span></span>|<span data-ttu-id="e78e6-153">O conteúdo de script.</span><span class="sxs-lookup"><span data-stu-id="e78e6-153">The script content.</span></span>|
|<span data-ttu-id="e78e6-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e78e6-154">createdDateTime</span></span>|<span data-ttu-id="e78e6-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e78e6-155">DateTimeOffset</span></span>|<span data-ttu-id="e78e6-156">A data e a hora em que o script de gerenciamento de dispositivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="e78e6-156">The date and time the device management script was created.</span></span> <span data-ttu-id="e78e6-157">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e78e6-157">This property is read-only.</span></span>|
|<span data-ttu-id="e78e6-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e78e6-158">lastModifiedDateTime</span></span>|<span data-ttu-id="e78e6-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e78e6-159">DateTimeOffset</span></span>|<span data-ttu-id="e78e6-160">A data e a hora em que o script de gerenciamento de dispositivo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="e78e6-160">The date and time the device management script was last modified.</span></span> <span data-ttu-id="e78e6-161">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e78e6-161">This property is read-only.</span></span>|
|<span data-ttu-id="e78e6-162">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="e78e6-162">runAsAccount</span></span>|[<span data-ttu-id="e78e6-163">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="e78e6-163">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="e78e6-164">Indica o tipo de contexto de execução.</span><span class="sxs-lookup"><span data-stu-id="e78e6-164">Indicates the type of execution context.</span></span> <span data-ttu-id="e78e6-165">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="e78e6-165">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="e78e6-166">fileName</span><span class="sxs-lookup"><span data-stu-id="e78e6-166">fileName</span></span>|<span data-ttu-id="e78e6-167">String</span><span class="sxs-lookup"><span data-stu-id="e78e6-167">String</span></span>|<span data-ttu-id="e78e6-168">O nome do arquivo de script.</span><span class="sxs-lookup"><span data-stu-id="e78e6-168">The script file name.</span></span>|
|<span data-ttu-id="e78e6-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e78e6-169">roleScopeTagIds</span></span>|<span data-ttu-id="e78e6-170">String collection</span><span class="sxs-lookup"><span data-stu-id="e78e6-170">String collection</span></span>|<span data-ttu-id="e78e6-171">A lista de IDs de marca de escopo para esta instância de PowerShellScript.</span><span class="sxs-lookup"><span data-stu-id="e78e6-171">The list of Scope Tag IDs for this PowerShellScript instance.</span></span>|



## <a name="response"></a><span data-ttu-id="e78e6-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="e78e6-172">Response</span></span>
<span data-ttu-id="e78e6-173">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceShellScript](../resources/intune-devices-deviceshellscript.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e78e6-173">If successful, this method returns a `200 OK` response code and an updated [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e78e6-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e78e6-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="e78e6-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e78e6-175">Request</span></span>
<span data-ttu-id="e78e6-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e78e6-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts/{deviceShellScriptId}
Content-type: application/json
Content-length: 409

{
  "@odata.type": "#microsoft.graph.deviceShellScript",
  "executionFrequency": "PT2M43.444327S",
  "retryCount": 10,
  "blockExecutionNotifications": true,
  "displayName": "Display Name value",
  "description": "Description value",
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "runAsAccount": "user",
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="e78e6-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="e78e6-177">Response</span></span>
<span data-ttu-id="e78e6-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e78e6-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 581

{
  "@odata.type": "#microsoft.graph.deviceShellScript",
  "executionFrequency": "PT2M43.444327S",
  "retryCount": 10,
  "blockExecutionNotifications": true,
  "id": "ca9e0ad8-0ad8-ca9e-d80a-9ecad80a9eca",
  "displayName": "Display Name value",
  "description": "Description value",
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "runAsAccount": "user",
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```



