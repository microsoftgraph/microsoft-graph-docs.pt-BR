---
title: Criar unsupportedDeviceConfiguration
description: Crie um novo objeto de unsupportedDeviceConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 098cd2b0cb5f318dba41a1268ebb8e56b752defc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408898"
---
# <a name="create-unsupporteddeviceconfiguration"></a><span data-ttu-id="56907-103">Criar unsupportedDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="56907-103">Create unsupportedDeviceConfiguration</span></span>

> <span data-ttu-id="56907-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="56907-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="56907-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="56907-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="56907-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="56907-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56907-107">Crie um novo objeto de [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="56907-107">Create a new [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="56907-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="56907-108">Prerequisites</span></span>
<span data-ttu-id="56907-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="56907-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="56907-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56907-111">Permission type</span></span>|<span data-ttu-id="56907-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="56907-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56907-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56907-113">Delegated (work or school account)</span></span>|<span data-ttu-id="56907-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56907-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="56907-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56907-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56907-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56907-116">Not supported.</span></span>|
|<span data-ttu-id="56907-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56907-117">Application</span></span>|<span data-ttu-id="56907-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56907-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56907-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56907-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="56907-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56907-120">Request headers</span></span>
|<span data-ttu-id="56907-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="56907-121">Header</span></span>|<span data-ttu-id="56907-122">Valor</span><span class="sxs-lookup"><span data-stu-id="56907-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56907-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="56907-123">Authorization</span></span>|<span data-ttu-id="56907-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56907-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56907-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="56907-125">Accept</span></span>|<span data-ttu-id="56907-126">application/json</span><span class="sxs-lookup"><span data-stu-id="56907-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56907-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56907-127">Request body</span></span>
<span data-ttu-id="56907-128">No corpo da solicitação, fornece uma representação JSON para o objeto unsupportedDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="56907-128">In the request body, supply a JSON representation for the unsupportedDeviceConfiguration object.</span></span>

<span data-ttu-id="56907-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o unsupportedDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="56907-129">The following table shows the properties that are required when you create the unsupportedDeviceConfiguration.</span></span>

|<span data-ttu-id="56907-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="56907-130">Property</span></span>|<span data-ttu-id="56907-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="56907-131">Type</span></span>|<span data-ttu-id="56907-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="56907-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56907-133">id</span><span class="sxs-lookup"><span data-stu-id="56907-133">id</span></span>|<span data-ttu-id="56907-134">String</span><span class="sxs-lookup"><span data-stu-id="56907-134">String</span></span>|<span data-ttu-id="56907-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="56907-135">Key of the entity.</span></span> <span data-ttu-id="56907-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56907-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56907-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="56907-137">lastModifiedDateTime</span></span>|<span data-ttu-id="56907-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56907-138">DateTimeOffset</span></span>|<span data-ttu-id="56907-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="56907-139">DateTime the object was last modified.</span></span> <span data-ttu-id="56907-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56907-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56907-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="56907-141">roleScopeTagIds</span></span>|<span data-ttu-id="56907-142">String collection</span><span class="sxs-lookup"><span data-stu-id="56907-142">String collection</span></span>|<span data-ttu-id="56907-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="56907-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="56907-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56907-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56907-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="56907-145">supportsScopeTags</span></span>|<span data-ttu-id="56907-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="56907-146">Boolean</span></span>|<span data-ttu-id="56907-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="56907-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="56907-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="56907-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="56907-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="56907-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="56907-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="56907-150">This property is read-only.</span></span> <span data-ttu-id="56907-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56907-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56907-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="56907-152">createdDateTime</span></span>|<span data-ttu-id="56907-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56907-153">DateTimeOffset</span></span>|<span data-ttu-id="56907-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="56907-154">DateTime the object was created.</span></span> <span data-ttu-id="56907-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56907-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56907-156">description</span><span class="sxs-lookup"><span data-stu-id="56907-156">description</span></span>|<span data-ttu-id="56907-157">String</span><span class="sxs-lookup"><span data-stu-id="56907-157">String</span></span>|<span data-ttu-id="56907-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="56907-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="56907-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56907-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56907-160">displayName</span><span class="sxs-lookup"><span data-stu-id="56907-160">displayName</span></span>|<span data-ttu-id="56907-161">String</span><span class="sxs-lookup"><span data-stu-id="56907-161">String</span></span>|<span data-ttu-id="56907-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="56907-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="56907-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56907-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56907-164">version</span><span class="sxs-lookup"><span data-stu-id="56907-164">version</span></span>|<span data-ttu-id="56907-165">Int32</span><span class="sxs-lookup"><span data-stu-id="56907-165">Int32</span></span>|<span data-ttu-id="56907-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="56907-166">Version of the device configuration.</span></span> <span data-ttu-id="56907-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="56907-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="56907-168">originalEntityTypeName</span><span class="sxs-lookup"><span data-stu-id="56907-168">originalEntityTypeName</span></span>|<span data-ttu-id="56907-169">String</span><span class="sxs-lookup"><span data-stu-id="56907-169">String</span></span>|<span data-ttu-id="56907-170">O tipo de entidade que será retornado caso contrário.</span><span class="sxs-lookup"><span data-stu-id="56907-170">The type of entity that would be returned otherwise.</span></span>|
|<span data-ttu-id="56907-171">detalhes</span><span class="sxs-lookup"><span data-stu-id="56907-171">details</span></span>|<span data-ttu-id="56907-172">coleção [unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md)</span><span class="sxs-lookup"><span data-stu-id="56907-172">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md) collection</span></span>|<span data-ttu-id="56907-173">Detalhes descrevendo por que não há suporte para a entidade.</span><span class="sxs-lookup"><span data-stu-id="56907-173">Details describing why the entity is unsupported.</span></span> <span data-ttu-id="56907-174">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="56907-174">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="56907-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="56907-175">Response</span></span>
<span data-ttu-id="56907-176">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56907-176">If successful, this method returns a `201 Created` response code and a [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56907-177">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56907-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="56907-178">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56907-178">Request</span></span>
<span data-ttu-id="56907-179">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="56907-179">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="56907-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="56907-180">Response</span></span>
<span data-ttu-id="56907-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="56907-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




