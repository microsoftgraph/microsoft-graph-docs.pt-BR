---
title: Criar androidForWorkWiFiConfiguration
description: Criar um novo objeto androidForWorkWiFiConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f66b1efd63baec06ca94a88a3d12f77d76190077
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162570"
---
# <a name="create-androidforworkwificonfiguration"></a><span data-ttu-id="9ff9d-103">Criar androidForWorkWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="9ff9d-103">Create androidForWorkWiFiConfiguration</span></span>

> <span data-ttu-id="9ff9d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9ff9d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ff9d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9ff9d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ff9d-106">Criar um novo objeto [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="9ff9d-106">Create a new [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ff9d-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9ff9d-107">Prerequisites</span></span>
<span data-ttu-id="9ff9d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9ff9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9ff9d-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ff9d-110">Permission type</span></span>|<span data-ttu-id="9ff9d-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9ff9d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ff9d-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ff9d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9ff9d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ff9d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9ff9d-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9ff9d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ff9d-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ff9d-115">Not supported.</span></span>|
|<span data-ttu-id="9ff9d-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ff9d-116">Application</span></span>|<span data-ttu-id="9ff9d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ff9d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ff9d-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ff9d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9ff9d-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ff9d-119">Request headers</span></span>
|<span data-ttu-id="9ff9d-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9ff9d-120">Header</span></span>|<span data-ttu-id="9ff9d-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9ff9d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ff9d-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9ff9d-122">Authorization</span></span>|<span data-ttu-id="9ff9d-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9ff9d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ff9d-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9ff9d-124">Accept</span></span>|<span data-ttu-id="9ff9d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9ff9d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ff9d-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ff9d-126">Request body</span></span>
<span data-ttu-id="9ff9d-127">No corpo da solicitação, forneça uma representação JSON do objeto androidForWorkWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="9ff9d-127">In the request body, supply a JSON representation for the androidForWorkWiFiConfiguration object.</span></span>

<span data-ttu-id="9ff9d-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidForWorkWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="9ff9d-128">The following table shows the properties that are required when you create the androidForWorkWiFiConfiguration.</span></span>

|<span data-ttu-id="9ff9d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ff9d-129">Property</span></span>|<span data-ttu-id="9ff9d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ff9d-130">Type</span></span>|<span data-ttu-id="9ff9d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ff9d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ff9d-132">id</span><span class="sxs-lookup"><span data-stu-id="9ff9d-132">id</span></span>|<span data-ttu-id="9ff9d-133">String</span><span class="sxs-lookup"><span data-stu-id="9ff9d-133">String</span></span>|<span data-ttu-id="9ff9d-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9ff9d-134">Key of the entity.</span></span> <span data-ttu-id="9ff9d-135">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ff9d-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ff9d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ff9d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9ff9d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ff9d-137">DateTimeOffset</span></span>|<span data-ttu-id="9ff9d-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="9ff9d-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9ff9d-139">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ff9d-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ff9d-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9ff9d-140">roleScopeTagIds</span></span>|<span data-ttu-id="9ff9d-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ff9d-141">String collection</span></span>|<span data-ttu-id="9ff9d-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="9ff9d-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9ff9d-143">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ff9d-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ff9d-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9ff9d-144">supportsScopeTags</span></span>|<span data-ttu-id="9ff9d-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="9ff9d-145">Boolean</span></span>|<span data-ttu-id="9ff9d-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="9ff9d-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9ff9d-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="9ff9d-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9ff9d-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="9ff9d-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9ff9d-149">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9ff9d-149">This property is read-only.</span></span> <span data-ttu-id="9ff9d-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ff9d-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ff9d-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ff9d-151">createdDateTime</span></span>|<span data-ttu-id="9ff9d-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ff9d-152">DateTimeOffset</span></span>|<span data-ttu-id="9ff9d-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="9ff9d-153">DateTime the object was created.</span></span> <span data-ttu-id="9ff9d-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ff9d-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ff9d-155">description</span><span class="sxs-lookup"><span data-stu-id="9ff9d-155">description</span></span>|<span data-ttu-id="9ff9d-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ff9d-156">String</span></span>|<span data-ttu-id="9ff9d-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9ff9d-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9ff9d-158">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ff9d-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ff9d-159">displayName</span><span class="sxs-lookup"><span data-stu-id="9ff9d-159">displayName</span></span>|<span data-ttu-id="9ff9d-160">String</span><span class="sxs-lookup"><span data-stu-id="9ff9d-160">String</span></span>|<span data-ttu-id="9ff9d-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9ff9d-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9ff9d-162">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ff9d-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ff9d-163">version</span><span class="sxs-lookup"><span data-stu-id="9ff9d-163">version</span></span>|<span data-ttu-id="9ff9d-164">Int32</span><span class="sxs-lookup"><span data-stu-id="9ff9d-164">Int32</span></span>|<span data-ttu-id="9ff9d-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9ff9d-165">Version of the device configuration.</span></span> <span data-ttu-id="9ff9d-166">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9ff9d-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ff9d-167">NetworkName</span><span class="sxs-lookup"><span data-stu-id="9ff9d-167">networkName</span></span>|<span data-ttu-id="9ff9d-168">String</span><span class="sxs-lookup"><span data-stu-id="9ff9d-168">String</span></span>|<span data-ttu-id="9ff9d-169">Nome da rede</span><span class="sxs-lookup"><span data-stu-id="9ff9d-169">Network Name</span></span>|
|<span data-ttu-id="9ff9d-170">SSID</span><span class="sxs-lookup"><span data-stu-id="9ff9d-170">ssid</span></span>|<span data-ttu-id="9ff9d-171">String</span><span class="sxs-lookup"><span data-stu-id="9ff9d-171">String</span></span>|<span data-ttu-id="9ff9d-172">Este é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="9ff9d-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="9ff9d-173">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="9ff9d-173">connectAutomatically</span></span>|<span data-ttu-id="9ff9d-174">Booliano</span><span class="sxs-lookup"><span data-stu-id="9ff9d-174">Boolean</span></span>|<span data-ttu-id="9ff9d-175">Conectar automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="9ff9d-175">Connect automatically when this network is in range.</span></span> <span data-ttu-id="9ff9d-176">A definição dessa opção como true ignorará o prompt do usuário e conectará automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="9ff9d-176">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="9ff9d-177">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="9ff9d-177">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="9ff9d-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="9ff9d-178">Boolean</span></span>|<span data-ttu-id="9ff9d-179">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="9ff9d-179">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="9ff9d-180">à</span><span class="sxs-lookup"><span data-stu-id="9ff9d-180">wiFiSecurityType</span></span>|[<span data-ttu-id="9ff9d-181">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="9ff9d-181">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="9ff9d-182">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="9ff9d-182">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="9ff9d-183">Os valores possíveis são: `open` e `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="9ff9d-183">Possible values are: `open`, `wpaEnterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="9ff9d-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ff9d-184">Response</span></span>
<span data-ttu-id="9ff9d-185">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ff9d-185">If successful, this method returns a `201 Created` response code and a [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ff9d-186">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9ff9d-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ff9d-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ff9d-187">Request</span></span>
<span data-ttu-id="9ff9d-188">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9ff9d-188">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 442

{
  "@odata.type": "#microsoft.graph.androidForWorkWiFiConfiguration",
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

### <a name="response"></a><span data-ttu-id="9ff9d-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ff9d-189">Response</span></span>
<span data-ttu-id="9ff9d-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9ff9d-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




