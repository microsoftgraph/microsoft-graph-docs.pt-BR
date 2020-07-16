---
title: Criar deviceManagementScript
description: Criar um novo objeto deviceManagementScript.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 370e0663907f7c45e63b306480d876fd2acce458
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791325"
---
# <a name="create-devicemanagementscript"></a><span data-ttu-id="0c820-103">Criar deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="0c820-103">Create deviceManagementScript</span></span>

<span data-ttu-id="0c820-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c820-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0c820-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0c820-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c820-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0c820-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c820-107">Criar um novo objeto [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) .</span><span class="sxs-lookup"><span data-stu-id="0c820-107">Create a new [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c820-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0c820-108">Prerequisites</span></span>
<span data-ttu-id="0c820-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0c820-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c820-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0c820-111">Permission type</span></span>|<span data-ttu-id="0c820-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0c820-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c820-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0c820-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="0c820-114">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="0c820-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="0c820-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c820-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="0c820-116">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="0c820-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="0c820-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c820-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="0c820-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0c820-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c820-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0c820-119">Not supported.</span></span>|
|<span data-ttu-id="0c820-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0c820-120">Application</span></span>||
| <span data-ttu-id="0c820-121">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="0c820-121">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="0c820-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c820-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="0c820-123">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="0c820-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="0c820-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c820-124">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c820-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0c820-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a><span data-ttu-id="0c820-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0c820-126">Request headers</span></span>
|<span data-ttu-id="0c820-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0c820-127">Header</span></span>|<span data-ttu-id="0c820-128">Valor</span><span class="sxs-lookup"><span data-stu-id="0c820-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c820-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="0c820-129">Authorization</span></span>|<span data-ttu-id="0c820-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0c820-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c820-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0c820-131">Accept</span></span>|<span data-ttu-id="0c820-132">application/json</span><span class="sxs-lookup"><span data-stu-id="0c820-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c820-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0c820-133">Request body</span></span>
<span data-ttu-id="0c820-134">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementScript.</span><span class="sxs-lookup"><span data-stu-id="0c820-134">In the request body, supply a JSON representation for the deviceManagementScript object.</span></span>

<span data-ttu-id="0c820-135">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementScript.</span><span class="sxs-lookup"><span data-stu-id="0c820-135">The following table shows the properties that are required when you create the deviceManagementScript.</span></span>

|<span data-ttu-id="0c820-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c820-136">Property</span></span>|<span data-ttu-id="0c820-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c820-137">Type</span></span>|<span data-ttu-id="0c820-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c820-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c820-139">id</span><span class="sxs-lookup"><span data-stu-id="0c820-139">id</span></span>|<span data-ttu-id="0c820-140">String</span><span class="sxs-lookup"><span data-stu-id="0c820-140">String</span></span>|<span data-ttu-id="0c820-141">Identificador exclusivo do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0c820-141">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="0c820-142">displayName</span><span class="sxs-lookup"><span data-stu-id="0c820-142">displayName</span></span>|<span data-ttu-id="0c820-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c820-143">String</span></span>|<span data-ttu-id="0c820-144">Nome do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0c820-144">Name of the device management script.</span></span>|
|<span data-ttu-id="0c820-145">description</span><span class="sxs-lookup"><span data-stu-id="0c820-145">description</span></span>|<span data-ttu-id="0c820-146">String</span><span class="sxs-lookup"><span data-stu-id="0c820-146">String</span></span>|<span data-ttu-id="0c820-147">Descrição opcional para o script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0c820-147">Optional description for the device management script.</span></span>|
|<span data-ttu-id="0c820-148">runSchedule</span><span class="sxs-lookup"><span data-stu-id="0c820-148">runSchedule</span></span>|<span data-ttu-id="0c820-149">runSchedule</span><span class="sxs-lookup"><span data-stu-id="0c820-149">runSchedule</span></span>|<span data-ttu-id="0c820-150">O intervalo de execução do script.</span><span class="sxs-lookup"><span data-stu-id="0c820-150">The interval for script to run.</span></span> <span data-ttu-id="0c820-151">Se não definido, o script será executado uma vez</span><span class="sxs-lookup"><span data-stu-id="0c820-151">If not defined the script will run once</span></span>|
|<span data-ttu-id="0c820-152">scriptContent</span><span class="sxs-lookup"><span data-stu-id="0c820-152">scriptContent</span></span>|<span data-ttu-id="0c820-153">Binária</span><span class="sxs-lookup"><span data-stu-id="0c820-153">Binary</span></span>|<span data-ttu-id="0c820-154">O conteúdo de script.</span><span class="sxs-lookup"><span data-stu-id="0c820-154">The script content.</span></span>|
|<span data-ttu-id="0c820-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0c820-155">createdDateTime</span></span>|<span data-ttu-id="0c820-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c820-156">DateTimeOffset</span></span>|<span data-ttu-id="0c820-157">A data e a hora em que o script de gerenciamento de dispositivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="0c820-157">The date and time the device management script was created.</span></span> <span data-ttu-id="0c820-158">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0c820-158">This property is read-only.</span></span>|
|<span data-ttu-id="0c820-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0c820-159">lastModifiedDateTime</span></span>|<span data-ttu-id="0c820-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c820-160">DateTimeOffset</span></span>|<span data-ttu-id="0c820-161">A data e a hora em que o script de gerenciamento de dispositivo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="0c820-161">The date and time the device management script was last modified.</span></span> <span data-ttu-id="0c820-162">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0c820-162">This property is read-only.</span></span>|
|<span data-ttu-id="0c820-163">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="0c820-163">runAsAccount</span></span>|[<span data-ttu-id="0c820-164">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="0c820-164">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="0c820-165">Indica o tipo de contexto de execução.</span><span class="sxs-lookup"><span data-stu-id="0c820-165">Indicates the type of execution context.</span></span> <span data-ttu-id="0c820-166">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="0c820-166">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="0c820-167">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="0c820-167">enforceSignatureCheck</span></span>|<span data-ttu-id="0c820-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c820-168">Boolean</span></span>|<span data-ttu-id="0c820-169">Indica se a assinatura do script precisa ser verificada.</span><span class="sxs-lookup"><span data-stu-id="0c820-169">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="0c820-170">fileName</span><span class="sxs-lookup"><span data-stu-id="0c820-170">fileName</span></span>|<span data-ttu-id="0c820-171">String</span><span class="sxs-lookup"><span data-stu-id="0c820-171">String</span></span>|<span data-ttu-id="0c820-172">Nome do arquivo de script.</span><span class="sxs-lookup"><span data-stu-id="0c820-172">Script file name.</span></span>|
|<span data-ttu-id="0c820-173">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0c820-173">roleScopeTagIds</span></span>|<span data-ttu-id="0c820-174">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c820-174">String collection</span></span>|<span data-ttu-id="0c820-175">Lista de IDs de marca de escopo para esta instância de PowerShellScript.</span><span class="sxs-lookup"><span data-stu-id="0c820-175">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="0c820-176">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="0c820-176">runAs32Bit</span></span>|<span data-ttu-id="0c820-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c820-177">Boolean</span></span>|<span data-ttu-id="0c820-178">Um valor que indica se o script do PowerShell deve ser executado como 32 bits</span><span class="sxs-lookup"><span data-stu-id="0c820-178">A value indicating whether the PowerShell script should run as 32-bit</span></span>|



## <a name="response"></a><span data-ttu-id="0c820-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c820-179">Response</span></span>
<span data-ttu-id="0c820-180">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0c820-180">If successful, this method returns a `201 Created` response code and a [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c820-181">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c820-181">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c820-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0c820-182">Request</span></span>
<span data-ttu-id="0c820-183">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0c820-183">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0c820-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="0c820-184">Response</span></span>
<span data-ttu-id="0c820-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0c820-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






