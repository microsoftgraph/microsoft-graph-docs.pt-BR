---
title: Criar unsupportedDeviceConfiguration
description: Crie um novo objeto de unsupportedDeviceConfiguration.
ms.openlocfilehash: 83dd3f14d564d2e8f0511772788281a5e5748b3a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036133"
---
# <a name="create-unsupporteddeviceconfiguration"></a><span data-ttu-id="4cf21-103">Criar unsupportedDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="4cf21-103">Create unsupportedDeviceConfiguration</span></span>

> <span data-ttu-id="4cf21-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4cf21-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4cf21-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4cf21-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4cf21-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4cf21-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4cf21-107">Crie um novo objeto de [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="4cf21-107">Create a new [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4cf21-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4cf21-108">Prerequisites</span></span>
<span data-ttu-id="4cf21-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cf21-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cf21-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4cf21-111">Permission type</span></span>|<span data-ttu-id="4cf21-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4cf21-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4cf21-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4cf21-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4cf21-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cf21-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4cf21-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4cf21-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4cf21-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4cf21-116">Not supported.</span></span>|
|<span data-ttu-id="4cf21-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4cf21-117">Application</span></span>|<span data-ttu-id="4cf21-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4cf21-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4cf21-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4cf21-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4cf21-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4cf21-120">Request headers</span></span>
|<span data-ttu-id="4cf21-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4cf21-121">Header</span></span>|<span data-ttu-id="4cf21-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4cf21-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4cf21-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4cf21-123">Authorization</span></span>|<span data-ttu-id="4cf21-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4cf21-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4cf21-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4cf21-125">Accept</span></span>|<span data-ttu-id="4cf21-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4cf21-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4cf21-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4cf21-127">Request body</span></span>
<span data-ttu-id="4cf21-128">No corpo da solicitação, fornece uma representação JSON para o objeto unsupportedDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4cf21-128">In the request body, supply a JSON representation for the unsupportedDeviceConfiguration object.</span></span>

<span data-ttu-id="4cf21-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o unsupportedDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4cf21-129">The following table shows the properties that are required when you create the unsupportedDeviceConfiguration.</span></span>

|<span data-ttu-id="4cf21-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4cf21-130">Property</span></span>|<span data-ttu-id="4cf21-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4cf21-131">Type</span></span>|<span data-ttu-id="4cf21-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4cf21-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cf21-133">id</span><span class="sxs-lookup"><span data-stu-id="4cf21-133">id</span></span>|<span data-ttu-id="4cf21-134">String</span><span class="sxs-lookup"><span data-stu-id="4cf21-134">String</span></span>|<span data-ttu-id="4cf21-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4cf21-135">Key of the entity.</span></span> <span data-ttu-id="4cf21-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4cf21-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4cf21-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4cf21-137">lastModifiedDateTime</span></span>|<span data-ttu-id="4cf21-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4cf21-138">DateTimeOffset</span></span>|<span data-ttu-id="4cf21-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="4cf21-139">DateTime the object was last modified.</span></span> <span data-ttu-id="4cf21-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4cf21-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4cf21-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4cf21-141">roleScopeTagIds</span></span>|<span data-ttu-id="4cf21-142">String collection</span><span class="sxs-lookup"><span data-stu-id="4cf21-142">String collection</span></span>|<span data-ttu-id="4cf21-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="4cf21-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4cf21-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4cf21-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4cf21-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4cf21-145">supportsScopeTags</span></span>|<span data-ttu-id="4cf21-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="4cf21-146">Boolean</span></span>|<span data-ttu-id="4cf21-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="4cf21-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4cf21-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="4cf21-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4cf21-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="4cf21-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4cf21-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4cf21-150">This property is read-only.</span></span> <span data-ttu-id="4cf21-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4cf21-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4cf21-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4cf21-152">createdDateTime</span></span>|<span data-ttu-id="4cf21-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4cf21-153">DateTimeOffset</span></span>|<span data-ttu-id="4cf21-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="4cf21-154">DateTime the object was created.</span></span> <span data-ttu-id="4cf21-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4cf21-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4cf21-156">description</span><span class="sxs-lookup"><span data-stu-id="4cf21-156">description</span></span>|<span data-ttu-id="4cf21-157">String</span><span class="sxs-lookup"><span data-stu-id="4cf21-157">String</span></span>|<span data-ttu-id="4cf21-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4cf21-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4cf21-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4cf21-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4cf21-160">displayName</span><span class="sxs-lookup"><span data-stu-id="4cf21-160">displayName</span></span>|<span data-ttu-id="4cf21-161">String</span><span class="sxs-lookup"><span data-stu-id="4cf21-161">String</span></span>|<span data-ttu-id="4cf21-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4cf21-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4cf21-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4cf21-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4cf21-164">version</span><span class="sxs-lookup"><span data-stu-id="4cf21-164">version</span></span>|<span data-ttu-id="4cf21-165">Int32</span><span class="sxs-lookup"><span data-stu-id="4cf21-165">Int32</span></span>|<span data-ttu-id="4cf21-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4cf21-166">Version of the device configuration.</span></span> <span data-ttu-id="4cf21-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4cf21-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4cf21-168">originalEntityTypeName</span><span class="sxs-lookup"><span data-stu-id="4cf21-168">originalEntityTypeName</span></span>|<span data-ttu-id="4cf21-169">String</span><span class="sxs-lookup"><span data-stu-id="4cf21-169">String</span></span>|<span data-ttu-id="4cf21-170">O tipo de entidade que será retornado caso contrário.</span><span class="sxs-lookup"><span data-stu-id="4cf21-170">The type of entity that would be returned otherwise.</span></span>|
|<span data-ttu-id="4cf21-171">detalhes</span><span class="sxs-lookup"><span data-stu-id="4cf21-171">details</span></span>|<span data-ttu-id="4cf21-172">coleção [unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md)</span><span class="sxs-lookup"><span data-stu-id="4cf21-172">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md) collection</span></span>|<span data-ttu-id="4cf21-173">Detalhes descrevendo por que não há suporte para a entidade.</span><span class="sxs-lookup"><span data-stu-id="4cf21-173">Details describing why the entity is unsupported.</span></span> <span data-ttu-id="4cf21-174">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="4cf21-174">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="4cf21-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="4cf21-175">Response</span></span>
<span data-ttu-id="4cf21-176">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4cf21-176">If successful, this method returns a `201 Created` response code and a [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4cf21-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4cf21-177">Example</span></span>
### <a name="request"></a><span data-ttu-id="4cf21-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4cf21-178">Request</span></span>
<span data-ttu-id="4cf21-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4cf21-179">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 582

{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="4cf21-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="4cf21-180">Response</span></span>
<span data-ttu-id="4cf21-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4cf21-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





