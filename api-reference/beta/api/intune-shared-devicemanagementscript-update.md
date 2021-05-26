---
title: Atualizar deviceManagementScript
description: Atualize as propriedades de um objeto deviceManagementScript.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f68184a74714ee8ce74af3f25019123fe69d0891
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52662932"
---
# <a name="update-devicemanagementscript"></a><span data-ttu-id="1a30c-103">Atualizar deviceManagementScript</span><span class="sxs-lookup"><span data-stu-id="1a30c-103">Update deviceManagementScript</span></span>

<span data-ttu-id="1a30c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a30c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a30c-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1a30c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a30c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1a30c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a30c-107">Atualize as propriedades de um [objeto deviceManagementScript.](../resources/intune-shared-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="1a30c-107">Update the properties of a [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a30c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1a30c-108">Prerequisites</span></span>
<span data-ttu-id="1a30c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1a30c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a30c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1a30c-111">Permission type</span></span>|<span data-ttu-id="1a30c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1a30c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a30c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1a30c-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="1a30c-114">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="1a30c-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="1a30c-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a30c-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="1a30c-116">&nbsp;&nbsp; **Conjunto de Políticas**</span><span class="sxs-lookup"><span data-stu-id="1a30c-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="1a30c-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a30c-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1a30c-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1a30c-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a30c-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a30c-119">Not supported.</span></span>|
|<span data-ttu-id="1a30c-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1a30c-120">Application</span></span>||
| <span data-ttu-id="1a30c-121">&nbsp;&nbsp; **Gerenciamento de dispositivos**</span><span class="sxs-lookup"><span data-stu-id="1a30c-121">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="1a30c-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a30c-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="1a30c-123">&nbsp;&nbsp; **Conjunto de Políticas**</span><span class="sxs-lookup"><span data-stu-id="1a30c-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="1a30c-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a30c-124">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a30c-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1a30c-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="1a30c-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1a30c-126">Request headers</span></span>
|<span data-ttu-id="1a30c-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1a30c-127">Header</span></span>|<span data-ttu-id="1a30c-128">Valor</span><span class="sxs-lookup"><span data-stu-id="1a30c-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a30c-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="1a30c-129">Authorization</span></span>|<span data-ttu-id="1a30c-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a30c-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a30c-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1a30c-131">Accept</span></span>|<span data-ttu-id="1a30c-132">application/json</span><span class="sxs-lookup"><span data-stu-id="1a30c-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a30c-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1a30c-133">Request body</span></span>
<span data-ttu-id="1a30c-134">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceManagementScript.](../resources/intune-shared-devicemanagementscript.md)</span><span class="sxs-lookup"><span data-stu-id="1a30c-134">In the request body, supply a JSON representation for the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object.</span></span>

<span data-ttu-id="1a30c-135">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).</span><span class="sxs-lookup"><span data-stu-id="1a30c-135">The following table shows the properties that are required when you create the [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md).</span></span>

|<span data-ttu-id="1a30c-136">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1a30c-136">Property</span></span>|<span data-ttu-id="1a30c-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a30c-137">Type</span></span>|<span data-ttu-id="1a30c-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a30c-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a30c-139">id</span><span class="sxs-lookup"><span data-stu-id="1a30c-139">id</span></span>|<span data-ttu-id="1a30c-140">String</span><span class="sxs-lookup"><span data-stu-id="1a30c-140">String</span></span>|<span data-ttu-id="1a30c-141">Identificador exclusivo do script de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="1a30c-141">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="1a30c-142">displayName</span><span class="sxs-lookup"><span data-stu-id="1a30c-142">displayName</span></span>|<span data-ttu-id="1a30c-143">String</span><span class="sxs-lookup"><span data-stu-id="1a30c-143">String</span></span>|<span data-ttu-id="1a30c-144">Nome do script de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="1a30c-144">Name of the device management script.</span></span>|
|<span data-ttu-id="1a30c-145">descrição</span><span class="sxs-lookup"><span data-stu-id="1a30c-145">description</span></span>|<span data-ttu-id="1a30c-146">String</span><span class="sxs-lookup"><span data-stu-id="1a30c-146">String</span></span>|<span data-ttu-id="1a30c-147">Descrição opcional para o script de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="1a30c-147">Optional description for the device management script.</span></span>|
|<span data-ttu-id="1a30c-148">scriptContent</span><span class="sxs-lookup"><span data-stu-id="1a30c-148">scriptContent</span></span>|<span data-ttu-id="1a30c-149">Binário</span><span class="sxs-lookup"><span data-stu-id="1a30c-149">Binary</span></span>|<span data-ttu-id="1a30c-150">O conteúdo do script.</span><span class="sxs-lookup"><span data-stu-id="1a30c-150">The script content.</span></span>|
|<span data-ttu-id="1a30c-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1a30c-151">createdDateTime</span></span>|<span data-ttu-id="1a30c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a30c-152">DateTimeOffset</span></span>|<span data-ttu-id="1a30c-153">A data e a hora em que o script de gerenciamento de dispositivos foi criado.</span><span class="sxs-lookup"><span data-stu-id="1a30c-153">The date and time the device management script was created.</span></span> <span data-ttu-id="1a30c-154">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1a30c-154">This property is read-only.</span></span>|
|<span data-ttu-id="1a30c-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a30c-155">lastModifiedDateTime</span></span>|<span data-ttu-id="1a30c-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a30c-156">DateTimeOffset</span></span>|<span data-ttu-id="1a30c-157">A data e a hora em que o script de gerenciamento de dispositivos foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="1a30c-157">The date and time the device management script was last modified.</span></span> <span data-ttu-id="1a30c-158">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1a30c-158">This property is read-only.</span></span>|
|<span data-ttu-id="1a30c-159">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="1a30c-159">runAsAccount</span></span>|[<span data-ttu-id="1a30c-160">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="1a30c-160">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="1a30c-161">Indica o tipo de contexto de execução.</span><span class="sxs-lookup"><span data-stu-id="1a30c-161">Indicates the type of execution context.</span></span> <span data-ttu-id="1a30c-162">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="1a30c-162">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="1a30c-163">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="1a30c-163">enforceSignatureCheck</span></span>|<span data-ttu-id="1a30c-164">Booleano</span><span class="sxs-lookup"><span data-stu-id="1a30c-164">Boolean</span></span>|<span data-ttu-id="1a30c-165">Indique se a assinatura de script precisa ser verificada.</span><span class="sxs-lookup"><span data-stu-id="1a30c-165">Indicate whether the script signature needs be checked.</span></span>|
|<span data-ttu-id="1a30c-166">fileName</span><span class="sxs-lookup"><span data-stu-id="1a30c-166">fileName</span></span>|<span data-ttu-id="1a30c-167">String</span><span class="sxs-lookup"><span data-stu-id="1a30c-167">String</span></span>|<span data-ttu-id="1a30c-168">Nome do arquivo de script.</span><span class="sxs-lookup"><span data-stu-id="1a30c-168">Script file name.</span></span>|
|<span data-ttu-id="1a30c-169">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1a30c-169">roleScopeTagIds</span></span>|<span data-ttu-id="1a30c-170">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a30c-170">String collection</span></span>|<span data-ttu-id="1a30c-171">Lista de IDs de marca de escopo para esta instância do PowerShellScript.</span><span class="sxs-lookup"><span data-stu-id="1a30c-171">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|
|<span data-ttu-id="1a30c-172">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="1a30c-172">runAs32Bit</span></span>|<span data-ttu-id="1a30c-173">Booleano</span><span class="sxs-lookup"><span data-stu-id="1a30c-173">Boolean</span></span>|<span data-ttu-id="1a30c-174">Um valor que indica se o script do PowerShell deve ser executado como 32 bits</span><span class="sxs-lookup"><span data-stu-id="1a30c-174">A value indicating whether the PowerShell script should run as 32-bit</span></span>|



## <a name="response"></a><span data-ttu-id="1a30c-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a30c-175">Response</span></span>
<span data-ttu-id="1a30c-176">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1a30c-176">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScript](../resources/intune-shared-devicemanagementscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a30c-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1a30c-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a30c-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1a30c-178">Request</span></span>
<span data-ttu-id="1a30c-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1a30c-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}
Content-type: application/json
Content-length: 443

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "displayName": "Display Name value",
  "description": "Description value",
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

### <a name="response"></a><span data-ttu-id="1a30c-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a30c-180">Response</span></span>
<span data-ttu-id="1a30c-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1a30c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 615

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "id": "59ea4525-4525-59ea-2545-ea592545ea59",
  "displayName": "Display Name value",
  "description": "Description value",
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







