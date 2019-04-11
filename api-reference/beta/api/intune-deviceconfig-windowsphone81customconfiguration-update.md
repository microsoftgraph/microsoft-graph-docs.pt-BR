---
title: Atualizar windowsPhone81CustomConfiguration
description: Atualizar as propriedades de um objeto windowsPhone81CustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 573bfdd8533399391b51de606afadeef151c269d
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31806927"
---
# <a name="update-windowsphone81customconfiguration"></a><span data-ttu-id="38944-103">Atualizar windowsPhone81CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="38944-103">Update windowsPhone81CustomConfiguration</span></span>

> <span data-ttu-id="38944-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="38944-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38944-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="38944-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38944-106">Atualizar as propriedades de um objeto [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38944-106">Update the properties of a [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38944-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="38944-107">Prerequisites</span></span>
<span data-ttu-id="38944-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38944-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38944-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="38944-110">Permission type</span></span>|<span data-ttu-id="38944-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="38944-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38944-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="38944-112">Delegated (work or school account)</span></span>|<span data-ttu-id="38944-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38944-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="38944-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="38944-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38944-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38944-115">Not supported.</span></span>|
|<span data-ttu-id="38944-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="38944-116">Application</span></span>|<span data-ttu-id="38944-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="38944-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="38944-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="38944-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="38944-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="38944-119">Request headers</span></span>
|<span data-ttu-id="38944-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="38944-120">Header</span></span>|<span data-ttu-id="38944-121">Valor</span><span class="sxs-lookup"><span data-stu-id="38944-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38944-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="38944-122">Authorization</span></span>|<span data-ttu-id="38944-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="38944-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38944-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="38944-124">Accept</span></span>|<span data-ttu-id="38944-125">application/json</span><span class="sxs-lookup"><span data-stu-id="38944-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38944-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="38944-126">Request body</span></span>
<span data-ttu-id="38944-127">No corpo da solicitação, forneça uma representação JSON do objeto [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38944-127">In the request body, supply a JSON representation for the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

<span data-ttu-id="38944-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="38944-128">The following table shows the properties that are required when you create the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span></span>

|<span data-ttu-id="38944-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="38944-129">Property</span></span>|<span data-ttu-id="38944-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="38944-130">Type</span></span>|<span data-ttu-id="38944-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="38944-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38944-132">id</span><span class="sxs-lookup"><span data-stu-id="38944-132">id</span></span>|<span data-ttu-id="38944-133">String</span><span class="sxs-lookup"><span data-stu-id="38944-133">String</span></span>|<span data-ttu-id="38944-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="38944-134">Key of the entity.</span></span> <span data-ttu-id="38944-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38944-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38944-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="38944-136">lastModifiedDateTime</span></span>|<span data-ttu-id="38944-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38944-137">DateTimeOffset</span></span>|<span data-ttu-id="38944-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="38944-138">DateTime the object was last modified.</span></span> <span data-ttu-id="38944-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38944-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38944-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="38944-140">roleScopeTagIds</span></span>|<span data-ttu-id="38944-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="38944-141">String collection</span></span>|<span data-ttu-id="38944-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="38944-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="38944-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38944-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38944-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="38944-144">supportsScopeTags</span></span>|<span data-ttu-id="38944-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="38944-145">Boolean</span></span>|<span data-ttu-id="38944-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="38944-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="38944-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="38944-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="38944-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="38944-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="38944-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="38944-149">This property is read-only.</span></span> <span data-ttu-id="38944-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38944-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38944-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="38944-151">createdDateTime</span></span>|<span data-ttu-id="38944-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38944-152">DateTimeOffset</span></span>|<span data-ttu-id="38944-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="38944-153">DateTime the object was created.</span></span> <span data-ttu-id="38944-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38944-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38944-155">description</span><span class="sxs-lookup"><span data-stu-id="38944-155">description</span></span>|<span data-ttu-id="38944-156">String</span><span class="sxs-lookup"><span data-stu-id="38944-156">String</span></span>|<span data-ttu-id="38944-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="38944-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="38944-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38944-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38944-159">displayName</span><span class="sxs-lookup"><span data-stu-id="38944-159">displayName</span></span>|<span data-ttu-id="38944-160">String</span><span class="sxs-lookup"><span data-stu-id="38944-160">String</span></span>|<span data-ttu-id="38944-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="38944-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="38944-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38944-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38944-163">versão</span><span class="sxs-lookup"><span data-stu-id="38944-163">version</span></span>|<span data-ttu-id="38944-164">Int32</span><span class="sxs-lookup"><span data-stu-id="38944-164">Int32</span></span>|<span data-ttu-id="38944-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="38944-165">Version of the device configuration.</span></span> <span data-ttu-id="38944-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38944-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38944-167">omaSettings</span><span class="sxs-lookup"><span data-stu-id="38944-167">omaSettings</span></span>|<span data-ttu-id="38944-168">Coleção [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="38944-168">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="38944-169">Configurações OMA.</span><span class="sxs-lookup"><span data-stu-id="38944-169">OMA settings.</span></span> <span data-ttu-id="38944-170">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="38944-170">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="38944-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="38944-171">Response</span></span>
<span data-ttu-id="38944-172">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="38944-172">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38944-173">Exemplo</span><span class="sxs-lookup"><span data-stu-id="38944-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="38944-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38944-174">Request</span></span>
<span data-ttu-id="38944-175">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="38944-175">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="38944-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="38944-176">Response</span></span>
<span data-ttu-id="38944-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="38944-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





