---
title: Atualizar unsupportedDeviceConfiguration
description: Atualiza as propriedades de um objeto unsupportedDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 82072acfe1a8f7638fd15aa4a866e78b71a23821
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33921930"
---
# <a name="update-unsupporteddeviceconfiguration"></a><span data-ttu-id="3b75e-103">Atualizar unsupportedDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="3b75e-103">Update unsupportedDeviceConfiguration</span></span>

> <span data-ttu-id="3b75e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3b75e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b75e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3b75e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b75e-106">Atualiza as propriedades de um objeto [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="3b75e-106">Update the properties of a [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b75e-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3b75e-107">Prerequisites</span></span>
<span data-ttu-id="3b75e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b75e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b75e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b75e-110">Permission type</span></span>|<span data-ttu-id="3b75e-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3b75e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b75e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b75e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3b75e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b75e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3b75e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b75e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b75e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b75e-115">Not supported.</span></span>|
|<span data-ttu-id="3b75e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b75e-116">Application</span></span>|<span data-ttu-id="3b75e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b75e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b75e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b75e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3b75e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b75e-119">Request headers</span></span>
|<span data-ttu-id="3b75e-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3b75e-120">Header</span></span>|<span data-ttu-id="3b75e-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3b75e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b75e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b75e-122">Authorization</span></span>|<span data-ttu-id="3b75e-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b75e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b75e-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3b75e-124">Accept</span></span>|<span data-ttu-id="3b75e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3b75e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b75e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b75e-126">Request body</span></span>
<span data-ttu-id="3b75e-127">No corpo da solicitação, forneça uma representação JSON do objeto [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="3b75e-127">In the request body, supply a JSON representation for the [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>

<span data-ttu-id="3b75e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3b75e-128">The following table shows the properties that are required when you create the [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md).</span></span>

|<span data-ttu-id="3b75e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3b75e-129">Property</span></span>|<span data-ttu-id="3b75e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b75e-130">Type</span></span>|<span data-ttu-id="3b75e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b75e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b75e-132">id</span><span class="sxs-lookup"><span data-stu-id="3b75e-132">id</span></span>|<span data-ttu-id="3b75e-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b75e-133">String</span></span>|<span data-ttu-id="3b75e-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3b75e-134">Key of the entity.</span></span> <span data-ttu-id="3b75e-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b75e-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b75e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3b75e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="3b75e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b75e-137">DateTimeOffset</span></span>|<span data-ttu-id="3b75e-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="3b75e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="3b75e-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b75e-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b75e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3b75e-140">roleScopeTagIds</span></span>|<span data-ttu-id="3b75e-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b75e-141">String collection</span></span>|<span data-ttu-id="3b75e-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="3b75e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3b75e-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b75e-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b75e-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3b75e-144">supportsScopeTags</span></span>|<span data-ttu-id="3b75e-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="3b75e-145">Boolean</span></span>|<span data-ttu-id="3b75e-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="3b75e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3b75e-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="3b75e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3b75e-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="3b75e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3b75e-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3b75e-149">This property is read-only.</span></span> <span data-ttu-id="3b75e-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b75e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b75e-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3b75e-151">createdDateTime</span></span>|<span data-ttu-id="3b75e-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b75e-152">DateTimeOffset</span></span>|<span data-ttu-id="3b75e-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="3b75e-153">DateTime the object was created.</span></span> <span data-ttu-id="3b75e-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b75e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b75e-155">description</span><span class="sxs-lookup"><span data-stu-id="3b75e-155">description</span></span>|<span data-ttu-id="3b75e-156">String</span><span class="sxs-lookup"><span data-stu-id="3b75e-156">String</span></span>|<span data-ttu-id="3b75e-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3b75e-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3b75e-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b75e-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b75e-159">displayName</span><span class="sxs-lookup"><span data-stu-id="3b75e-159">displayName</span></span>|<span data-ttu-id="3b75e-160">String</span><span class="sxs-lookup"><span data-stu-id="3b75e-160">String</span></span>|<span data-ttu-id="3b75e-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3b75e-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3b75e-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b75e-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b75e-163">versão</span><span class="sxs-lookup"><span data-stu-id="3b75e-163">version</span></span>|<span data-ttu-id="3b75e-164">Int32</span><span class="sxs-lookup"><span data-stu-id="3b75e-164">Int32</span></span>|<span data-ttu-id="3b75e-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3b75e-165">Version of the device configuration.</span></span> <span data-ttu-id="3b75e-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b75e-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b75e-167">originalEntityTypeName</span><span class="sxs-lookup"><span data-stu-id="3b75e-167">originalEntityTypeName</span></span>|<span data-ttu-id="3b75e-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b75e-168">String</span></span>|<span data-ttu-id="3b75e-169">O tipo de entidade que seria retornado de outra forma.</span><span class="sxs-lookup"><span data-stu-id="3b75e-169">The type of entity that would be returned otherwise.</span></span>|
|<span data-ttu-id="3b75e-170">detalhes</span><span class="sxs-lookup"><span data-stu-id="3b75e-170">details</span></span>|<span data-ttu-id="3b75e-171">coleção [unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md)</span><span class="sxs-lookup"><span data-stu-id="3b75e-171">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md) collection</span></span>|<span data-ttu-id="3b75e-172">Detalhes que descrevem por que a entidade não é suportada.</span><span class="sxs-lookup"><span data-stu-id="3b75e-172">Details describing why the entity is unsupported.</span></span> <span data-ttu-id="3b75e-173">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="3b75e-173">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="3b75e-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b75e-174">Response</span></span>
<span data-ttu-id="3b75e-175">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b75e-175">If successful, this method returns a `200 OK` response code and an updated [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b75e-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3b75e-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b75e-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b75e-177">Request</span></span>
<span data-ttu-id="3b75e-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b75e-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 518

{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "originalEntityTypeName": "Original Entity Type Name value",
  "details": [
    {
      "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail",
      "message": "Message value",
      "propertyName": "Property Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="3b75e-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b75e-179">Response</span></span>
<span data-ttu-id="3b75e-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b75e-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 690

{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfiguration",
  "id": "f80d6fc8-6fc8-f80d-c86f-0df8c86f0df8",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "originalEntityTypeName": "Original Entity Type Name value",
  "details": [
    {
      "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail",
      "message": "Message value",
      "propertyName": "Property Name value"
    }
  ]
}
```




