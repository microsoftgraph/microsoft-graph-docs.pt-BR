---
title: Atualizar deviceShellScript
description: Atualize as propriedades de um objeto deviceShellScript.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b340b51afda2b4d06f86456e34f36a5347fa36f3
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150224"
---
# <a name="update-deviceshellscript"></a><span data-ttu-id="130f9-103">Atualizar deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="130f9-103">Update deviceShellScript</span></span>

<span data-ttu-id="130f9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="130f9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="130f9-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="130f9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="130f9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="130f9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="130f9-107">Atualize as propriedades de um [objeto deviceShellScript.](../resources/intune-devices-deviceshellscript.md)</span><span class="sxs-lookup"><span data-stu-id="130f9-107">Update the properties of a [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="130f9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="130f9-108">Prerequisites</span></span>
<span data-ttu-id="130f9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="130f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="130f9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="130f9-111">Permission type</span></span>|<span data-ttu-id="130f9-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="130f9-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="130f9-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="130f9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="130f9-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="130f9-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="130f9-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="130f9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="130f9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="130f9-116">Not supported.</span></span>|
|<span data-ttu-id="130f9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="130f9-117">Application</span></span>|<span data-ttu-id="130f9-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="130f9-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="130f9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="130f9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceShellScripts/{deviceShellScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="130f9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="130f9-120">Request headers</span></span>
|<span data-ttu-id="130f9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="130f9-121">Header</span></span>|<span data-ttu-id="130f9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="130f9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="130f9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="130f9-123">Authorization</span></span>|<span data-ttu-id="130f9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="130f9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="130f9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="130f9-125">Accept</span></span>|<span data-ttu-id="130f9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="130f9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="130f9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="130f9-127">Request body</span></span>
<span data-ttu-id="130f9-128">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceShellScript.](../resources/intune-devices-deviceshellscript.md)</span><span class="sxs-lookup"><span data-stu-id="130f9-128">In the request body, supply a JSON representation for the [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>

<span data-ttu-id="130f9-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o deviceShellScript](../resources/intune-devices-deviceshellscript.md).</span><span class="sxs-lookup"><span data-stu-id="130f9-129">The following table shows the properties that are required when you create the [deviceShellScript](../resources/intune-devices-deviceshellscript.md).</span></span>

|<span data-ttu-id="130f9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="130f9-130">Property</span></span>|<span data-ttu-id="130f9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="130f9-131">Type</span></span>|<span data-ttu-id="130f9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="130f9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="130f9-133">executionFrequency</span><span class="sxs-lookup"><span data-stu-id="130f9-133">executionFrequency</span></span>|<span data-ttu-id="130f9-134">Duration</span><span class="sxs-lookup"><span data-stu-id="130f9-134">Duration</span></span>|<span data-ttu-id="130f9-135">O intervalo para que o script seja executado.</span><span class="sxs-lookup"><span data-stu-id="130f9-135">The interval for script to run.</span></span> <span data-ttu-id="130f9-136">Se não estiver definido, o script será executado uma vez</span><span class="sxs-lookup"><span data-stu-id="130f9-136">If not defined the script will run once</span></span>|
|<span data-ttu-id="130f9-137">retryCount</span><span class="sxs-lookup"><span data-stu-id="130f9-137">retryCount</span></span>|<span data-ttu-id="130f9-138">Int32</span><span class="sxs-lookup"><span data-stu-id="130f9-138">Int32</span></span>|<span data-ttu-id="130f9-139">Número de vezes em que o script será retridido se ele falhar</span><span class="sxs-lookup"><span data-stu-id="130f9-139">Number of times for the script to be retried if it fails</span></span>|
|<span data-ttu-id="130f9-140">blockExecutionNotifications</span><span class="sxs-lookup"><span data-stu-id="130f9-140">blockExecutionNotifications</span></span>|<span data-ttu-id="130f9-141">Booleano</span><span class="sxs-lookup"><span data-stu-id="130f9-141">Boolean</span></span>|<span data-ttu-id="130f9-142">Não notifica ao usuário que um script está sendo executado</span><span class="sxs-lookup"><span data-stu-id="130f9-142">Does not notify the user a script is being executed</span></span>|
|<span data-ttu-id="130f9-143">id</span><span class="sxs-lookup"><span data-stu-id="130f9-143">id</span></span>|<span data-ttu-id="130f9-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="130f9-144">String</span></span>|<span data-ttu-id="130f9-145">Identificador exclusivo do script de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="130f9-145">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="130f9-146">displayName</span><span class="sxs-lookup"><span data-stu-id="130f9-146">displayName</span></span>|<span data-ttu-id="130f9-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="130f9-147">String</span></span>|<span data-ttu-id="130f9-148">Nome do script de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="130f9-148">Name of the device management script.</span></span>|
|<span data-ttu-id="130f9-149">descrição</span><span class="sxs-lookup"><span data-stu-id="130f9-149">description</span></span>|<span data-ttu-id="130f9-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="130f9-150">String</span></span>|<span data-ttu-id="130f9-151">Descrição opcional para o script de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="130f9-151">Optional description for the device management script.</span></span>|
|<span data-ttu-id="130f9-152">scriptContent</span><span class="sxs-lookup"><span data-stu-id="130f9-152">scriptContent</span></span>|<span data-ttu-id="130f9-153">Binário</span><span class="sxs-lookup"><span data-stu-id="130f9-153">Binary</span></span>|<span data-ttu-id="130f9-154">O conteúdo do script.</span><span class="sxs-lookup"><span data-stu-id="130f9-154">The script content.</span></span>|
|<span data-ttu-id="130f9-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="130f9-155">createdDateTime</span></span>|<span data-ttu-id="130f9-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="130f9-156">DateTimeOffset</span></span>|<span data-ttu-id="130f9-157">A data e a hora em que o script de gerenciamento de dispositivos foi criado.</span><span class="sxs-lookup"><span data-stu-id="130f9-157">The date and time the device management script was created.</span></span> <span data-ttu-id="130f9-158">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="130f9-158">This property is read-only.</span></span>|
|<span data-ttu-id="130f9-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="130f9-159">lastModifiedDateTime</span></span>|<span data-ttu-id="130f9-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="130f9-160">DateTimeOffset</span></span>|<span data-ttu-id="130f9-161">A data e a hora em que o script de gerenciamento de dispositivos foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="130f9-161">The date and time the device management script was last modified.</span></span> <span data-ttu-id="130f9-162">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="130f9-162">This property is read-only.</span></span>|
|<span data-ttu-id="130f9-163">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="130f9-163">runAsAccount</span></span>|[<span data-ttu-id="130f9-164">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="130f9-164">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="130f9-165">Indica o tipo de contexto de execução.</span><span class="sxs-lookup"><span data-stu-id="130f9-165">Indicates the type of execution context.</span></span> <span data-ttu-id="130f9-166">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="130f9-166">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="130f9-167">fileName</span><span class="sxs-lookup"><span data-stu-id="130f9-167">fileName</span></span>|<span data-ttu-id="130f9-168">String</span><span class="sxs-lookup"><span data-stu-id="130f9-168">String</span></span>|<span data-ttu-id="130f9-169">Nome do arquivo de script.</span><span class="sxs-lookup"><span data-stu-id="130f9-169">Script file name.</span></span>|
|<span data-ttu-id="130f9-170">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="130f9-170">roleScopeTagIds</span></span>|<span data-ttu-id="130f9-171">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="130f9-171">String collection</span></span>|<span data-ttu-id="130f9-172">Lista de IDs de marca de escopo para esta instância do PowerShellScript.</span><span class="sxs-lookup"><span data-stu-id="130f9-172">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|



## <a name="response"></a><span data-ttu-id="130f9-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="130f9-173">Response</span></span>
<span data-ttu-id="130f9-174">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceShellScript](../resources/intune-devices-deviceshellscript.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="130f9-174">If successful, this method returns a `200 OK` response code and an updated [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="130f9-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="130f9-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="130f9-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="130f9-176">Request</span></span>
<span data-ttu-id="130f9-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="130f9-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="130f9-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="130f9-178">Response</span></span>
<span data-ttu-id="130f9-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="130f9-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




