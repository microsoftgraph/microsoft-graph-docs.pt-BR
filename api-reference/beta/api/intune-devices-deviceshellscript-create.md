---
title: Criar deviceShellScript
description: Criar um novo objeto deviceShellScript.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 662d0be06b4a714a271e12b1e813aa09f5c76187
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42469157"
---
# <a name="create-deviceshellscript"></a><span data-ttu-id="93ce6-103">Criar deviceShellScript</span><span class="sxs-lookup"><span data-stu-id="93ce6-103">Create deviceShellScript</span></span>

<span data-ttu-id="93ce6-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="93ce6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="93ce6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="93ce6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93ce6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="93ce6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93ce6-107">Criar um novo objeto [deviceShellScript](../resources/intune-devices-deviceshellscript.md) .</span><span class="sxs-lookup"><span data-stu-id="93ce6-107">Create a new [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="93ce6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="93ce6-108">Prerequisites</span></span>
<span data-ttu-id="93ce6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93ce6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="93ce6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="93ce6-111">Permission type</span></span>|<span data-ttu-id="93ce6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="93ce6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93ce6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="93ce6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="93ce6-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93ce6-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="93ce6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="93ce6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93ce6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93ce6-116">Not supported.</span></span>|
|<span data-ttu-id="93ce6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="93ce6-117">Application</span></span>|<span data-ttu-id="93ce6-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93ce6-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="93ce6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93ce6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceShellScripts
```

## <a name="request-headers"></a><span data-ttu-id="93ce6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="93ce6-120">Request headers</span></span>
|<span data-ttu-id="93ce6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="93ce6-121">Header</span></span>|<span data-ttu-id="93ce6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="93ce6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93ce6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="93ce6-123">Authorization</span></span>|<span data-ttu-id="93ce6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93ce6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93ce6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="93ce6-125">Accept</span></span>|<span data-ttu-id="93ce6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="93ce6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93ce6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="93ce6-127">Request body</span></span>
<span data-ttu-id="93ce6-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceShellScript.</span><span class="sxs-lookup"><span data-stu-id="93ce6-128">In the request body, supply a JSON representation for the deviceShellScript object.</span></span>

<span data-ttu-id="93ce6-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceShellScript.</span><span class="sxs-lookup"><span data-stu-id="93ce6-129">The following table shows the properties that are required when you create the deviceShellScript.</span></span>

|<span data-ttu-id="93ce6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93ce6-130">Property</span></span>|<span data-ttu-id="93ce6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="93ce6-131">Type</span></span>|<span data-ttu-id="93ce6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="93ce6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93ce6-133">id</span><span class="sxs-lookup"><span data-stu-id="93ce6-133">id</span></span>|<span data-ttu-id="93ce6-134">String</span><span class="sxs-lookup"><span data-stu-id="93ce6-134">String</span></span>|<span data-ttu-id="93ce6-135">Identificador exclusivo do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="93ce6-135">Unique Identifier for the device management script.</span></span>|
|<span data-ttu-id="93ce6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="93ce6-136">displayName</span></span>|<span data-ttu-id="93ce6-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="93ce6-137">String</span></span>|<span data-ttu-id="93ce6-138">Nome do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="93ce6-138">Name of the device management script.</span></span>|
|<span data-ttu-id="93ce6-139">description</span><span class="sxs-lookup"><span data-stu-id="93ce6-139">description</span></span>|<span data-ttu-id="93ce6-140">String</span><span class="sxs-lookup"><span data-stu-id="93ce6-140">String</span></span>|<span data-ttu-id="93ce6-141">Descrição opcional para o script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="93ce6-141">Optional description for the device management script.</span></span>|
|<span data-ttu-id="93ce6-142">scriptContent</span><span class="sxs-lookup"><span data-stu-id="93ce6-142">scriptContent</span></span>|<span data-ttu-id="93ce6-143">Binária</span><span class="sxs-lookup"><span data-stu-id="93ce6-143">Binary</span></span>|<span data-ttu-id="93ce6-144">O conteúdo de script.</span><span class="sxs-lookup"><span data-stu-id="93ce6-144">The script content.</span></span>|
|<span data-ttu-id="93ce6-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="93ce6-145">createdDateTime</span></span>|<span data-ttu-id="93ce6-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93ce6-146">DateTimeOffset</span></span>|<span data-ttu-id="93ce6-147">A data e a hora em que o script de gerenciamento de dispositivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="93ce6-147">The date and time the device management script was created.</span></span> <span data-ttu-id="93ce6-148">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="93ce6-148">This property is read-only.</span></span>|
|<span data-ttu-id="93ce6-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="93ce6-149">lastModifiedDateTime</span></span>|<span data-ttu-id="93ce6-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93ce6-150">DateTimeOffset</span></span>|<span data-ttu-id="93ce6-151">A data e a hora em que o script de gerenciamento de dispositivo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="93ce6-151">The date and time the device management script was last modified.</span></span> <span data-ttu-id="93ce6-152">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="93ce6-152">This property is read-only.</span></span>|
|<span data-ttu-id="93ce6-153">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="93ce6-153">runAsAccount</span></span>|[<span data-ttu-id="93ce6-154">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="93ce6-154">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="93ce6-155">Indica o tipo de contexto de execução.</span><span class="sxs-lookup"><span data-stu-id="93ce6-155">Indicates the type of execution context.</span></span> <span data-ttu-id="93ce6-156">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="93ce6-156">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="93ce6-157">fileName</span><span class="sxs-lookup"><span data-stu-id="93ce6-157">fileName</span></span>|<span data-ttu-id="93ce6-158">String</span><span class="sxs-lookup"><span data-stu-id="93ce6-158">String</span></span>|<span data-ttu-id="93ce6-159">Nome do arquivo de script.</span><span class="sxs-lookup"><span data-stu-id="93ce6-159">Script file name.</span></span>|
|<span data-ttu-id="93ce6-160">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="93ce6-160">roleScopeTagIds</span></span>|<span data-ttu-id="93ce6-161">String collection</span><span class="sxs-lookup"><span data-stu-id="93ce6-161">String collection</span></span>|<span data-ttu-id="93ce6-162">Lista de IDs de marca de escopo para esta instância de PowerShellScript.</span><span class="sxs-lookup"><span data-stu-id="93ce6-162">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|



## <a name="response"></a><span data-ttu-id="93ce6-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="93ce6-163">Response</span></span>
<span data-ttu-id="93ce6-164">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceShellScript](../resources/intune-devices-deviceshellscript.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="93ce6-164">If successful, this method returns a `201 Created` response code and a [deviceShellScript](../resources/intune-devices-deviceshellscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93ce6-165">Exemplo</span><span class="sxs-lookup"><span data-stu-id="93ce6-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="93ce6-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93ce6-166">Request</span></span>
<span data-ttu-id="93ce6-167">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="93ce6-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="93ce6-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="93ce6-168">Response</span></span>
<span data-ttu-id="93ce6-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="93ce6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





