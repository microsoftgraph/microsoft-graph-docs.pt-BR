---
title: Criar androidCustomConfiguration
description: Criar um novo objeto androidCustomConfiguration.
author: tfitzmac
ms.openlocfilehash: 1395119e1602ad59a5be2d8f96b37b12bf6e6124
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347821"
---
# <a name="create-androidcustomconfiguration"></a><span data-ttu-id="47168-103">Criar androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="47168-103">Create androidCustomConfiguration</span></span>

> <span data-ttu-id="47168-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="47168-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="47168-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="47168-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="47168-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="47168-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="47168-107">Criar um novo objeto [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="47168-107">Create a new [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="47168-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="47168-108">Prerequisites</span></span>
<span data-ttu-id="47168-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47168-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47168-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47168-111">Permission type</span></span>|<span data-ttu-id="47168-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="47168-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47168-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47168-113">Delegated (work or school account)</span></span>|<span data-ttu-id="47168-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47168-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="47168-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47168-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47168-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47168-116">Not supported.</span></span>|
|<span data-ttu-id="47168-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47168-117">Application</span></span>|<span data-ttu-id="47168-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47168-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="47168-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47168-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="47168-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47168-120">Request headers</span></span>
|<span data-ttu-id="47168-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="47168-121">Header</span></span>|<span data-ttu-id="47168-122">Valor</span><span class="sxs-lookup"><span data-stu-id="47168-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47168-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="47168-123">Authorization</span></span>|<span data-ttu-id="47168-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47168-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47168-125">Accept</span><span class="sxs-lookup"><span data-stu-id="47168-125">Accept</span></span>|<span data-ttu-id="47168-126">application/json</span><span class="sxs-lookup"><span data-stu-id="47168-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47168-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47168-127">Request body</span></span>
<span data-ttu-id="47168-128">No corpo da solicitação, forneça uma representação JSON do objeto androidCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="47168-128">In the request body, supply a JSON representation for the androidCustomConfiguration object.</span></span>

<span data-ttu-id="47168-129">A tabela a seguir mostra as propriedades que são necessárias ao criar androidCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="47168-129">The following table shows the properties that are required when you create the androidCustomConfiguration.</span></span>

|<span data-ttu-id="47168-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="47168-130">Property</span></span>|<span data-ttu-id="47168-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="47168-131">Type</span></span>|<span data-ttu-id="47168-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="47168-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47168-133">id</span><span class="sxs-lookup"><span data-stu-id="47168-133">id</span></span>|<span data-ttu-id="47168-134">String</span><span class="sxs-lookup"><span data-stu-id="47168-134">String</span></span>|<span data-ttu-id="47168-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="47168-135">Key of the entity.</span></span> <span data-ttu-id="47168-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47168-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47168-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="47168-137">lastModifiedDateTime</span></span>|<span data-ttu-id="47168-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47168-138">DateTimeOffset</span></span>|<span data-ttu-id="47168-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="47168-139">DateTime the object was last modified.</span></span> <span data-ttu-id="47168-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47168-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47168-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="47168-141">roleScopeTagIds</span></span>|<span data-ttu-id="47168-142">String collection</span><span class="sxs-lookup"><span data-stu-id="47168-142">String collection</span></span>|<span data-ttu-id="47168-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="47168-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="47168-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47168-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47168-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="47168-145">supportsScopeTags</span></span>|<span data-ttu-id="47168-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="47168-146">Boolean</span></span>|<span data-ttu-id="47168-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="47168-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="47168-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="47168-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="47168-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="47168-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="47168-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="47168-150">This property is read-only.</span></span> <span data-ttu-id="47168-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47168-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47168-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="47168-152">createdDateTime</span></span>|<span data-ttu-id="47168-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47168-153">DateTimeOffset</span></span>|<span data-ttu-id="47168-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="47168-154">DateTime the object was created.</span></span> <span data-ttu-id="47168-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47168-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47168-156">description</span><span class="sxs-lookup"><span data-stu-id="47168-156">description</span></span>|<span data-ttu-id="47168-157">String</span><span class="sxs-lookup"><span data-stu-id="47168-157">String</span></span>|<span data-ttu-id="47168-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="47168-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="47168-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47168-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47168-160">displayName</span><span class="sxs-lookup"><span data-stu-id="47168-160">displayName</span></span>|<span data-ttu-id="47168-161">String</span><span class="sxs-lookup"><span data-stu-id="47168-161">String</span></span>|<span data-ttu-id="47168-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="47168-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="47168-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47168-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47168-164">version</span><span class="sxs-lookup"><span data-stu-id="47168-164">version</span></span>|<span data-ttu-id="47168-165">Int32</span><span class="sxs-lookup"><span data-stu-id="47168-165">Int32</span></span>|<span data-ttu-id="47168-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="47168-166">Version of the device configuration.</span></span> <span data-ttu-id="47168-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="47168-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="47168-168">omaSettings</span><span class="sxs-lookup"><span data-stu-id="47168-168">omaSettings</span></span>|<span data-ttu-id="47168-169">Coleção [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="47168-169">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="47168-170">Configurações OMA.</span><span class="sxs-lookup"><span data-stu-id="47168-170">OMA settings.</span></span> <span data-ttu-id="47168-171">Essa coleção pode conter um máximo de 1.000 elementos.</span><span class="sxs-lookup"><span data-stu-id="47168-171">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="47168-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="47168-172">Response</span></span>
<span data-ttu-id="47168-173">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47168-173">If successful, this method returns a `201 Created` response code and a [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47168-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="47168-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="47168-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47168-175">Request</span></span>
<span data-ttu-id="47168-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="47168-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 558

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="47168-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="47168-177">Response</span></span>
<span data-ttu-id="47168-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="47168-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 666

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
  "id": "619b5e6d-5e6d-619b-6d5e-9b616d5e9b61",
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





