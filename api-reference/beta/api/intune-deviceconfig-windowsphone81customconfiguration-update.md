---
title: Atualizar windowsPhone81CustomConfiguration
description: Atualizar as propriedades de um objeto windowsPhone81CustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 00abfd6ae810e1d9f5e9b2d06128d1f25c444e8b
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30971567"
---
# <a name="update-windowsphone81customconfiguration"></a><span data-ttu-id="e92e7-103">Atualizar windowsPhone81CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="e92e7-103">Update windowsPhone81CustomConfiguration</span></span>

> <span data-ttu-id="e92e7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e92e7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e92e7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e92e7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e92e7-106">Atualizar as propriedades de um objeto [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e92e7-106">Update the properties of a [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e92e7-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e92e7-107">Prerequisites</span></span>
<span data-ttu-id="e92e7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e92e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e92e7-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e92e7-110">Permission type</span></span>|<span data-ttu-id="e92e7-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e92e7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e92e7-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e92e7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e92e7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e92e7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e92e7-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e92e7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e92e7-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e92e7-115">Not supported.</span></span>|
|<span data-ttu-id="e92e7-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e92e7-116">Application</span></span>|<span data-ttu-id="e92e7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e92e7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e92e7-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e92e7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e92e7-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e92e7-119">Request headers</span></span>
|<span data-ttu-id="e92e7-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e92e7-120">Header</span></span>|<span data-ttu-id="e92e7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e92e7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e92e7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e92e7-122">Authorization</span></span>|<span data-ttu-id="e92e7-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e92e7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e92e7-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e92e7-124">Accept</span></span>|<span data-ttu-id="e92e7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e92e7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e92e7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e92e7-126">Request body</span></span>
<span data-ttu-id="e92e7-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e92e7-127">In the request body, supply a JSON representation for the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

<span data-ttu-id="e92e7-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e92e7-128">The following table shows the properties that are required when you create the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span></span>

|<span data-ttu-id="e92e7-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e92e7-129">Property</span></span>|<span data-ttu-id="e92e7-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e92e7-130">Type</span></span>|<span data-ttu-id="e92e7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e92e7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e92e7-132">id</span><span class="sxs-lookup"><span data-stu-id="e92e7-132">id</span></span>|<span data-ttu-id="e92e7-133">String</span><span class="sxs-lookup"><span data-stu-id="e92e7-133">String</span></span>|<span data-ttu-id="e92e7-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e92e7-134">Key of the entity.</span></span> <span data-ttu-id="e92e7-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e92e7-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e92e7-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e92e7-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e92e7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e92e7-137">DateTimeOffset</span></span>|<span data-ttu-id="e92e7-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="e92e7-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e92e7-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e92e7-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e92e7-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e92e7-140">roleScopeTagIds</span></span>|<span data-ttu-id="e92e7-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="e92e7-141">String collection</span></span>|<span data-ttu-id="e92e7-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="e92e7-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e92e7-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e92e7-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e92e7-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e92e7-144">supportsScopeTags</span></span>|<span data-ttu-id="e92e7-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="e92e7-145">Boolean</span></span>|<span data-ttu-id="e92e7-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="e92e7-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e92e7-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="e92e7-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e92e7-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="e92e7-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e92e7-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e92e7-149">This property is read-only.</span></span> <span data-ttu-id="e92e7-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e92e7-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e92e7-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e92e7-151">createdDateTime</span></span>|<span data-ttu-id="e92e7-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e92e7-152">DateTimeOffset</span></span>|<span data-ttu-id="e92e7-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="e92e7-153">DateTime the object was created.</span></span> <span data-ttu-id="e92e7-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e92e7-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e92e7-155">descrição</span><span class="sxs-lookup"><span data-stu-id="e92e7-155">description</span></span>|<span data-ttu-id="e92e7-156">String</span><span class="sxs-lookup"><span data-stu-id="e92e7-156">String</span></span>|<span data-ttu-id="e92e7-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e92e7-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e92e7-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e92e7-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e92e7-159">displayName</span><span class="sxs-lookup"><span data-stu-id="e92e7-159">displayName</span></span>|<span data-ttu-id="e92e7-160">String</span><span class="sxs-lookup"><span data-stu-id="e92e7-160">String</span></span>|<span data-ttu-id="e92e7-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e92e7-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e92e7-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e92e7-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e92e7-163">versão</span><span class="sxs-lookup"><span data-stu-id="e92e7-163">version</span></span>|<span data-ttu-id="e92e7-164">Int32</span><span class="sxs-lookup"><span data-stu-id="e92e7-164">Int32</span></span>|<span data-ttu-id="e92e7-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e92e7-165">Version of the device configuration.</span></span> <span data-ttu-id="e92e7-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e92e7-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e92e7-167">omaSettings</span><span class="sxs-lookup"><span data-stu-id="e92e7-167">omaSettings</span></span>|<span data-ttu-id="e92e7-168">Coleção [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e92e7-168">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="e92e7-169">Configurações OMA.</span><span class="sxs-lookup"><span data-stu-id="e92e7-169">OMA settings.</span></span> <span data-ttu-id="e92e7-170">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="e92e7-170">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="e92e7-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="e92e7-171">Response</span></span>
<span data-ttu-id="e92e7-172">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e92e7-172">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e92e7-173">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e92e7-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="e92e7-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e92e7-174">Request</span></span>
<span data-ttu-id="e92e7-175">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e92e7-175">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 501

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="e92e7-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="e92e7-176">Response</span></span>
<span data-ttu-id="e92e7-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e92e7-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 673

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
  "id": "0d98693c-693c-0d98-3c69-980d3c69980d",
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




