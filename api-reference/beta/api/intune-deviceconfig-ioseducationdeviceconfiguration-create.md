---
title: Criar iosEducationDeviceConfiguration
description: Crie um novo objeto de iosEducationDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e64b59f6eb6dbaa0a627b5c52a3d29c356199718
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977735"
---
# <a name="create-ioseducationdeviceconfiguration"></a><span data-ttu-id="a56dc-103">Criar iosEducationDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="a56dc-103">Create iosEducationDeviceConfiguration</span></span>

> <span data-ttu-id="a56dc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a56dc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a56dc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a56dc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a56dc-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a56dc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a56dc-107">Crie um novo objeto de [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a56dc-107">Create a new [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a56dc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a56dc-108">Prerequisites</span></span>
<span data-ttu-id="a56dc-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a56dc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a56dc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a56dc-111">Permission type</span></span>|<span data-ttu-id="a56dc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a56dc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a56dc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a56dc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a56dc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a56dc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a56dc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a56dc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a56dc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a56dc-116">Not supported.</span></span>|
|<span data-ttu-id="a56dc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a56dc-117">Application</span></span>|<span data-ttu-id="a56dc-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a56dc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a56dc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a56dc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a56dc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a56dc-120">Request headers</span></span>
|<span data-ttu-id="a56dc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a56dc-121">Header</span></span>|<span data-ttu-id="a56dc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a56dc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a56dc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a56dc-123">Authorization</span></span>|<span data-ttu-id="a56dc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a56dc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a56dc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a56dc-125">Accept</span></span>|<span data-ttu-id="a56dc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a56dc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a56dc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a56dc-127">Request body</span></span>
<span data-ttu-id="a56dc-128">No corpo da solicitação, fornece uma representação JSON para o objeto iosEducationDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a56dc-128">In the request body, supply a JSON representation for the iosEducationDeviceConfiguration object.</span></span>

<span data-ttu-id="a56dc-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o iosEducationDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="a56dc-129">The following table shows the properties that are required when you create the iosEducationDeviceConfiguration.</span></span>

|<span data-ttu-id="a56dc-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a56dc-130">Property</span></span>|<span data-ttu-id="a56dc-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a56dc-131">Type</span></span>|<span data-ttu-id="a56dc-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a56dc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a56dc-133">id</span><span class="sxs-lookup"><span data-stu-id="a56dc-133">id</span></span>|<span data-ttu-id="a56dc-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a56dc-134">String</span></span>|<span data-ttu-id="a56dc-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a56dc-135">Key of the entity.</span></span> <span data-ttu-id="a56dc-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a56dc-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a56dc-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a56dc-137">lastModifiedDateTime</span></span>|<span data-ttu-id="a56dc-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a56dc-138">DateTimeOffset</span></span>|<span data-ttu-id="a56dc-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a56dc-139">DateTime the object was last modified.</span></span> <span data-ttu-id="a56dc-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a56dc-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a56dc-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a56dc-141">roleScopeTagIds</span></span>|<span data-ttu-id="a56dc-142">String collection</span><span class="sxs-lookup"><span data-stu-id="a56dc-142">String collection</span></span>|<span data-ttu-id="a56dc-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="a56dc-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a56dc-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a56dc-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a56dc-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a56dc-145">supportsScopeTags</span></span>|<span data-ttu-id="a56dc-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="a56dc-146">Boolean</span></span>|<span data-ttu-id="a56dc-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="a56dc-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a56dc-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="a56dc-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a56dc-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="a56dc-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a56dc-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a56dc-150">This property is read-only.</span></span> <span data-ttu-id="a56dc-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a56dc-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a56dc-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a56dc-152">createdDateTime</span></span>|<span data-ttu-id="a56dc-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a56dc-153">DateTimeOffset</span></span>|<span data-ttu-id="a56dc-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a56dc-154">DateTime the object was created.</span></span> <span data-ttu-id="a56dc-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a56dc-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a56dc-156">description</span><span class="sxs-lookup"><span data-stu-id="a56dc-156">description</span></span>|<span data-ttu-id="a56dc-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a56dc-157">String</span></span>|<span data-ttu-id="a56dc-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a56dc-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a56dc-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a56dc-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a56dc-160">displayName</span><span class="sxs-lookup"><span data-stu-id="a56dc-160">displayName</span></span>|<span data-ttu-id="a56dc-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a56dc-161">String</span></span>|<span data-ttu-id="a56dc-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a56dc-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a56dc-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a56dc-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a56dc-164">version</span><span class="sxs-lookup"><span data-stu-id="a56dc-164">version</span></span>|<span data-ttu-id="a56dc-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a56dc-165">Int32</span></span>|<span data-ttu-id="a56dc-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a56dc-166">Version of the device configuration.</span></span> <span data-ttu-id="a56dc-167">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a56dc-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="a56dc-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="a56dc-168">Response</span></span>
<span data-ttu-id="a56dc-169">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a56dc-169">If successful, this method returns a `201 Created` response code and a [iosEducationDeviceConfiguration](../resources/intune-deviceconfig-ioseducationdeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a56dc-170">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a56dc-170">Example</span></span>
### <a name="request"></a><span data-ttu-id="a56dc-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a56dc-171">Request</span></span>
<span data-ttu-id="a56dc-172">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a56dc-172">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 325

{
  "@odata.type": "#microsoft.graph.iosEducationDeviceConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="a56dc-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="a56dc-173">Response</span></span>
<span data-ttu-id="a56dc-p111">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a56dc-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 433

{
  "@odata.type": "#microsoft.graph.iosEducationDeviceConfiguration",
  "id": "3d563be4-3be4-3d56-e43b-563de43b563d",
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





