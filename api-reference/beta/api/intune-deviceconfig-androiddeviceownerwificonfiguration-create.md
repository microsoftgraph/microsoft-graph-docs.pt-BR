---
title: Criar androidDeviceOwnerWiFiConfiguration
description: Crie um novo objeto de androidDeviceOwnerWiFiConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cfe9c038a05933f8352830c4038881c956972d9d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401667"
---
# <a name="create-androiddeviceownerwificonfiguration"></a><span data-ttu-id="ab418-103">Criar androidDeviceOwnerWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="ab418-103">Create androidDeviceOwnerWiFiConfiguration</span></span>

> <span data-ttu-id="ab418-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="ab418-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ab418-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ab418-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ab418-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="ab418-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab418-107">Crie um novo objeto de [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ab418-107">Create a new [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ab418-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ab418-108">Prerequisites</span></span>
<span data-ttu-id="ab418-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ab418-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ab418-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab418-111">Permission type</span></span>|<span data-ttu-id="ab418-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ab418-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab418-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab418-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ab418-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab418-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ab418-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab418-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab418-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab418-116">Not supported.</span></span>|
|<span data-ttu-id="ab418-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab418-117">Application</span></span>|<span data-ttu-id="ab418-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab418-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab418-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab418-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ab418-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab418-120">Request headers</span></span>
|<span data-ttu-id="ab418-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ab418-121">Header</span></span>|<span data-ttu-id="ab418-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ab418-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab418-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab418-123">Authorization</span></span>|<span data-ttu-id="ab418-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab418-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab418-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ab418-125">Accept</span></span>|<span data-ttu-id="ab418-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ab418-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab418-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab418-127">Request body</span></span>
<span data-ttu-id="ab418-128">No corpo da solicitação, fornece uma representação JSON para o objeto androidDeviceOwnerWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ab418-128">In the request body, supply a JSON representation for the androidDeviceOwnerWiFiConfiguration object.</span></span>

<span data-ttu-id="ab418-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o androidDeviceOwnerWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ab418-129">The following table shows the properties that are required when you create the androidDeviceOwnerWiFiConfiguration.</span></span>

|<span data-ttu-id="ab418-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ab418-130">Property</span></span>|<span data-ttu-id="ab418-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab418-131">Type</span></span>|<span data-ttu-id="ab418-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab418-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab418-133">id</span><span class="sxs-lookup"><span data-stu-id="ab418-133">id</span></span>|<span data-ttu-id="ab418-134">String</span><span class="sxs-lookup"><span data-stu-id="ab418-134">String</span></span>|<span data-ttu-id="ab418-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ab418-135">Key of the entity.</span></span> <span data-ttu-id="ab418-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab418-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab418-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ab418-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ab418-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab418-138">DateTimeOffset</span></span>|<span data-ttu-id="ab418-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="ab418-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ab418-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab418-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab418-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ab418-141">roleScopeTagIds</span></span>|<span data-ttu-id="ab418-142">String collection</span><span class="sxs-lookup"><span data-stu-id="ab418-142">String collection</span></span>|<span data-ttu-id="ab418-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="ab418-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ab418-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab418-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab418-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ab418-145">supportsScopeTags</span></span>|<span data-ttu-id="ab418-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab418-146">Boolean</span></span>|<span data-ttu-id="ab418-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="ab418-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ab418-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="ab418-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ab418-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="ab418-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ab418-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ab418-150">This property is read-only.</span></span> <span data-ttu-id="ab418-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab418-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab418-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ab418-152">createdDateTime</span></span>|<span data-ttu-id="ab418-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab418-153">DateTimeOffset</span></span>|<span data-ttu-id="ab418-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="ab418-154">DateTime the object was created.</span></span> <span data-ttu-id="ab418-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab418-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab418-156">description</span><span class="sxs-lookup"><span data-stu-id="ab418-156">description</span></span>|<span data-ttu-id="ab418-157">String</span><span class="sxs-lookup"><span data-stu-id="ab418-157">String</span></span>|<span data-ttu-id="ab418-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab418-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ab418-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab418-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab418-160">displayName</span><span class="sxs-lookup"><span data-stu-id="ab418-160">displayName</span></span>|<span data-ttu-id="ab418-161">String</span><span class="sxs-lookup"><span data-stu-id="ab418-161">String</span></span>|<span data-ttu-id="ab418-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab418-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ab418-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab418-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab418-164">version</span><span class="sxs-lookup"><span data-stu-id="ab418-164">version</span></span>|<span data-ttu-id="ab418-165">Int32</span><span class="sxs-lookup"><span data-stu-id="ab418-165">Int32</span></span>|<span data-ttu-id="ab418-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ab418-166">Version of the device configuration.</span></span> <span data-ttu-id="ab418-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ab418-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab418-168">networkName</span><span class="sxs-lookup"><span data-stu-id="ab418-168">networkName</span></span>|<span data-ttu-id="ab418-169">String</span><span class="sxs-lookup"><span data-stu-id="ab418-169">String</span></span>|<span data-ttu-id="ab418-170">Nome da rede</span><span class="sxs-lookup"><span data-stu-id="ab418-170">Network Name</span></span>|
|<span data-ttu-id="ab418-171">SSID</span><span class="sxs-lookup"><span data-stu-id="ab418-171">ssid</span></span>|<span data-ttu-id="ab418-172">String</span><span class="sxs-lookup"><span data-stu-id="ab418-172">String</span></span>|<span data-ttu-id="ab418-173">Este é o nome da rede Wi-Fi que é difundido para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="ab418-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="ab418-174">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="ab418-174">connectAutomatically</span></span>|<span data-ttu-id="ab418-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab418-175">Boolean</span></span>|<span data-ttu-id="ab418-176">Conecte automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="ab418-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="ab418-177">Essa configuração como true ignorar o prompt do usuário e se conecte automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="ab418-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="ab418-178">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="ab418-178">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="ab418-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab418-179">Boolean</span></span>|<span data-ttu-id="ab418-180">Quando definido como true, esse perfil força o dispositivo para se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="ab418-180">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="ab418-181">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="ab418-181">wiFiSecurityType</span></span>|[<span data-ttu-id="ab418-182">androidDeviceOwnerWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="ab418-182">androidDeviceOwnerWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androiddeviceownerwifisecuritytype.md)|<span data-ttu-id="ab418-183">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseada em EAP.</span><span class="sxs-lookup"><span data-stu-id="ab418-183">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="ab418-184">Os valores possíveis são: `open`, `wep`, `wpaPersonal`.</span><span class="sxs-lookup"><span data-stu-id="ab418-184">Possible values are: `open`, `wep`, `wpaPersonal`.</span></span>|
|<span data-ttu-id="ab418-185">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="ab418-185">preSharedKey</span></span>|<span data-ttu-id="ab418-186">String</span><span class="sxs-lookup"><span data-stu-id="ab418-186">String</span></span>|<span data-ttu-id="ab418-187">Esta é a chave pré compartilhada para rede Wi-Fi WPA Pessoal.</span><span class="sxs-lookup"><span data-stu-id="ab418-187">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="ab418-188">preSharedKeyIsSet</span><span class="sxs-lookup"><span data-stu-id="ab418-188">preSharedKeyIsSet</span></span>|<span data-ttu-id="ab418-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab418-189">Boolean</span></span>|<span data-ttu-id="ab418-190">Esta é a chave pré compartilhada para rede Wi-Fi WPA Pessoal.</span><span class="sxs-lookup"><span data-stu-id="ab418-190">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="ab418-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab418-191">Response</span></span>
<span data-ttu-id="ab418-192">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab418-192">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab418-193">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ab418-193">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab418-194">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab418-194">Request</span></span>
<span data-ttu-id="ab418-195">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab418-195">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 509

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerWiFiConfiguration",
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

### <a name="response"></a><span data-ttu-id="ab418-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab418-196">Response</span></span>
<span data-ttu-id="ab418-p113">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ab418-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




