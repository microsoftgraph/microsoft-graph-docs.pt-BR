---
title: Criar deviceShellScript
description: Crie um novo objeto deviceShellScript.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7941779b023bc81dc1a1db9e8a89158822ad9bbd
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150266"
---
# <a name="create-deviceshellscript"></a><span data-ttu-id="82ddf-103">Criar deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="82ddf-103">Create deviceShellScript</span></span>

<span data-ttu-id="82ddf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82ddf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="82ddf-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="82ddf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82ddf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="82ddf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82ddf-107">Crie um novo [objeto deviceShellScript.](../resources/intune-devices-deviceshellscript.md)</span><span class="sxs-lookup"><span data-stu-id="82ddf-107">Create a new [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82ddf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="82ddf-108">Prerequisites</span></span>
<span data-ttu-id="82ddf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82ddf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82ddf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="82ddf-111">Permission type</span></span>|<span data-ttu-id="82ddf-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="82ddf-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82ddf-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="82ddf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="82ddf-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82ddf-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="82ddf-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="82ddf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82ddf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="82ddf-116">Not supported.</span></span>|
|<span data-ttu-id="82ddf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="82ddf-117">Application</span></span>|<span data-ttu-id="82ddf-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82ddf-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="82ddf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="82ddf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceShellScripts
```

## <a name="request-headers"></a><span data-ttu-id="82ddf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="82ddf-120">Request headers</span></span>
|<span data-ttu-id="82ddf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="82ddf-121">Header</span></span>|<span data-ttu-id="82ddf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="82ddf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82ddf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="82ddf-123">Authorization</span></span>|<span data-ttu-id="82ddf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="82ddf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82ddf-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="82ddf-125">Accept</span></span>|<span data-ttu-id="82ddf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="82ddf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82ddf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="82ddf-127">Request body</span></span>
<span data-ttu-id="82ddf-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceShellScript.</span><span class="sxs-lookup"><span data-stu-id="82ddf-128">In the request body, supply a JSON representation for the deviceShellScript object.</span></span>

<span data-ttu-id="82ddf-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o deviceShellScript.</span><span class="sxs-lookup"><span data-stu-id="82ddf-129">The following table shows the properties that are required when you create the deviceShellScript.</span></span>

|<span data-ttu-id="82ddf-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="82ddf-130">Property</span></span>|<span data-ttu-id="82ddf-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="82ddf-131">Type</span></span>|<span data-ttu-id="82ddf-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="82ddf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82ddf-133">executionFrequency</span><span class="sxs-lookup"><span data-stu-id="82ddf-133">executionFrequency</span></span>|<span data-ttu-id="82ddf-134">Duration</span><span class="sxs-lookup"><span data-stu-id="82ddf-134">Duration</span></span>|<span data-ttu-id="82ddf-135">O intervalo para que o script seja executado.</span><span class="sxs-lookup"><span data-stu-id="82ddf-135">The interval for script to run.</span></span> <span data-ttu-id="82ddf-136">Se não estiver definido, o script será executado uma vez</span><span class="sxs-lookup"><span data-stu-id="82ddf-136">If not defined the script will run once</span></span>|
|<span data-ttu-id="82ddf-137">retryCount</span><span class="sxs-lookup"><span data-stu-id="82ddf-137">retryCount</span></span>|<span data-ttu-id="82ddf-138">Int32</span><span class="sxs-lookup"><span data-stu-id="82ddf-138">Int32</span></span>|<span data-ttu-id="82ddf-139">Número de vezes em que o script será retridido se ele falhar</span><span class="sxs-lookup"><span data-stu-id="82ddf-139">Number of times for the script to be retried if it fails</span></span>|
|<span data-ttu-id="82ddf-140">blockExecutionNotifications</span><span class="sxs-lookup"><span data-stu-id="82ddf-140">blockExecutionNotifications</span></span>|<span data-ttu-id="82ddf-141">Booleano</span><span class="sxs-lookup"><span data-stu-id="82ddf-141">Boolean</span></span>|<span data-ttu-id="82ddf-142">Não notifica ao usuário que um script está sendo executado</span><span class="sxs-lookup"><span data-stu-id="82ddf-142">Does not notify the user a script is being executed</span></span>|
|<span data-ttu-id="82ddf-143">id</span><span class="sxs-lookup"><span data-stu-id="82ddf-143">id</span></span>|<span data-ttu-id="82ddf-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="82ddf-144">String</span></span>|<span data-ttu-id="82ddf-145">Identificador exclusivo do script de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="82ddf-145">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="82ddf-146">displayName</span><span class="sxs-lookup"><span data-stu-id="82ddf-146">displayName</span></span>|<span data-ttu-id="82ddf-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="82ddf-147">String</span></span>|<span data-ttu-id="82ddf-148">Nome do script de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="82ddf-148">Name of the device management script.</span></span>|
|<span data-ttu-id="82ddf-149">descrição</span><span class="sxs-lookup"><span data-stu-id="82ddf-149">description</span></span>|<span data-ttu-id="82ddf-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="82ddf-150">String</span></span>|<span data-ttu-id="82ddf-151">Descrição opcional para o script de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="82ddf-151">Optional description for the device management script.</span></span>|
|<span data-ttu-id="82ddf-152">scriptContent</span><span class="sxs-lookup"><span data-stu-id="82ddf-152">scriptContent</span></span>|<span data-ttu-id="82ddf-153">Binário</span><span class="sxs-lookup"><span data-stu-id="82ddf-153">Binary</span></span>|<span data-ttu-id="82ddf-154">O conteúdo do script.</span><span class="sxs-lookup"><span data-stu-id="82ddf-154">The script content.</span></span>|
|<span data-ttu-id="82ddf-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="82ddf-155">createdDateTime</span></span>|<span data-ttu-id="82ddf-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82ddf-156">DateTimeOffset</span></span>|<span data-ttu-id="82ddf-157">A data e a hora em que o script de gerenciamento de dispositivos foi criado.</span><span class="sxs-lookup"><span data-stu-id="82ddf-157">The date and time the device management script was created.</span></span> <span data-ttu-id="82ddf-158">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="82ddf-158">This property is read-only.</span></span>|
|<span data-ttu-id="82ddf-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="82ddf-159">lastModifiedDateTime</span></span>|<span data-ttu-id="82ddf-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82ddf-160">DateTimeOffset</span></span>|<span data-ttu-id="82ddf-161">A data e a hora em que o script de gerenciamento de dispositivos foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="82ddf-161">The date and time the device management script was last modified.</span></span> <span data-ttu-id="82ddf-162">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="82ddf-162">This property is read-only.</span></span>|
|<span data-ttu-id="82ddf-163">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="82ddf-163">runAsAccount</span></span>|[<span data-ttu-id="82ddf-164">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="82ddf-164">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="82ddf-165">Indica o tipo de contexto de execução.</span><span class="sxs-lookup"><span data-stu-id="82ddf-165">Indicates the type of execution context.</span></span> <span data-ttu-id="82ddf-166">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="82ddf-166">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="82ddf-167">fileName</span><span class="sxs-lookup"><span data-stu-id="82ddf-167">fileName</span></span>|<span data-ttu-id="82ddf-168">String</span><span class="sxs-lookup"><span data-stu-id="82ddf-168">String</span></span>|<span data-ttu-id="82ddf-169">Nome do arquivo de script.</span><span class="sxs-lookup"><span data-stu-id="82ddf-169">Script file name.</span></span>|
|<span data-ttu-id="82ddf-170">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="82ddf-170">roleScopeTagIds</span></span>|<span data-ttu-id="82ddf-171">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="82ddf-171">String collection</span></span>|<span data-ttu-id="82ddf-172">Lista de IDs de marca de escopo para esta instância do PowerShellScript.</span><span class="sxs-lookup"><span data-stu-id="82ddf-172">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|



## <a name="response"></a><span data-ttu-id="82ddf-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="82ddf-173">Response</span></span>
<span data-ttu-id="82ddf-174">Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [deviceShellScript](../resources/intune-devices-deviceshellscript.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="82ddf-174">If successful, this method returns a `201 Created` response code and a [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82ddf-175">Exemplo</span><span class="sxs-lookup"><span data-stu-id="82ddf-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="82ddf-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="82ddf-176">Request</span></span>
<span data-ttu-id="82ddf-177">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="82ddf-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="82ddf-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="82ddf-178">Response</span></span>
<span data-ttu-id="82ddf-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="82ddf-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




