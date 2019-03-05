---
title: Criar windows10CustomConfiguration
description: Cria um novo objeto windows10CustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dea947a1e9f4034d51a8a9965cf70e9863ae2e04
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171279"
---
# <a name="create-windows10customconfiguration"></a><span data-ttu-id="a925a-103">Criar windows10CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="a925a-103">Create windows10CustomConfiguration</span></span>

> <span data-ttu-id="a925a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a925a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a925a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a925a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a925a-106">Cria um novo objeto [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a925a-106">Create a new [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a925a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a925a-107">Prerequisites</span></span>
<span data-ttu-id="a925a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a925a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a925a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a925a-110">Permission type</span></span>|<span data-ttu-id="a925a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a925a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a925a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a925a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a925a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a925a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a925a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a925a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a925a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a925a-115">Not supported.</span></span>|
|<span data-ttu-id="a925a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a925a-116">Application</span></span>|<span data-ttu-id="a925a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a925a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a925a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a925a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a925a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a925a-119">Request headers</span></span>
|<span data-ttu-id="a925a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a925a-120">Header</span></span>|<span data-ttu-id="a925a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a925a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a925a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a925a-122">Authorization</span></span>|<span data-ttu-id="a925a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a925a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a925a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a925a-124">Accept</span></span>|<span data-ttu-id="a925a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a925a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a925a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a925a-126">Request body</span></span>
<span data-ttu-id="a925a-127">No corpo da solicitação, forneça uma representação JSON do objeto windows10CustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a925a-127">In the request body, supply a JSON representation for the windows10CustomConfiguration object.</span></span>

<span data-ttu-id="a925a-128">A tabela a seguir mostra as propriedades que são necessárias ao criar windows10CustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a925a-128">The following table shows the properties that are required when you create the windows10CustomConfiguration.</span></span>

|<span data-ttu-id="a925a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a925a-129">Property</span></span>|<span data-ttu-id="a925a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a925a-130">Type</span></span>|<span data-ttu-id="a925a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a925a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a925a-132">id</span><span class="sxs-lookup"><span data-stu-id="a925a-132">id</span></span>|<span data-ttu-id="a925a-133">String</span><span class="sxs-lookup"><span data-stu-id="a925a-133">String</span></span>|<span data-ttu-id="a925a-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a925a-134">Key of the entity.</span></span> <span data-ttu-id="a925a-135">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a925a-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a925a-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a925a-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a925a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a925a-137">DateTimeOffset</span></span>|<span data-ttu-id="a925a-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a925a-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a925a-139">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a925a-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a925a-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a925a-140">roleScopeTagIds</span></span>|<span data-ttu-id="a925a-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a925a-141">String collection</span></span>|<span data-ttu-id="a925a-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="a925a-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a925a-143">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a925a-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a925a-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a925a-144">supportsScopeTags</span></span>|<span data-ttu-id="a925a-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a925a-145">Boolean</span></span>|<span data-ttu-id="a925a-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="a925a-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a925a-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="a925a-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a925a-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="a925a-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a925a-149">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a925a-149">This property is read-only.</span></span> <span data-ttu-id="a925a-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a925a-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a925a-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a925a-151">createdDateTime</span></span>|<span data-ttu-id="a925a-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a925a-152">DateTimeOffset</span></span>|<span data-ttu-id="a925a-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a925a-153">DateTime the object was created.</span></span> <span data-ttu-id="a925a-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a925a-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a925a-155">description</span><span class="sxs-lookup"><span data-stu-id="a925a-155">description</span></span>|<span data-ttu-id="a925a-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a925a-156">String</span></span>|<span data-ttu-id="a925a-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a925a-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a925a-158">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a925a-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a925a-159">displayName</span><span class="sxs-lookup"><span data-stu-id="a925a-159">displayName</span></span>|<span data-ttu-id="a925a-160">String</span><span class="sxs-lookup"><span data-stu-id="a925a-160">String</span></span>|<span data-ttu-id="a925a-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a925a-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a925a-162">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a925a-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a925a-163">version</span><span class="sxs-lookup"><span data-stu-id="a925a-163">version</span></span>|<span data-ttu-id="a925a-164">Int32</span><span class="sxs-lookup"><span data-stu-id="a925a-164">Int32</span></span>|<span data-ttu-id="a925a-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a925a-165">Version of the device configuration.</span></span> <span data-ttu-id="a925a-166">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a925a-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a925a-167">omaSettings</span><span class="sxs-lookup"><span data-stu-id="a925a-167">omaSettings</span></span>|<span data-ttu-id="a925a-168">Coleção [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a925a-168">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="a925a-169">Configurações OMA.</span><span class="sxs-lookup"><span data-stu-id="a925a-169">OMA settings.</span></span> <span data-ttu-id="a925a-170">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="a925a-170">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="a925a-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="a925a-171">Response</span></span>
<span data-ttu-id="a925a-172">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a925a-172">If successful, this method returns a `201 Created` response code and a [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a925a-173">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a925a-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="a925a-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a925a-174">Request</span></span>
<span data-ttu-id="a925a-175">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a925a-175">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 496

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="a925a-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="a925a-176">Response</span></span>
<span data-ttu-id="a925a-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a925a-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 668

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
  "id": "d8ae266e-266e-d8ae-6e26-aed86e26aed8",
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




