---
title: Criar androidForWorkCustomConfiguration
description: Crie um novo objeto de androidForWorkCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9f1563573503ede9f49bb8a758220fcf9cd324fb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832604"
---
# <a name="create-androidforworkcustomconfiguration"></a><span data-ttu-id="d221a-103">Criar androidForWorkCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="d221a-103">Create androidForWorkCustomConfiguration</span></span>

> <span data-ttu-id="d221a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d221a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d221a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d221a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d221a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d221a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d221a-107">Crie um novo objeto de [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d221a-107">Create a new [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d221a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d221a-108">Prerequisites</span></span>
<span data-ttu-id="d221a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d221a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d221a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d221a-111">Permission type</span></span>|<span data-ttu-id="d221a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d221a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d221a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d221a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d221a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d221a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d221a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d221a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d221a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d221a-116">Not supported.</span></span>|
|<span data-ttu-id="d221a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d221a-117">Application</span></span>|<span data-ttu-id="d221a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d221a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d221a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d221a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d221a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d221a-120">Request headers</span></span>
|<span data-ttu-id="d221a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d221a-121">Header</span></span>|<span data-ttu-id="d221a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d221a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d221a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d221a-123">Authorization</span></span>|<span data-ttu-id="d221a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d221a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d221a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d221a-125">Accept</span></span>|<span data-ttu-id="d221a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d221a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d221a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d221a-127">Request body</span></span>
<span data-ttu-id="d221a-128">No corpo da solicitação, fornece uma representação JSON para o objeto androidForWorkCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d221a-128">In the request body, supply a JSON representation for the androidForWorkCustomConfiguration object.</span></span>

<span data-ttu-id="d221a-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o androidForWorkCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="d221a-129">The following table shows the properties that are required when you create the androidForWorkCustomConfiguration.</span></span>

|<span data-ttu-id="d221a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d221a-130">Property</span></span>|<span data-ttu-id="d221a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d221a-131">Type</span></span>|<span data-ttu-id="d221a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d221a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d221a-133">id</span><span class="sxs-lookup"><span data-stu-id="d221a-133">id</span></span>|<span data-ttu-id="d221a-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d221a-134">String</span></span>|<span data-ttu-id="d221a-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="d221a-135">Key of the entity.</span></span> <span data-ttu-id="d221a-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d221a-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d221a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d221a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d221a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d221a-138">DateTimeOffset</span></span>|<span data-ttu-id="d221a-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="d221a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d221a-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d221a-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d221a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d221a-141">roleScopeTagIds</span></span>|<span data-ttu-id="d221a-142">String collection</span><span class="sxs-lookup"><span data-stu-id="d221a-142">String collection</span></span>|<span data-ttu-id="d221a-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="d221a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d221a-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d221a-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d221a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d221a-145">supportsScopeTags</span></span>|<span data-ttu-id="d221a-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="d221a-146">Boolean</span></span>|<span data-ttu-id="d221a-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="d221a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d221a-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="d221a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d221a-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="d221a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d221a-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d221a-150">This property is read-only.</span></span> <span data-ttu-id="d221a-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d221a-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d221a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d221a-152">createdDateTime</span></span>|<span data-ttu-id="d221a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d221a-153">DateTimeOffset</span></span>|<span data-ttu-id="d221a-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="d221a-154">DateTime the object was created.</span></span> <span data-ttu-id="d221a-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d221a-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d221a-156">description</span><span class="sxs-lookup"><span data-stu-id="d221a-156">description</span></span>|<span data-ttu-id="d221a-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d221a-157">String</span></span>|<span data-ttu-id="d221a-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d221a-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d221a-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d221a-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d221a-160">displayName</span><span class="sxs-lookup"><span data-stu-id="d221a-160">displayName</span></span>|<span data-ttu-id="d221a-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d221a-161">String</span></span>|<span data-ttu-id="d221a-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d221a-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d221a-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d221a-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d221a-164">version</span><span class="sxs-lookup"><span data-stu-id="d221a-164">version</span></span>|<span data-ttu-id="d221a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="d221a-165">Int32</span></span>|<span data-ttu-id="d221a-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d221a-166">Version of the device configuration.</span></span> <span data-ttu-id="d221a-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d221a-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d221a-168">omaSettings</span><span class="sxs-lookup"><span data-stu-id="d221a-168">omaSettings</span></span>|<span data-ttu-id="d221a-169">Coleção [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d221a-169">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="d221a-170">Configurações OMA.</span><span class="sxs-lookup"><span data-stu-id="d221a-170">OMA settings.</span></span> <span data-ttu-id="d221a-171">Esta coleção pode conter um máximo de 500 elementos.</span><span class="sxs-lookup"><span data-stu-id="d221a-171">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="d221a-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="d221a-172">Response</span></span>
<span data-ttu-id="d221a-173">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d221a-173">If successful, this method returns a `201 Created` response code and a [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d221a-174">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d221a-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="d221a-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d221a-175">Request</span></span>
<span data-ttu-id="d221a-176">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d221a-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 565

{
  "@odata.type": "#microsoft.graph.androidForWorkCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="d221a-177">Resposta</span><span class="sxs-lookup"><span data-stu-id="d221a-177">Response</span></span>
<span data-ttu-id="d221a-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d221a-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





