---
title: Atualizar deviceShellScript
description: Atualiza as propriedades de um objeto deviceShellScript.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2791932af6b9c9e4963dd5fa1da66a32876c1541
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49228509"
---
# <a name="update-deviceshellscript"></a><span data-ttu-id="0735d-103">Atualizar deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="0735d-103">Update deviceShellScript</span></span>

<span data-ttu-id="0735d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0735d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0735d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0735d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0735d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0735d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0735d-107">Atualiza as propriedades de um objeto [deviceShellScript](../resources/intune-devices-deviceshellscript.md) .</span><span class="sxs-lookup"><span data-stu-id="0735d-107">Update the properties of a [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0735d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0735d-108">Prerequisites</span></span>
<span data-ttu-id="0735d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0735d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0735d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0735d-111">Permission type</span></span>|<span data-ttu-id="0735d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0735d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0735d-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0735d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0735d-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0735d-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0735d-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0735d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0735d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0735d-116">Not supported.</span></span>|
|<span data-ttu-id="0735d-117">Application</span><span class="sxs-lookup"><span data-stu-id="0735d-117">Application</span></span>|<span data-ttu-id="0735d-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0735d-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0735d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0735d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="0735d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0735d-120">Request headers</span></span>
|<span data-ttu-id="0735d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0735d-121">Header</span></span>|<span data-ttu-id="0735d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0735d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0735d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0735d-123">Authorization</span></span>|<span data-ttu-id="0735d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0735d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0735d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0735d-125">Accept</span></span>|<span data-ttu-id="0735d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0735d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0735d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0735d-127">Request body</span></span>
<span data-ttu-id="0735d-128">No corpo da solicitação, forneça uma representação JSON do objeto [deviceShellScript](../resources/intune-devices-deviceshellscript.md) .</span><span class="sxs-lookup"><span data-stu-id="0735d-128">In the request body, supply a JSON representation for the [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>

<span data-ttu-id="0735d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceShellScript](../resources/intune-devices-deviceshellscript.md).</span><span class="sxs-lookup"><span data-stu-id="0735d-129">The following table shows the properties that are required when you create the [deviceShellScript](../resources/intune-devices-deviceshellscript.md).</span></span>

|<span data-ttu-id="0735d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0735d-130">Property</span></span>|<span data-ttu-id="0735d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0735d-131">Type</span></span>|<span data-ttu-id="0735d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0735d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0735d-133">executionFrequency</span><span class="sxs-lookup"><span data-stu-id="0735d-133">executionFrequency</span></span>|<span data-ttu-id="0735d-134">Duração</span><span class="sxs-lookup"><span data-stu-id="0735d-134">Duration</span></span>|<span data-ttu-id="0735d-135">O intervalo de execução do script.</span><span class="sxs-lookup"><span data-stu-id="0735d-135">The interval for script to run.</span></span> <span data-ttu-id="0735d-136">Se não definido, o script será executado uma vez</span><span class="sxs-lookup"><span data-stu-id="0735d-136">If not defined the script will run once</span></span>|
|<span data-ttu-id="0735d-137">retryCount</span><span class="sxs-lookup"><span data-stu-id="0735d-137">retryCount</span></span>|<span data-ttu-id="0735d-138">Int32</span><span class="sxs-lookup"><span data-stu-id="0735d-138">Int32</span></span>|<span data-ttu-id="0735d-139">Número de vezes que o script deve ser repetido se falhar</span><span class="sxs-lookup"><span data-stu-id="0735d-139">Number of times for the script to be retried if it fails</span></span>|
|<span data-ttu-id="0735d-140">blockExecutionNotifications</span><span class="sxs-lookup"><span data-stu-id="0735d-140">blockExecutionNotifications</span></span>|<span data-ttu-id="0735d-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="0735d-141">Boolean</span></span>|<span data-ttu-id="0735d-142">Não notifica o usuário de que um script está sendo executado</span><span class="sxs-lookup"><span data-stu-id="0735d-142">Does not notify the user a script is being executed</span></span>|
|<span data-ttu-id="0735d-143">id</span><span class="sxs-lookup"><span data-stu-id="0735d-143">id</span></span>|<span data-ttu-id="0735d-144">String</span><span class="sxs-lookup"><span data-stu-id="0735d-144">String</span></span>|<span data-ttu-id="0735d-145">Identificador exclusivo do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0735d-145">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="0735d-146">displayName</span><span class="sxs-lookup"><span data-stu-id="0735d-146">displayName</span></span>|<span data-ttu-id="0735d-147">String</span><span class="sxs-lookup"><span data-stu-id="0735d-147">String</span></span>|<span data-ttu-id="0735d-148">Nome do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0735d-148">Name of the device management script.</span></span>|
|<span data-ttu-id="0735d-149">description</span><span class="sxs-lookup"><span data-stu-id="0735d-149">description</span></span>|<span data-ttu-id="0735d-150">String</span><span class="sxs-lookup"><span data-stu-id="0735d-150">String</span></span>|<span data-ttu-id="0735d-151">Descrição opcional para o script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0735d-151">Optional description for the device management script.</span></span>|
|<span data-ttu-id="0735d-152">scriptContent</span><span class="sxs-lookup"><span data-stu-id="0735d-152">scriptContent</span></span>|<span data-ttu-id="0735d-153">Binária</span><span class="sxs-lookup"><span data-stu-id="0735d-153">Binary</span></span>|<span data-ttu-id="0735d-154">O conteúdo de script.</span><span class="sxs-lookup"><span data-stu-id="0735d-154">The script content.</span></span>|
|<span data-ttu-id="0735d-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0735d-155">createdDateTime</span></span>|<span data-ttu-id="0735d-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0735d-156">DateTimeOffset</span></span>|<span data-ttu-id="0735d-157">A data e a hora em que o script de gerenciamento de dispositivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="0735d-157">The date and time the device management script was created.</span></span> <span data-ttu-id="0735d-158">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0735d-158">This property is read-only.</span></span>|
|<span data-ttu-id="0735d-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0735d-159">lastModifiedDateTime</span></span>|<span data-ttu-id="0735d-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0735d-160">DateTimeOffset</span></span>|<span data-ttu-id="0735d-161">A data e a hora em que o script de gerenciamento de dispositivo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="0735d-161">The date and time the device management script was last modified.</span></span> <span data-ttu-id="0735d-162">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0735d-162">This property is read-only.</span></span>|
|<span data-ttu-id="0735d-163">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="0735d-163">runAsAccount</span></span>|[<span data-ttu-id="0735d-164">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="0735d-164">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="0735d-165">Indica o tipo de contexto de execução.</span><span class="sxs-lookup"><span data-stu-id="0735d-165">Indicates the type of execution context.</span></span> <span data-ttu-id="0735d-166">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="0735d-166">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="0735d-167">fileName</span><span class="sxs-lookup"><span data-stu-id="0735d-167">fileName</span></span>|<span data-ttu-id="0735d-168">String</span><span class="sxs-lookup"><span data-stu-id="0735d-168">String</span></span>|<span data-ttu-id="0735d-169">Nome do arquivo de script.</span><span class="sxs-lookup"><span data-stu-id="0735d-169">Script file name.</span></span>|
|<span data-ttu-id="0735d-170">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0735d-170">roleScopeTagIds</span></span>|<span data-ttu-id="0735d-171">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0735d-171">String collection</span></span>|<span data-ttu-id="0735d-172">Lista de IDs de marca de escopo para esta instância de PowerShellScript.</span><span class="sxs-lookup"><span data-stu-id="0735d-172">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|



## <a name="response"></a><span data-ttu-id="0735d-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="0735d-173">Response</span></span>
<span data-ttu-id="0735d-174">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [deviceShellScript](../resources/intune-devices-deviceshellscript.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0735d-174">If successful, this method returns a `200 OK` response code and an updated [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0735d-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0735d-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="0735d-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0735d-176">Request</span></span>
<span data-ttu-id="0735d-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0735d-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0735d-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="0735d-178">Response</span></span>
<span data-ttu-id="0735d-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0735d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




