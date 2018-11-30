---
title: Criar androidForWorkWiFiConfiguration
description: Crie um novo objeto de androidForWorkWiFiConfiguration.
ms.openlocfilehash: 90019b0934a9dfd2b374f082b6e153bb18e7c9c5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036578"
---
# <a name="create-androidforworkwificonfiguration"></a><span data-ttu-id="f402b-103">Criar androidForWorkWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="f402b-103">Create androidForWorkWiFiConfiguration</span></span>

> <span data-ttu-id="f402b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f402b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f402b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f402b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f402b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f402b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f402b-107">Crie um novo objeto de [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f402b-107">Create a new [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f402b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f402b-108">Prerequisites</span></span>
<span data-ttu-id="f402b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f402b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f402b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f402b-111">Permission type</span></span>|<span data-ttu-id="f402b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f402b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f402b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f402b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f402b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f402b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f402b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f402b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f402b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f402b-116">Not supported.</span></span>|
|<span data-ttu-id="f402b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f402b-117">Application</span></span>|<span data-ttu-id="f402b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f402b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f402b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f402b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f402b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f402b-120">Request headers</span></span>
|<span data-ttu-id="f402b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f402b-121">Header</span></span>|<span data-ttu-id="f402b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f402b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f402b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f402b-123">Authorization</span></span>|<span data-ttu-id="f402b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f402b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f402b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f402b-125">Accept</span></span>|<span data-ttu-id="f402b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f402b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f402b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f402b-127">Request body</span></span>
<span data-ttu-id="f402b-128">No corpo da solicitação, fornece uma representação JSON para o objeto androidForWorkWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f402b-128">In the request body, supply a JSON representation for the androidForWorkWiFiConfiguration object.</span></span>

<span data-ttu-id="f402b-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o androidForWorkWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f402b-129">The following table shows the properties that are required when you create the androidForWorkWiFiConfiguration.</span></span>

|<span data-ttu-id="f402b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f402b-130">Property</span></span>|<span data-ttu-id="f402b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f402b-131">Type</span></span>|<span data-ttu-id="f402b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f402b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f402b-133">id</span><span class="sxs-lookup"><span data-stu-id="f402b-133">id</span></span>|<span data-ttu-id="f402b-134">String</span><span class="sxs-lookup"><span data-stu-id="f402b-134">String</span></span>|<span data-ttu-id="f402b-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f402b-135">Key of the entity.</span></span> <span data-ttu-id="f402b-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f402b-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f402b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f402b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f402b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f402b-138">DateTimeOffset</span></span>|<span data-ttu-id="f402b-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f402b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f402b-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f402b-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f402b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f402b-141">roleScopeTagIds</span></span>|<span data-ttu-id="f402b-142">String collection</span><span class="sxs-lookup"><span data-stu-id="f402b-142">String collection</span></span>|<span data-ttu-id="f402b-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="f402b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f402b-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f402b-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f402b-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f402b-145">supportsScopeTags</span></span>|<span data-ttu-id="f402b-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="f402b-146">Boolean</span></span>|<span data-ttu-id="f402b-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="f402b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f402b-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="f402b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f402b-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="f402b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f402b-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f402b-150">This property is read-only.</span></span> <span data-ttu-id="f402b-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f402b-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f402b-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f402b-152">createdDateTime</span></span>|<span data-ttu-id="f402b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f402b-153">DateTimeOffset</span></span>|<span data-ttu-id="f402b-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f402b-154">DateTime the object was created.</span></span> <span data-ttu-id="f402b-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f402b-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f402b-156">description</span><span class="sxs-lookup"><span data-stu-id="f402b-156">description</span></span>|<span data-ttu-id="f402b-157">String</span><span class="sxs-lookup"><span data-stu-id="f402b-157">String</span></span>|<span data-ttu-id="f402b-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f402b-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f402b-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f402b-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f402b-160">displayName</span><span class="sxs-lookup"><span data-stu-id="f402b-160">displayName</span></span>|<span data-ttu-id="f402b-161">String</span><span class="sxs-lookup"><span data-stu-id="f402b-161">String</span></span>|<span data-ttu-id="f402b-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f402b-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f402b-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f402b-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f402b-164">version</span><span class="sxs-lookup"><span data-stu-id="f402b-164">version</span></span>|<span data-ttu-id="f402b-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f402b-165">Int32</span></span>|<span data-ttu-id="f402b-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f402b-166">Version of the device configuration.</span></span> <span data-ttu-id="f402b-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f402b-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f402b-168">networkName</span><span class="sxs-lookup"><span data-stu-id="f402b-168">networkName</span></span>|<span data-ttu-id="f402b-169">String</span><span class="sxs-lookup"><span data-stu-id="f402b-169">String</span></span>|<span data-ttu-id="f402b-170">Nome da rede</span><span class="sxs-lookup"><span data-stu-id="f402b-170">Network Name</span></span>|
|<span data-ttu-id="f402b-171">SSID</span><span class="sxs-lookup"><span data-stu-id="f402b-171">ssid</span></span>|<span data-ttu-id="f402b-172">String</span><span class="sxs-lookup"><span data-stu-id="f402b-172">String</span></span>|<span data-ttu-id="f402b-173">Este é o nome da rede Wi-Fi que é difundido para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="f402b-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="f402b-174">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="f402b-174">connectAutomatically</span></span>|<span data-ttu-id="f402b-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="f402b-175">Boolean</span></span>|<span data-ttu-id="f402b-176">Conecte automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="f402b-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="f402b-177">Essa configuração como true ignorar o prompt do usuário e se conecte automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="f402b-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="f402b-178">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="f402b-178">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="f402b-179">Booliano</span><span class="sxs-lookup"><span data-stu-id="f402b-179">Boolean</span></span>|<span data-ttu-id="f402b-180">Quando definido como true, esse perfil força o dispositivo para se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="f402b-180">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="f402b-181">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="f402b-181">wiFiSecurityType</span></span>|[<span data-ttu-id="f402b-182">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="f402b-182">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="f402b-183">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseada em EAP.</span><span class="sxs-lookup"><span data-stu-id="f402b-183">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="f402b-184">Os valores possíveis são: `open` e `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="f402b-184">Possible values are: `open`, `wpaEnterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="f402b-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="f402b-185">Response</span></span>
<span data-ttu-id="f402b-186">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f402b-186">If successful, this method returns a `201 Created` response code and a [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f402b-187">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f402b-187">Example</span></span>
### <a name="request"></a><span data-ttu-id="f402b-188">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f402b-188">Request</span></span>
<span data-ttu-id="f402b-189">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f402b-189">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 506

{
  "@odata.type": "#microsoft.graph.androidForWorkWiFiConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaEnterprise"
}
```

### <a name="response"></a><span data-ttu-id="f402b-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="f402b-190">Response</span></span>
<span data-ttu-id="f402b-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f402b-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 614

{
  "@odata.type": "#microsoft.graph.androidForWorkWiFiConfiguration",
  "id": "58bcfe05-fe05-58bc-05fe-bc5805febc58",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaEnterprise"
}
```





