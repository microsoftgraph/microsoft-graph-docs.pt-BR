---
title: Atualizar windows81WifiImportConfiguration
description: Atualize as propriedades de um objeto windows81WifiImportConfiguration.
ms.openlocfilehash: 7ce28ed3c59053da7165c2377975d4b284513874
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037164"
---
# <a name="update-windows81wifiimportconfiguration"></a><span data-ttu-id="bdfb6-103">Atualizar windows81WifiImportConfiguration</span><span class="sxs-lookup"><span data-stu-id="bdfb6-103">Update windows81WifiImportConfiguration</span></span>

> <span data-ttu-id="bdfb6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bdfb6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bdfb6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bdfb6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bdfb6-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bdfb6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bdfb6-107">Atualize as propriedades de um objeto [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="bdfb6-107">Update the properties of a [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bdfb6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bdfb6-108">Prerequisites</span></span>
<span data-ttu-id="bdfb6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdfb6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdfb6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bdfb6-111">Permission type</span></span>|<span data-ttu-id="bdfb6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bdfb6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bdfb6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bdfb6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bdfb6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdfb6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bdfb6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bdfb6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bdfb6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bdfb6-116">Not supported.</span></span>|
|<span data-ttu-id="bdfb6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bdfb6-117">Application</span></span>|<span data-ttu-id="bdfb6-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bdfb6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bdfb6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bdfb6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="bdfb6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bdfb6-120">Request headers</span></span>
|<span data-ttu-id="bdfb6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bdfb6-121">Header</span></span>|<span data-ttu-id="bdfb6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="bdfb6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bdfb6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="bdfb6-123">Authorization</span></span>|<span data-ttu-id="bdfb6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bdfb6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bdfb6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bdfb6-125">Accept</span></span>|<span data-ttu-id="bdfb6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bdfb6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bdfb6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bdfb6-127">Request body</span></span>
<span data-ttu-id="bdfb6-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="bdfb6-128">In the request body, supply a JSON representation for the [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object.</span></span>

<span data-ttu-id="bdfb6-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="bdfb6-129">The following table shows the properties that are required when you create the [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md).</span></span>

|<span data-ttu-id="bdfb6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bdfb6-130">Property</span></span>|<span data-ttu-id="bdfb6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="bdfb6-131">Type</span></span>|<span data-ttu-id="bdfb6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdfb6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdfb6-133">id</span><span class="sxs-lookup"><span data-stu-id="bdfb6-133">id</span></span>|<span data-ttu-id="bdfb6-134">String</span><span class="sxs-lookup"><span data-stu-id="bdfb6-134">String</span></span>|<span data-ttu-id="bdfb6-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bdfb6-135">Key of the entity.</span></span> <span data-ttu-id="bdfb6-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bdfb6-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdfb6-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bdfb6-137">lastModifiedDateTime</span></span>|<span data-ttu-id="bdfb6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdfb6-138">DateTimeOffset</span></span>|<span data-ttu-id="bdfb6-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="bdfb6-139">DateTime the object was last modified.</span></span> <span data-ttu-id="bdfb6-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bdfb6-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdfb6-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="bdfb6-141">roleScopeTagIds</span></span>|<span data-ttu-id="bdfb6-142">String collection</span><span class="sxs-lookup"><span data-stu-id="bdfb6-142">String collection</span></span>|<span data-ttu-id="bdfb6-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="bdfb6-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="bdfb6-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bdfb6-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdfb6-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="bdfb6-145">supportsScopeTags</span></span>|<span data-ttu-id="bdfb6-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="bdfb6-146">Boolean</span></span>|<span data-ttu-id="bdfb6-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="bdfb6-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="bdfb6-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="bdfb6-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="bdfb6-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="bdfb6-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="bdfb6-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bdfb6-150">This property is read-only.</span></span> <span data-ttu-id="bdfb6-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bdfb6-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdfb6-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bdfb6-152">createdDateTime</span></span>|<span data-ttu-id="bdfb6-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bdfb6-153">DateTimeOffset</span></span>|<span data-ttu-id="bdfb6-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="bdfb6-154">DateTime the object was created.</span></span> <span data-ttu-id="bdfb6-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bdfb6-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdfb6-156">description</span><span class="sxs-lookup"><span data-stu-id="bdfb6-156">description</span></span>|<span data-ttu-id="bdfb6-157">String</span><span class="sxs-lookup"><span data-stu-id="bdfb6-157">String</span></span>|<span data-ttu-id="bdfb6-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bdfb6-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="bdfb6-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bdfb6-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdfb6-160">displayName</span><span class="sxs-lookup"><span data-stu-id="bdfb6-160">displayName</span></span>|<span data-ttu-id="bdfb6-161">String</span><span class="sxs-lookup"><span data-stu-id="bdfb6-161">String</span></span>|<span data-ttu-id="bdfb6-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bdfb6-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="bdfb6-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bdfb6-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdfb6-164">version</span><span class="sxs-lookup"><span data-stu-id="bdfb6-164">version</span></span>|<span data-ttu-id="bdfb6-165">Int32</span><span class="sxs-lookup"><span data-stu-id="bdfb6-165">Int32</span></span>|<span data-ttu-id="bdfb6-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bdfb6-166">Version of the device configuration.</span></span> <span data-ttu-id="bdfb6-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="bdfb6-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="bdfb6-168">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="bdfb6-168">payloadFileName</span></span>|<span data-ttu-id="bdfb6-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bdfb6-169">String</span></span>|<span data-ttu-id="bdfb6-170">Nome de arquivo de carga (\*. xml).</span><span class="sxs-lookup"><span data-stu-id="bdfb6-170">Payload file name (\*.xml).</span></span>|
|<span data-ttu-id="bdfb6-171">profileName</span><span class="sxs-lookup"><span data-stu-id="bdfb6-171">profileName</span></span>|<span data-ttu-id="bdfb6-172">String</span><span class="sxs-lookup"><span data-stu-id="bdfb6-172">String</span></span>|<span data-ttu-id="bdfb6-173">Nome do perfil exibido na interface do usuário.</span><span class="sxs-lookup"><span data-stu-id="bdfb6-173">Profile name displayed in the UI.</span></span>|
|<span data-ttu-id="bdfb6-174">payload</span><span class="sxs-lookup"><span data-stu-id="bdfb6-174">payload</span></span>|<span data-ttu-id="bdfb6-175">Binária</span><span class="sxs-lookup"><span data-stu-id="bdfb6-175">Binary</span></span>|<span data-ttu-id="bdfb6-176">Carga.</span><span class="sxs-lookup"><span data-stu-id="bdfb6-176">Payload.</span></span> <span data-ttu-id="bdfb6-177">(Array de byte codificado UTF8).</span><span class="sxs-lookup"><span data-stu-id="bdfb6-177">(UTF8 encoded byte array).</span></span> <span data-ttu-id="bdfb6-178">Este é o arquivo XML salvo no dispositivo usado para conectar ao ponto de extremidade Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="bdfb6-178">This is the XML file saved on the device you used to connect to the Wi-Fi endpoint.</span></span>|



## <a name="response"></a><span data-ttu-id="bdfb6-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdfb6-179">Response</span></span>
<span data-ttu-id="bdfb6-180">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bdfb6-180">If successful, this method returns a `200 OK` response code and an updated [windows81WifiImportConfiguration](../resources/intune-deviceconfig-windows81wifiimportconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdfb6-181">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bdfb6-181">Example</span></span>
### <a name="request"></a><span data-ttu-id="bdfb6-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bdfb6-182">Request</span></span>
<span data-ttu-id="bdfb6-183">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bdfb6-183">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 374

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadFileName": "Payload File Name value",
  "profileName": "Profile Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="bdfb6-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdfb6-184">Response</span></span>
<span data-ttu-id="bdfb6-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bdfb6-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 553

{
  "@odata.type": "#microsoft.graph.windows81WifiImportConfiguration",
  "id": "534a2f07-2f07-534a-072f-4a53072f4a53",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadFileName": "Payload File Name value",
  "profileName": "Profile Name value",
  "payload": "cGF5bG9hZA=="
}
```





