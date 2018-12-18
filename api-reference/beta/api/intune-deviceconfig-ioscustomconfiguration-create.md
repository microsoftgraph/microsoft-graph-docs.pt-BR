---
title: Criar iosCustomConfiguration
description: Cria um novo objeto iosCustomConfiguration.
author: tfitzmac
ms.openlocfilehash: e22a670316ca7ffb4216c45cab5e8f3e6d7f3d65
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343306"
---
# <a name="create-ioscustomconfiguration"></a><span data-ttu-id="9fde4-103">Criar iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="9fde4-103">Create iosCustomConfiguration</span></span>

> <span data-ttu-id="9fde4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9fde4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9fde4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9fde4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9fde4-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9fde4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9fde4-107">Cria um novo objeto [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9fde4-107">Create a new [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9fde4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9fde4-108">Prerequisites</span></span>
<span data-ttu-id="9fde4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9fde4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fde4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9fde4-111">Permission type</span></span>|<span data-ttu-id="9fde4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9fde4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9fde4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9fde4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9fde4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fde4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9fde4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9fde4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9fde4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9fde4-116">Not supported.</span></span>|
|<span data-ttu-id="9fde4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9fde4-117">Application</span></span>|<span data-ttu-id="9fde4-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9fde4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9fde4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9fde4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9fde4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9fde4-120">Request headers</span></span>
|<span data-ttu-id="9fde4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9fde4-121">Header</span></span>|<span data-ttu-id="9fde4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9fde4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9fde4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9fde4-123">Authorization</span></span>|<span data-ttu-id="9fde4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9fde4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9fde4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9fde4-125">Accept</span></span>|<span data-ttu-id="9fde4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9fde4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9fde4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9fde4-127">Request body</span></span>
<span data-ttu-id="9fde4-128">No corpo da solicitação, forneça uma representação JSON do objeto iosCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="9fde4-128">In the request body, supply a JSON representation for the iosCustomConfiguration object.</span></span>

<span data-ttu-id="9fde4-129">A tabela a seguir mostra as propriedades que são necessárias ao criar iosCustomConfiguration.</span><span class="sxs-lookup"><span data-stu-id="9fde4-129">The following table shows the properties that are required when you create the iosCustomConfiguration.</span></span>

|<span data-ttu-id="9fde4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9fde4-130">Property</span></span>|<span data-ttu-id="9fde4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9fde4-131">Type</span></span>|<span data-ttu-id="9fde4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9fde4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fde4-133">id</span><span class="sxs-lookup"><span data-stu-id="9fde4-133">id</span></span>|<span data-ttu-id="9fde4-134">String</span><span class="sxs-lookup"><span data-stu-id="9fde4-134">String</span></span>|<span data-ttu-id="9fde4-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9fde4-135">Key of the entity.</span></span> <span data-ttu-id="9fde4-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9fde4-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9fde4-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9fde4-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9fde4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fde4-138">DateTimeOffset</span></span>|<span data-ttu-id="9fde4-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="9fde4-139">DateTime the object was last modified.</span></span> <span data-ttu-id="9fde4-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9fde4-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9fde4-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9fde4-141">roleScopeTagIds</span></span>|<span data-ttu-id="9fde4-142">String collection</span><span class="sxs-lookup"><span data-stu-id="9fde4-142">String collection</span></span>|<span data-ttu-id="9fde4-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="9fde4-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9fde4-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9fde4-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9fde4-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9fde4-145">supportsScopeTags</span></span>|<span data-ttu-id="9fde4-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="9fde4-146">Boolean</span></span>|<span data-ttu-id="9fde4-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="9fde4-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9fde4-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="9fde4-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9fde4-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="9fde4-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9fde4-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9fde4-150">This property is read-only.</span></span> <span data-ttu-id="9fde4-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9fde4-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9fde4-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9fde4-152">createdDateTime</span></span>|<span data-ttu-id="9fde4-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fde4-153">DateTimeOffset</span></span>|<span data-ttu-id="9fde4-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="9fde4-154">DateTime the object was created.</span></span> <span data-ttu-id="9fde4-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9fde4-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9fde4-156">description</span><span class="sxs-lookup"><span data-stu-id="9fde4-156">description</span></span>|<span data-ttu-id="9fde4-157">String</span><span class="sxs-lookup"><span data-stu-id="9fde4-157">String</span></span>|<span data-ttu-id="9fde4-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9fde4-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9fde4-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9fde4-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9fde4-160">displayName</span><span class="sxs-lookup"><span data-stu-id="9fde4-160">displayName</span></span>|<span data-ttu-id="9fde4-161">String</span><span class="sxs-lookup"><span data-stu-id="9fde4-161">String</span></span>|<span data-ttu-id="9fde4-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9fde4-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9fde4-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9fde4-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9fde4-164">version</span><span class="sxs-lookup"><span data-stu-id="9fde4-164">version</span></span>|<span data-ttu-id="9fde4-165">Int32</span><span class="sxs-lookup"><span data-stu-id="9fde4-165">Int32</span></span>|<span data-ttu-id="9fde4-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9fde4-166">Version of the device configuration.</span></span> <span data-ttu-id="9fde4-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9fde4-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9fde4-168">payloadName</span><span class="sxs-lookup"><span data-stu-id="9fde4-168">payloadName</span></span>|<span data-ttu-id="9fde4-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9fde4-169">String</span></span>|<span data-ttu-id="9fde4-170">Nome que é exibido para o usuário.</span><span class="sxs-lookup"><span data-stu-id="9fde4-170">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="9fde4-171">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="9fde4-171">payloadFileName</span></span>|<span data-ttu-id="9fde4-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9fde4-172">String</span></span>|<span data-ttu-id="9fde4-173">O nome do arquivo de carga (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="9fde4-173">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="9fde4-174">\*.xml).</span><span class="sxs-lookup"><span data-stu-id="9fde4-174">\*.xml).</span></span>|
|<span data-ttu-id="9fde4-175">payload</span><span class="sxs-lookup"><span data-stu-id="9fde4-175">payload</span></span>|<span data-ttu-id="9fde4-176">Binária</span><span class="sxs-lookup"><span data-stu-id="9fde4-176">Binary</span></span>|<span data-ttu-id="9fde4-177">Carga.</span><span class="sxs-lookup"><span data-stu-id="9fde4-177">Payload.</span></span> <span data-ttu-id="9fde4-178">(Matriz de bytes codificados em UTF8)</span><span class="sxs-lookup"><span data-stu-id="9fde4-178">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="9fde4-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fde4-179">Response</span></span>
<span data-ttu-id="9fde4-180">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9fde4-180">If successful, this method returns a `201 Created` response code and a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fde4-181">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9fde4-181">Example</span></span>
### <a name="request"></a><span data-ttu-id="9fde4-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9fde4-182">Request</span></span>
<span data-ttu-id="9fde4-183">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9fde4-183">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 435

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="9fde4-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="9fde4-184">Response</span></span>
<span data-ttu-id="9fde4-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9fde4-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 543

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
  "id": "f34428e3-28e3-f344-e328-44f3e32844f3",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```





