---
title: Criar deviceShellScript
description: Criar um novo objeto deviceShellScript.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 64a6cece52e76e7ca5ae5f376913901a8a185e42
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42814334"
---
# <a name="create-deviceshellscript"></a><span data-ttu-id="cfbe2-103">Criar deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="cfbe2-103">Create deviceShellScript</span></span>

> <span data-ttu-id="cfbe2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cfbe2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cfbe2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cfbe2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfbe2-106">Criar um novo objeto [deviceShellScript](../resources/intune-devices-deviceshellscript.md) .</span><span class="sxs-lookup"><span data-stu-id="cfbe2-106">Create a new [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cfbe2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cfbe2-107">Prerequisites</span></span>
<span data-ttu-id="cfbe2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfbe2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfbe2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cfbe2-110">Permission type</span></span>|<span data-ttu-id="cfbe2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cfbe2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cfbe2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cfbe2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cfbe2-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfbe2-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cfbe2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cfbe2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cfbe2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cfbe2-115">Not supported.</span></span>|
|<span data-ttu-id="cfbe2-116">Application</span><span class="sxs-lookup"><span data-stu-id="cfbe2-116">Application</span></span>|<span data-ttu-id="cfbe2-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfbe2-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cfbe2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cfbe2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceShellScripts
```

## <a name="request-headers"></a><span data-ttu-id="cfbe2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cfbe2-119">Request headers</span></span>
|<span data-ttu-id="cfbe2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cfbe2-120">Header</span></span>|<span data-ttu-id="cfbe2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="cfbe2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cfbe2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cfbe2-122">Authorization</span></span>|<span data-ttu-id="cfbe2-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cfbe2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cfbe2-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cfbe2-124">Accept</span></span>|<span data-ttu-id="cfbe2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cfbe2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cfbe2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cfbe2-126">Request body</span></span>
<span data-ttu-id="cfbe2-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceShellScript.</span><span class="sxs-lookup"><span data-stu-id="cfbe2-127">In the request body, supply a JSON representation for the deviceShellScript object.</span></span>

<span data-ttu-id="cfbe2-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceShellScript.</span><span class="sxs-lookup"><span data-stu-id="cfbe2-128">The following table shows the properties that are required when you create the deviceShellScript.</span></span>

|<span data-ttu-id="cfbe2-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cfbe2-129">Property</span></span>|<span data-ttu-id="cfbe2-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="cfbe2-130">Type</span></span>|<span data-ttu-id="cfbe2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfbe2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfbe2-132">id</span><span class="sxs-lookup"><span data-stu-id="cfbe2-132">id</span></span>|<span data-ttu-id="cfbe2-133">String</span><span class="sxs-lookup"><span data-stu-id="cfbe2-133">String</span></span>|<span data-ttu-id="cfbe2-134">Identificador exclusivo do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cfbe2-134">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="cfbe2-135">displayName</span><span class="sxs-lookup"><span data-stu-id="cfbe2-135">displayName</span></span>|<span data-ttu-id="cfbe2-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cfbe2-136">String</span></span>|<span data-ttu-id="cfbe2-137">Nome do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cfbe2-137">Name of the device management script.</span></span>|
|<span data-ttu-id="cfbe2-138">description</span><span class="sxs-lookup"><span data-stu-id="cfbe2-138">description</span></span>|<span data-ttu-id="cfbe2-139">String</span><span class="sxs-lookup"><span data-stu-id="cfbe2-139">String</span></span>|<span data-ttu-id="cfbe2-140">Descrição opcional para o script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cfbe2-140">Optional description for the device management script.</span></span>|
|<span data-ttu-id="cfbe2-141">scriptContent</span><span class="sxs-lookup"><span data-stu-id="cfbe2-141">scriptContent</span></span>|<span data-ttu-id="cfbe2-142">Binária</span><span class="sxs-lookup"><span data-stu-id="cfbe2-142">Binary</span></span>|<span data-ttu-id="cfbe2-143">O conteúdo de script.</span><span class="sxs-lookup"><span data-stu-id="cfbe2-143">The script content.</span></span>|
|<span data-ttu-id="cfbe2-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cfbe2-144">createdDateTime</span></span>|<span data-ttu-id="cfbe2-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfbe2-145">DateTimeOffset</span></span>|<span data-ttu-id="cfbe2-146">A data e a hora em que o script de gerenciamento de dispositivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="cfbe2-146">The date and time the device management script was created.</span></span> <span data-ttu-id="cfbe2-147">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cfbe2-147">This property is read-only.</span></span>|
|<span data-ttu-id="cfbe2-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cfbe2-148">lastModifiedDateTime</span></span>|<span data-ttu-id="cfbe2-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfbe2-149">DateTimeOffset</span></span>|<span data-ttu-id="cfbe2-150">A data e a hora em que o script de gerenciamento de dispositivo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="cfbe2-150">The date and time the device management script was last modified.</span></span> <span data-ttu-id="cfbe2-151">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cfbe2-151">This property is read-only.</span></span>|
|<span data-ttu-id="cfbe2-152">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="cfbe2-152">runAsAccount</span></span>|[<span data-ttu-id="cfbe2-153">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="cfbe2-153">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="cfbe2-154">Indica o tipo de contexto de execução.</span><span class="sxs-lookup"><span data-stu-id="cfbe2-154">Indicates the type of execution context.</span></span> <span data-ttu-id="cfbe2-155">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="cfbe2-155">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="cfbe2-156">fileName</span><span class="sxs-lookup"><span data-stu-id="cfbe2-156">fileName</span></span>|<span data-ttu-id="cfbe2-157">String</span><span class="sxs-lookup"><span data-stu-id="cfbe2-157">String</span></span>|<span data-ttu-id="cfbe2-158">Nome do arquivo de script.</span><span class="sxs-lookup"><span data-stu-id="cfbe2-158">Script file name.</span></span>|
|<span data-ttu-id="cfbe2-159">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cfbe2-159">roleScopeTagIds</span></span>|<span data-ttu-id="cfbe2-160">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="cfbe2-160">String collection</span></span>|<span data-ttu-id="cfbe2-161">Lista de IDs de marca de escopo para esta instância de PowerShellScript.</span><span class="sxs-lookup"><span data-stu-id="cfbe2-161">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|



## <a name="response"></a><span data-ttu-id="cfbe2-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfbe2-162">Response</span></span>
<span data-ttu-id="cfbe2-163">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceShellScript](../resources/intune-devices-deviceshellscript.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cfbe2-163">If successful, this method returns a `201 Created` response code and a [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfbe2-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cfbe2-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="cfbe2-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cfbe2-165">Request</span></span>
<span data-ttu-id="cfbe2-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cfbe2-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceShellScripts
Content-type: application/json
Content-length: 305

{
  "@odata.type": "#microsoft.graph.deviceShellScript",
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

### <a name="response"></a><span data-ttu-id="cfbe2-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfbe2-167">Response</span></span>
<span data-ttu-id="cfbe2-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cfbe2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 477

{
  "@odata.type": "#microsoft.graph.deviceShellScript",
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




