---
title: Criar androidWiFiConfiguration
description: Criar um novo objeto androidWiFiConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3bd1d275ca75b3412221e88bbbfbe33b9fb2535f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776588"
---
# <a name="create-androidwificonfiguration"></a><span data-ttu-id="6c050-103">Criar androidWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="6c050-103">Create androidWiFiConfiguration</span></span>

> <span data-ttu-id="6c050-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6c050-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c050-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6c050-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c050-106">Criar um novo objeto [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="6c050-106">Create a new [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c050-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6c050-107">Prerequisites</span></span>
<span data-ttu-id="6c050-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c050-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c050-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c050-110">Permission type</span></span>|<span data-ttu-id="6c050-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6c050-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c050-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c050-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6c050-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c050-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6c050-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c050-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c050-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c050-115">Not supported.</span></span>|
|<span data-ttu-id="6c050-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c050-116">Application</span></span>|<span data-ttu-id="6c050-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c050-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c050-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c050-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6c050-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c050-119">Request headers</span></span>
|<span data-ttu-id="6c050-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6c050-120">Header</span></span>|<span data-ttu-id="6c050-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6c050-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c050-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c050-122">Authorization</span></span>|<span data-ttu-id="6c050-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c050-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c050-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6c050-124">Accept</span></span>|<span data-ttu-id="6c050-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6c050-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c050-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c050-126">Request body</span></span>
<span data-ttu-id="6c050-127">No corpo da solicitação, forneça uma representação JSON do objeto androidWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6c050-127">In the request body, supply a JSON representation for the androidWiFiConfiguration object.</span></span>

<span data-ttu-id="6c050-128">A tabela a seguir mostra as propriedades que são necessárias ao criar androidWiFiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="6c050-128">The following table shows the properties that are required when you create the androidWiFiConfiguration.</span></span>

|<span data-ttu-id="6c050-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c050-129">Property</span></span>|<span data-ttu-id="6c050-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c050-130">Type</span></span>|<span data-ttu-id="6c050-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c050-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c050-132">id</span><span class="sxs-lookup"><span data-stu-id="6c050-132">id</span></span>|<span data-ttu-id="6c050-133">String</span><span class="sxs-lookup"><span data-stu-id="6c050-133">String</span></span>|<span data-ttu-id="6c050-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="6c050-134">Key of the entity.</span></span> <span data-ttu-id="6c050-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c050-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c050-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c050-136">lastModifiedDateTime</span></span>|<span data-ttu-id="6c050-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c050-137">DateTimeOffset</span></span>|<span data-ttu-id="6c050-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="6c050-138">DateTime the object was last modified.</span></span> <span data-ttu-id="6c050-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c050-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c050-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6c050-140">roleScopeTagIds</span></span>|<span data-ttu-id="6c050-141">Coleção String</span><span class="sxs-lookup"><span data-stu-id="6c050-141">String collection</span></span>|<span data-ttu-id="6c050-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="6c050-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6c050-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c050-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c050-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6c050-144">supportsScopeTags</span></span>|<span data-ttu-id="6c050-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c050-145">Boolean</span></span>|<span data-ttu-id="6c050-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="6c050-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6c050-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="6c050-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6c050-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="6c050-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6c050-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6c050-149">This property is read-only.</span></span> <span data-ttu-id="6c050-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c050-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c050-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c050-151">createdDateTime</span></span>|<span data-ttu-id="6c050-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c050-152">DateTimeOffset</span></span>|<span data-ttu-id="6c050-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="6c050-153">DateTime the object was created.</span></span> <span data-ttu-id="6c050-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c050-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c050-155">description</span><span class="sxs-lookup"><span data-stu-id="6c050-155">description</span></span>|<span data-ttu-id="6c050-156">String</span><span class="sxs-lookup"><span data-stu-id="6c050-156">String</span></span>|<span data-ttu-id="6c050-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6c050-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6c050-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c050-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c050-159">displayName</span><span class="sxs-lookup"><span data-stu-id="6c050-159">displayName</span></span>|<span data-ttu-id="6c050-160">String</span><span class="sxs-lookup"><span data-stu-id="6c050-160">String</span></span>|<span data-ttu-id="6c050-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6c050-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6c050-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c050-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c050-163">versão</span><span class="sxs-lookup"><span data-stu-id="6c050-163">version</span></span>|<span data-ttu-id="6c050-164">Int32</span><span class="sxs-lookup"><span data-stu-id="6c050-164">Int32</span></span>|<span data-ttu-id="6c050-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6c050-165">Version of the device configuration.</span></span> <span data-ttu-id="6c050-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6c050-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6c050-167">NetworkName</span><span class="sxs-lookup"><span data-stu-id="6c050-167">networkName</span></span>|<span data-ttu-id="6c050-168">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c050-168">String</span></span>|<span data-ttu-id="6c050-169">Nome da rede</span><span class="sxs-lookup"><span data-stu-id="6c050-169">Network Name</span></span>|
|<span data-ttu-id="6c050-170">SSID</span><span class="sxs-lookup"><span data-stu-id="6c050-170">ssid</span></span>|<span data-ttu-id="6c050-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c050-171">String</span></span>|<span data-ttu-id="6c050-172">Este é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="6c050-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="6c050-173">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="6c050-173">connectAutomatically</span></span>|<span data-ttu-id="6c050-174">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c050-174">Boolean</span></span>|<span data-ttu-id="6c050-175">Conectar automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="6c050-175">Connect automatically when this network is in range.</span></span> <span data-ttu-id="6c050-176">A definição dessa opção como true ignorará o prompt do usuário e conectará automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="6c050-176">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="6c050-177">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="6c050-177">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="6c050-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="6c050-178">Boolean</span></span>|<span data-ttu-id="6c050-179">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="6c050-179">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="6c050-180">à</span><span class="sxs-lookup"><span data-stu-id="6c050-180">wiFiSecurityType</span></span>|[<span data-ttu-id="6c050-181">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="6c050-181">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="6c050-182">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="6c050-182">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="6c050-183">Os valores possíveis são: `open` e `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="6c050-183">Possible values are: `open`, `wpaEnterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="6c050-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c050-184">Response</span></span>
<span data-ttu-id="6c050-185">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6c050-185">If successful, this method returns a `201 Created` response code and a [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c050-186">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6c050-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c050-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c050-187">Request</span></span>
<span data-ttu-id="6c050-188">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c050-188">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 435

{
  "@odata.type": "#microsoft.graph.androidWiFiConfiguration",
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

### <a name="response"></a><span data-ttu-id="6c050-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c050-189">Response</span></span>
<span data-ttu-id="6c050-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c050-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 607

{
  "@odata.type": "#microsoft.graph.androidWiFiConfiguration",
  "id": "51cfd26f-d26f-51cf-6fd2-cf516fd2cf51",
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





