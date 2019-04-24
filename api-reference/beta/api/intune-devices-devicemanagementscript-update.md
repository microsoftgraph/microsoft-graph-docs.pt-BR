---
title: Atualizar deviceManagementScript
description: Atualiza as propriedades de um objeto deviceManagementScript.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aac5c1592dd9e18f791f93829192dc9bfe2125f3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465808"
---
# <a name="update-devicemanagementscript"></a><span data-ttu-id="e8158-103">Atualizar deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="e8158-103">Update deviceManagementScript</span></span>

> <span data-ttu-id="e8158-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e8158-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8158-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e8158-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8158-106">Atualiza as propriedades de um objeto [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="e8158-106">Update the properties of a [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8158-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e8158-107">Prerequisites</span></span>
<span data-ttu-id="e8158-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8158-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8158-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8158-110">Permission type</span></span>|<span data-ttu-id="e8158-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e8158-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8158-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8158-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e8158-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8158-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e8158-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8158-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8158-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8158-115">Not supported.</span></span>|
|<span data-ttu-id="e8158-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8158-116">Application</span></span>|<span data-ttu-id="e8158-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8158-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8158-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8158-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="e8158-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8158-119">Request headers</span></span>
|<span data-ttu-id="e8158-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e8158-120">Header</span></span>|<span data-ttu-id="e8158-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e8158-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8158-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8158-122">Authorization</span></span>|<span data-ttu-id="e8158-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8158-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8158-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e8158-124">Accept</span></span>|<span data-ttu-id="e8158-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e8158-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8158-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8158-126">Request body</span></span>
<span data-ttu-id="e8158-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="e8158-127">In the request body, supply a JSON representation for the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object.</span></span>

<span data-ttu-id="e8158-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).</span><span class="sxs-lookup"><span data-stu-id="e8158-128">The following table shows the properties that are required when you create the [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md).</span></span>

|<span data-ttu-id="e8158-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e8158-129">Property</span></span>|<span data-ttu-id="e8158-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8158-130">Type</span></span>|<span data-ttu-id="e8158-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8158-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8158-132">id</span><span class="sxs-lookup"><span data-stu-id="e8158-132">id</span></span>|<span data-ttu-id="e8158-133">String</span><span class="sxs-lookup"><span data-stu-id="e8158-133">String</span></span>|<span data-ttu-id="e8158-134">Identificador exclusivo do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e8158-134">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="e8158-135">displayName</span><span class="sxs-lookup"><span data-stu-id="e8158-135">displayName</span></span>|<span data-ttu-id="e8158-136">String</span><span class="sxs-lookup"><span data-stu-id="e8158-136">String</span></span>|<span data-ttu-id="e8158-137">Nome do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e8158-137">Name of the device management script.</span></span>|
|<span data-ttu-id="e8158-138">description</span><span class="sxs-lookup"><span data-stu-id="e8158-138">description</span></span>|<span data-ttu-id="e8158-139">String</span><span class="sxs-lookup"><span data-stu-id="e8158-139">String</span></span>|<span data-ttu-id="e8158-140">Descrição opcional para o script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e8158-140">Optional description for the device management script.</span></span>|
|<span data-ttu-id="e8158-141">runSchedule</span><span class="sxs-lookup"><span data-stu-id="e8158-141">runSchedule</span></span>|[<span data-ttu-id="e8158-142">runSchedule</span><span class="sxs-lookup"><span data-stu-id="e8158-142">runSchedule</span></span>](../resources/intune-devices-runschedule.md)|<span data-ttu-id="e8158-143">O intervalo de execução do script.</span><span class="sxs-lookup"><span data-stu-id="e8158-143">The interval for script to run.</span></span> <span data-ttu-id="e8158-144">Se não definido, o script será executado uma vez</span><span class="sxs-lookup"><span data-stu-id="e8158-144">If not defined the script will run once</span></span>|
|<span data-ttu-id="e8158-145">scriptContent</span><span class="sxs-lookup"><span data-stu-id="e8158-145">scriptContent</span></span>|<span data-ttu-id="e8158-146">Binary</span><span class="sxs-lookup"><span data-stu-id="e8158-146">Binary</span></span>|<span data-ttu-id="e8158-147">O conteúdo de script.</span><span class="sxs-lookup"><span data-stu-id="e8158-147">The script content.</span></span>|
|<span data-ttu-id="e8158-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e8158-148">createdDateTime</span></span>|<span data-ttu-id="e8158-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8158-149">DateTimeOffset</span></span>|<span data-ttu-id="e8158-150">A data e a hora em que o script de gerenciamento de dispositivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="e8158-150">The date and time the device management script was created.</span></span>|
|<span data-ttu-id="e8158-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e8158-151">lastModifiedDateTime</span></span>|<span data-ttu-id="e8158-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8158-152">DateTimeOffset</span></span>|<span data-ttu-id="e8158-153">A data e a hora em que o script de gerenciamento de dispositivo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="e8158-153">The date and time the device management script was last modified.</span></span>|
|<span data-ttu-id="e8158-154">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="e8158-154">runAsAccount</span></span>|[<span data-ttu-id="e8158-155">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="e8158-155">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="e8158-156">Indica o tipo de contexto de execução.</span><span class="sxs-lookup"><span data-stu-id="e8158-156">Indicates the type of execution context.</span></span> <span data-ttu-id="e8158-157">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="e8158-157">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="e8158-158">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="e8158-158">enforceSignatureCheck</span></span>|<span data-ttu-id="e8158-159">Booliano</span><span class="sxs-lookup"><span data-stu-id="e8158-159">Boolean</span></span>|<span data-ttu-id="e8158-160">Indica se a assinatura do script precisa ser verificada.</span><span class="sxs-lookup"><span data-stu-id="e8158-160">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="e8158-161">fileName</span><span class="sxs-lookup"><span data-stu-id="e8158-161">fileName</span></span>|<span data-ttu-id="e8158-162">String</span><span class="sxs-lookup"><span data-stu-id="e8158-162">String</span></span>|<span data-ttu-id="e8158-163">Nome do arquivo de script.</span><span class="sxs-lookup"><span data-stu-id="e8158-163">Script file name.</span></span>|
|<span data-ttu-id="e8158-164">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e8158-164">roleScopeTagIds</span></span>|<span data-ttu-id="e8158-165">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e8158-165">String collection</span></span>|<span data-ttu-id="e8158-166">Lista de IDs de marca de escopo para esta instância de PowerShellScript.</span><span class="sxs-lookup"><span data-stu-id="e8158-166">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="e8158-167">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="e8158-167">runAs32Bit</span></span>|<span data-ttu-id="e8158-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="e8158-168">Boolean</span></span>|<span data-ttu-id="e8158-169">Um valor que indica se o script do PowerShell deve ser executado como 32 bits</span><span class="sxs-lookup"><span data-stu-id="e8158-169">A value indicating whether the PowerShell script should run as 32-bit</span></span>|



## <a name="response"></a><span data-ttu-id="e8158-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8158-170">Response</span></span>
<span data-ttu-id="e8158-171">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8158-171">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8158-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8158-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8158-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8158-173">Request</span></span>
<span data-ttu-id="e8158-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8158-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e8158-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8158-175">Response</span></span>
<span data-ttu-id="e8158-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8158-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





