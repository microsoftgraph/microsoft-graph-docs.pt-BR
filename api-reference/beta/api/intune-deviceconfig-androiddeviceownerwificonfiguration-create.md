---
title: Criar androidDeviceOwnerWiFiConfiguration
description: Crie um novo objeto de androidDeviceOwnerWiFiConfiguration.
author: tfitzmac
ms.openlocfilehash: f3933e28bb0c47ccc104adb00358237c51920dfb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327325"
---
# <a name="create-androiddeviceownerwificonfiguration"></a><span data-ttu-id="1cb6f-103">Criar androidDeviceOwnerWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="1cb6f-103">Create androidDeviceOwnerWiFiConfiguration</span></span>

> <span data-ttu-id="1cb6f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1cb6f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1cb6f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1cb6f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1cb6f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1cb6f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1cb6f-107">Crie um novo objeto de [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="1cb6f-107">Create a new [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1cb6f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1cb6f-108">Prerequisites</span></span>
<span data-ttu-id="1cb6f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cb6f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cb6f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1cb6f-111">Permission type</span></span>|<span data-ttu-id="1cb6f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1cb6f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1cb6f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1cb6f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1cb6f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cb6f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1cb6f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1cb6f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1cb6f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1cb6f-116">Not supported.</span></span>|
|<span data-ttu-id="1cb6f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1cb6f-117">Application</span></span>|<span data-ttu-id="1cb6f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1cb6f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1cb6f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1cb6f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1cb6f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1cb6f-120">Request headers</span></span>
|<span data-ttu-id="1cb6f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1cb6f-121">Header</span></span>|<span data-ttu-id="1cb6f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1cb6f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1cb6f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1cb6f-123">Authorization</span></span>|<span data-ttu-id="1cb6f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1cb6f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1cb6f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1cb6f-125">Accept</span></span>|<span data-ttu-id="1cb6f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1cb6f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1cb6f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1cb6f-127">Request body</span></span>
<span data-ttu-id="1cb6f-128">No corpo da solicitação, fornece uma representação JSON para o objeto androidDeviceOwnerWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="1cb6f-128">In the request body, supply a JSON representation for the androidDeviceOwnerWiFiConfiguration object.</span></span>

<span data-ttu-id="1cb6f-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o androidDeviceOwnerWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="1cb6f-129">The following table shows the properties that are required when you create the androidDeviceOwnerWiFiConfiguration.</span></span>

|<span data-ttu-id="1cb6f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1cb6f-130">Property</span></span>|<span data-ttu-id="1cb6f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="1cb6f-131">Type</span></span>|<span data-ttu-id="1cb6f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cb6f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cb6f-133">id</span><span class="sxs-lookup"><span data-stu-id="1cb6f-133">id</span></span>|<span data-ttu-id="1cb6f-134">String</span><span class="sxs-lookup"><span data-stu-id="1cb6f-134">String</span></span>|<span data-ttu-id="1cb6f-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1cb6f-135">Key of the entity.</span></span> <span data-ttu-id="1cb6f-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1cb6f-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cb6f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1cb6f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1cb6f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cb6f-138">DateTimeOffset</span></span>|<span data-ttu-id="1cb6f-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="1cb6f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="1cb6f-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1cb6f-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cb6f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1cb6f-141">roleScopeTagIds</span></span>|<span data-ttu-id="1cb6f-142">String collection</span><span class="sxs-lookup"><span data-stu-id="1cb6f-142">String collection</span></span>|<span data-ttu-id="1cb6f-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="1cb6f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1cb6f-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1cb6f-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cb6f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1cb6f-145">supportsScopeTags</span></span>|<span data-ttu-id="1cb6f-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="1cb6f-146">Boolean</span></span>|<span data-ttu-id="1cb6f-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="1cb6f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1cb6f-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="1cb6f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1cb6f-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="1cb6f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1cb6f-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1cb6f-150">This property is read-only.</span></span> <span data-ttu-id="1cb6f-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1cb6f-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cb6f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1cb6f-152">createdDateTime</span></span>|<span data-ttu-id="1cb6f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1cb6f-153">DateTimeOffset</span></span>|<span data-ttu-id="1cb6f-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="1cb6f-154">DateTime the object was created.</span></span> <span data-ttu-id="1cb6f-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1cb6f-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cb6f-156">description</span><span class="sxs-lookup"><span data-stu-id="1cb6f-156">description</span></span>|<span data-ttu-id="1cb6f-157">String</span><span class="sxs-lookup"><span data-stu-id="1cb6f-157">String</span></span>|<span data-ttu-id="1cb6f-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1cb6f-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1cb6f-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1cb6f-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cb6f-160">displayName</span><span class="sxs-lookup"><span data-stu-id="1cb6f-160">displayName</span></span>|<span data-ttu-id="1cb6f-161">String</span><span class="sxs-lookup"><span data-stu-id="1cb6f-161">String</span></span>|<span data-ttu-id="1cb6f-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1cb6f-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1cb6f-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1cb6f-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cb6f-164">version</span><span class="sxs-lookup"><span data-stu-id="1cb6f-164">version</span></span>|<span data-ttu-id="1cb6f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="1cb6f-165">Int32</span></span>|<span data-ttu-id="1cb6f-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1cb6f-166">Version of the device configuration.</span></span> <span data-ttu-id="1cb6f-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1cb6f-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1cb6f-168">networkName</span><span class="sxs-lookup"><span data-stu-id="1cb6f-168">networkName</span></span>|<span data-ttu-id="1cb6f-169">String</span><span class="sxs-lookup"><span data-stu-id="1cb6f-169">String</span></span>|<span data-ttu-id="1cb6f-170">Nome da rede</span><span class="sxs-lookup"><span data-stu-id="1cb6f-170">Network Name</span></span>|
|<span data-ttu-id="1cb6f-171">SSID</span><span class="sxs-lookup"><span data-stu-id="1cb6f-171">ssid</span></span>|<span data-ttu-id="1cb6f-172">String</span><span class="sxs-lookup"><span data-stu-id="1cb6f-172">String</span></span>|<span data-ttu-id="1cb6f-173">Este é o nome da rede Wi-Fi que é difundido para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="1cb6f-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="1cb6f-174">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="1cb6f-174">connectAutomatically</span></span>|<span data-ttu-id="1cb6f-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="1cb6f-175">Boolean</span></span>|<span data-ttu-id="1cb6f-176">Conecte automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="1cb6f-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="1cb6f-177">Essa configuração como true ignorar o prompt do usuário e se conecte automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="1cb6f-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="1cb6f-178">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="1cb6f-178">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="1cb6f-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="1cb6f-179">Boolean</span></span>|<span data-ttu-id="1cb6f-180">Quando definido como true, esse perfil força o dispositivo para se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="1cb6f-180">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="1cb6f-181">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="1cb6f-181">wiFiSecurityType</span></span>|[<span data-ttu-id="1cb6f-182">androidDeviceOwnerWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="1cb6f-182">androidDeviceOwnerWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androiddeviceownerwifisecuritytype.md)|<span data-ttu-id="1cb6f-183">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseada em EAP.</span><span class="sxs-lookup"><span data-stu-id="1cb6f-183">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="1cb6f-184">Os valores possíveis são: `open`, `wep`, `wpaPersonal`.</span><span class="sxs-lookup"><span data-stu-id="1cb6f-184">Possible values are: `open`, `wep`, `wpaPersonal`.</span></span>|
|<span data-ttu-id="1cb6f-185">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="1cb6f-185">preSharedKey</span></span>|<span data-ttu-id="1cb6f-186">String</span><span class="sxs-lookup"><span data-stu-id="1cb6f-186">String</span></span>|<span data-ttu-id="1cb6f-187">Esta é a chave pré compartilhada para rede Wi-Fi WPA Pessoal.</span><span class="sxs-lookup"><span data-stu-id="1cb6f-187">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="1cb6f-188">preSharedKeyIsSet</span><span class="sxs-lookup"><span data-stu-id="1cb6f-188">preSharedKeyIsSet</span></span>|<span data-ttu-id="1cb6f-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="1cb6f-189">Boolean</span></span>|<span data-ttu-id="1cb6f-190">Esta é a chave pré compartilhada para rede Wi-Fi WPA Pessoal.</span><span class="sxs-lookup"><span data-stu-id="1cb6f-190">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="1cb6f-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cb6f-191">Response</span></span>
<span data-ttu-id="1cb6f-192">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1cb6f-192">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1cb6f-193">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1cb6f-193">Example</span></span>
### <a name="request"></a><span data-ttu-id="1cb6f-194">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1cb6f-194">Request</span></span>
<span data-ttu-id="1cb6f-195">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1cb6f-195">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 573

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerWiFiConfiguration",
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
  "wiFiSecurityType": "wep",
  "preSharedKey": "Pre Shared Key value",
  "preSharedKeyIsSet": true
}
```

### <a name="response"></a><span data-ttu-id="1cb6f-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cb6f-196">Response</span></span>
<span data-ttu-id="1cb6f-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1cb6f-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 681

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerWiFiConfiguration",
  "id": "8d25beba-beba-8d25-babe-258dbabe258d",
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
  "wiFiSecurityType": "wep",
  "preSharedKey": "Pre Shared Key value",
  "preSharedKeyIsSet": true
}
```





