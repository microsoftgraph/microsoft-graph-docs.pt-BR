---
title: Criar iosDerivedCredentialAuthenticationConfiguration
description: Criar um novo objeto iosDerivedCredentialAuthenticationConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f5b75ffdd5153e03e8c6e5145394dfc10c125f90
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33956869"
---
# <a name="create-iosderivedcredentialauthenticationconfiguration"></a><span data-ttu-id="ef0af-103">Criar iosDerivedCredentialAuthenticationConfiguration</span><span class="sxs-lookup"><span data-stu-id="ef0af-103">Create iosDerivedCredentialAuthenticationConfiguration</span></span>

> <span data-ttu-id="ef0af-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ef0af-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ef0af-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ef0af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef0af-106">Criar um novo objeto [iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ef0af-106">Create a new [iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef0af-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ef0af-107">Prerequisites</span></span>
<span data-ttu-id="ef0af-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef0af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef0af-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef0af-110">Permission type</span></span>|<span data-ttu-id="ef0af-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ef0af-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef0af-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef0af-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ef0af-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef0af-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ef0af-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ef0af-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef0af-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef0af-115">Not supported.</span></span>|
|<span data-ttu-id="ef0af-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ef0af-116">Application</span></span>|<span data-ttu-id="ef0af-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef0af-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef0af-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef0af-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ef0af-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ef0af-119">Request headers</span></span>
|<span data-ttu-id="ef0af-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ef0af-120">Header</span></span>|<span data-ttu-id="ef0af-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ef0af-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef0af-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef0af-122">Authorization</span></span>|<span data-ttu-id="ef0af-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef0af-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef0af-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ef0af-124">Accept</span></span>|<span data-ttu-id="ef0af-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ef0af-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef0af-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ef0af-126">Request body</span></span>
<span data-ttu-id="ef0af-127">No corpo da solicitação, forneça uma representação JSON do objeto iosDerivedCredentialAuthenticationConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ef0af-127">In the request body, supply a JSON representation for the iosDerivedCredentialAuthenticationConfiguration object.</span></span>

<span data-ttu-id="ef0af-128">A tabela a seguir mostra as propriedades que são necessárias ao criar iosDerivedCredentialAuthenticationConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ef0af-128">The following table shows the properties that are required when you create the iosDerivedCredentialAuthenticationConfiguration.</span></span>

|<span data-ttu-id="ef0af-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ef0af-129">Property</span></span>|<span data-ttu-id="ef0af-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ef0af-130">Type</span></span>|<span data-ttu-id="ef0af-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ef0af-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef0af-132">id</span><span class="sxs-lookup"><span data-stu-id="ef0af-132">id</span></span>|<span data-ttu-id="ef0af-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ef0af-133">String</span></span>|<span data-ttu-id="ef0af-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ef0af-134">Key of the entity.</span></span> <span data-ttu-id="ef0af-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef0af-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef0af-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ef0af-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ef0af-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef0af-137">DateTimeOffset</span></span>|<span data-ttu-id="ef0af-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ef0af-138">DateTime the object was last modified.</span></span> <span data-ttu-id="ef0af-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef0af-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef0af-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ef0af-140">roleScopeTagIds</span></span>|<span data-ttu-id="ef0af-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="ef0af-141">String collection</span></span>|<span data-ttu-id="ef0af-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="ef0af-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ef0af-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef0af-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef0af-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ef0af-144">supportsScopeTags</span></span>|<span data-ttu-id="ef0af-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="ef0af-145">Boolean</span></span>|<span data-ttu-id="ef0af-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="ef0af-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ef0af-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="ef0af-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ef0af-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="ef0af-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ef0af-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ef0af-149">This property is read-only.</span></span> <span data-ttu-id="ef0af-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef0af-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef0af-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ef0af-151">createdDateTime</span></span>|<span data-ttu-id="ef0af-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef0af-152">DateTimeOffset</span></span>|<span data-ttu-id="ef0af-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ef0af-153">DateTime the object was created.</span></span> <span data-ttu-id="ef0af-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef0af-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef0af-155">description</span><span class="sxs-lookup"><span data-stu-id="ef0af-155">description</span></span>|<span data-ttu-id="ef0af-156">String</span><span class="sxs-lookup"><span data-stu-id="ef0af-156">String</span></span>|<span data-ttu-id="ef0af-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ef0af-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ef0af-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef0af-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef0af-159">displayName</span><span class="sxs-lookup"><span data-stu-id="ef0af-159">displayName</span></span>|<span data-ttu-id="ef0af-160">String</span><span class="sxs-lookup"><span data-stu-id="ef0af-160">String</span></span>|<span data-ttu-id="ef0af-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ef0af-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ef0af-162">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef0af-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef0af-163">versão</span><span class="sxs-lookup"><span data-stu-id="ef0af-163">version</span></span>|<span data-ttu-id="ef0af-164">Int32</span><span class="sxs-lookup"><span data-stu-id="ef0af-164">Int32</span></span>|<span data-ttu-id="ef0af-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ef0af-165">Version of the device configuration.</span></span> <span data-ttu-id="ef0af-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef0af-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ef0af-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef0af-167">Response</span></span>
<span data-ttu-id="ef0af-168">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef0af-168">If successful, this method returns a `201 Created` response code and a [iosDerivedCredentialAuthenticationConfiguration](../resources/intune-deviceconfig-iosderivedcredentialauthenticationconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef0af-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ef0af-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef0af-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef0af-170">Request</span></span>
<span data-ttu-id="ef0af-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef0af-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 277

{
  "@odata.type": "#microsoft.graph.iosDerivedCredentialAuthenticationConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="ef0af-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef0af-172">Response</span></span>
<span data-ttu-id="ef0af-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ef0af-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 449

{
  "@odata.type": "#microsoft.graph.iosDerivedCredentialAuthenticationConfiguration",
  "id": "01713f58-3f58-0171-583f-7101583f7101",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```




