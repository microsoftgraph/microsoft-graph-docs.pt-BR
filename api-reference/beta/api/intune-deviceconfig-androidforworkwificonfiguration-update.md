---
title: Atualizar androidForWorkWiFiConfiguration
description: Atualiza as propriedades de um objeto androidForWorkWiFiConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5a649e662e2e9542ee97c8ce1d8276e8786cd057
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32477983"
---
# <a name="update-androidforworkwificonfiguration"></a><span data-ttu-id="a9fbf-103">Atualizar androidForWorkWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="a9fbf-103">Update androidForWorkWiFiConfiguration</span></span>

> <span data-ttu-id="a9fbf-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a9fbf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9fbf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a9fbf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9fbf-106">Atualiza as propriedades de um objeto [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a9fbf-106">Update the properties of a [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9fbf-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a9fbf-107">Prerequisites</span></span>
<span data-ttu-id="a9fbf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9fbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9fbf-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a9fbf-110">Permission type</span></span>|<span data-ttu-id="a9fbf-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a9fbf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9fbf-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a9fbf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a9fbf-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9fbf-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a9fbf-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a9fbf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9fbf-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9fbf-115">Not supported.</span></span>|
|<span data-ttu-id="a9fbf-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a9fbf-116">Application</span></span>|<span data-ttu-id="a9fbf-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a9fbf-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9fbf-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a9fbf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a9fbf-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a9fbf-119">Request headers</span></span>
|<span data-ttu-id="a9fbf-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a9fbf-120">Header</span></span>|<span data-ttu-id="a9fbf-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a9fbf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9fbf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a9fbf-122">Authorization</span></span>|<span data-ttu-id="a9fbf-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a9fbf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9fbf-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a9fbf-124">Accept</span></span>|<span data-ttu-id="a9fbf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a9fbf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9fbf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a9fbf-126">Request body</span></span>
<span data-ttu-id="a9fbf-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a9fbf-127">In the request body, supply a JSON representation for the [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object.</span></span>

<span data-ttu-id="a9fbf-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a9fbf-128">The following table shows the properties that are required when you create the [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span></span>

|<span data-ttu-id="a9fbf-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9fbf-129">Property</span></span>|<span data-ttu-id="a9fbf-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9fbf-130">Type</span></span>|<span data-ttu-id="a9fbf-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9fbf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9fbf-132">id</span><span class="sxs-lookup"><span data-stu-id="a9fbf-132">id</span></span>|<span data-ttu-id="a9fbf-133">String</span><span class="sxs-lookup"><span data-stu-id="a9fbf-133">String</span></span>|<span data-ttu-id="a9fbf-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a9fbf-134">Key of the entity.</span></span> <span data-ttu-id="a9fbf-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9fbf-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9fbf-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9fbf-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a9fbf-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9fbf-137">DateTimeOffset</span></span>|<span data-ttu-id="a9fbf-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a9fbf-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a9fbf-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9fbf-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9fbf-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a9fbf-140">roleScopeTagIds</span></span>|<span data-ttu-id="a9fbf-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a9fbf-141">String collection</span></span>|<span data-ttu-id="a9fbf-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="a9fbf-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a9fbf-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9fbf-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9fbf-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a9fbf-144">supportsScopeTags</span></span>|<span data-ttu-id="a9fbf-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="a9fbf-145">Boolean</span></span>|<span data-ttu-id="a9fbf-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="a9fbf-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a9fbf-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="a9fbf-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a9fbf-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="a9fbf-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a9fbf-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a9fbf-149">This property is read-only.</span></span> <span data-ttu-id="a9fbf-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9fbf-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9fbf-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a9fbf-151">createdDateTime</span></span>|<span data-ttu-id="a9fbf-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9fbf-152">DateTimeOffset</span></span>|<span data-ttu-id="a9fbf-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a9fbf-153">DateTime the object was created.</span></span> <span data-ttu-id="a9fbf-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9fbf-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9fbf-155">description</span><span class="sxs-lookup"><span data-stu-id="a9fbf-155">description</span></span>|<span data-ttu-id="a9fbf-156">String</span><span class="sxs-lookup"><span data-stu-id="a9fbf-156">String</span></span>|<span data-ttu-id="a9fbf-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a9fbf-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a9fbf-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9fbf-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9fbf-159">displayName</span><span class="sxs-lookup"><span data-stu-id="a9fbf-159">displayName</span></span>|<span data-ttu-id="a9fbf-160">String</span><span class="sxs-lookup"><span data-stu-id="a9fbf-160">String</span></span>|<span data-ttu-id="a9fbf-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a9fbf-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a9fbf-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9fbf-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9fbf-163">versão</span><span class="sxs-lookup"><span data-stu-id="a9fbf-163">version</span></span>|<span data-ttu-id="a9fbf-164">Int32</span><span class="sxs-lookup"><span data-stu-id="a9fbf-164">Int32</span></span>|<span data-ttu-id="a9fbf-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a9fbf-165">Version of the device configuration.</span></span> <span data-ttu-id="a9fbf-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a9fbf-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a9fbf-167">NetworkName</span><span class="sxs-lookup"><span data-stu-id="a9fbf-167">networkName</span></span>|<span data-ttu-id="a9fbf-168">String</span><span class="sxs-lookup"><span data-stu-id="a9fbf-168">String</span></span>|<span data-ttu-id="a9fbf-169">Nome da rede</span><span class="sxs-lookup"><span data-stu-id="a9fbf-169">Network Name</span></span>|
|<span data-ttu-id="a9fbf-170">SSID</span><span class="sxs-lookup"><span data-stu-id="a9fbf-170">ssid</span></span>|<span data-ttu-id="a9fbf-171">String</span><span class="sxs-lookup"><span data-stu-id="a9fbf-171">String</span></span>|<span data-ttu-id="a9fbf-172">Este é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="a9fbf-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="a9fbf-173">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="a9fbf-173">connectAutomatically</span></span>|<span data-ttu-id="a9fbf-174">Booliano</span><span class="sxs-lookup"><span data-stu-id="a9fbf-174">Boolean</span></span>|<span data-ttu-id="a9fbf-175">Conectar automaticamente quando esta rede estiver no intervalo.</span><span class="sxs-lookup"><span data-stu-id="a9fbf-175">Connect automatically when this network is in range.</span></span> <span data-ttu-id="a9fbf-176">A definição dessa opção como true ignorará o prompt do usuário e conectará automaticamente o dispositivo à rede Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="a9fbf-176">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="a9fbf-177">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="a9fbf-177">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="a9fbf-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="a9fbf-178">Boolean</span></span>|<span data-ttu-id="a9fbf-179">Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.</span><span class="sxs-lookup"><span data-stu-id="a9fbf-179">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="a9fbf-180">à</span><span class="sxs-lookup"><span data-stu-id="a9fbf-180">wiFiSecurityType</span></span>|[<span data-ttu-id="a9fbf-181">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="a9fbf-181">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="a9fbf-182">Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseado em EAP.</span><span class="sxs-lookup"><span data-stu-id="a9fbf-182">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="a9fbf-183">Os valores possíveis são: `open` e `wpaEnterprise`.</span><span class="sxs-lookup"><span data-stu-id="a9fbf-183">Possible values are: `open`, `wpaEnterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="a9fbf-184">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9fbf-184">Response</span></span>
<span data-ttu-id="a9fbf-185">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a9fbf-185">If successful, this method returns a `200 OK` response code and an updated [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9fbf-186">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a9fbf-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9fbf-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a9fbf-187">Request</span></span>
<span data-ttu-id="a9fbf-188">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a9fbf-188">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="a9fbf-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="a9fbf-189">Response</span></span>
<span data-ttu-id="a9fbf-p112">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a9fbf-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





