---
title: Criar androidDeviceOwnerWiFiConfiguration
description: Criar um novo objeto androidDeviceOwnerWiFiConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7062e0bb32643474905d8c26921da6cb631b99b1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147520"
---
# <a name="create-androiddeviceownerwificonfiguration"></a><span data-ttu-id="dc4bc-103">Criar androidDeviceOwnerWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="dc4bc-103">Create androidDeviceOwnerWiFiConfiguration</span></span>

> <span data-ttu-id="dc4bc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dc4bc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc4bc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dc4bc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc4bc-106">Criar um novo objeto [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="dc4bc-106">Create a new [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dc4bc-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dc4bc-107">Prerequisites</span></span>
<span data-ttu-id="dc4bc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="dc4bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="dc4bc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc4bc-110">Permission type</span></span>|<span data-ttu-id="dc4bc-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dc4bc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc4bc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc4bc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dc4bc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc4bc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dc4bc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc4bc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc4bc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc4bc-115">Not supported.</span></span>|
|<span data-ttu-id="dc4bc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc4bc-116">Application</span></span>|<span data-ttu-id="dc4bc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc4bc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc4bc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc4bc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="dc4bc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc4bc-119">Request headers</span></span>
|<span data-ttu-id="dc4bc-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dc4bc-120">Header</span></span>|<span data-ttu-id="dc4bc-121">Valor</span><span class="sxs-lookup"><span data-stu-id="dc4bc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc4bc-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc4bc-122">Authorization</span></span>|<span data-ttu-id="dc4bc-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc4bc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc4bc-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dc4bc-124">Accept</span></span>|<span data-ttu-id="dc4bc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dc4bc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc4bc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dc4bc-126">Request body</span></span>
<span data-ttu-id="dc4bc-127">No corpo da solicitação, forneça uma representação JSON do objeto androidDeviceOwnerWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="dc4bc-127">In the request body, supply a JSON representation for the androidDeviceOwnerWiFiConfiguration object.</span></span>

<span data-ttu-id="dc4bc-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidDeviceOwnerWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="dc4bc-128">The following table shows the properties that are required when you create the androidDeviceOwnerWiFiConfiguration.</span></span>

|<span data-ttu-id="dc4bc-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dc4bc-129">Property</span></span>|<span data-ttu-id="dc4bc-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc4bc-130">Type</span></span>|<span data-ttu-id="dc4bc-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc4bc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc4bc-132">id</span><span class="sxs-lookup"><span data-stu-id="dc4bc-132">id</span></span>|<span data-ttu-id="dc4bc-133">String</span><span class="sxs-lookup"><span data-stu-id="dc4bc-133">String</span></span>|<span data-ttu-id="dc4bc-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="dc4bc-134">Key of the entity.</span></span> <span data-ttu-id="dc4bc-135">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dc4bc-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dc4bc-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dc4bc-136">lastModifiedDateTime</span></span>|<span data-ttu-id="dc4bc-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc4bc-137">DateTimeOffset</span></span>|<span data-ttu-id="dc4bc-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="dc4bc-138">DateTime the object was last modified.</span></span> <span data-ttu-id="dc4bc-139">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dc4bc-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dc4bc-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="dc4bc-140">roleScopeTagIds</span></span>|<span data-ttu-id="dc4bc-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="dc4bc-141">String collection</span></span>|<span data-ttu-id="dc4bc-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="dc4bc-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="dc4bc-143">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dc4bc-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dc4bc-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="dc4bc-144">supportsScopeTags</span></span>|<span data-ttu-id="dc4bc-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="dc4bc-145">Boolean</span></span>|<span data-ttu-id="dc4bc-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="dc4bc-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="dc4bc-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="dc4bc-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="dc4bc-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="dc4bc-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="dc4bc-149">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dc4bc-149">This property is read-only.</span></span> <span data-ttu-id="dc4bc-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dc4bc-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dc4bc-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dc4bc-151">createdDateTime</span></span>|<span data-ttu-id="dc4bc-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc4bc-152">DateTimeOffset</span></span>|<span data-ttu-id="dc4bc-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="dc4bc-153">DateTime the object was created.</span></span> <span data-ttu-id="dc4bc-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dc4bc-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dc4bc-155">description</span><span class="sxs-lookup"><span data-stu-id="dc4bc-155">description</span></span>|<span data-ttu-id="dc4bc-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dc4bc-156">String</span></span>|<span data-ttu-id="dc4bc-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dc4bc-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="dc4bc-158">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dc4bc-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dc4bc-159">displayName</span><span class="sxs-lookup"><span data-stu-id="dc4bc-159">displayName</span></span>|<span data-ttu-id="dc4bc-160">String</span><span class="sxs-lookup"><span data-stu-id="dc4bc-160">String</span></span>|<span data-ttu-id="dc4bc-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dc4bc-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="dc4bc-162">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dc4bc-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dc4bc-163">version</span><span class="sxs-lookup"><span data-stu-id="dc4bc-163">version</span></span>|<span data-ttu-id="dc4bc-164">Int32</span><span class="sxs-lookup"><span data-stu-id="dc4bc-164">Int32</span></span>|<span data-ttu-id="dc4bc-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dc4bc-165">Version of the device configuration.</span></span> <span data-ttu-id="dc4bc-166">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dc4bc-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dc4bc-167">NetworkName</span><span class="sxs-lookup"><span data-stu-id="dc4bc-167">networkName</span></span>|<span data-ttu-id="dc4bc-168">String</span><span class="sxs-lookup"><span data-stu-id="dc4bc-168">String</span></span>|<span data-ttu-id="dc4bc-169">Nome da rede</span><span class="sxs-lookup"><span data-stu-id="dc4bc-169">Network Name</span></span>|
|<span data-ttu-id="dc4bc-170">SSID</span><span class="sxs-lookup"><span data-stu-id="dc4bc-170">ssid</span></span>|<span data-ttu-id="dc4bc-171">String</span><span class="sxs-lookup"><span data-stu-id="dc4bc-171">String</span></span>|<span data-ttu-id="dc4bc-172">Este é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="dc4bc-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="dc4bc-173">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="dc4bc-173">connectAutomatically</span></span>|<span data-ttu-id="dc4bc-174">Booliano</span><span class="sxs-lookup"><span data-stu-id="dc4bc-174">Boolean</span></span>|<span data-ttu-id="dc4bc-175">Conectar automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="dc4bc-175">Connect automatically when this network is in range.</span></span> <span data-ttu-id="dc4bc-176">A definição dessa opção como true ignorará o prompt do usuário e conectará automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="dc4bc-176">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="dc4bc-177">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="dc4bc-177">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="dc4bc-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="dc4bc-178">Boolean</span></span>|<span data-ttu-id="dc4bc-179">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="dc4bc-179">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="dc4bc-180">à</span><span class="sxs-lookup"><span data-stu-id="dc4bc-180">wiFiSecurityType</span></span>|[<span data-ttu-id="dc4bc-181">androidDeviceOwnerWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="dc4bc-181">androidDeviceOwnerWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androiddeviceownerwifisecuritytype.md)|<span data-ttu-id="dc4bc-182">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="dc4bc-182">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="dc4bc-183">Os valores possíveis são: `open`, `wep`, `wpaPersonal`.</span><span class="sxs-lookup"><span data-stu-id="dc4bc-183">Possible values are: `open`, `wep`, `wpaPersonal`.</span></span>|
|<span data-ttu-id="dc4bc-184">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="dc4bc-184">preSharedKey</span></span>|<span data-ttu-id="dc4bc-185">String</span><span class="sxs-lookup"><span data-stu-id="dc4bc-185">String</span></span>|<span data-ttu-id="dc4bc-186">Esta é a chave pré-compartilhada para a rede Wi-Fi pessoal WPA.</span><span class="sxs-lookup"><span data-stu-id="dc4bc-186">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="dc4bc-187">preSharedKeyIsSet</span><span class="sxs-lookup"><span data-stu-id="dc4bc-187">preSharedKeyIsSet</span></span>|<span data-ttu-id="dc4bc-188">Booliano</span><span class="sxs-lookup"><span data-stu-id="dc4bc-188">Boolean</span></span>|<span data-ttu-id="dc4bc-189">Esta é a chave pré-compartilhada para a rede Wi-Fi pessoal WPA.</span><span class="sxs-lookup"><span data-stu-id="dc4bc-189">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="dc4bc-190">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc4bc-190">Response</span></span>
<span data-ttu-id="dc4bc-191">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dc4bc-191">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc4bc-192">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dc4bc-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc4bc-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc4bc-193">Request</span></span>
<span data-ttu-id="dc4bc-194">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc4bc-194">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dc4bc-195">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc4bc-195">Response</span></span>
<span data-ttu-id="dc4bc-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dc4bc-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




