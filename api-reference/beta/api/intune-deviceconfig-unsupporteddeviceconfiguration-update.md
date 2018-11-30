---
title: Atualizar unsupportedDeviceConfiguration
description: Atualize as propriedades de um objeto unsupportedDeviceConfiguration.
ms.openlocfilehash: 0f8594642908aef125556f06fdca911c9530db76
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034880"
---
# <a name="update-unsupporteddeviceconfiguration"></a><span data-ttu-id="a7b11-103">Atualizar unsupportedDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="a7b11-103">Update unsupportedDeviceConfiguration</span></span>

> <span data-ttu-id="a7b11-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a7b11-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a7b11-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a7b11-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a7b11-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a7b11-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a7b11-107">Atualize as propriedades de um objeto [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a7b11-107">Update the properties of a [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a7b11-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a7b11-108">Prerequisites</span></span>
<span data-ttu-id="a7b11-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7b11-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7b11-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a7b11-111">Permission type</span></span>|<span data-ttu-id="a7b11-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a7b11-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7b11-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a7b11-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a7b11-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7b11-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a7b11-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a7b11-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7b11-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7b11-116">Not supported.</span></span>|
|<span data-ttu-id="a7b11-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a7b11-117">Application</span></span>|<span data-ttu-id="a7b11-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7b11-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7b11-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a7b11-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a7b11-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a7b11-120">Request headers</span></span>
|<span data-ttu-id="a7b11-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a7b11-121">Header</span></span>|<span data-ttu-id="a7b11-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a7b11-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7b11-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a7b11-123">Authorization</span></span>|<span data-ttu-id="a7b11-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a7b11-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7b11-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a7b11-125">Accept</span></span>|<span data-ttu-id="a7b11-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a7b11-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7b11-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a7b11-127">Request body</span></span>
<span data-ttu-id="a7b11-128">No corpo da solicitação, fornece uma representação JSON para o objeto [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a7b11-128">In the request body, supply a JSON representation for the [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>

<span data-ttu-id="a7b11-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a7b11-129">The following table shows the properties that are required when you create the [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md).</span></span>

|<span data-ttu-id="a7b11-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a7b11-130">Property</span></span>|<span data-ttu-id="a7b11-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a7b11-131">Type</span></span>|<span data-ttu-id="a7b11-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7b11-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7b11-133">id</span><span class="sxs-lookup"><span data-stu-id="a7b11-133">id</span></span>|<span data-ttu-id="a7b11-134">String</span><span class="sxs-lookup"><span data-stu-id="a7b11-134">String</span></span>|<span data-ttu-id="a7b11-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a7b11-135">Key of the entity.</span></span> <span data-ttu-id="a7b11-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7b11-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7b11-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a7b11-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a7b11-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7b11-138">DateTimeOffset</span></span>|<span data-ttu-id="a7b11-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a7b11-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a7b11-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7b11-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7b11-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a7b11-141">roleScopeTagIds</span></span>|<span data-ttu-id="a7b11-142">String collection</span><span class="sxs-lookup"><span data-stu-id="a7b11-142">String collection</span></span>|<span data-ttu-id="a7b11-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="a7b11-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a7b11-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7b11-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7b11-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a7b11-145">supportsScopeTags</span></span>|<span data-ttu-id="a7b11-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="a7b11-146">Boolean</span></span>|<span data-ttu-id="a7b11-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="a7b11-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a7b11-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="a7b11-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a7b11-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="a7b11-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a7b11-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a7b11-150">This property is read-only.</span></span> <span data-ttu-id="a7b11-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7b11-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7b11-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a7b11-152">createdDateTime</span></span>|<span data-ttu-id="a7b11-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7b11-153">DateTimeOffset</span></span>|<span data-ttu-id="a7b11-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a7b11-154">DateTime the object was created.</span></span> <span data-ttu-id="a7b11-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7b11-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7b11-156">description</span><span class="sxs-lookup"><span data-stu-id="a7b11-156">description</span></span>|<span data-ttu-id="a7b11-157">String</span><span class="sxs-lookup"><span data-stu-id="a7b11-157">String</span></span>|<span data-ttu-id="a7b11-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a7b11-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a7b11-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7b11-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7b11-160">displayName</span><span class="sxs-lookup"><span data-stu-id="a7b11-160">displayName</span></span>|<span data-ttu-id="a7b11-161">String</span><span class="sxs-lookup"><span data-stu-id="a7b11-161">String</span></span>|<span data-ttu-id="a7b11-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a7b11-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a7b11-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7b11-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7b11-164">version</span><span class="sxs-lookup"><span data-stu-id="a7b11-164">version</span></span>|<span data-ttu-id="a7b11-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a7b11-165">Int32</span></span>|<span data-ttu-id="a7b11-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a7b11-166">Version of the device configuration.</span></span> <span data-ttu-id="a7b11-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a7b11-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a7b11-168">originalEntityTypeName</span><span class="sxs-lookup"><span data-stu-id="a7b11-168">originalEntityTypeName</span></span>|<span data-ttu-id="a7b11-169">String</span><span class="sxs-lookup"><span data-stu-id="a7b11-169">String</span></span>|<span data-ttu-id="a7b11-170">O tipo de entidade que será retornado caso contrário.</span><span class="sxs-lookup"><span data-stu-id="a7b11-170">The type of entity that would be returned otherwise.</span></span>|
|<span data-ttu-id="a7b11-171">detalhes</span><span class="sxs-lookup"><span data-stu-id="a7b11-171">details</span></span>|<span data-ttu-id="a7b11-172">coleção [unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md)</span><span class="sxs-lookup"><span data-stu-id="a7b11-172">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md) collection</span></span>|<span data-ttu-id="a7b11-173">Detalhes descrevendo por que não há suporte para a entidade.</span><span class="sxs-lookup"><span data-stu-id="a7b11-173">Details describing why the entity is unsupported.</span></span> <span data-ttu-id="a7b11-174">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="a7b11-174">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="a7b11-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7b11-175">Response</span></span>
<span data-ttu-id="a7b11-176">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a7b11-176">If successful, this method returns a `200 OK` response code and an updated [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7b11-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a7b11-177">Example</span></span>
### <a name="request"></a><span data-ttu-id="a7b11-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a7b11-178">Request</span></span>
<span data-ttu-id="a7b11-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a7b11-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 513

{
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

### <a name="response"></a><span data-ttu-id="a7b11-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7b11-180">Response</span></span>
<span data-ttu-id="a7b11-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a7b11-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





