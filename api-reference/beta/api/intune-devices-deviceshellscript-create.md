---
title: Criar deviceShellScript
description: Criar um novo objeto deviceShellScript.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: de06b3bb33def4f9278dcc247169d167dcbc2edd
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49228635"
---
# <a name="create-deviceshellscript"></a><span data-ttu-id="1070b-103">Criar deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="1070b-103">Create deviceShellScript</span></span>

<span data-ttu-id="1070b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1070b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1070b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1070b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1070b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1070b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1070b-107">Criar um novo objeto [deviceShellScript](../resources/intune-devices-deviceshellscript.md) .</span><span class="sxs-lookup"><span data-stu-id="1070b-107">Create a new [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1070b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1070b-108">Prerequisites</span></span>
<span data-ttu-id="1070b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1070b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1070b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1070b-111">Permission type</span></span>|<span data-ttu-id="1070b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1070b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1070b-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1070b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1070b-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1070b-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1070b-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1070b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1070b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1070b-116">Not supported.</span></span>|
|<span data-ttu-id="1070b-117">Application</span><span class="sxs-lookup"><span data-stu-id="1070b-117">Application</span></span>|<span data-ttu-id="1070b-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1070b-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1070b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1070b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceShellScripts
```

## <a name="request-headers"></a><span data-ttu-id="1070b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1070b-120">Request headers</span></span>
|<span data-ttu-id="1070b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1070b-121">Header</span></span>|<span data-ttu-id="1070b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1070b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1070b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1070b-123">Authorization</span></span>|<span data-ttu-id="1070b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1070b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1070b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1070b-125">Accept</span></span>|<span data-ttu-id="1070b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1070b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1070b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1070b-127">Request body</span></span>
<span data-ttu-id="1070b-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceShellScript.</span><span class="sxs-lookup"><span data-stu-id="1070b-128">In the request body, supply a JSON representation for the deviceShellScript object.</span></span>

<span data-ttu-id="1070b-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceShellScript.</span><span class="sxs-lookup"><span data-stu-id="1070b-129">The following table shows the properties that are required when you create the deviceShellScript.</span></span>

|<span data-ttu-id="1070b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1070b-130">Property</span></span>|<span data-ttu-id="1070b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1070b-131">Type</span></span>|<span data-ttu-id="1070b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1070b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1070b-133">executionFrequency</span><span class="sxs-lookup"><span data-stu-id="1070b-133">executionFrequency</span></span>|<span data-ttu-id="1070b-134">Duração</span><span class="sxs-lookup"><span data-stu-id="1070b-134">Duration</span></span>|<span data-ttu-id="1070b-135">O intervalo de execução do script.</span><span class="sxs-lookup"><span data-stu-id="1070b-135">The interval for script to run.</span></span> <span data-ttu-id="1070b-136">Se não definido, o script será executado uma vez</span><span class="sxs-lookup"><span data-stu-id="1070b-136">If not defined the script will run once</span></span>|
|<span data-ttu-id="1070b-137">retryCount</span><span class="sxs-lookup"><span data-stu-id="1070b-137">retryCount</span></span>|<span data-ttu-id="1070b-138">Int32</span><span class="sxs-lookup"><span data-stu-id="1070b-138">Int32</span></span>|<span data-ttu-id="1070b-139">Número de vezes que o script deve ser repetido se falhar</span><span class="sxs-lookup"><span data-stu-id="1070b-139">Number of times for the script to be retried if it fails</span></span>|
|<span data-ttu-id="1070b-140">blockExecutionNotifications</span><span class="sxs-lookup"><span data-stu-id="1070b-140">blockExecutionNotifications</span></span>|<span data-ttu-id="1070b-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="1070b-141">Boolean</span></span>|<span data-ttu-id="1070b-142">Não notifica o usuário de que um script está sendo executado</span><span class="sxs-lookup"><span data-stu-id="1070b-142">Does not notify the user a script is being executed</span></span>|
|<span data-ttu-id="1070b-143">id</span><span class="sxs-lookup"><span data-stu-id="1070b-143">id</span></span>|<span data-ttu-id="1070b-144">String</span><span class="sxs-lookup"><span data-stu-id="1070b-144">String</span></span>|<span data-ttu-id="1070b-145">Identificador exclusivo do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1070b-145">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="1070b-146">displayName</span><span class="sxs-lookup"><span data-stu-id="1070b-146">displayName</span></span>|<span data-ttu-id="1070b-147">String</span><span class="sxs-lookup"><span data-stu-id="1070b-147">String</span></span>|<span data-ttu-id="1070b-148">Nome do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1070b-148">Name of the device management script.</span></span>|
|<span data-ttu-id="1070b-149">description</span><span class="sxs-lookup"><span data-stu-id="1070b-149">description</span></span>|<span data-ttu-id="1070b-150">String</span><span class="sxs-lookup"><span data-stu-id="1070b-150">String</span></span>|<span data-ttu-id="1070b-151">Descrição opcional para o script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1070b-151">Optional description for the device management script.</span></span>|
|<span data-ttu-id="1070b-152">scriptContent</span><span class="sxs-lookup"><span data-stu-id="1070b-152">scriptContent</span></span>|<span data-ttu-id="1070b-153">Binária</span><span class="sxs-lookup"><span data-stu-id="1070b-153">Binary</span></span>|<span data-ttu-id="1070b-154">O conteúdo de script.</span><span class="sxs-lookup"><span data-stu-id="1070b-154">The script content.</span></span>|
|<span data-ttu-id="1070b-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1070b-155">createdDateTime</span></span>|<span data-ttu-id="1070b-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1070b-156">DateTimeOffset</span></span>|<span data-ttu-id="1070b-157">A data e a hora em que o script de gerenciamento de dispositivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="1070b-157">The date and time the device management script was created.</span></span> <span data-ttu-id="1070b-158">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1070b-158">This property is read-only.</span></span>|
|<span data-ttu-id="1070b-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1070b-159">lastModifiedDateTime</span></span>|<span data-ttu-id="1070b-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1070b-160">DateTimeOffset</span></span>|<span data-ttu-id="1070b-161">A data e a hora em que o script de gerenciamento de dispositivo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="1070b-161">The date and time the device management script was last modified.</span></span> <span data-ttu-id="1070b-162">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1070b-162">This property is read-only.</span></span>|
|<span data-ttu-id="1070b-163">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="1070b-163">runAsAccount</span></span>|[<span data-ttu-id="1070b-164">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="1070b-164">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="1070b-165">Indica o tipo de contexto de execução.</span><span class="sxs-lookup"><span data-stu-id="1070b-165">Indicates the type of execution context.</span></span> <span data-ttu-id="1070b-166">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="1070b-166">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="1070b-167">fileName</span><span class="sxs-lookup"><span data-stu-id="1070b-167">fileName</span></span>|<span data-ttu-id="1070b-168">String</span><span class="sxs-lookup"><span data-stu-id="1070b-168">String</span></span>|<span data-ttu-id="1070b-169">Nome do arquivo de script.</span><span class="sxs-lookup"><span data-stu-id="1070b-169">Script file name.</span></span>|
|<span data-ttu-id="1070b-170">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1070b-170">roleScopeTagIds</span></span>|<span data-ttu-id="1070b-171">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1070b-171">String collection</span></span>|<span data-ttu-id="1070b-172">Lista de IDs de marca de escopo para esta instância de PowerShellScript.</span><span class="sxs-lookup"><span data-stu-id="1070b-172">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|



## <a name="response"></a><span data-ttu-id="1070b-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="1070b-173">Response</span></span>
<span data-ttu-id="1070b-174">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceShellScript](../resources/intune-devices-deviceshellscript.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1070b-174">If successful, this method returns a `201 Created` response code and a [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1070b-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1070b-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="1070b-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1070b-176">Request</span></span>
<span data-ttu-id="1070b-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1070b-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1070b-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="1070b-178">Response</span></span>
<span data-ttu-id="1070b-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1070b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




