---
title: Criar androidOmaCpConfiguration
description: Criar um novo objeto androidOmaCpConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 577b6beeb141ab84147506c9666ef3bf0353402d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33929711"
---
# <a name="create-androidomacpconfiguration"></a><span data-ttu-id="d6c76-103">Criar androidOmaCpConfiguration</span><span class="sxs-lookup"><span data-stu-id="d6c76-103">Create androidOmaCpConfiguration</span></span>

> <span data-ttu-id="d6c76-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d6c76-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6c76-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d6c76-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6c76-106">Criar um novo objeto [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d6c76-106">Create a new [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6c76-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d6c76-107">Prerequisites</span></span>
<span data-ttu-id="d6c76-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d6c76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6c76-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d6c76-110">Permission type</span></span>|<span data-ttu-id="d6c76-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d6c76-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6c76-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d6c76-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d6c76-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6c76-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d6c76-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d6c76-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6c76-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6c76-115">Not supported.</span></span>|
|<span data-ttu-id="d6c76-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d6c76-116">Application</span></span>|<span data-ttu-id="d6c76-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d6c76-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6c76-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d6c76-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d6c76-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d6c76-119">Request headers</span></span>
|<span data-ttu-id="d6c76-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d6c76-120">Header</span></span>|<span data-ttu-id="d6c76-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d6c76-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6c76-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d6c76-122">Authorization</span></span>|<span data-ttu-id="d6c76-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d6c76-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6c76-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d6c76-124">Accept</span></span>|<span data-ttu-id="d6c76-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d6c76-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6c76-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d6c76-126">Request body</span></span>
<span data-ttu-id="d6c76-127">No corpo da solicitação, forneça uma representação JSON do objeto androidOmaCpConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d6c76-127">In the request body, supply a JSON representation for the androidOmaCpConfiguration object.</span></span>

<span data-ttu-id="d6c76-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidOmaCpConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d6c76-128">The following table shows the properties that are required when you create the androidOmaCpConfiguration.</span></span>

|<span data-ttu-id="d6c76-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d6c76-129">Property</span></span>|<span data-ttu-id="d6c76-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d6c76-130">Type</span></span>|<span data-ttu-id="d6c76-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6c76-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6c76-132">id</span><span class="sxs-lookup"><span data-stu-id="d6c76-132">id</span></span>|<span data-ttu-id="d6c76-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6c76-133">String</span></span>|<span data-ttu-id="d6c76-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d6c76-134">Key of the entity.</span></span> <span data-ttu-id="d6c76-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6c76-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6c76-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d6c76-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d6c76-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6c76-137">DateTimeOffset</span></span>|<span data-ttu-id="d6c76-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d6c76-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d6c76-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6c76-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6c76-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d6c76-140">roleScopeTagIds</span></span>|<span data-ttu-id="d6c76-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d6c76-141">String collection</span></span>|<span data-ttu-id="d6c76-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="d6c76-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d6c76-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6c76-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6c76-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d6c76-144">supportsScopeTags</span></span>|<span data-ttu-id="d6c76-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="d6c76-145">Boolean</span></span>|<span data-ttu-id="d6c76-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="d6c76-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d6c76-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="d6c76-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d6c76-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="d6c76-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d6c76-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d6c76-149">This property is read-only.</span></span> <span data-ttu-id="d6c76-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6c76-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6c76-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d6c76-151">createdDateTime</span></span>|<span data-ttu-id="d6c76-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6c76-152">DateTimeOffset</span></span>|<span data-ttu-id="d6c76-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d6c76-153">DateTime the object was created.</span></span> <span data-ttu-id="d6c76-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6c76-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6c76-155">description</span><span class="sxs-lookup"><span data-stu-id="d6c76-155">description</span></span>|<span data-ttu-id="d6c76-156">String</span><span class="sxs-lookup"><span data-stu-id="d6c76-156">String</span></span>|<span data-ttu-id="d6c76-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6c76-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d6c76-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6c76-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6c76-159">displayName</span><span class="sxs-lookup"><span data-stu-id="d6c76-159">displayName</span></span>|<span data-ttu-id="d6c76-160">String</span><span class="sxs-lookup"><span data-stu-id="d6c76-160">String</span></span>|<span data-ttu-id="d6c76-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6c76-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d6c76-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6c76-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6c76-163">versão</span><span class="sxs-lookup"><span data-stu-id="d6c76-163">version</span></span>|<span data-ttu-id="d6c76-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d6c76-164">Int32</span></span>|<span data-ttu-id="d6c76-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6c76-165">Version of the device configuration.</span></span> <span data-ttu-id="d6c76-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6c76-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6c76-167">configurationXml</span><span class="sxs-lookup"><span data-stu-id="d6c76-167">configurationXml</span></span>|<span data-ttu-id="d6c76-168">Binária</span><span class="sxs-lookup"><span data-stu-id="d6c76-168">Binary</span></span>|<span data-ttu-id="d6c76-169">XML de configuração que será aplicada ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d6c76-169">Configuration XML that will be applied to the device.</span></span> <span data-ttu-id="d6c76-170">Quando ele é lido, ele só fornece uma cadeia de caracteres de espaço reservado, pois os dados originais são criptografados e armazenados.</span><span class="sxs-lookup"><span data-stu-id="d6c76-170">When it is read, it only provides a placeholder string since the original data is encrypted and stored.</span></span>|



## <a name="response"></a><span data-ttu-id="d6c76-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6c76-171">Response</span></span>
<span data-ttu-id="d6c76-172">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d6c76-172">If successful, this method returns a `201 Created` response code and a [androidOmaCpConfiguration](../resources/intune-deviceconfig-androidomacpconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6c76-173">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d6c76-173">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6c76-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d6c76-174">Request</span></span>
<span data-ttu-id="d6c76-175">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6c76-175">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 306

{
  "@odata.type": "#microsoft.graph.androidOmaCpConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "configurationXml": "Y29uZmlndXJhdGlvblhtbA=="
}
```

### <a name="response"></a><span data-ttu-id="d6c76-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="d6c76-176">Response</span></span>
<span data-ttu-id="d6c76-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d6c76-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 478

{
  "@odata.type": "#microsoft.graph.androidOmaCpConfiguration",
  "id": "5f682e4a-2e4a-5f68-4a2e-685f4a2e685f",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "configurationXml": "Y29uZmlndXJhdGlvblhtbA=="
}
```




