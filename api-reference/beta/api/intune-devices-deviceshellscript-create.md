---
title: Criar deviceShellScript
description: Criar um novo objeto deviceShellScript.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 37e2777d766335d0d8ddade5eba1ea889b535113
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944859"
---
# <a name="create-deviceshellscript"></a><span data-ttu-id="f3f8e-103">Criar deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="f3f8e-103">Create deviceShellScript</span></span>

> <span data-ttu-id="f3f8e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f3f8e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3f8e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f3f8e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3f8e-106">Criar um novo objeto [deviceShellScript](../resources/intune-devices-deviceshellscript.md) .</span><span class="sxs-lookup"><span data-stu-id="f3f8e-106">Create a new [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3f8e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f3f8e-107">Prerequisites</span></span>
<span data-ttu-id="f3f8e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3f8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3f8e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f3f8e-110">Permission type</span></span>|<span data-ttu-id="f3f8e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f3f8e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3f8e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f3f8e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f3f8e-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3f8e-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f3f8e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f3f8e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3f8e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3f8e-115">Not supported.</span></span>|
|<span data-ttu-id="f3f8e-116">Application</span><span class="sxs-lookup"><span data-stu-id="f3f8e-116">Application</span></span>|<span data-ttu-id="f3f8e-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3f8e-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3f8e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f3f8e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceShellScripts
```

## <a name="request-headers"></a><span data-ttu-id="f3f8e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f3f8e-119">Request headers</span></span>
|<span data-ttu-id="f3f8e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f3f8e-120">Header</span></span>|<span data-ttu-id="f3f8e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f3f8e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3f8e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f3f8e-122">Authorization</span></span>|<span data-ttu-id="f3f8e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f3f8e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3f8e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f3f8e-124">Accept</span></span>|<span data-ttu-id="f3f8e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f3f8e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3f8e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f3f8e-126">Request body</span></span>
<span data-ttu-id="f3f8e-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceShellScript.</span><span class="sxs-lookup"><span data-stu-id="f3f8e-127">In the request body, supply a JSON representation for the deviceShellScript object.</span></span>

<span data-ttu-id="f3f8e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceShellScript.</span><span class="sxs-lookup"><span data-stu-id="f3f8e-128">The following table shows the properties that are required when you create the deviceShellScript.</span></span>

|<span data-ttu-id="f3f8e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f3f8e-129">Property</span></span>|<span data-ttu-id="f3f8e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3f8e-130">Type</span></span>|<span data-ttu-id="f3f8e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3f8e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3f8e-132">id</span><span class="sxs-lookup"><span data-stu-id="f3f8e-132">id</span></span>|<span data-ttu-id="f3f8e-133">String</span><span class="sxs-lookup"><span data-stu-id="f3f8e-133">String</span></span>|<span data-ttu-id="f3f8e-134">Identificador exclusivo do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f3f8e-134">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="f3f8e-135">displayName</span><span class="sxs-lookup"><span data-stu-id="f3f8e-135">displayName</span></span>|<span data-ttu-id="f3f8e-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f3f8e-136">String</span></span>|<span data-ttu-id="f3f8e-137">Nome do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f3f8e-137">Name of the device management script.</span></span>|
|<span data-ttu-id="f3f8e-138">description</span><span class="sxs-lookup"><span data-stu-id="f3f8e-138">description</span></span>|<span data-ttu-id="f3f8e-139">String</span><span class="sxs-lookup"><span data-stu-id="f3f8e-139">String</span></span>|<span data-ttu-id="f3f8e-140">Descrição opcional para o script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f3f8e-140">Optional description for the device management script.</span></span>|
|<span data-ttu-id="f3f8e-141">scriptContent</span><span class="sxs-lookup"><span data-stu-id="f3f8e-141">scriptContent</span></span>|<span data-ttu-id="f3f8e-142">Binária</span><span class="sxs-lookup"><span data-stu-id="f3f8e-142">Binary</span></span>|<span data-ttu-id="f3f8e-143">O conteúdo de script.</span><span class="sxs-lookup"><span data-stu-id="f3f8e-143">The script content.</span></span>|
|<span data-ttu-id="f3f8e-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f3f8e-144">createdDateTime</span></span>|<span data-ttu-id="f3f8e-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3f8e-145">DateTimeOffset</span></span>|<span data-ttu-id="f3f8e-146">A data e a hora em que o script de gerenciamento de dispositivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="f3f8e-146">The date and time the device management script was created.</span></span> <span data-ttu-id="f3f8e-147">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f3f8e-147">This property is read-only.</span></span>|
|<span data-ttu-id="f3f8e-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3f8e-148">lastModifiedDateTime</span></span>|<span data-ttu-id="f3f8e-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3f8e-149">DateTimeOffset</span></span>|<span data-ttu-id="f3f8e-150">A data e a hora em que o script de gerenciamento de dispositivo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f3f8e-150">The date and time the device management script was last modified.</span></span> <span data-ttu-id="f3f8e-151">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f3f8e-151">This property is read-only.</span></span>|
|<span data-ttu-id="f3f8e-152">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="f3f8e-152">runAsAccount</span></span>|[<span data-ttu-id="f3f8e-153">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="f3f8e-153">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="f3f8e-154">Indica o tipo de contexto de execução.</span><span class="sxs-lookup"><span data-stu-id="f3f8e-154">Indicates the type of execution context.</span></span> <span data-ttu-id="f3f8e-155">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="f3f8e-155">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="f3f8e-156">fileName</span><span class="sxs-lookup"><span data-stu-id="f3f8e-156">fileName</span></span>|<span data-ttu-id="f3f8e-157">String</span><span class="sxs-lookup"><span data-stu-id="f3f8e-157">String</span></span>|<span data-ttu-id="f3f8e-158">Nome do arquivo de script.</span><span class="sxs-lookup"><span data-stu-id="f3f8e-158">Script file name.</span></span>|
|<span data-ttu-id="f3f8e-159">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f3f8e-159">roleScopeTagIds</span></span>|<span data-ttu-id="f3f8e-160">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f3f8e-160">String collection</span></span>|<span data-ttu-id="f3f8e-161">Lista de IDs de marca de escopo para esta instância de PowerShellScript.</span><span class="sxs-lookup"><span data-stu-id="f3f8e-161">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|



## <a name="response"></a><span data-ttu-id="f3f8e-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3f8e-162">Response</span></span>
<span data-ttu-id="f3f8e-163">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceShellScript](../resources/intune-devices-deviceshellscript.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f3f8e-163">If successful, this method returns a `201 Created` response code and a [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3f8e-164">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f3f8e-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3f8e-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3f8e-165">Request</span></span>
<span data-ttu-id="f3f8e-166">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f3f8e-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f3f8e-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3f8e-167">Response</span></span>
<span data-ttu-id="f3f8e-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f3f8e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





