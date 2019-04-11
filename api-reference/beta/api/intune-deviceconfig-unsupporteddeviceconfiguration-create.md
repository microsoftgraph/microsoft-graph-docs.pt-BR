---
title: Criar unsupportedDeviceConfiguration
description: Criar um novo objeto unsupportedDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e6012a286a98f676986fb8cb4aa6bb45948f50c
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31797596"
---
# <a name="create-unsupporteddeviceconfiguration"></a><span data-ttu-id="84da4-103">Criar unsupportedDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="84da4-103">Create unsupportedDeviceConfiguration</span></span>

> <span data-ttu-id="84da4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="84da4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84da4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="84da4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84da4-106">Criar um novo objeto [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="84da4-106">Create a new [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84da4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="84da4-107">Prerequisites</span></span>
<span data-ttu-id="84da4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84da4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84da4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="84da4-110">Permission type</span></span>|<span data-ttu-id="84da4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="84da4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84da4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="84da4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="84da4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84da4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="84da4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="84da4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84da4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84da4-115">Not supported.</span></span>|
|<span data-ttu-id="84da4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="84da4-116">Application</span></span>|<span data-ttu-id="84da4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84da4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84da4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="84da4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="84da4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="84da4-119">Request headers</span></span>
|<span data-ttu-id="84da4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="84da4-120">Header</span></span>|<span data-ttu-id="84da4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="84da4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84da4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="84da4-122">Authorization</span></span>|<span data-ttu-id="84da4-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84da4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84da4-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="84da4-124">Accept</span></span>|<span data-ttu-id="84da4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="84da4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84da4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="84da4-126">Request body</span></span>
<span data-ttu-id="84da4-127">No corpo da solicitação, forneça uma representação JSON do objeto unsupportedDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="84da4-127">In the request body, supply a JSON representation for the unsupportedDeviceConfiguration object.</span></span>

<span data-ttu-id="84da4-128">A tabela a seguir mostra as propriedades que são necessárias ao criar unsupportedDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="84da4-128">The following table shows the properties that are required when you create the unsupportedDeviceConfiguration.</span></span>

|<span data-ttu-id="84da4-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="84da4-129">Property</span></span>|<span data-ttu-id="84da4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="84da4-130">Type</span></span>|<span data-ttu-id="84da4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="84da4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84da4-132">id</span><span class="sxs-lookup"><span data-stu-id="84da4-132">id</span></span>|<span data-ttu-id="84da4-133">String</span><span class="sxs-lookup"><span data-stu-id="84da4-133">String</span></span>|<span data-ttu-id="84da4-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="84da4-134">Key of the entity.</span></span> <span data-ttu-id="84da4-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84da4-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84da4-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="84da4-136">lastModifiedDateTime</span></span>|<span data-ttu-id="84da4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84da4-137">DateTimeOffset</span></span>|<span data-ttu-id="84da4-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="84da4-138">DateTime the object was last modified.</span></span> <span data-ttu-id="84da4-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84da4-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84da4-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="84da4-140">roleScopeTagIds</span></span>|<span data-ttu-id="84da4-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="84da4-141">String collection</span></span>|<span data-ttu-id="84da4-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="84da4-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="84da4-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84da4-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84da4-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="84da4-144">supportsScopeTags</span></span>|<span data-ttu-id="84da4-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="84da4-145">Boolean</span></span>|<span data-ttu-id="84da4-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="84da4-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="84da4-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="84da4-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="84da4-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="84da4-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="84da4-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="84da4-149">This property is read-only.</span></span> <span data-ttu-id="84da4-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84da4-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84da4-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="84da4-151">createdDateTime</span></span>|<span data-ttu-id="84da4-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84da4-152">DateTimeOffset</span></span>|<span data-ttu-id="84da4-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="84da4-153">DateTime the object was created.</span></span> <span data-ttu-id="84da4-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84da4-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84da4-155">description</span><span class="sxs-lookup"><span data-stu-id="84da4-155">description</span></span>|<span data-ttu-id="84da4-156">String</span><span class="sxs-lookup"><span data-stu-id="84da4-156">String</span></span>|<span data-ttu-id="84da4-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84da4-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="84da4-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84da4-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84da4-159">displayName</span><span class="sxs-lookup"><span data-stu-id="84da4-159">displayName</span></span>|<span data-ttu-id="84da4-160">String</span><span class="sxs-lookup"><span data-stu-id="84da4-160">String</span></span>|<span data-ttu-id="84da4-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84da4-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="84da4-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84da4-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84da4-163">versão</span><span class="sxs-lookup"><span data-stu-id="84da4-163">version</span></span>|<span data-ttu-id="84da4-164">Int32</span><span class="sxs-lookup"><span data-stu-id="84da4-164">Int32</span></span>|<span data-ttu-id="84da4-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="84da4-165">Version of the device configuration.</span></span> <span data-ttu-id="84da4-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="84da4-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="84da4-167">originalEntityTypeName</span><span class="sxs-lookup"><span data-stu-id="84da4-167">originalEntityTypeName</span></span>|<span data-ttu-id="84da4-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84da4-168">String</span></span>|<span data-ttu-id="84da4-169">O tipo de entidade que seria retornado de outra forma.</span><span class="sxs-lookup"><span data-stu-id="84da4-169">The type of entity that would be returned otherwise.</span></span>|
|<span data-ttu-id="84da4-170">detalhes</span><span class="sxs-lookup"><span data-stu-id="84da4-170">details</span></span>|<span data-ttu-id="84da4-171">coleção [unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md)</span><span class="sxs-lookup"><span data-stu-id="84da4-171">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md) collection</span></span>|<span data-ttu-id="84da4-172">Detalhes que descrevem por que a entidade não é suportada.</span><span class="sxs-lookup"><span data-stu-id="84da4-172">Details describing why the entity is unsupported.</span></span> <span data-ttu-id="84da4-173">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="84da4-173">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="84da4-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="84da4-174">Response</span></span>
<span data-ttu-id="84da4-175">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="84da4-175">If successful, this method returns a `201 Created` response code and a [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84da4-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="84da4-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="84da4-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="84da4-177">Request</span></span>
<span data-ttu-id="84da4-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="84da4-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="84da4-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="84da4-179">Response</span></span>
<span data-ttu-id="84da4-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="84da4-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





