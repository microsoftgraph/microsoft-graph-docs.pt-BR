---
title: Criar deviceShellScript
description: Criar um novo objeto deviceShellScript.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f310a1b2b83effda2af1a2a73406325f78a06f3d
ms.sourcegitcommit: d93fcc2212491567f8322b1cc0c02d37829b6051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/28/2020
ms.locfileid: "43034752"
---
# <a name="create-deviceshellscript"></a><span data-ttu-id="80514-103">Criar deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="80514-103">Create deviceShellScript</span></span>

> <span data-ttu-id="80514-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="80514-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="80514-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="80514-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80514-106">Criar um novo objeto [deviceShellScript](../resources/intune-devices-deviceshellscript.md) .</span><span class="sxs-lookup"><span data-stu-id="80514-106">Create a new [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80514-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="80514-107">Prerequisites</span></span>
<span data-ttu-id="80514-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80514-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80514-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="80514-110">Permission type</span></span>|<span data-ttu-id="80514-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="80514-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80514-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="80514-112">Delegated (work or school account)</span></span>|<span data-ttu-id="80514-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80514-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="80514-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="80514-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80514-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80514-115">Not supported.</span></span>|
|<span data-ttu-id="80514-116">Application</span><span class="sxs-lookup"><span data-stu-id="80514-116">Application</span></span>|<span data-ttu-id="80514-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80514-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="80514-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="80514-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceShellScripts
```

## <a name="request-headers"></a><span data-ttu-id="80514-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="80514-119">Request headers</span></span>
|<span data-ttu-id="80514-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="80514-120">Header</span></span>|<span data-ttu-id="80514-121">Valor</span><span class="sxs-lookup"><span data-stu-id="80514-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80514-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="80514-122">Authorization</span></span>|<span data-ttu-id="80514-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="80514-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80514-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="80514-124">Accept</span></span>|<span data-ttu-id="80514-125">application/json</span><span class="sxs-lookup"><span data-stu-id="80514-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80514-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="80514-126">Request body</span></span>
<span data-ttu-id="80514-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceShellScript.</span><span class="sxs-lookup"><span data-stu-id="80514-127">In the request body, supply a JSON representation for the deviceShellScript object.</span></span>

<span data-ttu-id="80514-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceShellScript.</span><span class="sxs-lookup"><span data-stu-id="80514-128">The following table shows the properties that are required when you create the deviceShellScript.</span></span>

|<span data-ttu-id="80514-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80514-129">Property</span></span>|<span data-ttu-id="80514-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="80514-130">Type</span></span>|<span data-ttu-id="80514-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="80514-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80514-132">executionFrequency</span><span class="sxs-lookup"><span data-stu-id="80514-132">executionFrequency</span></span>|<span data-ttu-id="80514-133">Duração</span><span class="sxs-lookup"><span data-stu-id="80514-133">Duration</span></span>|<span data-ttu-id="80514-134">O intervalo do script a ser executado.</span><span class="sxs-lookup"><span data-stu-id="80514-134">The interval for the script to run.</span></span> <span data-ttu-id="80514-135">Se não definido, o script é executado uma vez.</span><span class="sxs-lookup"><span data-stu-id="80514-135">If not defined, the script runs once.</span></span>|
|<span data-ttu-id="80514-136">retryCount</span><span class="sxs-lookup"><span data-stu-id="80514-136">retryCount</span></span>|<span data-ttu-id="80514-137">Int32</span><span class="sxs-lookup"><span data-stu-id="80514-137">Int32</span></span>| <span data-ttu-id="80514-138">O número de vezes que o script deve ser repetido se falhar.</span><span class="sxs-lookup"><span data-stu-id="80514-138">The number of times for the script to be retried if it fails.</span></span> |
|<span data-ttu-id="80514-139">blockExecutionNotifications</span><span class="sxs-lookup"><span data-stu-id="80514-139">blockExecutionNotifications</span></span>|<span data-ttu-id="80514-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="80514-140">Boolean</span></span>|<span data-ttu-id="80514-141">Indica se o usuário é notificado quando um script está sendo executado.</span><span class="sxs-lookup"><span data-stu-id="80514-141">Indicates whether the user is notified when a script is being executed.</span></span>|
|<span data-ttu-id="80514-142">id</span><span class="sxs-lookup"><span data-stu-id="80514-142">id</span></span>|<span data-ttu-id="80514-143">String</span><span class="sxs-lookup"><span data-stu-id="80514-143">String</span></span>|<span data-ttu-id="80514-144">Identificador exclusivo do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="80514-144">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="80514-145">displayName</span><span class="sxs-lookup"><span data-stu-id="80514-145">displayName</span></span>|<span data-ttu-id="80514-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80514-146">String</span></span>|<span data-ttu-id="80514-147">Nome do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="80514-147">Name of the device management script.</span></span>|
|<span data-ttu-id="80514-148">description</span><span class="sxs-lookup"><span data-stu-id="80514-148">description</span></span>|<span data-ttu-id="80514-149">String</span><span class="sxs-lookup"><span data-stu-id="80514-149">String</span></span>|<span data-ttu-id="80514-150">Descrição opcional para o script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="80514-150">Optional description for the device management script.</span></span>|
|<span data-ttu-id="80514-151">scriptContent</span><span class="sxs-lookup"><span data-stu-id="80514-151">scriptContent</span></span>|<span data-ttu-id="80514-152">Binária</span><span class="sxs-lookup"><span data-stu-id="80514-152">Binary</span></span>|<span data-ttu-id="80514-153">O conteúdo de script.</span><span class="sxs-lookup"><span data-stu-id="80514-153">The script content.</span></span>|
|<span data-ttu-id="80514-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="80514-154">createdDateTime</span></span>|<span data-ttu-id="80514-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80514-155">DateTimeOffset</span></span>|<span data-ttu-id="80514-156">A data e a hora em que o script de gerenciamento de dispositivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="80514-156">The date and time the device management script was created.</span></span> <span data-ttu-id="80514-157">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="80514-157">This property is read-only.</span></span>|
|<span data-ttu-id="80514-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="80514-158">lastModifiedDateTime</span></span>|<span data-ttu-id="80514-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80514-159">DateTimeOffset</span></span>|<span data-ttu-id="80514-160">A data e a hora em que o script de gerenciamento de dispositivo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="80514-160">The date and time the device management script was last modified.</span></span> <span data-ttu-id="80514-161">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="80514-161">This property is read-only.</span></span>|
|<span data-ttu-id="80514-162">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="80514-162">runAsAccount</span></span>|[<span data-ttu-id="80514-163">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="80514-163">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="80514-164">Indica o tipo de contexto de execução.</span><span class="sxs-lookup"><span data-stu-id="80514-164">Indicates the type of execution context.</span></span> <span data-ttu-id="80514-165">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="80514-165">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="80514-166">fileName</span><span class="sxs-lookup"><span data-stu-id="80514-166">fileName</span></span>|<span data-ttu-id="80514-167">String</span><span class="sxs-lookup"><span data-stu-id="80514-167">String</span></span>|<span data-ttu-id="80514-168">O nome do arquivo de script.</span><span class="sxs-lookup"><span data-stu-id="80514-168">The script file name.</span></span>|
|<span data-ttu-id="80514-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="80514-169">roleScopeTagIds</span></span>|<span data-ttu-id="80514-170">String collection</span><span class="sxs-lookup"><span data-stu-id="80514-170">String collection</span></span>|<span data-ttu-id="80514-171">A lista de IDs de marca de escopo para esta instância de PowerShellScript.</span><span class="sxs-lookup"><span data-stu-id="80514-171">The list of Scope Tag IDs for this PowerShellScript instance.</span></span>|



## <a name="response"></a><span data-ttu-id="80514-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="80514-172">Response</span></span>
<span data-ttu-id="80514-173">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceShellScript](../resources/intune-devices-deviceshellscript.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="80514-173">If successful, this method returns a `201 Created` response code and a [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80514-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="80514-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="80514-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80514-175">Request</span></span>
<span data-ttu-id="80514-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="80514-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts
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

### <a name="response"></a><span data-ttu-id="80514-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="80514-177">Response</span></span>
<span data-ttu-id="80514-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="80514-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



