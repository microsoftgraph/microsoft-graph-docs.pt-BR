---
title: Criar androidDeviceOwnerWiFiConfiguration
description: Criar um novo objeto androidDeviceOwnerWiFiConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c1a76c274546815fc6004871b77e08502c4e908e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33933155"
---
# <a name="create-androiddeviceownerwificonfiguration"></a><span data-ttu-id="2f711-103">Criar androidDeviceOwnerWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="2f711-103">Create androidDeviceOwnerWiFiConfiguration</span></span>

> <span data-ttu-id="2f711-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2f711-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f711-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2f711-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f711-106">Criar um novo objeto [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="2f711-106">Create a new [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f711-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2f711-107">Prerequisites</span></span>
<span data-ttu-id="2f711-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f711-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f711-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f711-110">Permission type</span></span>|<span data-ttu-id="2f711-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2f711-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f711-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f711-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2f711-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f711-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2f711-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f711-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f711-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f711-115">Not supported.</span></span>|
|<span data-ttu-id="2f711-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f711-116">Application</span></span>|<span data-ttu-id="2f711-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f711-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f711-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f711-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2f711-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f711-119">Request headers</span></span>
|<span data-ttu-id="2f711-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2f711-120">Header</span></span>|<span data-ttu-id="2f711-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2f711-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f711-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f711-122">Authorization</span></span>|<span data-ttu-id="2f711-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f711-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f711-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2f711-124">Accept</span></span>|<span data-ttu-id="2f711-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2f711-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f711-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f711-126">Request body</span></span>
<span data-ttu-id="2f711-127">No corpo da solicitação, forneça uma representação JSON do objeto androidDeviceOwnerWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2f711-127">In the request body, supply a JSON representation for the androidDeviceOwnerWiFiConfiguration object.</span></span>

<span data-ttu-id="2f711-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidDeviceOwnerWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="2f711-128">The following table shows the properties that are required when you create the androidDeviceOwnerWiFiConfiguration.</span></span>

|<span data-ttu-id="2f711-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2f711-129">Property</span></span>|<span data-ttu-id="2f711-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f711-130">Type</span></span>|<span data-ttu-id="2f711-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f711-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f711-132">id</span><span class="sxs-lookup"><span data-stu-id="2f711-132">id</span></span>|<span data-ttu-id="2f711-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f711-133">String</span></span>|<span data-ttu-id="2f711-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2f711-134">Key of the entity.</span></span> <span data-ttu-id="2f711-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f711-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f711-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f711-136">lastModifiedDateTime</span></span>|<span data-ttu-id="2f711-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f711-137">DateTimeOffset</span></span>|<span data-ttu-id="2f711-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="2f711-138">DateTime the object was last modified.</span></span> <span data-ttu-id="2f711-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f711-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f711-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2f711-140">roleScopeTagIds</span></span>|<span data-ttu-id="2f711-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f711-141">String collection</span></span>|<span data-ttu-id="2f711-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="2f711-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2f711-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f711-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f711-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2f711-144">supportsScopeTags</span></span>|<span data-ttu-id="2f711-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f711-145">Boolean</span></span>|<span data-ttu-id="2f711-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="2f711-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2f711-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="2f711-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2f711-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="2f711-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2f711-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2f711-149">This property is read-only.</span></span> <span data-ttu-id="2f711-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f711-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f711-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2f711-151">createdDateTime</span></span>|<span data-ttu-id="2f711-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f711-152">DateTimeOffset</span></span>|<span data-ttu-id="2f711-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="2f711-153">DateTime the object was created.</span></span> <span data-ttu-id="2f711-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f711-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f711-155">description</span><span class="sxs-lookup"><span data-stu-id="2f711-155">description</span></span>|<span data-ttu-id="2f711-156">String</span><span class="sxs-lookup"><span data-stu-id="2f711-156">String</span></span>|<span data-ttu-id="2f711-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2f711-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2f711-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f711-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f711-159">displayName</span><span class="sxs-lookup"><span data-stu-id="2f711-159">displayName</span></span>|<span data-ttu-id="2f711-160">String</span><span class="sxs-lookup"><span data-stu-id="2f711-160">String</span></span>|<span data-ttu-id="2f711-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2f711-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2f711-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f711-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f711-163">versão</span><span class="sxs-lookup"><span data-stu-id="2f711-163">version</span></span>|<span data-ttu-id="2f711-164">Int32</span><span class="sxs-lookup"><span data-stu-id="2f711-164">Int32</span></span>|<span data-ttu-id="2f711-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2f711-165">Version of the device configuration.</span></span> <span data-ttu-id="2f711-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2f711-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f711-167">NetworkName</span><span class="sxs-lookup"><span data-stu-id="2f711-167">networkName</span></span>|<span data-ttu-id="2f711-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f711-168">String</span></span>|<span data-ttu-id="2f711-169">Nome da rede</span><span class="sxs-lookup"><span data-stu-id="2f711-169">Network Name</span></span>|
|<span data-ttu-id="2f711-170">SSID</span><span class="sxs-lookup"><span data-stu-id="2f711-170">ssid</span></span>|<span data-ttu-id="2f711-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f711-171">String</span></span>|<span data-ttu-id="2f711-172">Este é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="2f711-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="2f711-173">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="2f711-173">connectAutomatically</span></span>|<span data-ttu-id="2f711-174">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f711-174">Boolean</span></span>|<span data-ttu-id="2f711-175">Conectar automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="2f711-175">Connect automatically when this network is in range.</span></span> <span data-ttu-id="2f711-176">A definição dessa opção como true ignorará o prompt do usuário e conectará automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="2f711-176">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="2f711-177">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="2f711-177">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="2f711-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f711-178">Boolean</span></span>|<span data-ttu-id="2f711-179">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="2f711-179">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="2f711-180">à</span><span class="sxs-lookup"><span data-stu-id="2f711-180">wiFiSecurityType</span></span>|[<span data-ttu-id="2f711-181">androidDeviceOwnerWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="2f711-181">androidDeviceOwnerWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androiddeviceownerwifisecuritytype.md)|<span data-ttu-id="2f711-182">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="2f711-182">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="2f711-183">Os valores possíveis são: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="2f711-183">Possible values are: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.</span></span>|
|<span data-ttu-id="2f711-184">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="2f711-184">preSharedKey</span></span>|<span data-ttu-id="2f711-185">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f711-185">String</span></span>|<span data-ttu-id="2f711-186">Esta é a chave pré-compartilhada para a rede Wi-Fi pessoal WPA.</span><span class="sxs-lookup"><span data-stu-id="2f711-186">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="2f711-187">preSharedKeyIsSet</span><span class="sxs-lookup"><span data-stu-id="2f711-187">preSharedKeyIsSet</span></span>|<span data-ttu-id="2f711-188">Booliano</span><span class="sxs-lookup"><span data-stu-id="2f711-188">Boolean</span></span>|<span data-ttu-id="2f711-189">Esta é a chave pré-compartilhada para a rede Wi-Fi pessoal WPA.</span><span class="sxs-lookup"><span data-stu-id="2f711-189">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="2f711-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f711-190">Response</span></span>
<span data-ttu-id="2f711-191">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f711-191">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f711-192">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f711-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f711-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f711-193">Request</span></span>
<span data-ttu-id="2f711-194">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f711-194">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2f711-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f711-195">Response</span></span>
<span data-ttu-id="2f711-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f711-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




