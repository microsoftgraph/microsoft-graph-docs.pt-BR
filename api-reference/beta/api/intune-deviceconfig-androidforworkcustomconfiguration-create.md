---
title: Criar androidForWorkCustomConfiguration
description: Criar um novo objeto androidForWorkCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aee4817159ad94e301141f07cb027ac7887f9e7b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32479376"
---
# <a name="create-androidforworkcustomconfiguration"></a><span data-ttu-id="c48f4-103">Criar androidForWorkCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="c48f4-103">Create androidForWorkCustomConfiguration</span></span>

> <span data-ttu-id="c48f4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c48f4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c48f4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c48f4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c48f4-106">Criar um novo objeto [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c48f4-106">Create a new [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c48f4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c48f4-107">Prerequisites</span></span>
<span data-ttu-id="c48f4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c48f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c48f4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c48f4-110">Permission type</span></span>|<span data-ttu-id="c48f4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c48f4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c48f4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c48f4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c48f4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c48f4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c48f4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c48f4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c48f4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c48f4-115">Not supported.</span></span>|
|<span data-ttu-id="c48f4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c48f4-116">Application</span></span>|<span data-ttu-id="c48f4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c48f4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c48f4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c48f4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c48f4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c48f4-119">Request headers</span></span>
|<span data-ttu-id="c48f4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c48f4-120">Header</span></span>|<span data-ttu-id="c48f4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="c48f4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c48f4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="c48f4-122">Authorization</span></span>|<span data-ttu-id="c48f4-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c48f4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c48f4-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c48f4-124">Accept</span></span>|<span data-ttu-id="c48f4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c48f4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c48f4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c48f4-126">Request body</span></span>
<span data-ttu-id="c48f4-127">No corpo da solicitação, forneça uma representação JSON do objeto androidForWorkCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c48f4-127">In the request body, supply a JSON representation for the androidForWorkCustomConfiguration object.</span></span>

<span data-ttu-id="c48f4-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidForWorkCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="c48f4-128">The following table shows the properties that are required when you create the androidForWorkCustomConfiguration.</span></span>

|<span data-ttu-id="c48f4-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c48f4-129">Property</span></span>|<span data-ttu-id="c48f4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c48f4-130">Type</span></span>|<span data-ttu-id="c48f4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c48f4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c48f4-132">id</span><span class="sxs-lookup"><span data-stu-id="c48f4-132">id</span></span>|<span data-ttu-id="c48f4-133">String</span><span class="sxs-lookup"><span data-stu-id="c48f4-133">String</span></span>|<span data-ttu-id="c48f4-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c48f4-134">Key of the entity.</span></span> <span data-ttu-id="c48f4-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c48f4-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c48f4-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c48f4-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c48f4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c48f4-137">DateTimeOffset</span></span>|<span data-ttu-id="c48f4-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="c48f4-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c48f4-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c48f4-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c48f4-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c48f4-140">roleScopeTagIds</span></span>|<span data-ttu-id="c48f4-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c48f4-141">String collection</span></span>|<span data-ttu-id="c48f4-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="c48f4-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c48f4-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c48f4-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c48f4-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c48f4-144">supportsScopeTags</span></span>|<span data-ttu-id="c48f4-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="c48f4-145">Boolean</span></span>|<span data-ttu-id="c48f4-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="c48f4-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c48f4-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="c48f4-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c48f4-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="c48f4-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c48f4-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c48f4-149">This property is read-only.</span></span> <span data-ttu-id="c48f4-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c48f4-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c48f4-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c48f4-151">createdDateTime</span></span>|<span data-ttu-id="c48f4-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c48f4-152">DateTimeOffset</span></span>|<span data-ttu-id="c48f4-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="c48f4-153">DateTime the object was created.</span></span> <span data-ttu-id="c48f4-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c48f4-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c48f4-155">description</span><span class="sxs-lookup"><span data-stu-id="c48f4-155">description</span></span>|<span data-ttu-id="c48f4-156">String</span><span class="sxs-lookup"><span data-stu-id="c48f4-156">String</span></span>|<span data-ttu-id="c48f4-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c48f4-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c48f4-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c48f4-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c48f4-159">displayName</span><span class="sxs-lookup"><span data-stu-id="c48f4-159">displayName</span></span>|<span data-ttu-id="c48f4-160">String</span><span class="sxs-lookup"><span data-stu-id="c48f4-160">String</span></span>|<span data-ttu-id="c48f4-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c48f4-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c48f4-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c48f4-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c48f4-163">versão</span><span class="sxs-lookup"><span data-stu-id="c48f4-163">version</span></span>|<span data-ttu-id="c48f4-164">Int32</span><span class="sxs-lookup"><span data-stu-id="c48f4-164">Int32</span></span>|<span data-ttu-id="c48f4-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c48f4-165">Version of the device configuration.</span></span> <span data-ttu-id="c48f4-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c48f4-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c48f4-167">omaSettings</span><span class="sxs-lookup"><span data-stu-id="c48f4-167">omaSettings</span></span>|<span data-ttu-id="c48f4-168">Coleção [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c48f4-168">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="c48f4-169">Configurações OMA.</span><span class="sxs-lookup"><span data-stu-id="c48f4-169">OMA settings.</span></span> <span data-ttu-id="c48f4-170">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="c48f4-170">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="c48f4-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="c48f4-171">Response</span></span>
<span data-ttu-id="c48f4-172">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c48f4-172">If successful, this method returns a `201 Created` response code and a [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c48f4-173">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c48f4-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="c48f4-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c48f4-174">Request</span></span>
<span data-ttu-id="c48f4-175">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c48f4-175">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 501

{
  "@odata.type": "#microsoft.graph.androidForWorkCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="c48f4-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="c48f4-176">Response</span></span>
<span data-ttu-id="c48f4-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c48f4-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 673

{
  "@odata.type": "#microsoft.graph.androidForWorkCustomConfiguration",
  "id": "cca8b2bb-b2bb-cca8-bbb2-a8ccbbb2a8cc",
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





