---
title: Atualizar deviceManagementScript
description: Atualiza as propriedades de um objeto deviceManagementScript.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5dc0554456be285f8f6306bfa52033e851164874
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33909901"
---
# <a name="update-devicemanagementscript"></a><span data-ttu-id="938ef-103">Atualizar deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="938ef-103">Update deviceManagementScript</span></span>

> <span data-ttu-id="938ef-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="938ef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="938ef-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="938ef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="938ef-106">Atualiza as propriedades de um objeto [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="938ef-106">Update the properties of a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="938ef-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="938ef-107">Prerequisites</span></span>
<span data-ttu-id="938ef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="938ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="938ef-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="938ef-110">Permission type</span></span>|<span data-ttu-id="938ef-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="938ef-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="938ef-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="938ef-112">Delegated (work or school account)</span></span>|<span data-ttu-id="938ef-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="938ef-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="938ef-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="938ef-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="938ef-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="938ef-115">Not supported.</span></span>|
|<span data-ttu-id="938ef-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="938ef-116">Application</span></span>|<span data-ttu-id="938ef-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="938ef-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="938ef-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="938ef-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="938ef-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="938ef-119">Request headers</span></span>
|<span data-ttu-id="938ef-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="938ef-120">Header</span></span>|<span data-ttu-id="938ef-121">Valor</span><span class="sxs-lookup"><span data-stu-id="938ef-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="938ef-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="938ef-122">Authorization</span></span>|<span data-ttu-id="938ef-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="938ef-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="938ef-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="938ef-124">Accept</span></span>|<span data-ttu-id="938ef-125">application/json</span><span class="sxs-lookup"><span data-stu-id="938ef-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="938ef-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="938ef-126">Request body</span></span>
<span data-ttu-id="938ef-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="938ef-127">In the request body, supply a JSON representation for the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>

<span data-ttu-id="938ef-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).</span><span class="sxs-lookup"><span data-stu-id="938ef-128">The following table shows the properties that are required when you create the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).</span></span>

|<span data-ttu-id="938ef-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="938ef-129">Property</span></span>|<span data-ttu-id="938ef-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="938ef-130">Type</span></span>|<span data-ttu-id="938ef-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="938ef-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="938ef-132">id</span><span class="sxs-lookup"><span data-stu-id="938ef-132">id</span></span>|<span data-ttu-id="938ef-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="938ef-133">String</span></span>|<span data-ttu-id="938ef-134">Identificador exclusivo do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="938ef-134">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="938ef-135">displayName</span><span class="sxs-lookup"><span data-stu-id="938ef-135">displayName</span></span>|<span data-ttu-id="938ef-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="938ef-136">String</span></span>|<span data-ttu-id="938ef-137">Nome do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="938ef-137">Name of the device management script.</span></span>|
|<span data-ttu-id="938ef-138">description</span><span class="sxs-lookup"><span data-stu-id="938ef-138">description</span></span>|<span data-ttu-id="938ef-139">String</span><span class="sxs-lookup"><span data-stu-id="938ef-139">String</span></span>|<span data-ttu-id="938ef-140">Descrição opcional para o script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="938ef-140">Optional description for the device management script.</span></span>|
|<span data-ttu-id="938ef-141">runSchedule</span><span class="sxs-lookup"><span data-stu-id="938ef-141">runSchedule</span></span>|[<span data-ttu-id="938ef-142">runSchedule</span><span class="sxs-lookup"><span data-stu-id="938ef-142">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="938ef-143">O intervalo de execução do script.</span><span class="sxs-lookup"><span data-stu-id="938ef-143">The interval for script to run.</span></span> <span data-ttu-id="938ef-144">Se não definido, o script será executado uma vez</span><span class="sxs-lookup"><span data-stu-id="938ef-144">If not defined the script will run once</span></span>|
|<span data-ttu-id="938ef-145">scriptContent</span><span class="sxs-lookup"><span data-stu-id="938ef-145">scriptContent</span></span>|<span data-ttu-id="938ef-146">Binária</span><span class="sxs-lookup"><span data-stu-id="938ef-146">Binary</span></span>|<span data-ttu-id="938ef-147">O conteúdo de script.</span><span class="sxs-lookup"><span data-stu-id="938ef-147">The script content.</span></span>|
|<span data-ttu-id="938ef-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="938ef-148">createdDateTime</span></span>|<span data-ttu-id="938ef-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="938ef-149">DateTimeOffset</span></span>|<span data-ttu-id="938ef-150">A data e a hora em que o script de gerenciamento de dispositivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="938ef-150">The date and time the device management script was created.</span></span>|
|<span data-ttu-id="938ef-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="938ef-151">lastModifiedDateTime</span></span>|<span data-ttu-id="938ef-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="938ef-152">DateTimeOffset</span></span>|<span data-ttu-id="938ef-153">A data e a hora em que o script de gerenciamento de dispositivo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="938ef-153">The date and time the device management script was last modified.</span></span>|
|<span data-ttu-id="938ef-154">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="938ef-154">runAsAccount</span></span>|[<span data-ttu-id="938ef-155">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="938ef-155">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="938ef-156">Indica o tipo de contexto de execução.</span><span class="sxs-lookup"><span data-stu-id="938ef-156">Indicates the type of execution context.</span></span> <span data-ttu-id="938ef-157">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="938ef-157">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="938ef-158">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="938ef-158">enforceSignatureCheck</span></span>|<span data-ttu-id="938ef-159">Booliano</span><span class="sxs-lookup"><span data-stu-id="938ef-159">Boolean</span></span>|<span data-ttu-id="938ef-160">Indica se a assinatura do script precisa ser verificada.</span><span class="sxs-lookup"><span data-stu-id="938ef-160">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="938ef-161">fileName</span><span class="sxs-lookup"><span data-stu-id="938ef-161">fileName</span></span>|<span data-ttu-id="938ef-162">String</span><span class="sxs-lookup"><span data-stu-id="938ef-162">String</span></span>|<span data-ttu-id="938ef-163">Nome do arquivo de script.</span><span class="sxs-lookup"><span data-stu-id="938ef-163">Script file name.</span></span>|
|<span data-ttu-id="938ef-164">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="938ef-164">roleScopeTagIds</span></span>|<span data-ttu-id="938ef-165">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="938ef-165">String collection</span></span>|<span data-ttu-id="938ef-166">Lista de IDs de marca de escopo para esta instância de PowerShellScript.</span><span class="sxs-lookup"><span data-stu-id="938ef-166">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="938ef-167">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="938ef-167">runAs32Bit</span></span>|<span data-ttu-id="938ef-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="938ef-168">Boolean</span></span>|<span data-ttu-id="938ef-169">Um valor que indica se o script do PowerShell deve ser executado como 32 bits</span><span class="sxs-lookup"><span data-stu-id="938ef-169">A value indicating whether the PowerShell script should run as 32-bit</span></span>|



## <a name="response"></a><span data-ttu-id="938ef-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="938ef-170">Response</span></span>
<span data-ttu-id="938ef-171">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="938ef-171">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="938ef-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="938ef-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="938ef-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="938ef-173">Request</span></span>
<span data-ttu-id="938ef-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="938ef-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="938ef-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="938ef-175">Response</span></span>
<span data-ttu-id="938ef-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="938ef-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




