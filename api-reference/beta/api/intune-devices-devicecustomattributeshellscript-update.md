---
title: Atualizar deviceCustomAttributeShellScript
description: Atualize as propriedades de um objeto deviceCustomAttributeShellScript.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dfe529650029c27aa03441b2d2c1e90ee6068b56
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150602"
---
# <a name="update-devicecustomattributeshellscript"></a><span data-ttu-id="53df6-103">Atualizar deviceCustomAttributeShellScript</span><span class="sxs-lookup"><span data-stu-id="53df6-103">Update deviceCustomAttributeShellScript</span></span>

<span data-ttu-id="53df6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53df6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="53df6-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="53df6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53df6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="53df6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53df6-107">Atualize as propriedades de [um objeto deviceCustomAttributeShellScript.](../resources/intune-devices-devicecustomattributeshellscript.md)</span><span class="sxs-lookup"><span data-stu-id="53df6-107">Update the properties of a [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53df6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="53df6-108">Prerequisites</span></span>
<span data-ttu-id="53df6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53df6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53df6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="53df6-111">Permission type</span></span>|<span data-ttu-id="53df6-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="53df6-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53df6-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="53df6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="53df6-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53df6-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="53df6-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="53df6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53df6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="53df6-116">Not supported.</span></span>|
|<span data-ttu-id="53df6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="53df6-117">Application</span></span>|<span data-ttu-id="53df6-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53df6-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="53df6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="53df6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}
```

## <a name="request-headers"></a><span data-ttu-id="53df6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="53df6-120">Request headers</span></span>
|<span data-ttu-id="53df6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="53df6-121">Header</span></span>|<span data-ttu-id="53df6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="53df6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53df6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="53df6-123">Authorization</span></span>|<span data-ttu-id="53df6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="53df6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53df6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="53df6-125">Accept</span></span>|<span data-ttu-id="53df6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="53df6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53df6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="53df6-127">Request body</span></span>
<span data-ttu-id="53df6-128">No corpo da solicitação, fornece uma representação JSON para o [objeto deviceCustomAttributeShellScript.](../resources/intune-devices-devicecustomattributeshellscript.md)</span><span class="sxs-lookup"><span data-stu-id="53df6-128">In the request body, supply a JSON representation for the [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) object.</span></span>

<span data-ttu-id="53df6-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md).</span><span class="sxs-lookup"><span data-stu-id="53df6-129">The following table shows the properties that are required when you create the [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md).</span></span>

|<span data-ttu-id="53df6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="53df6-130">Property</span></span>|<span data-ttu-id="53df6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="53df6-131">Type</span></span>|<span data-ttu-id="53df6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="53df6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53df6-133">id</span><span class="sxs-lookup"><span data-stu-id="53df6-133">id</span></span>|<span data-ttu-id="53df6-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53df6-134">String</span></span>|<span data-ttu-id="53df6-135">Identificador exclusivo da entidade de atributo personalizado.</span><span class="sxs-lookup"><span data-stu-id="53df6-135">Unique Identifier for the custom attribute entity.</span></span>|
|<span data-ttu-id="53df6-136">customAttributeName</span><span class="sxs-lookup"><span data-stu-id="53df6-136">customAttributeName</span></span>|<span data-ttu-id="53df6-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53df6-137">String</span></span>|<span data-ttu-id="53df6-138">O nome do atributo personalizado.</span><span class="sxs-lookup"><span data-stu-id="53df6-138">The name of the custom attribute.</span></span>|
|<span data-ttu-id="53df6-139">customAttributeType</span><span class="sxs-lookup"><span data-stu-id="53df6-139">customAttributeType</span></span>|[<span data-ttu-id="53df6-140">deviceCustomAttributeValueType</span><span class="sxs-lookup"><span data-stu-id="53df6-140">deviceCustomAttributeValueType</span></span>](../resources/intune-devices-devicecustomattributevaluetype.md)|<span data-ttu-id="53df6-141">O tipo esperado do valor do atributo personalizado.</span><span class="sxs-lookup"><span data-stu-id="53df6-141">The expected type of the custom attribute's value.</span></span> <span data-ttu-id="53df6-142">Os valores possíveis são: `integer`, `string`, `dateTime`.</span><span class="sxs-lookup"><span data-stu-id="53df6-142">Possible values are: `integer`, `string`, `dateTime`.</span></span>|
|<span data-ttu-id="53df6-143">displayName</span><span class="sxs-lookup"><span data-stu-id="53df6-143">displayName</span></span>|<span data-ttu-id="53df6-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53df6-144">String</span></span>|<span data-ttu-id="53df6-145">Nome do script de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="53df6-145">Name of the device management script.</span></span>|
|<span data-ttu-id="53df6-146">descrição</span><span class="sxs-lookup"><span data-stu-id="53df6-146">description</span></span>|<span data-ttu-id="53df6-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53df6-147">String</span></span>|<span data-ttu-id="53df6-148">Descrição opcional para o script de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="53df6-148">Optional description for the device management script.</span></span>|
|<span data-ttu-id="53df6-149">scriptContent</span><span class="sxs-lookup"><span data-stu-id="53df6-149">scriptContent</span></span>|<span data-ttu-id="53df6-150">Binário</span><span class="sxs-lookup"><span data-stu-id="53df6-150">Binary</span></span>|<span data-ttu-id="53df6-151">O conteúdo do script.</span><span class="sxs-lookup"><span data-stu-id="53df6-151">The script content.</span></span>|
|<span data-ttu-id="53df6-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="53df6-152">createdDateTime</span></span>|<span data-ttu-id="53df6-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53df6-153">DateTimeOffset</span></span>|<span data-ttu-id="53df6-154">A data e a hora em que o script de gerenciamento de dispositivos foi criado.</span><span class="sxs-lookup"><span data-stu-id="53df6-154">The date and time the device management script was created.</span></span> <span data-ttu-id="53df6-155">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="53df6-155">This property is read-only.</span></span>|
|<span data-ttu-id="53df6-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="53df6-156">lastModifiedDateTime</span></span>|<span data-ttu-id="53df6-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53df6-157">DateTimeOffset</span></span>|<span data-ttu-id="53df6-158">A data e a hora em que o script de gerenciamento de dispositivos foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="53df6-158">The date and time the device management script was last modified.</span></span> <span data-ttu-id="53df6-159">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="53df6-159">This property is read-only.</span></span>|
|<span data-ttu-id="53df6-160">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="53df6-160">runAsAccount</span></span>|[<span data-ttu-id="53df6-161">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="53df6-161">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="53df6-162">Indica o tipo de contexto de execução.</span><span class="sxs-lookup"><span data-stu-id="53df6-162">Indicates the type of execution context.</span></span> <span data-ttu-id="53df6-163">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="53df6-163">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="53df6-164">fileName</span><span class="sxs-lookup"><span data-stu-id="53df6-164">fileName</span></span>|<span data-ttu-id="53df6-165">String</span><span class="sxs-lookup"><span data-stu-id="53df6-165">String</span></span>|<span data-ttu-id="53df6-166">Nome do arquivo de script.</span><span class="sxs-lookup"><span data-stu-id="53df6-166">Script file name.</span></span>|
|<span data-ttu-id="53df6-167">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="53df6-167">roleScopeTagIds</span></span>|<span data-ttu-id="53df6-168">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="53df6-168">String collection</span></span>|<span data-ttu-id="53df6-169">Lista de IDs de marca de escopo para esta instância do PowerShellScript.</span><span class="sxs-lookup"><span data-stu-id="53df6-169">List of Scope Tag IDs for this PowerShellScript instance.</span></span>|



## <a name="response"></a><span data-ttu-id="53df6-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="53df6-170">Response</span></span>
<span data-ttu-id="53df6-171">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="53df6-171">If successful, this method returns a `200 OK` response code and an updated [deviceCustomAttributeShellScript](../resources/intune-devices-devicecustomattributeshellscript.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53df6-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="53df6-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="53df6-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="53df6-173">Request</span></span>
<span data-ttu-id="53df6-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="53df6-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCustomAttributeShellScripts/{deviceCustomAttributeShellScriptId}
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

### <a name="response"></a><span data-ttu-id="53df6-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="53df6-175">Response</span></span>
<span data-ttu-id="53df6-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="53df6-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




