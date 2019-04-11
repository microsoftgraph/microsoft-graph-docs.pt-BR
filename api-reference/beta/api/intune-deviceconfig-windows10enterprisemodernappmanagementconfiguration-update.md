---
title: Atualizar windows10EnterpriseModernAppManagementConfiguration
description: Atualizar as propriedades de um objeto windows10EnterpriseModernAppManagementConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 85d760b4274b2ab8c2a0b93a0c936868c2fbe683
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31790239"
---
# <a name="update-windows10enterprisemodernappmanagementconfiguration"></a><span data-ttu-id="eb6b3-103">Atualizar windows10EnterpriseModernAppManagementConfiguration</span><span class="sxs-lookup"><span data-stu-id="eb6b3-103">Update windows10EnterpriseModernAppManagementConfiguration</span></span>

> <span data-ttu-id="eb6b3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eb6b3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb6b3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eb6b3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb6b3-106">Atualizar as propriedades de um objeto [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eb6b3-106">Update the properties of a [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb6b3-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eb6b3-107">Prerequisites</span></span>
<span data-ttu-id="eb6b3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb6b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb6b3-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb6b3-110">Permission type</span></span>|<span data-ttu-id="eb6b3-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eb6b3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb6b3-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb6b3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eb6b3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb6b3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="eb6b3-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb6b3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb6b3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb6b3-115">Not supported.</span></span>|
|<span data-ttu-id="eb6b3-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb6b3-116">Application</span></span>|<span data-ttu-id="eb6b3-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb6b3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb6b3-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb6b3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="eb6b3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb6b3-119">Request headers</span></span>
|<span data-ttu-id="eb6b3-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eb6b3-120">Header</span></span>|<span data-ttu-id="eb6b3-121">Valor</span><span class="sxs-lookup"><span data-stu-id="eb6b3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb6b3-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb6b3-122">Authorization</span></span>|<span data-ttu-id="eb6b3-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb6b3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb6b3-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="eb6b3-124">Accept</span></span>|<span data-ttu-id="eb6b3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eb6b3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb6b3-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb6b3-126">Request body</span></span>
<span data-ttu-id="eb6b3-127">No corpo da solicitação, forneça uma representação JSON do objeto [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eb6b3-127">In the request body, supply a JSON representation for the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

<span data-ttu-id="eb6b3-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="eb6b3-128">The following table shows the properties that are required when you create the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span></span>

|<span data-ttu-id="eb6b3-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb6b3-129">Property</span></span>|<span data-ttu-id="eb6b3-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb6b3-130">Type</span></span>|<span data-ttu-id="eb6b3-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb6b3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb6b3-132">id</span><span class="sxs-lookup"><span data-stu-id="eb6b3-132">id</span></span>|<span data-ttu-id="eb6b3-133">String</span><span class="sxs-lookup"><span data-stu-id="eb6b3-133">String</span></span>|<span data-ttu-id="eb6b3-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="eb6b3-134">Key of the entity.</span></span> <span data-ttu-id="eb6b3-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eb6b3-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eb6b3-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eb6b3-136">lastModifiedDateTime</span></span>|<span data-ttu-id="eb6b3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb6b3-137">DateTimeOffset</span></span>|<span data-ttu-id="eb6b3-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="eb6b3-138">DateTime the object was last modified.</span></span> <span data-ttu-id="eb6b3-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eb6b3-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eb6b3-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="eb6b3-140">roleScopeTagIds</span></span>|<span data-ttu-id="eb6b3-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="eb6b3-141">String collection</span></span>|<span data-ttu-id="eb6b3-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="eb6b3-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="eb6b3-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eb6b3-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eb6b3-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="eb6b3-144">supportsScopeTags</span></span>|<span data-ttu-id="eb6b3-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb6b3-145">Boolean</span></span>|<span data-ttu-id="eb6b3-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="eb6b3-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="eb6b3-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="eb6b3-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="eb6b3-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="eb6b3-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="eb6b3-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eb6b3-149">This property is read-only.</span></span> <span data-ttu-id="eb6b3-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eb6b3-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eb6b3-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eb6b3-151">createdDateTime</span></span>|<span data-ttu-id="eb6b3-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb6b3-152">DateTimeOffset</span></span>|<span data-ttu-id="eb6b3-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="eb6b3-153">DateTime the object was created.</span></span> <span data-ttu-id="eb6b3-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eb6b3-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eb6b3-155">description</span><span class="sxs-lookup"><span data-stu-id="eb6b3-155">description</span></span>|<span data-ttu-id="eb6b3-156">String</span><span class="sxs-lookup"><span data-stu-id="eb6b3-156">String</span></span>|<span data-ttu-id="eb6b3-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="eb6b3-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="eb6b3-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eb6b3-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eb6b3-159">displayName</span><span class="sxs-lookup"><span data-stu-id="eb6b3-159">displayName</span></span>|<span data-ttu-id="eb6b3-160">String</span><span class="sxs-lookup"><span data-stu-id="eb6b3-160">String</span></span>|<span data-ttu-id="eb6b3-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="eb6b3-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="eb6b3-162">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eb6b3-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eb6b3-163">versão</span><span class="sxs-lookup"><span data-stu-id="eb6b3-163">version</span></span>|<span data-ttu-id="eb6b3-164">Int32</span><span class="sxs-lookup"><span data-stu-id="eb6b3-164">Int32</span></span>|<span data-ttu-id="eb6b3-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="eb6b3-165">Version of the device configuration.</span></span> <span data-ttu-id="eb6b3-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eb6b3-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eb6b3-167">uninstallBuiltInApps</span><span class="sxs-lookup"><span data-stu-id="eb6b3-167">uninstallBuiltInApps</span></span>|<span data-ttu-id="eb6b3-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb6b3-168">Boolean</span></span>|<span data-ttu-id="eb6b3-169">Indica se deseja ou não desinstalar uma lista fixa de aplicativos internos do Windows.</span><span class="sxs-lookup"><span data-stu-id="eb6b3-169">Indicates whether or not to uninstall a fixed list of built-in Windows apps.</span></span>|



## <a name="response"></a><span data-ttu-id="eb6b3-170">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb6b3-170">Response</span></span>
<span data-ttu-id="eb6b3-171">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb6b3-171">If successful, this method returns a `200 OK` response code and an updated [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb6b3-172">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eb6b3-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb6b3-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb6b3-173">Request</span></span>
<span data-ttu-id="eb6b3-174">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb6b3-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 314

{
  "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "uninstallBuiltInApps": true
}
```

### <a name="response"></a><span data-ttu-id="eb6b3-175">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb6b3-175">Response</span></span>
<span data-ttu-id="eb6b3-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eb6b3-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 486

{
  "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
  "id": "d6577687-7687-d657-8776-57d6877657d6",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "uninstallBuiltInApps": true
}
```





