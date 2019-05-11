---
title: Criar androidWorkProfileCustomConfiguration
description: Criar um novo objeto androidWorkProfileCustomConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 73bca18f8a8d91f3dd0f78827deab25abae5c5c2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33928635"
---
# <a name="create-androidworkprofilecustomconfiguration"></a><span data-ttu-id="dfbed-103">Criar androidWorkProfileCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="dfbed-103">Create androidWorkProfileCustomConfiguration</span></span>

> <span data-ttu-id="dfbed-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dfbed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dfbed-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dfbed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dfbed-106">Criar um novo objeto [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="dfbed-106">Create a new [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dfbed-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dfbed-107">Prerequisites</span></span>
<span data-ttu-id="dfbed-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfbed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfbed-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dfbed-110">Permission type</span></span>|<span data-ttu-id="dfbed-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dfbed-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dfbed-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dfbed-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dfbed-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfbed-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dfbed-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dfbed-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dfbed-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dfbed-115">Not supported.</span></span>|
|<span data-ttu-id="dfbed-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dfbed-116">Application</span></span>|<span data-ttu-id="dfbed-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dfbed-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dfbed-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dfbed-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="dfbed-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dfbed-119">Request headers</span></span>
|<span data-ttu-id="dfbed-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dfbed-120">Header</span></span>|<span data-ttu-id="dfbed-121">Valor</span><span class="sxs-lookup"><span data-stu-id="dfbed-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dfbed-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="dfbed-122">Authorization</span></span>|<span data-ttu-id="dfbed-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dfbed-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dfbed-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dfbed-124">Accept</span></span>|<span data-ttu-id="dfbed-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dfbed-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dfbed-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dfbed-126">Request body</span></span>
<span data-ttu-id="dfbed-127">No corpo da solicitação, forneça uma representação JSON do objeto androidWorkProfileCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="dfbed-127">In the request body, supply a JSON representation for the androidWorkProfileCustomConfiguration object.</span></span>

<span data-ttu-id="dfbed-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidWorkProfileCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="dfbed-128">The following table shows the properties that are required when you create the androidWorkProfileCustomConfiguration.</span></span>

|<span data-ttu-id="dfbed-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dfbed-129">Property</span></span>|<span data-ttu-id="dfbed-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="dfbed-130">Type</span></span>|<span data-ttu-id="dfbed-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="dfbed-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfbed-132">id</span><span class="sxs-lookup"><span data-stu-id="dfbed-132">id</span></span>|<span data-ttu-id="dfbed-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dfbed-133">String</span></span>|<span data-ttu-id="dfbed-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="dfbed-134">Key of the entity.</span></span> <span data-ttu-id="dfbed-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfbed-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfbed-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dfbed-136">lastModifiedDateTime</span></span>|<span data-ttu-id="dfbed-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dfbed-137">DateTimeOffset</span></span>|<span data-ttu-id="dfbed-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="dfbed-138">DateTime the object was last modified.</span></span> <span data-ttu-id="dfbed-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfbed-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfbed-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="dfbed-140">roleScopeTagIds</span></span>|<span data-ttu-id="dfbed-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="dfbed-141">String collection</span></span>|<span data-ttu-id="dfbed-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="dfbed-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="dfbed-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfbed-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfbed-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="dfbed-144">supportsScopeTags</span></span>|<span data-ttu-id="dfbed-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="dfbed-145">Boolean</span></span>|<span data-ttu-id="dfbed-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="dfbed-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="dfbed-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="dfbed-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="dfbed-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="dfbed-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="dfbed-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dfbed-149">This property is read-only.</span></span> <span data-ttu-id="dfbed-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfbed-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfbed-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dfbed-151">createdDateTime</span></span>|<span data-ttu-id="dfbed-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dfbed-152">DateTimeOffset</span></span>|<span data-ttu-id="dfbed-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="dfbed-153">DateTime the object was created.</span></span> <span data-ttu-id="dfbed-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfbed-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfbed-155">description</span><span class="sxs-lookup"><span data-stu-id="dfbed-155">description</span></span>|<span data-ttu-id="dfbed-156">String</span><span class="sxs-lookup"><span data-stu-id="dfbed-156">String</span></span>|<span data-ttu-id="dfbed-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dfbed-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="dfbed-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfbed-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfbed-159">displayName</span><span class="sxs-lookup"><span data-stu-id="dfbed-159">displayName</span></span>|<span data-ttu-id="dfbed-160">String</span><span class="sxs-lookup"><span data-stu-id="dfbed-160">String</span></span>|<span data-ttu-id="dfbed-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dfbed-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="dfbed-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfbed-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfbed-163">versão</span><span class="sxs-lookup"><span data-stu-id="dfbed-163">version</span></span>|<span data-ttu-id="dfbed-164">Int32</span><span class="sxs-lookup"><span data-stu-id="dfbed-164">Int32</span></span>|<span data-ttu-id="dfbed-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dfbed-165">Version of the device configuration.</span></span> <span data-ttu-id="dfbed-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfbed-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfbed-167">omaSettings</span><span class="sxs-lookup"><span data-stu-id="dfbed-167">omaSettings</span></span>|<span data-ttu-id="dfbed-168">Coleção [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="dfbed-168">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="dfbed-169">Configurações OMA.</span><span class="sxs-lookup"><span data-stu-id="dfbed-169">OMA settings.</span></span> <span data-ttu-id="dfbed-170">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="dfbed-170">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="dfbed-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfbed-171">Response</span></span>
<span data-ttu-id="dfbed-172">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dfbed-172">If successful, this method returns a `201 Created` response code and a [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfbed-173">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dfbed-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="dfbed-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dfbed-174">Request</span></span>
<span data-ttu-id="dfbed-175">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dfbed-175">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 505

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="dfbed-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfbed-176">Response</span></span>
<span data-ttu-id="dfbed-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dfbed-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 677

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "id": "76c5d59b-d59b-76c5-9bd5-c5769bd5c576",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```




