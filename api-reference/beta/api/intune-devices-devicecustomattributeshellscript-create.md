---
title: Criar deviceCustomAttributeShellScript
description: Criar um novo objeto deviceCustomAttributeShellScript.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cab38c372bfea1185fdee6fa2015608ebb9fde8c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49219430"
---
# <a name="create-devicecustomattributeshellscript"></a><span data-ttu-id="987d6-103">Criar deviceCustomAttributeShellScript</span><span class="sxs-lookup"><span data-stu-id="987d6-103">Create deviceCustomAttributeShellScript</span></span>

<span data-ttu-id="987d6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="987d6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="987d6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="987d6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="987d6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="987d6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="987d6-107">Criar um novo objeto [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) .</span><span class="sxs-lookup"><span data-stu-id="987d6-107">Create a new [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="987d6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="987d6-108">Prerequisites</span></span>
<span data-ttu-id="987d6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="987d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="987d6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="987d6-111">Permission type</span></span>|<span data-ttu-id="987d6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="987d6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="987d6-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="987d6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="987d6-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="987d6-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="987d6-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="987d6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="987d6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="987d6-116">Not supported.</span></span>|
|<span data-ttu-id="987d6-117">Application</span><span class="sxs-lookup"><span data-stu-id="987d6-117">Application</span></span>|<span data-ttu-id="987d6-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="987d6-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="987d6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="987d6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCustomAttributeShellScripts
```

## <a name="request-headers"></a><span data-ttu-id="987d6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="987d6-120">Request headers</span></span>
|<span data-ttu-id="987d6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="987d6-121">Header</span></span>|<span data-ttu-id="987d6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="987d6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="987d6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="987d6-123">Authorization</span></span>|<span data-ttu-id="987d6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="987d6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="987d6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="987d6-125">Accept</span></span>|<span data-ttu-id="987d6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="987d6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="987d6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="987d6-127">Request body</span></span>
<span data-ttu-id="987d6-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceCustomAttributeShellScript.</span><span class="sxs-lookup"><span data-stu-id="987d6-128">In the request body, supply a JSON representation for the deviceCustomAttributeShellScript object.</span></span>

<span data-ttu-id="987d6-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceCustomAttributeShellScript.</span><span class="sxs-lookup"><span data-stu-id="987d6-129">The following table shows the properties that are required when you create the deviceCustomAttributeShellScript.</span></span>

|<span data-ttu-id="987d6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="987d6-130">Property</span></span>|<span data-ttu-id="987d6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="987d6-131">Type</span></span>|<span data-ttu-id="987d6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="987d6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="987d6-133">id</span><span class="sxs-lookup"><span data-stu-id="987d6-133">id</span></span>|<span data-ttu-id="987d6-134">String</span><span class="sxs-lookup"><span data-stu-id="987d6-134">String</span></span>|<span data-ttu-id="987d6-135">Identificador exclusivo da entidade de atributo Personalizada.</span><span class="sxs-lookup"><span data-stu-id="987d6-135">Unique Identifier for the custom attribute entity.</span></span>|
|<span data-ttu-id="987d6-136">customAttributeName</span><span class="sxs-lookup"><span data-stu-id="987d6-136">customAttributeName</span></span>|<span data-ttu-id="987d6-137">String</span><span class="sxs-lookup"><span data-stu-id="987d6-137">String</span></span>|<span data-ttu-id="987d6-138">O nome do atributo personalizado.</span><span class="sxs-lookup"><span data-stu-id="987d6-138">The name of the custom attribute.</span></span>|
|<span data-ttu-id="987d6-139">customAttributeType</span><span class="sxs-lookup"><span data-stu-id="987d6-139">customAttributeType</span></span>|[<span data-ttu-id="987d6-140">deviceCustomAttributeValueType</span><span class="sxs-lookup"><span data-stu-id="987d6-140">deviceCustomAttributeValueType</span></span>](../resources/intune-devices-devicecustomattributevaluetype.md)|<span data-ttu-id="987d6-141">O tipo esperado do valor do atributo personalizado.</span><span class="sxs-lookup"><span data-stu-id="987d6-141">The expected type of the custom attribute's value.</span></span> <span data-ttu-id="987d6-142">Os valores possíveis são: `integer`, `string`, `dateTime`.</span><span class="sxs-lookup"><span data-stu-id="987d6-142">Possible values are: `integer`, `string`, `dateTime`.</span></span>|
|<span data-ttu-id="987d6-143">displayName</span><span class="sxs-lookup"><span data-stu-id="987d6-143">displayName</span></span>|<span data-ttu-id="987d6-144">String</span><span class="sxs-lookup"><span data-stu-id="987d6-144">String</span></span>|<span data-ttu-id="987d6-145">Nome do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="987d6-145">Name of the device management script.</span></span>|
|<span data-ttu-id="987d6-146">description</span><span class="sxs-lookup"><span data-stu-id="987d6-146">description</span></span>|<span data-ttu-id="987d6-147">String</span><span class="sxs-lookup"><span data-stu-id="987d6-147">String</span></span>|<span data-ttu-id="987d6-148">Descrição opcional para o script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="987d6-148">Optional description for the device management script.</span></span>|
|<span data-ttu-id="987d6-149">scriptContent</span><span class="sxs-lookup"><span data-stu-id="987d6-149">scriptContent</span></span>|<span data-ttu-id="987d6-150">Binária</span><span class="sxs-lookup"><span data-stu-id="987d6-150">Binary</span></span>|<span data-ttu-id="987d6-151">O conteúdo de script.</span><span class="sxs-lookup"><span data-stu-id="987d6-151">The script content.</span></span>|
|<span data-ttu-id="987d6-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="987d6-152">createdDateTime</span></span>|<span data-ttu-id="987d6-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="987d6-153">DateTimeOffset</span></span>|<span data-ttu-id="987d6-154">A data e a hora em que o script de gerenciamento de dispositivo foi criado.</span><span class="sxs-lookup"><span data-stu-id="987d6-154">The date and time the device management script was created.</span></span> <span data-ttu-id="987d6-155">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="987d6-155">This property is read-only.</span></span>|
|<span data-ttu-id="987d6-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="987d6-156">lastModifiedDateTime</span></span>|<span data-ttu-id="987d6-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="987d6-157">DateTimeOffset</span></span>|<span data-ttu-id="987d6-158">A data e a hora em que o script de gerenciamento de dispositivo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="987d6-158">The date and time the device management script was last modified.</span></span> <span data-ttu-id="987d6-159">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="987d6-159">This property is read-only.</span></span>|
|<span data-ttu-id="987d6-160">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="987d6-160">runAsAccount</span></span>|[<span data-ttu-id="987d6-161">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="987d6-161">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="987d6-162">Indica o tipo de contexto de execução.</span><span class="sxs-lookup"><span data-stu-id="987d6-162">Indicates the type of execution context.</span></span> <span data-ttu-id="987d6-163">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="987d6-163">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="987d6-164">fileName</span><span class="sxs-lookup"><span data-stu-id="987d6-164">fileName</span></span>|<span data-ttu-id="987d6-165">String</span><span class="sxs-lookup"><span data-stu-id="987d6-165">String</span></span>|<span data-ttu-id="987d6-166">Nome do arquivo de script.</span><span class="sxs-lookup"><span data-stu-id="987d6-166">Script file name.</span></span>|
|<span data-ttu-id="987d6-167">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="987d6-167">roleScopeTagIds</span></span>|<span data-ttu-id="987d6-168">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="987d6-168">String collection</span></span>|<span data-ttu-id="987d6-169">Lista de IDs de marca de escopo para esta instância de PowerShellScript.</span><span class="sxs-lookup"><span data-stu-id="987d6-169">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|



## <a name="response"></a><span data-ttu-id="987d6-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="987d6-170">Response</span></span>
<span data-ttu-id="987d6-171">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="987d6-171">If successful, this method returns a `201 Created` response code and a [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="987d6-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="987d6-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="987d6-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="987d6-173">Request</span></span>
<span data-ttu-id="987d6-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="987d6-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="987d6-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="987d6-175">Response</span></span>
<span data-ttu-id="987d6-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="987d6-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




