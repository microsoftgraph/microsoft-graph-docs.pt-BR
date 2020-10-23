---
title: Criar deviceCustomAttributeShellScript
description: Criar um novo objeto deviceCustomAttributeShellScript.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ba72710bfeec5d0b5549837eff0fec4d2bed5510
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48704865"
---
# <a name="create-devicecustomattributeshellscript"></a><span data-ttu-id="cf990-103">Criar deviceCustomAttributeShellScript</span><span class="sxs-lookup"><span data-stu-id="cf990-103">Create deviceCustomAttributeShellScript</span></span>

<span data-ttu-id="cf990-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf990-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cf990-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cf990-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf990-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cf990-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf990-107">Criar um novo objeto [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) .</span><span class="sxs-lookup"><span data-stu-id="cf990-107">Create a new [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf990-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cf990-108">Prerequisites</span></span>
<span data-ttu-id="cf990-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf990-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf990-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf990-111">Permission type</span></span>|<span data-ttu-id="cf990-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cf990-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf990-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf990-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cf990-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf990-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="cf990-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf990-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf990-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf990-116">Not supported.</span></span>|
|<span data-ttu-id="cf990-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf990-117">Application</span></span>|<span data-ttu-id="cf990-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf990-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf990-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf990-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCustomAttributeShellScripts
```

## <a name="request-headers"></a><span data-ttu-id="cf990-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf990-120">Request headers</span></span>
|<span data-ttu-id="cf990-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cf990-121">Header</span></span>|<span data-ttu-id="cf990-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cf990-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf990-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf990-123">Authorization</span></span>|<span data-ttu-id="cf990-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf990-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf990-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cf990-125">Accept</span></span>|<span data-ttu-id="cf990-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cf990-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf990-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf990-127">Request body</span></span>
<span data-ttu-id="cf990-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceCustomAttributeShellScript.</span><span class="sxs-lookup"><span data-stu-id="cf990-128">In the request body, supply a JSON representation for the deviceCustomAttributeShellScript object.</span></span>

<span data-ttu-id="cf990-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceCustomAttributeShellScript.</span><span class="sxs-lookup"><span data-stu-id="cf990-129">The following table shows the properties that are required when you create the deviceCustomAttributeShellScript.</span></span>

|<span data-ttu-id="cf990-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf990-130">Property</span></span>|<span data-ttu-id="cf990-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf990-131">Type</span></span>|<span data-ttu-id="cf990-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf990-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf990-133">id</span><span class="sxs-lookup"><span data-stu-id="cf990-133">id</span></span>|<span data-ttu-id="cf990-134">String</span><span class="sxs-lookup"><span data-stu-id="cf990-134">String</span></span>|<span data-ttu-id="cf990-135">Identificador exclusivo da entidade de atributo Personalizada.</span><span class="sxs-lookup"><span data-stu-id="cf990-135">Unique Identifier for the custom attribute entity.</span></span>|
|<span data-ttu-id="cf990-136">customAttributeName</span><span class="sxs-lookup"><span data-stu-id="cf990-136">customAttributeName</span></span>|<span data-ttu-id="cf990-137">String</span><span class="sxs-lookup"><span data-stu-id="cf990-137">String</span></span>|<span data-ttu-id="cf990-138">O nome do atributo personalizado.</span><span class="sxs-lookup"><span data-stu-id="cf990-138">The name of the custom attribute.</span></span>|
|<span data-ttu-id="cf990-139">customAttributeType</span><span class="sxs-lookup"><span data-stu-id="cf990-139">customAttributeType</span></span>|[<span data-ttu-id="cf990-140">deviceCustomAttributeValueType</span><span class="sxs-lookup"><span data-stu-id="cf990-140">deviceCustomAttributeValueType</span></span>](../resources/intune-devices-devicecustomattributevaluetype.md)|<span data-ttu-id="cf990-141">O tipo esperado do valor do atributo personalizado.</span><span class="sxs-lookup"><span data-stu-id="cf990-141">The expected type of the custom attribute's value.</span></span> <span data-ttu-id="cf990-142">Os valores possíveis são: `integer`, `string`, `dateTime`.</span><span class="sxs-lookup"><span data-stu-id="cf990-142">Possible values are: `integer`, `string`, `dateTime`.</span></span>|
|<span data-ttu-id="cf990-143">displayName</span><span class="sxs-lookup"><span data-stu-id="cf990-143">displayName</span></span>|<span data-ttu-id="cf990-144">String</span><span class="sxs-lookup"><span data-stu-id="cf990-144">String</span></span>|<span data-ttu-id="cf990-145">Nome do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cf990-145">Name of the device management script.</span></span>|
|<span data-ttu-id="cf990-146">description</span><span class="sxs-lookup"><span data-stu-id="cf990-146">description</span></span>|<span data-ttu-id="cf990-147">String</span><span class="sxs-lookup"><span data-stu-id="cf990-147">String</span></span>|<span data-ttu-id="cf990-148">Descrição opcional para o script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cf990-148">Optional description for the device management script.</span></span>|
|<span data-ttu-id="cf990-149">scriptContent</span><span class="sxs-lookup"><span data-stu-id="cf990-149">scriptContent</span></span>|<span data-ttu-id="cf990-150">Binária</span><span class="sxs-lookup"><span data-stu-id="cf990-150">Binary</span></span>|<span data-ttu-id="cf990-151">O conteúdo de script.</span><span class="sxs-lookup"><span data-stu-id="cf990-151">The script content.</span></span>|
|<span data-ttu-id="cf990-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cf990-152">createdDateTime</span></span>|<span data-ttu-id="cf990-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf990-153">DateTimeOffset</span></span>|<span data-ttu-id="cf990-154">A data e a hora em que o script de gerenciamento de dispositivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="cf990-154">The date and time the device management script was created.</span></span> <span data-ttu-id="cf990-155">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cf990-155">This property is read-only.</span></span>|
|<span data-ttu-id="cf990-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cf990-156">lastModifiedDateTime</span></span>|<span data-ttu-id="cf990-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf990-157">DateTimeOffset</span></span>|<span data-ttu-id="cf990-158">A data e a hora em que o script de gerenciamento de dispositivo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="cf990-158">The date and time the device management script was last modified.</span></span> <span data-ttu-id="cf990-159">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cf990-159">This property is read-only.</span></span>|
|<span data-ttu-id="cf990-160">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="cf990-160">runAsAccount</span></span>|[<span data-ttu-id="cf990-161">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="cf990-161">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="cf990-162">Indica o tipo de contexto de execução.</span><span class="sxs-lookup"><span data-stu-id="cf990-162">Indicates the type of execution context.</span></span> <span data-ttu-id="cf990-163">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="cf990-163">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="cf990-164">fileName</span><span class="sxs-lookup"><span data-stu-id="cf990-164">fileName</span></span>|<span data-ttu-id="cf990-165">String</span><span class="sxs-lookup"><span data-stu-id="cf990-165">String</span></span>|<span data-ttu-id="cf990-166">Nome do arquivo de script.</span><span class="sxs-lookup"><span data-stu-id="cf990-166">Script file name.</span></span>|
|<span data-ttu-id="cf990-167">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cf990-167">roleScopeTagIds</span></span>|<span data-ttu-id="cf990-168">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf990-168">String collection</span></span>|<span data-ttu-id="cf990-169">Lista de IDs de marca de escopo para esta instância de PowerShellScript.</span><span class="sxs-lookup"><span data-stu-id="cf990-169">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|



## <a name="response"></a><span data-ttu-id="cf990-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf990-170">Response</span></span>
<span data-ttu-id="cf990-171">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf990-171">If successful, this method returns a `201 Created` response code and a [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf990-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cf990-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf990-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf990-173">Request</span></span>
<span data-ttu-id="cf990-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf990-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCustomAttributeShellScripts
Content-type: application/json
Content-length: 413

{
  "@odata.type": "#microsoft.graph.deviceCustomAttributeShellScript",
  "customAttributeName": "Custom Attribute Name value",
  "customAttributeType": "string",
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

### <a name="response"></a><span data-ttu-id="cf990-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf990-175">Response</span></span>
<span data-ttu-id="cf990-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cf990-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 585

{
  "@odata.type": "#microsoft.graph.deviceCustomAttributeShellScript",
  "id": "929d921b-921b-929d-1b92-9d921b929d92",
  "customAttributeName": "Custom Attribute Name value",
  "customAttributeType": "string",
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





